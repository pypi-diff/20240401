# Comparing `tmp/autovenv-0.3.1671337560.tar.gz` & `tmp/autovenv-0.3.1671337561.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autovenv-0.3.1671337560.tar", last modified: Sun Dec 18 04:41:42 2022, max compression
+gzip compressed data, was "autovenv-0.3.1671337561.tar", last modified: Mon Apr  1 12:08:33 2024, max compression
```

## Comparing `autovenv-0.3.1671337560.tar` & `autovenv-0.3.1671337561.tar`

### file list

```diff
@@ -1,1084 +1,1303 @@
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.868799 autovenv-0.3.1671337560/
--rw-r--r--   0 rob        (501) staff       (20)     1210 2016-01-01 06:14:00.000000 autovenv-0.3.1671337560/LICENSE
--rw-r--r--   0 rob        (501) staff       (20)       42 2016-01-03 06:39:26.000000 autovenv-0.3.1671337560/MANIFEST.in
--rw-r--r--   0 rob        (501) staff       (20)      538 2022-12-18 04:41:42.868523 autovenv-0.3.1671337560/PKG-INFO
--rwxr--r--   0 rob        (501) staff       (20)     2234 2017-03-29 11:57:30.000000 autovenv-0.3.1671337560/README.rst
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.447584 autovenv-0.3.1671337560/autovenv/
--rwxr--r--   0 rob        (501) staff       (20)      492 2018-07-16 12:34:06.000000 autovenv-0.3.1671337560/autovenv/__init__.py
--rw-r--r--   0 rob        (501) staff       (20)     2609 2019-10-17 22:55:47.000000 autovenv-0.3.1671337560/autovenv/command.py
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.449895 autovenv-0.3.1671337560/autovenv/python-build/
--rw-r--r--   0 rob        (501) staff       (20)     1097 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/LICENSE
--rwxr-xr-x   0 rob        (501) staff       (20)    67834 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/autovenv-python-build
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.421503 autovenv-0.3.1671337560/autovenv/python-build/share/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.745975 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/
--rw-r--r--   0 rob        (501) staff       (20)      732 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.1.3
--rw-r--r--   0 rob        (501) staff       (20)      732 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.2.3
--rw-r--r--   0 rob        (501) staff       (20)      732 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.3.7
--rw-r--r--   0 rob        (501) staff       (20)      724 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.0
--rw-r--r--   0 rob        (501) staff       (20)      730 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.1
--rw-r--r--   0 rob        (501) staff       (20)      730 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.2
--rw-r--r--   0 rob        (501) staff       (20)      730 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.3
--rw-r--r--   0 rob        (501) staff       (20)      730 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.4
--rw-r--r--   0 rob        (501) staff       (20)      730 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.5
--rw-r--r--   0 rob        (501) staff       (20)      730 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.6
--rw-r--r--   0 rob        (501) staff       (20)      716 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.0
--rw-r--r--   0 rob        (501) staff       (20)      722 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.1
--rw-r--r--   0 rob        (501) staff       (20)      722 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.2
--rw-r--r--   0 rob        (501) staff       (20)      722 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.3
--rw-r--r--   0 rob        (501) staff       (20)      722 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.4
--rw-r--r--   0 rob        (501) staff       (20)      722 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.5
--rw-r--r--   0 rob        (501) staff       (20)      722 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.6
--rw-r--r--   0 rob        (501) staff       (20)      578 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.0
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.1
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.2
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.3
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.4
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.5
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.6
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.7
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.8
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.9
--rw-r--r--   0 rob        (501) staff       (20)      533 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7-dev
--rw-r--r--   0 rob        (501) staff       (20)      594 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.0
--rw-r--r--   0 rob        (501) staff       (20)      600 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.1
--rw-r--r--   0 rob        (501) staff       (20)      851 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.10
--rw-r--r--   0 rob        (501) staff       (20)      851 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.11
--rw-r--r--   0 rob        (501) staff       (20)      851 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.12
--rw-r--r--   0 rob        (501) staff       (20)      851 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.13
--rw-r--r--   0 rob        (501) staff       (20)      868 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.14
--rw-r--r--   0 rob        (501) staff       (20)      868 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.15
--rw-r--r--   0 rob        (501) staff       (20)      851 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.16
--rw-r--r--   0 rob        (501) staff       (20)      851 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.17
--rw-r--r--   0 rob        (501) staff       (20)      930 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.18
--rw-r--r--   0 rob        (501) staff       (20)      600 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.2
--rw-r--r--   0 rob        (501) staff       (20)      600 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.3
--rw-r--r--   0 rob        (501) staff       (20)      600 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.4
--rw-r--r--   0 rob        (501) staff       (20)      600 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.5
--rw-r--r--   0 rob        (501) staff       (20)      600 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.6
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.7
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.8
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.9
--rw-r--r--   0 rob        (501) staff       (20)     1228 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.0.1
--rw-r--r--   0 rob        (501) staff       (20)      921 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.0
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.1
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.2
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.3
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.4
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.5
--rw-r--r--   0 rob        (501) staff       (20)      569 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10-dev
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.1
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.2
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.3
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.4
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.5
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.6
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.7
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.8
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.9
--rw-r--r--   0 rob        (501) staff       (20)      611 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.11-dev
--rw-r--r--   0 rob        (501) staff       (20)      951 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.11.0
--rw-r--r--   0 rob        (501) staff       (20)      951 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.11.1
--rw-r--r--   0 rob        (501) staff       (20)      657 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.12-dev
--rw-r--r--   0 rob        (501) staff       (20)      917 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.12.0a3
--rw-r--r--   0 rob        (501) staff       (20)      921 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.0
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.1
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.2
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.3
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.4
--rw-r--r--   0 rob        (501) staff       (20)      927 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.5
--rw-r--r--   0 rob        (501) staff       (20)     1146 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.6
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.0
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.1
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.2
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.3
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.4
--rw-r--r--   0 rob        (501) staff       (20)      584 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.5
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.6
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.7
--rw-r--r--   0 rob        (501) staff       (20)      517 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4-dev
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.0
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.1
--rw-r--r--   0 rob        (501) staff       (20)      764 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.10
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.2
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.3
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.4
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.5
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.6
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.7
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.8
--rw-r--r--   0 rob        (501) staff       (20)      813 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.9
--rw-r--r--   0 rob        (501) staff       (20)      533 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5-dev
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.0
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.1
--rw-r--r--   0 rob        (501) staff       (20)      836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.10
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.2
--rw-r--r--   0 rob        (501) staff       (20)      862 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.3
--rw-r--r--   0 rob        (501) staff       (20)      862 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.4
--rw-r--r--   0 rob        (501) staff       (20)      862 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.5
--rw-r--r--   0 rob        (501) staff       (20)      862 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.6
--rw-r--r--   0 rob        (501) staff       (20)      830 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.7
--rw-r--r--   0 rob        (501) staff       (20)      830 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.8
--rw-r--r--   0 rob        (501) staff       (20)      830 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.9
--rw-r--r--   0 rob        (501) staff       (20)      533 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6-dev
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.0
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.1
--rw-r--r--   0 rob        (501) staff       (20)      868 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.10
--rw-r--r--   0 rob        (501) staff       (20)      868 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.11
--rw-r--r--   0 rob        (501) staff       (20)      868 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.12
--rw-r--r--   0 rob        (501) staff       (20)      868 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.13
--rw-r--r--   0 rob        (501) staff       (20)      858 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.14
--rw-r--r--   0 rob        (501) staff       (20)      858 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.15
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.2
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.3
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.4
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.5
--rw-r--r--   0 rob        (501) staff       (20)      845 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.6
--rw-r--r--   0 rob        (501) staff       (20)      862 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.7
--rw-r--r--   0 rob        (501) staff       (20)      862 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.8
--rw-r--r--   0 rob        (501) staff       (20)      862 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.9
--rw-r--r--   0 rob        (501) staff       (20)      568 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7-dev
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.0
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.1
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.10
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.11
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.12
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.13
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.14
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.15
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.16
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.2
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.3
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.4
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.5
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.6
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.7
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.8
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.9
--rw-r--r--   0 rob        (501) staff       (20)      568 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8-dev
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.0
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.1
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.10
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.11
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.12
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.13
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.14
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.15
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.16
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.2
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.3
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.4
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.5
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.6
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.7
--rw-r--r--   0 rob        (501) staff       (20)      907 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.8
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.9
--rw-r--r--   0 rob        (501) staff       (20)      566 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9-dev
--rw-r--r--   0 rob        (501) staff       (20)      902 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.0
--rw-r--r--   0 rob        (501) staff       (20)      902 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.1
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.10
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.11
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.12
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.13
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.14
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.15
--rw-r--r--   0 rob        (501) staff       (20)      903 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.16
--rw-r--r--   0 rob        (501) staff       (20)      912 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.2
--rw-r--r--   0 rob        (501) staff       (20)      901 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.4
--rw-r--r--   0 rob        (501) staff       (20)      901 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.5
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.6
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.7
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.8
--rw-r--r--   0 rob        (501) staff       (20)      897 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.9
--rw-r--r--   0 rob        (501) staff       (20)      666 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/activepython-2.7.14
--rw-r--r--   0 rob        (501) staff       (20)      662 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/activepython-3.5.4
--rw-r--r--   0 rob        (501) staff       (20)      976 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/activepython-3.6.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.4.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.5.0
--rw-r--r--   0 rob        (501) staff       (20)      470 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.5.1
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.6.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.6.1
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.7.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.8.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.9.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.9.1
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.9.2
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.0.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.0.1
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.1.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.2.0
--rw-r--r--   0 rob        (501) staff       (20)      909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.3.0
--rw-r--r--   0 rob        (501) staff       (20)       43 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.4.0
--rw-r--r--   0 rob        (501) staff       (20)       43 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-4.0.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2.4.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2.4.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2.5.0
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2018.12
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2019.03
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2019.07
--rw-r--r--   0 rob        (501) staff       (20)      843 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2019.10
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.0.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.1.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.1.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.2.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.3.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.3.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.4.0
--rw-r--r--   0 rob        (501) staff       (20)      924 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.0.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.0.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.1.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.2.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.3.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.3.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.0.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.0.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.1.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.2.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.3.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.4.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.4.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.5.0
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2018.12
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2019.03
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2019.07
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2019.10
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2020.02
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2020.07
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2020.11
--rw-r--r--   0 rob        (501) staff       (20)     1239 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2021.04
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2021.05
--rw-r--r--   0 rob        (501) staff       (20)      940 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2021.11
--rw-r--r--   0 rob        (501) staff       (20)     1437 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2022.05
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.0.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.1.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.1.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.2.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.3.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.3.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.4.0
--rw-r--r--   0 rob        (501) staff       (20)      924 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.0.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.0.1
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.1.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.2.0
--rw-r--r--   0 rob        (501) staff       (20)      916 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.3.0
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.3.1
--rw-r--r--   0 rob        (501) staff       (20)     1152 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/cinder-3.8-dev
--rw-r--r--   0 rob        (501) staff       (20)     2144 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpy-22.3.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-20.1.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-20.2.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-20.3.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.0.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.1.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.2.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.3.0
--rw-r--r--   0 rob        (501) staff       (20)     2012 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-22.0.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-22.1.0
--rw-r--r--   0 rob        (501) staff       (20)     2010 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-22.2.0
--rw-r--r--   0 rob        (501) staff       (20)      266 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/ironpython-2.7.4
--rw-r--r--   0 rob        (501) staff       (20)      266 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/ironpython-2.7.5
--rw-r--r--   0 rob        (501) staff       (20)      272 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/ironpython-2.7.6.3
--rw-r--r--   0 rob        (501) staff       (20)      211 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/ironpython-2.7.7
--rw-r--r--   0 rob        (501) staff       (20)      176 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/ironpython-dev
--rw-r--r--   0 rob        (501) staff       (20)      561 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5-dev
--rw-r--r--   0 rob        (501) staff       (20)      870 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.0
--rw-r--r--   0 rob        (501) staff       (20)      870 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.1
--rw-r--r--   0 rob        (501) staff       (20)      671 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.2
--rw-r--r--   0 rob        (501) staff       (20)      691 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.3
--rw-r--r--   0 rob        (501) staff       (20)      703 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.4-rc1
--rw-r--r--   0 rob        (501) staff       (20)      604 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.7.0
--rw-r--r--   0 rob        (501) staff       (20)      604 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.7.1
--rw-r--r--   0 rob        (501) staff       (20)      604 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.7.2
--rw-r--r--   0 rob        (501) staff       (20)      403 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-dev
--rw-r--r--   0 rob        (501) staff       (20)     1205 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge
--rw-r--r--   0 rob        (501) staff       (20)     1619 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-22.9.0-2
--rw-r--r--   0 rob        (501) staff       (20)     1326 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-4.10.1-4
--rw-r--r--   0 rob        (501) staff       (20)     1326 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-4.10.1-5
--rw-r--r--   0 rob        (501) staff       (20)     1338 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-4.10.3-10
--rw-r--r--   0 rob        (501) staff       (20)     1073 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-pypy3
--rw-r--r--   0 rob        (501) staff       (20)      383 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.10
--rw-r--r--   0 rob        (501) staff       (20)      383 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.11
--rw-r--r--   0 rob        (501) staff       (20)      383 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.12
--rw-r--r--   0 rob        (501) staff       (20)      383 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.13
--rw-r--r--   0 rob        (501) staff       (20)      403 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.14
--rw-r--r--   0 rob        (501) staff       (20)      403 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.15
--rw-r--r--   0 rob        (501) staff       (20)      403 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.16
--rw-r--r--   0 rob        (501) staff       (20)      403 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.17
--rw-r--r--   0 rob        (501) staff       (20)      403 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.18
--rw-r--r--   0 rob        (501) staff       (20)      409 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.19.1
--rw-r--r--   0 rob        (501) staff       (20)      387 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.9.3
--rw-r--r--   0 rob        (501) staff       (20)      387 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-1.9.4
--rw-r--r--   0 rob        (501) staff       (20)       90 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/micropython-dev
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-2.2.2
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.0.0
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.0.4
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.0.5
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.10.1
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.16.0
--rw-r--r--   0 rob        (501) staff       (20)       45 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.18.3
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.3.0
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.4.2
--rw-r--r--   0 rob        (501) staff       (20)      919 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.7.0
--rw-r--r--   0 rob        (501) staff       (20)      919 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.8.3
--rw-r--r--   0 rob        (501) staff       (20)      925 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.9.1
--rw-r--r--   0 rob        (501) staff       (20)       45 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-latest
--rw-r--r--   0 rob        (501) staff       (20)      877 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-2.7-4.8.3
--rw-r--r--   0 rob        (501) staff       (20)      938 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-3.18.3
--rw-r--r--   0 rob        (501) staff       (20)      938 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-3.19.0
--rw-r--r--   0 rob        (501) staff       (20)      932 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.0.5
--rw-r--r--   0 rob        (501) staff       (20)      938 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.1.11
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.14
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.21
--rw-r--r--   0 rob        (501) staff       (20)      945 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.27
--rw-r--r--   0 rob        (501) staff       (20)      941 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.30
--rw-r--r--   0 rob        (501) staff       (20)      841 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.31
--rw-r--r--   0 rob        (501) staff       (20)     1045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.4.10
--rw-r--r--   0 rob        (501) staff       (20)     1037 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.1
--rw-r--r--   0 rob        (501) staff       (20)     1045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.11
--rw-r--r--   0 rob        (501) staff       (20)     1045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.12
--rw-r--r--   0 rob        (501) staff       (20)     1037 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.4
--rw-r--r--   0 rob        (501) staff       (20)      853 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.6.14
--rw-r--r--   0 rob        (501) staff       (20)      853 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.7.10
--rw-r--r--   0 rob        (501) staff       (20)     1474 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.7.12
--rw-r--r--   0 rob        (501) staff       (20)      743 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-latest
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-2.2.2
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.0.0
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.0.4
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.0.5
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.10.1
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.16.0
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.18.3
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.19.0
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.3.0
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.4.2
--rw-r--r--   0 rob        (501) staff       (20)      666 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.1
--rw-r--r--   0 rob        (501) staff       (20)     1305 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.3
--rw-r--r--   0 rob        (501) staff       (20)     1305 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.11.0
--rw-r--r--   0 rob        (501) staff       (20)     1305 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.12.0
--rw-r--r--   0 rob        (501) staff       (20)      877 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.2
--rw-r--r--   0 rob        (501) staff       (20)      877 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.3
--rw-r--r--   0 rob        (501) staff       (20)     1295 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.9.2
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7.0
--rw-r--r--   0 rob        (501) staff       (20)      877 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.1
--rw-r--r--   0 rob        (501) staff       (20)     1305 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.3
--rw-r--r--   0 rob        (501) staff       (20)     1516 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.11.0
--rw-r--r--   0 rob        (501) staff       (20)     1516 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.12.0
--rw-r--r--   0 rob        (501) staff       (20)      877 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.2
--rw-r--r--   0 rob        (501) staff       (20)      877 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.3
--rw-r--r--   0 rob        (501) staff       (20)     1295 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.9.2
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8.3
--rw-r--r--   0 rob        (501) staff       (20)      666 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.1
--rw-r--r--   0 rob        (501) staff       (20)     1305 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.3
--rw-r--r--   0 rob        (501) staff       (20)     1516 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.11.0
--rw-r--r--   0 rob        (501) staff       (20)     1516 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.12.0
--rw-r--r--   0 rob        (501) staff       (20)     1295 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.9.2
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9.1
--rw-r--r--   0 rob        (501) staff       (20)      931 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.0.5
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.1.11
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.2.12
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.11
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.14
--rw-r--r--   0 rob        (501) staff       (20)      937 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.21
--rw-r--r--   0 rob        (501) staff       (20)      945 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.27
--rw-r--r--   0 rob        (501) staff       (20)      941 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.30
--rw-r--r--   0 rob        (501) staff       (20)      841 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.31
--rw-r--r--   0 rob        (501) staff       (20)     1045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.4.10
--rw-r--r--   0 rob        (501) staff       (20)     1037 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.1
--rw-r--r--   0 rob        (501) staff       (20)     1045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.11
--rw-r--r--   0 rob        (501) staff       (20)      841 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.12
--rw-r--r--   0 rob        (501) staff       (20)     1037 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.4
--rw-r--r--   0 rob        (501) staff       (20)      853 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.6.14
--rw-r--r--   0 rob        (501) staff       (20)      853 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.7.10
--rw-r--r--   0 rob        (501) staff       (20)     1474 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.7.12
--rw-r--r--   0 rob        (501) staff       (20)     1119 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-latest
--rw-r--r--   0 rob        (501) staff       (20)     1065 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge-pypy3
--rw-r--r--   0 rob        (501) staff       (20)     1618 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-22.9.0-2
--rw-r--r--   0 rob        (501) staff       (20)     1438 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10
--rw-r--r--   0 rob        (501) staff       (20)     1438 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.1-1
--rw-r--r--   0 rob        (501) staff       (20)     1598 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.1-3
--rw-r--r--   0 rob        (501) staff       (20)     1598 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.1-5
--rw-r--r--   0 rob        (501) staff       (20)     1613 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.3-10
--rw-r--r--   0 rob        (501) staff       (20)     1423 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.9.2
--rw-r--r--   0 rob        (501) staff       (20)     1204 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-latest
--rw-r--r--   0 rob        (501) staff       (20)      669 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/nogil-3.9.10
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.444463 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.421748 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.1.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.746317 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.1.3/Python-2.1.3/
--rw-r--r--   0 rob        (501) staff       (20)     2443 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.1.3/Python-2.1.3/000_patch-setup.py.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.421918 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.2.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.746887 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.2.3/Python-2.2.3/
--rw-r--r--   0 rob        (501) staff       (20)     2379 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.2.3/Python-2.2.3/000_patch-setup.py.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.422083 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.3.7/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.747680 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/
--rw-r--r--   0 rob        (501) staff       (20)     1841 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1397 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/001_fortify_crash_workaround.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.422253 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.748761 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1397 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/001_fortify_crash_workaround.diff
--rw-r--r--   0 rob        (501) staff       (20)      848 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/002_patch-posixmodule.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.422566 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.750078 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1397 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/001_fortify_crash_workaround.diff
--rw-r--r--   0 rob        (501) staff       (20)      848 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/002_patch-posixmodule.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.422805 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.751083 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1397 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/001_fortify_crash_workaround.diff
--rw-r--r--   0 rob        (501) staff       (20)      848 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/002_patch-posixmodule.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.422993 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.751962 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1397 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/001_fortify_crash_workaround.diff
--rw-r--r--   0 rob        (501) staff       (20)      848 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/002_patch-posixmodule.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.423179 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.752594 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)      848 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/001_patch-posixmodule.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.423352 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.753321 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)      848 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/001_patch-posixmodule.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.423524 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.753837 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)      848 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/001_patch-posixmodule.diff
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.423685 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.757063 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1734 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     5815 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/002_darwin_c_source.patch
--rw-r--r--   0 rob        (501) staff       (20)     9060 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/003_osx_lp64.patch
--rw-r--r--   0 rob        (501) staff       (20)   191586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/004_osx_libffi.patch
--rw-r--r--   0 rob        (501) staff       (20)     3995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/005_osx_failed_modules.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.423851 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.759506 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1754 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     5815 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/002_darwin_c_source.patch
--rw-r--r--   0 rob        (501) staff       (20)     9060 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/003_osx_lp64.patch
--rw-r--r--   0 rob        (501) staff       (20)   191586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/004_osx_libffi.patch
--rw-r--r--   0 rob        (501) staff       (20)     3995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/005_osx_failed_modules.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.424016 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.761457 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1270 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     5815 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/002_darwin_c_source.patch
--rw-r--r--   0 rob        (501) staff       (20)     9060 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/003_osx_lp64.patch
--rw-r--r--   0 rob        (501) staff       (20)   191586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/004_osx_libffi.patch
--rw-r--r--   0 rob        (501) staff       (20)     3995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/005_osx_failed_modules.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.424186 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.763762 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1270 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     5815 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/002_darwin_c_source.patch
--rw-r--r--   0 rob        (501) staff       (20)     9060 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/003_osx_lp64.patch
--rw-r--r--   0 rob        (501) staff       (20)   191586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/004_osx_libffi.patch
--rw-r--r--   0 rob        (501) staff       (20)     3995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/005_osx_failed_modules.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.424356 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.766200 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1270 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     5815 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/002_darwin_c_source.patch
--rw-r--r--   0 rob        (501) staff       (20)     9060 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/003_osx_lp64.patch
--rw-r--r--   0 rob        (501) staff       (20)   191586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/004_osx_libffi.patch
--rw-r--r--   0 rob        (501) staff       (20)     3995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/005_osx_failed_modules.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.424525 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.769012 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1270 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     5815 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/002_darwin_c_source.patch
--rw-r--r--   0 rob        (501) staff       (20)     9060 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/003_osx_lp64.patch
--rw-r--r--   0 rob        (501) staff       (20)   191586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/004_osx_libffi.patch
--rw-r--r--   0 rob        (501) staff       (20)     3995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/005_osx_failed_modules.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.424716 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.771146 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/
--rw-r--r--   0 rob        (501) staff       (20)     1873 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1270 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     5815 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/002_darwin_c_source.patch
--rw-r--r--   0 rob        (501) staff       (20)     9060 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/003_osx_lp64.patch
--rw-r--r--   0 rob        (501) staff       (20)   191586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/004_osx_libffi.patch
--rw-r--r--   0 rob        (501) staff       (20)     3995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/005_osx_failed_modules.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.424925 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.772953 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/
--rw-r--r--   0 rob        (501) staff       (20)     2771 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1728 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      747 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3143 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.425099 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.774105 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/
--rw-r--r--   0 rob        (501) staff       (20)     2771 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1732 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3143 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.425269 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.775395 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/
--rw-r--r--   0 rob        (501) staff       (20)     2771 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1732 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3143 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.425443 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.776294 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/
--rw-r--r--   0 rob        (501) staff       (20)     2771 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1732 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3143 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.425615 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.777213 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/
--rw-r--r--   0 rob        (501) staff       (20)     2771 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1732 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3143 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.425785 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.778225 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/
--rw-r--r--   0 rob        (501) staff       (20)     2771 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1772 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3142 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.425944 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.779646 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/
--rw-r--r--   0 rob        (501) staff       (20)     2450 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3319 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.426110 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.780971 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/
--rw-r--r--   0 rob        (501) staff       (20)     2450 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3319 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.426279 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.781955 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/
--rw-r--r--   0 rob        (501) staff       (20)     2450 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3319 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.426648 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.783180 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/
--rw-r--r--   0 rob        (501) staff       (20)     2450 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)      618 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/001_remove_systemstubs.patch
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/003_tk86.patch
--rw-r--r--   0 rob        (501) staff       (20)     3156 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.426868 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.784237 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/
--rw-r--r--   0 rob        (501) staff       (20)     1805 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3513 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.427053 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.785093 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/
--rw-r--r--   0 rob        (501) staff       (20)     1805 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3513 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.427243 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.10/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.785364 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.10/Python-2.7.10/
--rw-r--r--   0 rob        (501) staff       (20)      610 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.10/Python-2.7.10/003_system_library_path_in_sys_path.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.427430 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.787338 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/
--rw-r--r--   0 rob        (501) staff       (20)      995 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0001-Detect-arm64-in-configure.patch
--rw-r--r--   0 rob        (501) staff       (20)    10287 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0002-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch
--rw-r--r--   0 rob        (501) staff       (20)      887 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0003-Support-arm64-in-Mac-Tools-pythonw.patch
--rw-r--r--   0 rob        (501) staff       (20)     3379 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0004-Use-system-libffi-for-Mac-OS-10.15-and-up.patch
--rw-r--r--   0 rob        (501) staff       (20)     8453 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0005-ctypes-use-the-correct-ABI-for-variadic-functions.patch
--rw-r--r--   0 rob        (501) staff       (20)     4148 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0006-ctypes-probe-libffi-for-ffi_closure_alloc-and-ffi_pr.patch
--rw-r--r--   0 rob        (501) staff       (20)     1493 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0007-Remove-QuickTime-from-link-args.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.427620 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.788131 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      696 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)     3435 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.427790 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.789022 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      608 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)     3443 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.427960 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.789996 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      608 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)     3443 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.428130 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.790838 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      608 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)     3443 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.428306 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.792064 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/
--rw-r--r--   0 rob        (501) staff       (20)     1850 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)      608 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)     3443 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/010_ssl_no_ssl3.patch
--rw-r--r--   0 rob        (501) staff       (20)     2263 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/012_fix_bundle_loader_for_new_osx.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.428478 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.7/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.792648 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/
--rw-r--r--   0 rob        (501) staff       (20)      608 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)     3443 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.428648 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.8/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.793181 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/
--rw-r--r--   0 rob        (501) staff       (20)      608 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)     3443 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.428816 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.9/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.793772 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/
--rw-r--r--   0 rob        (501) staff       (20)      608 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/003_system_library_path_in_sys_path.patch
--rw-r--r--   0 rob        (501) staff       (20)      625 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.428990 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.794698 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/
--rw-r--r--   0 rob        (501) staff       (20)     1856 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     1270 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/001_patch-svnversion.patch
--rw-r--r--   0 rob        (501) staff       (20)     3194 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.429156 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.809180 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/
--rw-r--r--   0 rob        (501) staff       (20)     2333 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     3194 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.429328 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.810626 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/
--rw-r--r--   0 rob        (501) staff       (20)     2333 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     3194 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.429495 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.811699 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/
--rw-r--r--   0 rob        (501) staff       (20)     2333 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     3194 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.429656 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.813607 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/
--rw-r--r--   0 rob        (501) staff       (20)     2225 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3358 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.429826 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.814927 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/
--rw-r--r--   0 rob        (501) staff       (20)      524 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3317 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.429993 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.815682 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/
--rw-r--r--   0 rob        (501) staff       (20)      524 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3317 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.430161 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.10.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.816946 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/
--rw-r--r--   0 rob        (501) staff       (20)    18326 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0001-bpo-45350-Rerun-autoreconf-with-the-pkg-config-macro.patch
--rw-r--r--   0 rob        (501) staff       (20)     2846 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0002-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.430327 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.11.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.817192 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.11.0/openssl-1.1.1q/
--rw-r--r--   0 rob        (501) staff       (20)      264 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.11.0/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.430493 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.818632 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/
--rw-r--r--   0 rob        (501) staff       (20)     1648 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/000_patch-setup.py.diff
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3457 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/010_ssl_no_ssl2_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.430664 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.819128 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3447 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.430830 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.820244 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3489 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.430993 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.820913 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3445 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.431154 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.821929 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3445 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.431320 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.822558 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3445 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.431490 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.823568 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3445 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.431653 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.824060 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.431824 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.824997 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.431988 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.825589 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.432143 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.3/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.826335 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.432299 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.826737 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.4/Python-3.3.4/
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.4/Python-3.3.4/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.432452 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.827033 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.5/Python-3.3.5/
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.5/Python-3.3.5/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.436597 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.827409 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.6/Python-3.3.6/
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.6/Python-3.3.6/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.436900 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.7/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.827696 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.7/Python-3.3.7/
--rw-r--r--   0 rob        (501) staff       (20)     3503 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.7/Python-3.3.7/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.437080 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.827991 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.0/Python-3.4.0/
--rw-r--r--   0 rob        (501) staff       (20)     2783 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.0/Python-3.4.0/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.437357 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.828192 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.1/Python-3.4.1/
--rw-r--r--   0 rob        (501) staff       (20)     2783 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.1/Python-3.4.1/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.437581 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.828476 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.2/Python-3.4.2/
--rw-r--r--   0 rob        (501) staff       (20)     2783 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.2/Python-3.4.2/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.437767 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.5.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.828766 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.5.2/Python-3.5.2/
--rw-r--r--   0 rob        (501) staff       (20)      957 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.5.2/Python-3.5.2/venv.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.437952 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.850591 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/
--rw-r--r--   0 rob        (501) staff       (20)     1009 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0001-Detect-arm64-in-configure.patch
--rw-r--r--   0 rob        (501) staff       (20)     3478 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0002-bpo-36231-Support-building-on-macOS-without-usr-incl.patch
--rw-r--r--   0 rob        (501) staff       (20)    10491 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0003-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch
--rw-r--r--   0 rob        (501) staff       (20)    12468 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0004-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
--rw-r--r--   0 rob        (501) staff       (20)     1962 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0005-BPO-41100-Support-macOS-11-when-building-GH-21113.patch
--rw-r--r--   0 rob        (501) staff       (20)     1480 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0006-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
--rw-r--r--   0 rob        (501) staff       (20)      904 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0007-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
--rw-r--r--   0 rob        (501) staff       (20)     3137 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0008-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.438138 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.10/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.851368 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.10/Python-3.7.10/
--rw-r--r--   0 rob        (501) staff       (20)     2846 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.10/Python-3.7.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.438317 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.11/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.851764 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.11/Python-3.7.11/
--rw-r--r--   0 rob        (501) staff       (20)     2846 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.11/Python-3.7.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.438494 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.852855 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/
--rw-r--r--   0 rob        (501) staff       (20)    12192 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
--rw-r--r--   0 rob        (501) staff       (20)     1479 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
--rw-r--r--   0 rob        (501) staff       (20)      904 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
--rw-r--r--   0 rob        (501) staff       (20)     1461 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0004-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.438661 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.853909 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/
--rw-r--r--   0 rob        (501) staff       (20)    12192 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
--rw-r--r--   0 rob        (501) staff       (20)     1479 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
--rw-r--r--   0 rob        (501) staff       (20)      904 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.438835 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.854659 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/
--rw-r--r--   0 rob        (501) staff       (20)    12192 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
--rw-r--r--   0 rob        (501) staff       (20)     1464 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
--rw-r--r--   0 rob        (501) staff       (20)      904 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.439108 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.855573 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/
--rw-r--r--   0 rob        (501) staff       (20)    12192 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
--rw-r--r--   0 rob        (501) staff       (20)     1464 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
--rw-r--r--   0 rob        (501) staff       (20)      904 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.855864 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/openssl-1.1.1q/
--rw-r--r--   0 rob        (501) staff       (20)      264 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.439382 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.856729 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/
--rw-r--r--   0 rob        (501) staff       (20)    12192 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
--rw-r--r--   0 rob        (501) staff       (20)     1464 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
--rw-r--r--   0 rob        (501) staff       (20)      904 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.857016 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/openssl-1.1.1q/
--rw-r--r--   0 rob        (501) staff       (20)      264 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.439551 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.8/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.857266 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.8/Python-3.7.8/
--rw-r--r--   0 rob        (501) staff       (20)     2846 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.8/Python-3.7.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.439753 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.9/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.857498 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.9/Python-3.7.9/
--rw-r--r--   0 rob        (501) staff       (20)     2846 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.9/Python-3.7.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.439973 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.10/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.857732 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.10/Python-3.8.10/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.10/Python-3.8.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.440170 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.11/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.857961 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.11/Python-3.8.11/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.11/Python-3.8.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.440349 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.12/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.859144 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.12/Python-3.8.12/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.12/Python-3.8.12/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.440535 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.15/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.859511 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.15/openssl-1.1.1q/
--rw-r--r--   0 rob        (501) staff       (20)      264 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.440970 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.16/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.859816 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.16/openssl-1.1.1q/
--rw-r--r--   0 rob        (501) staff       (20)      264 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.441179 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.860180 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.4/Python-3.8.4/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.4/Python-3.8.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.441372 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.860491 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.5/Python-3.8.5/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.5/Python-3.8.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.441539 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.860826 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.6/Python-3.8.6/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.6/Python-3.8.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.441715 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.7/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.861120 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.7/Python-3.8.7/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.7/Python-3.8.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.441896 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.8/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.861827 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.8/Python-3.8.8/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.8/Python-3.8.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.442259 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.9/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.862112 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.9/Python-3.8.9/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.9/Python-3.8.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.442572 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.0/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.862408 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.0/Python-3.9.0/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.0/Python-3.9.0/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.442778 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.1/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.862689 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.1/Python-3.9.1/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.1/Python-3.9.1/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.442977 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.15/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.862971 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.15/openssl-1.1.1q/
--rw-r--r--   0 rob        (501) staff       (20)      264 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.443187 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.16/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.863204 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.16/openssl-1.1.1q/
--rw-r--r--   0 rob        (501) staff       (20)      264 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.443387 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.863500 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.2/Python-3.9.2/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.2/Python-3.9.2/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.443581 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.4/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.863737 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.4/Python-3.9.4/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.4/Python-3.9.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.443775 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.863999 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.5/Python-3.9.5/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.5/Python-3.9.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.443967 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.6/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.864348 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.6/Python-3.9.6/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.6/Python-3.9.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.444154 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.7/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.864625 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.7/Python-3.9.7/
--rw-r--r--   0 rob        (501) staff       (20)     2836 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.7/Python-3.9.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.444355 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.2/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.865164 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3489 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/010_ssl_no_ssl3.patch
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.444532 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.5/
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.865660 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/
--rw-r--r--   0 rob        (501) staff       (20)     2045 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/002_readline63.patch
--rw-r--r--   0 rob        (501) staff       (20)     3445 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/010_ssl_no_ssl3.patch
--rw-r--r--   0 rob        (501) staff       (20)      372 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.5-src
--rw-r--r--   0 rob        (501) staff       (20)     1052 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.6
--rw-r--r--   0 rob        (501) staff       (20)     1102 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.7
--rw-r--r--   0 rob        (501) staff       (20)     1102 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.8
--rw-r--r--   0 rob        (501) staff       (20)     1102 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.9
--rw-r--r--   0 rob        (501) staff       (20)     1710 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0
--rw-r--r--   0 rob        (501) staff       (20)      410 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0-src
--rw-r--r--   0 rob        (501) staff       (20)     1200 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0.1-src
--rw-r--r--   0 rob        (501) staff       (20)     1200 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0.2
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0.2-src
--rw-r--r--   0 rob        (501) staff       (20)     1974 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.1
--rw-r--r--   0 rob        (501) staff       (20)      410 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2052 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.2
--rw-r--r--   0 rob        (501) staff       (20)      410 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.2-src
--rw-r--r--   0 rob        (501) staff       (20)     2082 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.2.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.2.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2052 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.3
--rw-r--r--   0 rob        (501) staff       (20)      420 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.3-src
--rw-r--r--   0 rob        (501) staff       (20)     2738 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.3.1
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.3.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2730 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.4.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.4.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2790 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.5.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.5.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2798 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.5.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.5.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2790 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.6.0
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.6.0-src
--rw-r--r--   0 rob        (501) staff       (20)     3017 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.6.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.6.1-src
--rw-r--r--   0 rob        (501) staff       (20)     3296 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-4.0.0
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-4.0.0-src
--rw-r--r--   0 rob        (501) staff       (20)     3174 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-4.0.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-4.0.1-src
--rw-r--r--   0 rob        (501) staff       (20)     3290 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.0.0
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.0.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2798 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.0.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.0.1-src
--rw-r--r--   0 rob        (501) staff       (20)     3356 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2858 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.1.1
--rw-r--r--   0 rob        (501) staff       (20)      414 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.1.1-src
--rw-r--r--   0 rob        (501) staff       (20)       37 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.3
--rw-r--r--   0 rob        (501) staff       (20)       41 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.3-src
--rw-r--r--   0 rob        (501) staff       (20)       39 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.3.1
--rw-r--r--   0 rob        (501) staff       (20)       43 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.3.1-src
--rw-r--r--   0 rob        (501) staff       (20)       37 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.4
--rw-r--r--   0 rob        (501) staff       (20)       41 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.4-src
--rw-r--r--   0 rob        (501) staff       (20)       39 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.4.1
--rw-r--r--   0 rob        (501) staff       (20)       43 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.4.1-src
--rw-r--r--   0 rob        (501) staff       (20)       39 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.6.0
--rw-r--r--   0 rob        (501) staff       (20)       43 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.6.0-src
--rw-r--r--   0 rob        (501) staff       (20)       39 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.7.0
--rw-r--r--   0 rob        (501) staff       (20)       43 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.7.0-src
--rw-r--r--   0 rob        (501) staff       (20)       39 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.7.1
--rw-r--r--   0 rob        (501) staff       (20)       43 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.7.1-src
--rw-r--r--   0 rob        (501) staff       (20)     1681 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-c-jit-latest
--rw-r--r--   0 rob        (501) staff       (20)      327 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-dev
--rw-r--r--   0 rob        (501) staff       (20)      552 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-stm-2.3
--rw-r--r--   0 rob        (501) staff       (20)      556 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-stm-2.5.1
--rw-r--r--   0 rob        (501) staff       (20)     2760 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.3
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.3-src
--rw-r--r--   0 rob        (501) staff       (20)     2889 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.3.1
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.3.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2879 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.4
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.4-src
--rw-r--r--   0 rob        (501) staff       (20)     2891 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.4.1
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.4.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2883 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.6.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.6.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2586 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.7.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.7.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2590 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.7.1
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.7.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2474 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.10.0
--rw-r--r--   0 rob        (501) staff       (20)      420 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.10.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2470 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.8.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.8.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2468 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.9.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.9.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2817 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-6.0.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-6.0.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2193 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.0.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.0.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2193 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.1.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.1.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2193 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.1.1
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.1.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2160 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.2.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.2.0-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.0-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.1
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2285 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.10
--rw-r--r--   0 rob        (501) staff       (20)      603 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.10-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.2
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.2-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.3
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.3-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.4
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.4-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.5
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.5-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.6
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.6-src
--rw-r--r--   0 rob        (501) staff       (20)     2512 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.8
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.8-src
--rw-r--r--   0 rob        (501) staff       (20)     2357 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.9
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.9-src
--rw-r--r--   0 rob        (501) staff       (20)     2756 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3-2.3.1
--rw-r--r--   0 rob        (501) staff       (20)      416 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3-2.3.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2808 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3-2.4.0
--rw-r--r--   0 rob        (501) staff       (20)      416 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3-2.4.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2770 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1
--rw-r--r--   0 rob        (501) staff       (20)      436 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1-src
--rw-r--r--   0 rob        (501) staff       (20)     2740 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.3-5.5-alpha
--rw-r--r--   0 rob        (501) staff       (20)      426 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.3-5.5-alpha-src
--rw-r--r--   0 rob        (501) staff       (20)     2737 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.10.0
--rw-r--r--   0 rob        (501) staff       (20)      420 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.10.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2988 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.10.1
--rw-r--r--   0 rob        (501) staff       (20)      420 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.10.1-src
--rw-r--r--   0 rob        (501) staff       (20)      950 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.7-beta
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.7-beta-src
--rw-r--r--   0 rob        (501) staff       (20)      954 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.7.1-beta
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.7.1-beta-src
--rw-r--r--   0 rob        (501) staff       (20)      889 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.8.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.8.0-src
--rw-r--r--   0 rob        (501) staff       (20)      887 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.9.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.9.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2768 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-6.0.0
--rw-r--r--   0 rob        (501) staff       (20)      418 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-6.0.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2199 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-7.0.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-7.0.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2183 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-c-jit-latest
--rw-r--r--   0 rob        (501) staff       (20)     1909 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.0.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.0.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2209 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.1.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.1.0-src
--rw-r--r--   0 rob        (501) staff       (20)     2209 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.1.1
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.1.1-src
--rw-r--r--   0 rob        (501) staff       (20)     2174 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.2.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.2.0-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.0
--rw-r--r--   0 rob        (501) staff       (20)      422 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.0-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.1
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.1-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.2
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.2-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.3
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.3-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.2
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.2-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.3
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.3-src
--rw-r--r--   0 rob        (501) staff       (20)     1890 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.4
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.4-src
--rw-r--r--   0 rob        (501) staff       (20)     1891 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.5
--rw-r--r--   0 rob        (501) staff       (20)      412 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.5-src
--rw-r--r--   0 rob        (501) staff       (20)     2175 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.6
--rw-r--r--   0 rob        (501) staff       (20)      473 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.6-src
--rw-r--r--   0 rob        (501) staff       (20)     2175 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.7
--rw-r--r--   0 rob        (501) staff       (20)      511 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.7-src
--rw-r--r--   0 rob        (501) staff       (20)     2512 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.8
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.8-src
--rw-r--r--   0 rob        (501) staff       (20)     2357 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.9
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.9-src
--rw-r--r--   0 rob        (501) staff       (20)     1734 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-c-jit-latest
--rw-r--r--   0 rob        (501) staff       (20)     2285 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.10
--rw-r--r--   0 rob        (501) staff       (20)      603 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.10-src
--rw-r--r--   0 rob        (501) staff       (20)     2171 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.6
--rw-r--r--   0 rob        (501) staff       (20)      511 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.6-src
--rw-r--r--   0 rob        (501) staff       (20)     2171 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.7
--rw-r--r--   0 rob        (501) staff       (20)      511 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.7-src
--rw-r--r--   0 rob        (501) staff       (20)     2512 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.8
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.8-src
--rw-r--r--   0 rob        (501) staff       (20)     2357 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.9
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.9-src
--rw-r--r--   0 rob        (501) staff       (20)     2285 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.10
--rw-r--r--   0 rob        (501) staff       (20)      603 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.10-src
--rw-r--r--   0 rob        (501) staff       (20)     2512 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.8
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.8-src
--rw-r--r--   0 rob        (501) staff       (20)     2357 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.9
--rw-r--r--   0 rob        (501) staff       (20)      602 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.9-src
--rw-r--r--   0 rob        (501) staff       (20)      638 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.2
--rw-r--r--   0 rob        (501) staff       (20)      635 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3
--rw-r--r--   0 rob        (501) staff       (20)      646 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.1
--rw-r--r--   0 rob        (501) staff       (20)      643 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.2
--rw-r--r--   0 rob        (501) staff       (20)      751 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.3
--rw-r--r--   0 rob        (501) staff       (20)      843 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.4
--rw-r--r--   0 rob        (501) staff       (20)      843 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.5
--rw-r--r--   0 rob        (501) staff       (20)      534 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7-dev
--rw-r--r--   0 rob        (501) staff       (20)      582 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.10
--rw-r--r--   0 rob        (501) staff       (20)      582 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.11
--rw-r--r--   0 rob        (501) staff       (20)      582 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.12
--rw-r--r--   0 rob        (501) staff       (20)      622 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.14
--rw-r--r--   0 rob        (501) staff       (20)      604 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.16
--rw-r--r--   0 rob        (501) staff       (20)      598 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.2
--rw-r--r--   0 rob        (501) staff       (20)      598 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.3
--rw-r--r--   0 rob        (501) staff       (20)      598 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.4
--rw-r--r--   0 rob        (501) staff       (20)      598 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.5
--rw-r--r--   0 rob        (501) staff       (20)      598 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.6
--rw-r--r--   0 rob        (501) staff       (20)      582 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.7
--rw-r--r--   0 rob        (501) staff       (20)      582 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.8
--rw-r--r--   0 rob        (501) staff       (20)      581 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.9
--rw-r--r--   0 rob        (501) staff       (20)      941 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.2.2
--rw-r--r--   0 rob        (501) staff       (20)      941 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.2.5
--rw-r--r--   0 rob        (501) staff       (20)      581 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.3.5
--rw-r--r--   0 rob        (501) staff       (20)      603 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.3.7
--rw-r--r--   0 rob        (501) staff       (20)      534 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.4-dev
--rw-r--r--   0 rob        (501) staff       (20)      613 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.4.2
--rw-r--r--   0 rob        (501) staff       (20)      603 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.4.7
--rw-r--r--   0 rob        (501) staff       (20)      603 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.5.4
--rw-r--r--   0 rob        (501) staff       (20)      603 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.7.5
--rw-r--r--   0 rob        (501) staff       (20)      533 2022-12-18 04:24:58.000000 autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-dev
--rw-r--r--   0 rob        (501) staff       (20)     1429 2021-04-23 03:34:41.000000 autovenv-0.3.1671337560/autovenv/util.py
--rw-r--r--   0 rob        (501) staff       (20)    14293 2021-09-13 09:59:55.000000 autovenv-0.3.1671337560/autovenv/virtualenvs.py
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.449274 autovenv-0.3.1671337560/autovenv.egg-info/
--rw-r--r--   0 rob        (501) staff       (20)      538 2022-12-18 04:41:42.000000 autovenv-0.3.1671337560/autovenv.egg-info/PKG-INFO
--rw-r--r--   0 rob        (501) staff       (20)    58363 2022-12-18 04:41:42.000000 autovenv-0.3.1671337560/autovenv.egg-info/SOURCES.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2022-12-18 04:41:42.000000 autovenv-0.3.1671337560/autovenv.egg-info/dependency_links.txt
--rw-r--r--   0 rob        (501) staff       (20)       49 2022-12-18 04:41:42.000000 autovenv-0.3.1671337560/autovenv.egg-info/entry_points.txt
--rw-r--r--   0 rob        (501) staff       (20)       26 2022-12-18 04:41:42.000000 autovenv-0.3.1671337560/autovenv.egg-info/requires.txt
--rw-r--r--   0 rob        (501) staff       (20)       15 2022-12-18 04:41:42.000000 autovenv-0.3.1671337560/autovenv.egg-info/top_level.txt
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.867138 autovenv-0.3.1671337560/scripts/
--rwxr--r--   0 rob        (501) staff       (20)      713 2019-10-17 05:35:46.000000 autovenv-0.3.1671337560/scripts/autovenv-build
--rw-r--r--   0 rob        (501) staff       (20)      107 2016-01-02 23:46:00.000000 autovenv-0.3.1671337560/scripts/autovenv-pythons-available
--rw-r--r--   0 rob        (501) staff       (20)      118 2016-01-02 09:43:39.000000 autovenv-0.3.1671337560/scripts/autovenv.sh
--rw-r--r--   0 rob        (501) staff       (20)       38 2022-12-18 04:41:42.868860 autovenv-0.3.1671337560/setup.cfg
--rw-r--r--   0 rob        (501) staff       (20)     1103 2022-12-18 04:26:15.000000 autovenv-0.3.1671337560/setup.py
-drwxr-xr-x   0 rob        (501) staff       (20)        0 2022-12-18 04:41:42.867869 autovenv-0.3.1671337560/tests/
--rw-r--r--   0 rob        (501) staff       (20)        0 2017-01-22 00:01:00.000000 autovenv-0.3.1671337560/tests/__init__.py
--rwxr--r--   0 rob        (501) staff       (20)     3390 2021-04-23 03:26:00.000000 autovenv-0.3.1671337560/tests/test_autovenv.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.864315 autovenv-0.3.1671337561/
+-rw-r--r--   0 rob        (501) staff       (20)     1210 2016-01-01 06:14:00.000000 autovenv-0.3.1671337561/LICENSE
+-rw-r--r--   0 rob        (501) staff       (20)       42 2016-01-03 06:39:26.000000 autovenv-0.3.1671337561/MANIFEST.in
+-rw-r--r--   0 rob        (501) staff       (20)      609 2024-04-01 12:08:33.863762 autovenv-0.3.1671337561/PKG-INFO
+-rwxr--r--   0 rob        (501) staff       (20)     2234 2017-03-29 11:57:30.000000 autovenv-0.3.1671337561/README.rst
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.370644 autovenv-0.3.1671337561/autovenv/
+-rwxr--r--   0 rob        (501) staff       (20)      492 2018-07-16 12:34:06.000000 autovenv-0.3.1671337561/autovenv/__init__.py
+-rw-r--r--   0 rob        (501) staff       (20)     2609 2019-10-17 22:55:47.000000 autovenv-0.3.1671337561/autovenv/command.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.372979 autovenv-0.3.1671337561/autovenv/python-build/
+-rw-r--r--   0 rob        (501) staff       (20)     1097 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/LICENSE
+-rwxr-xr-x   0 rob        (501) staff       (20)    72260 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/autovenv-python-build
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.338853 autovenv-0.3.1671337561/autovenv/python-build/share/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.740418 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/
+-rw-r--r--   0 rob        (501) staff       (20)      732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.1.3
+-rw-r--r--   0 rob        (501) staff       (20)      732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.2.3
+-rw-r--r--   0 rob        (501) staff       (20)      732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.3.7
+-rw-r--r--   0 rob        (501) staff       (20)      724 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      730 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.1
+-rw-r--r--   0 rob        (501) staff       (20)      730 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.2
+-rw-r--r--   0 rob        (501) staff       (20)      730 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.3
+-rw-r--r--   0 rob        (501) staff       (20)      730 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.4
+-rw-r--r--   0 rob        (501) staff       (20)      730 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.5
+-rw-r--r--   0 rob        (501) staff       (20)      730 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.6
+-rw-r--r--   0 rob        (501) staff       (20)      716 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.0
+-rw-r--r--   0 rob        (501) staff       (20)      722 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.1
+-rw-r--r--   0 rob        (501) staff       (20)      722 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.2
+-rw-r--r--   0 rob        (501) staff       (20)      722 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.3
+-rw-r--r--   0 rob        (501) staff       (20)      722 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.4
+-rw-r--r--   0 rob        (501) staff       (20)      722 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.5
+-rw-r--r--   0 rob        (501) staff       (20)      722 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.6
+-rw-r--r--   0 rob        (501) staff       (20)      578 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.0
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.1
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.2
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.3
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.4
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.5
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.6
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.7
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.8
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.9
+-rw-r--r--   0 rob        (501) staff       (20)      533 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7-dev
+-rw-r--r--   0 rob        (501) staff       (20)      594 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.0
+-rw-r--r--   0 rob        (501) staff       (20)      600 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.1
+-rw-r--r--   0 rob        (501) staff       (20)      851 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.10
+-rw-r--r--   0 rob        (501) staff       (20)      851 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.11
+-rw-r--r--   0 rob        (501) staff       (20)      851 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.12
+-rw-r--r--   0 rob        (501) staff       (20)      851 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.13
+-rw-r--r--   0 rob        (501) staff       (20)      868 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.14
+-rw-r--r--   0 rob        (501) staff       (20)      868 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.15
+-rw-r--r--   0 rob        (501) staff       (20)      851 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.16
+-rw-r--r--   0 rob        (501) staff       (20)      851 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.17
+-rw-r--r--   0 rob        (501) staff       (20)      865 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.18
+-rw-r--r--   0 rob        (501) staff       (20)      600 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.2
+-rw-r--r--   0 rob        (501) staff       (20)      600 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.3
+-rw-r--r--   0 rob        (501) staff       (20)      600 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.4
+-rw-r--r--   0 rob        (501) staff       (20)      600 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.5
+-rw-r--r--   0 rob        (501) staff       (20)      600 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.6
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.7
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.8
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.9
+-rw-r--r--   0 rob        (501) staff       (20)     1228 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      921 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.1
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.2
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.3
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.4
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.5
+-rw-r--r--   0 rob        (501) staff       (20)      569 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10-dev
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.1
+-rw-r--r--   0 rob        (501) staff       (20)      915 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.10
+-rw-r--r--   0 rob        (501) staff       (20)      915 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.11
+-rw-r--r--   0 rob        (501) staff       (20)      915 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.12
+-rw-r--r--   0 rob        (501) staff       (20)      915 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.13
+-rw-r--r--   0 rob        (501) staff       (20)      915 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.14
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.2
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.3
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.4
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.5
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.6
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.7
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.8
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.9
+-rw-r--r--   0 rob        (501) staff       (20)      611 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11-dev
+-rw-r--r--   0 rob        (501) staff       (20)      951 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.0
+-rw-r--r--   0 rob        (501) staff       (20)      951 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.1
+-rw-r--r--   0 rob        (501) staff       (20)      951 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.2
+-rw-r--r--   0 rob        (501) staff       (20)      951 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.3
+-rw-r--r--   0 rob        (501) staff       (20)      951 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.4
+-rw-r--r--   0 rob        (501) staff       (20)      948 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.5
+-rw-r--r--   0 rob        (501) staff       (20)      948 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.6
+-rw-r--r--   0 rob        (501) staff       (20)      948 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.7
+-rw-r--r--   0 rob        (501) staff       (20)      948 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.8
+-rw-r--r--   0 rob        (501) staff       (20)      654 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.12-dev
+-rw-r--r--   0 rob        (501) staff       (20)      906 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.12.0
+-rw-r--r--   0 rob        (501) staff       (20)      906 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.12.1
+-rw-r--r--   0 rob        (501) staff       (20)      906 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.12.2
+-rw-r--r--   0 rob        (501) staff       (20)      654 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.13-dev
+-rw-r--r--   0 rob        (501) staff       (20)      914 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.13.0a5
+-rw-r--r--   0 rob        (501) staff       (20)      921 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.1
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.2
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.3
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.4
+-rw-r--r--   0 rob        (501) staff       (20)      927 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.5
+-rw-r--r--   0 rob        (501) staff       (20)     1146 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.6
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.2
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.3
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.4
+-rw-r--r--   0 rob        (501) staff       (20)      584 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.5
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.6
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.7
+-rw-r--r--   0 rob        (501) staff       (20)      517 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4-dev
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.1
+-rw-r--r--   0 rob        (501) staff       (20)      764 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.10
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.2
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.3
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.4
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.5
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.6
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.7
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.8
+-rw-r--r--   0 rob        (501) staff       (20)      813 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.9
+-rw-r--r--   0 rob        (501) staff       (20)      533 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5-dev
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.0
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.1
+-rw-r--r--   0 rob        (501) staff       (20)      836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.10
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.2
+-rw-r--r--   0 rob        (501) staff       (20)      862 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.3
+-rw-r--r--   0 rob        (501) staff       (20)      862 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.4
+-rw-r--r--   0 rob        (501) staff       (20)      862 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.5
+-rw-r--r--   0 rob        (501) staff       (20)      862 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.6
+-rw-r--r--   0 rob        (501) staff       (20)      830 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.7
+-rw-r--r--   0 rob        (501) staff       (20)      830 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.8
+-rw-r--r--   0 rob        (501) staff       (20)      830 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.9
+-rw-r--r--   0 rob        (501) staff       (20)      533 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6-dev
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.0
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.1
+-rw-r--r--   0 rob        (501) staff       (20)      868 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.10
+-rw-r--r--   0 rob        (501) staff       (20)      868 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.11
+-rw-r--r--   0 rob        (501) staff       (20)      868 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.12
+-rw-r--r--   0 rob        (501) staff       (20)      868 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.13
+-rw-r--r--   0 rob        (501) staff       (20)      858 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.14
+-rw-r--r--   0 rob        (501) staff       (20)      858 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.15
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.2
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.3
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.4
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.5
+-rw-r--r--   0 rob        (501) staff       (20)      845 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.6
+-rw-r--r--   0 rob        (501) staff       (20)      862 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.7
+-rw-r--r--   0 rob        (501) staff       (20)      862 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.8
+-rw-r--r--   0 rob        (501) staff       (20)      862 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.9
+-rw-r--r--   0 rob        (501) staff       (20)      568 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7-dev
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.0
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.1
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.10
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.11
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.12
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.13
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.14
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.15
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.16
+-rw-r--r--   0 rob        (501) staff       (20)      903 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.17
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.2
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.3
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.4
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.5
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.6
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.7
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.8
+-rw-r--r--   0 rob        (501) staff       (20)      897 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.9
+-rw-r--r--   0 rob        (501) staff       (20)      568 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8-dev
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.0
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.1
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.10
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.11
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.12
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.13
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.14
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.15
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.16
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.17
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.18
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.19
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.2
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.3
+-rw-r--r--   0 rob        (501) staff       (20)      897 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.4
+-rw-r--r--   0 rob        (501) staff       (20)      897 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.5
+-rw-r--r--   0 rob        (501) staff       (20)      897 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.6
+-rw-r--r--   0 rob        (501) staff       (20)      897 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.7
+-rw-r--r--   0 rob        (501) staff       (20)      907 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.8
+-rw-r--r--   0 rob        (501) staff       (20)      897 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.9
+-rw-r--r--   0 rob        (501) staff       (20)      566 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9-dev
+-rw-r--r--   0 rob        (501) staff       (20)      902 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.0
+-rw-r--r--   0 rob        (501) staff       (20)      902 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.1
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.10
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.11
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.12
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.13
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.14
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.15
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.16
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.17
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.18
+-rw-r--r--   0 rob        (501) staff       (20)     1086 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.19
+-rw-r--r--   0 rob        (501) staff       (20)      912 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.2
+-rw-r--r--   0 rob        (501) staff       (20)      901 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.4
+-rw-r--r--   0 rob        (501) staff       (20)     1084 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.5
+-rw-r--r--   0 rob        (501) staff       (20)     1080 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.6
+-rw-r--r--   0 rob        (501) staff       (20)     1080 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.7
+-rw-r--r--   0 rob        (501) staff       (20)     1080 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.8
+-rw-r--r--   0 rob        (501) staff       (20)     1080 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.9
+-rw-r--r--   0 rob        (501) staff       (20)      666 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/activepython-2.7.14
+-rw-r--r--   0 rob        (501) staff       (20)      662 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/activepython-3.5.4
+-rw-r--r--   0 rob        (501) staff       (20)      976 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/activepython-3.6.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.5.0
+-rw-r--r--   0 rob        (501) staff       (20)      470 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.5.1
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.6.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.6.1
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.7.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.8.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.9.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.9.1
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.9.2
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.3.0
+-rw-r--r--   0 rob        (501) staff       (20)       43 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.4.0
+-rw-r--r--   0 rob        (501) staff       (20)       43 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-4.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2.4.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2.5.0
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2018.12
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2019.03
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2019.07
+-rw-r--r--   0 rob        (501) staff       (20)      843 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2019.10
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.1.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      924 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.4.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.5.0
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2018.12
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2019.03
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2019.07
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2019.10
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2020.02
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2020.07
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2020.11
+-rw-r--r--   0 rob        (501) staff       (20)     1239 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2021.04
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2021.05
+-rw-r--r--   0 rob        (501) staff       (20)      940 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2021.11
+-rw-r--r--   0 rob        (501) staff       (20)     1437 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2022.05
+-rw-r--r--   0 rob        (501) staff       (20)     1437 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2022.10
+-rw-r--r--   0 rob        (501) staff       (20)     1635 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2023.03
+-rw-r--r--   0 rob        (501) staff       (20)     1653 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2023.03-0
+-rw-r--r--   0 rob        (501) staff       (20)     1653 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2023.03-1
+-rw-r--r--   0 rob        (501) staff       (20)     1653 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2023.07-0
+-rw-r--r--   0 rob        (501) staff       (20)     1659 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2023.07-1
+-rw-r--r--   0 rob        (501) staff       (20)     1659 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2023.07-2
+-rw-r--r--   0 rob        (501) staff       (20)     1659 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2023.09-0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.1.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      924 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      916 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.3.1
+-rw-r--r--   0 rob        (501) staff       (20)     1495 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/cinder-3.10-dev
+-rw-r--r--   0 rob        (501) staff       (20)     1492 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/cinder-3.8-dev
+-rw-r--r--   0 rob        (501) staff       (20)     2144 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-22.3.0
+-rw-r--r--   0 rob        (501) staff       (20)     2151 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-23.0.0
+-rw-r--r--   0 rob        (501) staff       (20)     2588 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-23.1.0
+-rw-r--r--   0 rob        (501) staff       (20)     2589 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-23.1.2
+-rw-r--r--   0 rob        (501) staff       (20)     2593 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-24.0.0
+-rw-r--r--   0 rob        (501) staff       (20)     2198 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-community-23.1.0
+-rw-r--r--   0 rob        (501) staff       (20)     2198 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-community-23.1.2
+-rw-r--r--   0 rob        (501) staff       (20)     2198 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-community-24.0.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-20.1.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-20.2.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-20.3.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.0.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.1.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.2.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.3.0
+-rw-r--r--   0 rob        (501) staff       (20)     2012 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-22.0.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-22.1.0
+-rw-r--r--   0 rob        (501) staff       (20)     2010 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-22.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      266 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/ironpython-2.7.4
+-rw-r--r--   0 rob        (501) staff       (20)      266 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/ironpython-2.7.5
+-rw-r--r--   0 rob        (501) staff       (20)      272 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/ironpython-2.7.6.3
+-rw-r--r--   0 rob        (501) staff       (20)      211 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/ironpython-2.7.7
+-rw-r--r--   0 rob        (501) staff       (20)      176 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/ironpython-dev
+-rw-r--r--   0 rob        (501) staff       (20)      561 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5-dev
+-rw-r--r--   0 rob        (501) staff       (20)      870 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.0
+-rw-r--r--   0 rob        (501) staff       (20)      870 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.1
+-rw-r--r--   0 rob        (501) staff       (20)      671 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.2
+-rw-r--r--   0 rob        (501) staff       (20)      691 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.3
+-rw-r--r--   0 rob        (501) staff       (20)      703 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.4-rc1
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.7.0
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.7.1
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.7.2
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.7.3
+-rw-r--r--   0 rob        (501) staff       (20)      403 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-dev
+-rw-r--r--   0 rob        (501) staff       (20)     1205 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge
+-rw-r--r--   0 rob        (501) staff       (20)     1634 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-22.11.1-3
+-rw-r--r--   0 rob        (501) staff       (20)     1634 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-22.11.1-4
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-22.9.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-22.9.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-22.9.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-22.9.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.1.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.1.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.1.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.1.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.1.0-4
+-rw-r--r--   0 rob        (501) staff       (20)     1634 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.10.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1634 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.11.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.3.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.3.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-23.3.1-1
+-rw-r--r--   0 rob        (501) staff       (20)     1326 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.1-4
+-rw-r--r--   0 rob        (501) staff       (20)     1326 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.1-5
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.2-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-1
+-rw-r--r--   0 rob        (501) staff       (20)     1338 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-10
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-2
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-3
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-4
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-5
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-6
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-7
+-rw-r--r--   0 rob        (501) staff       (20)      794 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-8
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-9
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.11.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.11.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.11.0-2
+-rw-r--r--   0 rob        (501) staff       (20)      794 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.11.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.11.0-4
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.12.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.12.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.12.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.12.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.13.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.14.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.14.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1619 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.14.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1073 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-pypy3
+-rw-r--r--   0 rob        (501) staff       (20)      383 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.10
+-rw-r--r--   0 rob        (501) staff       (20)      383 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.11
+-rw-r--r--   0 rob        (501) staff       (20)      383 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.12
+-rw-r--r--   0 rob        (501) staff       (20)      383 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.13
+-rw-r--r--   0 rob        (501) staff       (20)      403 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.14
+-rw-r--r--   0 rob        (501) staff       (20)      403 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.15
+-rw-r--r--   0 rob        (501) staff       (20)      403 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.16
+-rw-r--r--   0 rob        (501) staff       (20)      403 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.17
+-rw-r--r--   0 rob        (501) staff       (20)      403 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.18
+-rw-r--r--   0 rob        (501) staff       (20)      409 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.19.1
+-rw-r--r--   0 rob        (501) staff       (20)      409 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.20.0
+-rw-r--r--   0 rob        (501) staff       (20)      408 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.21.0
+-rw-r--r--   0 rob        (501) staff       (20)      391 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.9.3
+-rw-r--r--   0 rob        (501) staff       (20)      391 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-1.9.4
+-rw-r--r--   0 rob        (501) staff       (20)       90 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/micropython-dev
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-2.2.2
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.0.4
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.0.5
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.10.1
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.16.0
+-rw-r--r--   0 rob        (501) staff       (20)       45 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.18.3
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.4.2
+-rw-r--r--   0 rob        (501) staff       (20)      919 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.7.0
+-rw-r--r--   0 rob        (501) staff       (20)      919 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.8.3
+-rw-r--r--   0 rob        (501) staff       (20)      925 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.9.1
+-rw-r--r--   0 rob        (501) staff       (20)       45 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-latest
+-rw-r--r--   0 rob        (501) staff       (20)      877 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-2.7-4.8.3
+-rw-r--r--   0 rob        (501) staff       (20)      938 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-3.18.3
+-rw-r--r--   0 rob        (501) staff       (20)      938 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-3.19.0
+-rw-r--r--   0 rob        (501) staff       (20)      932 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.0.5
+-rw-r--r--   0 rob        (501) staff       (20)      938 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.1.11
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.14
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.21
+-rw-r--r--   0 rob        (501) staff       (20)      945 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.27
+-rw-r--r--   0 rob        (501) staff       (20)      941 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.30
+-rw-r--r--   0 rob        (501) staff       (20)      841 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.31
+-rw-r--r--   0 rob        (501) staff       (20)     1045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.4.10
+-rw-r--r--   0 rob        (501) staff       (20)     1037 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.1
+-rw-r--r--   0 rob        (501) staff       (20)     1045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.11
+-rw-r--r--   0 rob        (501) staff       (20)     1045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.12
+-rw-r--r--   0 rob        (501) staff       (20)     1037 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.4
+-rw-r--r--   0 rob        (501) staff       (20)      853 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.6.14
+-rw-r--r--   0 rob        (501) staff       (20)      853 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.7.10
+-rw-r--r--   0 rob        (501) staff       (20)     1474 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.7.12
+-rw-r--r--   0 rob        (501) staff       (20)      743 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-latest
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-2.2.2
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.0.4
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.0.5
+-rw-r--r--   0 rob        (501) staff       (20)     1762 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-22.11.1-1
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.1.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1780 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.10.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1522 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.11.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1522 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.11.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.3.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.5.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.5.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.5.2-0
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-23.9.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1497 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10-24.1.2-0
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10.1
+-rw-r--r--   0 rob        (501) staff       (20)     1780 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-23.10.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1522 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-23.11.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1522 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-23.11.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-23.5.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-23.5.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-23.5.2-0
+-rw-r--r--   0 rob        (501) staff       (20)     1750 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-23.9.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1497 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.11-24.1.2-0
+-rw-r--r--   0 rob        (501) staff       (20)     1497 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.12-24.1.2-0
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.16.0
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.18.3
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.19.0
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.4.2
+-rw-r--r--   0 rob        (501) staff       (20)     1495 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-22.11.1-1
+-rw-r--r--   0 rob        (501) staff       (20)     1485 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-23.1.0-1
+-rw-r--r--   0 rob        (501) staff       (20)      666 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.1
+-rw-r--r--   0 rob        (501) staff       (20)     1305 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.3
+-rw-r--r--   0 rob        (501) staff       (20)     1305 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.11.0
+-rw-r--r--   0 rob        (501) staff       (20)     1305 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.12.0
+-rw-r--r--   0 rob        (501) staff       (20)      877 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.2
+-rw-r--r--   0 rob        (501) staff       (20)      877 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.3
+-rw-r--r--   0 rob        (501) staff       (20)     1295 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.9.2
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7.0
+-rw-r--r--   0 rob        (501) staff       (20)     1744 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-22.11.1-1
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.1.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1762 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.10.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1507 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.11.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1507 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.11.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.3.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.5.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.5.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.5.2-0
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-23.9.0-0
+-rw-r--r--   0 rob        (501) staff       (20)      877 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.1
+-rw-r--r--   0 rob        (501) staff       (20)     1305 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.3
+-rw-r--r--   0 rob        (501) staff       (20)     1516 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.11.0
+-rw-r--r--   0 rob        (501) staff       (20)     1516 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.12.0
+-rw-r--r--   0 rob        (501) staff       (20)      877 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.2
+-rw-r--r--   0 rob        (501) staff       (20)      877 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.3
+-rw-r--r--   0 rob        (501) staff       (20)     1295 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.9.2
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8.3
+-rw-r--r--   0 rob        (501) staff       (20)     1744 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-22.11.1-1
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.1.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1762 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.10.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1507 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.11.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1507 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.11.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.3.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.5.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.5.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.5.2-0
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-23.9.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1487 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-24.1.2-0
+-rw-r--r--   0 rob        (501) staff       (20)      666 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.1
+-rw-r--r--   0 rob        (501) staff       (20)     1305 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.3
+-rw-r--r--   0 rob        (501) staff       (20)     1516 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.11.0
+-rw-r--r--   0 rob        (501) staff       (20)     1516 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.12.0
+-rw-r--r--   0 rob        (501) staff       (20)     1295 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.9.2
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9.1
+-rw-r--r--   0 rob        (501) staff       (20)      931 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.0.5
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.1.11
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.2.12
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.11
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.14
+-rw-r--r--   0 rob        (501) staff       (20)      937 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.21
+-rw-r--r--   0 rob        (501) staff       (20)      945 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.27
+-rw-r--r--   0 rob        (501) staff       (20)      941 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.30
+-rw-r--r--   0 rob        (501) staff       (20)      841 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.31
+-rw-r--r--   0 rob        (501) staff       (20)     1045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.4.10
+-rw-r--r--   0 rob        (501) staff       (20)     1037 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.1
+-rw-r--r--   0 rob        (501) staff       (20)     1045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.11
+-rw-r--r--   0 rob        (501) staff       (20)      841 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.12
+-rw-r--r--   0 rob        (501) staff       (20)     1037 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.4
+-rw-r--r--   0 rob        (501) staff       (20)      853 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.6.14
+-rw-r--r--   0 rob        (501) staff       (20)      853 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.7.10
+-rw-r--r--   0 rob        (501) staff       (20)     1474 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.7.12
+-rw-r--r--   0 rob        (501) staff       (20)     1119 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-latest
+-rw-r--r--   0 rob        (501) staff       (20)     1065 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge-pypy3
+-rw-r--r--   0 rob        (501) staff       (20)     1633 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-22.11.1-3
+-rw-r--r--   0 rob        (501) staff       (20)     1633 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-22.11.1-4
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-22.9.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-22.9.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-22.9.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-22.9.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.1.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.1.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.1.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.1.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.1.0-4
+-rw-r--r--   0 rob        (501) staff       (20)     1633 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.10.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1633 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.11.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.3.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.3.1-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-23.3.1-1
+-rw-r--r--   0 rob        (501) staff       (20)     1438 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10
+-rw-r--r--   0 rob        (501) staff       (20)     1438 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.1-1
+-rw-r--r--   0 rob        (501) staff       (20)     1598 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.1-3
+-rw-r--r--   0 rob        (501) staff       (20)     1598 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.1-5
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.2-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-1
+-rw-r--r--   0 rob        (501) staff       (20)     1613 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-10
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-2
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-3
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-4
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-5
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-6
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-7
+-rw-r--r--   0 rob        (501) staff       (20)      793 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-8
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-9
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.11.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.11.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.11.0-2
+-rw-r--r--   0 rob        (501) staff       (20)      793 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.11.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.11.0-4
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.12.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.12.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.12.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.12.0-3
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.13.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.13.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.14.0-0
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.14.0-1
+-rw-r--r--   0 rob        (501) staff       (20)     1618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.14.0-2
+-rw-r--r--   0 rob        (501) staff       (20)     1423 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.9.2
+-rw-r--r--   0 rob        (501) staff       (20)     1204 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-latest
+-rw-r--r--   0 rob        (501) staff       (20)      669 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/nogil-3.9.10
+-rw-r--r--   0 rob        (501) staff       (20)      682 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/nogil-3.9.10-1
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.366790 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.339187 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.1.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.740927 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.1.3/Python-2.1.3/
+-rw-r--r--   0 rob        (501) staff       (20)     2443 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.1.3/Python-2.1.3/000_patch-setup.py.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.339411 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.2.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.741374 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.2.3/Python-2.2.3/
+-rw-r--r--   0 rob        (501) staff       (20)     2379 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.2.3/Python-2.2.3/000_patch-setup.py.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.339613 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.3.7/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.742818 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/
+-rw-r--r--   0 rob        (501) staff       (20)     1841 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1397 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/001_fortify_crash_workaround.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.339812 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.744043 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1397 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/001_fortify_crash_workaround.diff
+-rw-r--r--   0 rob        (501) staff       (20)      848 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/002_patch-posixmodule.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.340006 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.745655 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1397 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/001_fortify_crash_workaround.diff
+-rw-r--r--   0 rob        (501) staff       (20)      848 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/002_patch-posixmodule.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.340207 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.747171 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1397 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/001_fortify_crash_workaround.diff
+-rw-r--r--   0 rob        (501) staff       (20)      848 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/002_patch-posixmodule.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.340423 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.748376 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1397 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/001_fortify_crash_workaround.diff
+-rw-r--r--   0 rob        (501) staff       (20)      848 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/002_patch-posixmodule.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.340649 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.749349 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)      848 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/001_patch-posixmodule.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.340891 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.751032 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)      848 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/001_patch-posixmodule.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.341148 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.751912 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)      848 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/001_patch-posixmodule.diff
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.341358 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.756035 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1734 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5815 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/002_darwin_c_source.patch
+-rw-r--r--   0 rob        (501) staff       (20)     9060 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/003_osx_lp64.patch
+-rw-r--r--   0 rob        (501) staff       (20)   191582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/004_osx_libffi.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/005_osx_failed_modules.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.341567 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.760510 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1754 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5815 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/002_darwin_c_source.patch
+-rw-r--r--   0 rob        (501) staff       (20)     9060 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/003_osx_lp64.patch
+-rw-r--r--   0 rob        (501) staff       (20)   191582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/004_osx_libffi.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/005_osx_failed_modules.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.341769 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.764086 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1270 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5815 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/002_darwin_c_source.patch
+-rw-r--r--   0 rob        (501) staff       (20)     9060 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/003_osx_lp64.patch
+-rw-r--r--   0 rob        (501) staff       (20)   191582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/004_osx_libffi.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/005_osx_failed_modules.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.341984 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.767661 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1270 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5815 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/002_darwin_c_source.patch
+-rw-r--r--   0 rob        (501) staff       (20)     9060 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/003_osx_lp64.patch
+-rw-r--r--   0 rob        (501) staff       (20)   191582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/004_osx_libffi.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/005_osx_failed_modules.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.342178 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.772318 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1270 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5815 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/002_darwin_c_source.patch
+-rw-r--r--   0 rob        (501) staff       (20)     9060 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/003_osx_lp64.patch
+-rw-r--r--   0 rob        (501) staff       (20)   191582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/004_osx_libffi.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/005_osx_failed_modules.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.342368 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.775020 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1270 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5815 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/002_darwin_c_source.patch
+-rw-r--r--   0 rob        (501) staff       (20)     9060 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/003_osx_lp64.patch
+-rw-r--r--   0 rob        (501) staff       (20)   191582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/004_osx_libffi.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/005_osx_failed_modules.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.342557 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.777875 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/
+-rw-r--r--   0 rob        (501) staff       (20)     1873 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1270 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5815 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/002_darwin_c_source.patch
+-rw-r--r--   0 rob        (501) staff       (20)     9060 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/003_osx_lp64.patch
+-rw-r--r--   0 rob        (501) staff       (20)   191582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/004_osx_libffi.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/005_osx_failed_modules.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.342763 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.779683 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/
+-rw-r--r--   0 rob        (501) staff       (20)     2771 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1728 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      747 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3143 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.342971 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.780992 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/
+-rw-r--r--   0 rob        (501) staff       (20)     2771 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3143 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.343163 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.782667 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/
+-rw-r--r--   0 rob        (501) staff       (20)     2771 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3143 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.343359 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.784204 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/
+-rw-r--r--   0 rob        (501) staff       (20)     2771 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3143 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.343572 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.785667 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/
+-rw-r--r--   0 rob        (501) staff       (20)     2771 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1732 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3143 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.343787 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.787207 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/
+-rw-r--r--   0 rob        (501) staff       (20)     2771 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1772 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3142 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.343988 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.788521 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/
+-rw-r--r--   0 rob        (501) staff       (20)     2450 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3319 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.344187 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.789802 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/
+-rw-r--r--   0 rob        (501) staff       (20)     2450 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3319 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.344378 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.791469 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/
+-rw-r--r--   0 rob        (501) staff       (20)     2450 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3319 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.344566 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.793496 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/
+-rw-r--r--   0 rob        (501) staff       (20)     2450 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)      618 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/001_remove_systemstubs.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/003_tk86.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3156 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.345052 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.794865 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/
+-rw-r--r--   0 rob        (501) staff       (20)     1805 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3513 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.345311 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.796488 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/
+-rw-r--r--   0 rob        (501) staff       (20)     1805 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3513 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.345522 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.10/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.796831 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.10/Python-2.7.10/
+-rw-r--r--   0 rob        (501) staff       (20)      610 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.10/Python-2.7.10/003_system_library_path_in_sys_path.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.345894 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.800037 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/
+-rw-r--r--   0 rob        (501) staff       (20)      995 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0001-Detect-arm64-in-configure.patch
+-rw-r--r--   0 rob        (501) staff       (20)    10287 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0002-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch
+-rw-r--r--   0 rob        (501) staff       (20)      887 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0003-Support-arm64-in-Mac-Tools-pythonw.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3379 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0004-Use-system-libffi-for-Mac-OS-10.15-and-up.patch
+-rw-r--r--   0 rob        (501) staff       (20)     8453 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0005-ctypes-use-the-correct-ABI-for-variadic-functions.patch
+-rw-r--r--   0 rob        (501) staff       (20)     4148 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0006-ctypes-probe-libffi-for-ffi_closure_alloc-and-ffi_pr.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1493 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0007-Remove-QuickTime-from-link-args.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.346324 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.801081 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      696 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3435 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.346626 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.802024 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3443 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.346922 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.803398 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3443 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.347205 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.804382 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3443 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.347520 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.805406 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/
+-rw-r--r--   0 rob        (501) staff       (20)     1850 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3443 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/010_ssl_no_ssl3.patch
+-rw-r--r--   0 rob        (501) staff       (20)     2263 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/012_fix_bundle_loader_for_new_osx.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.347863 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.7/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.805963 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3443 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.348109 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.8/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.806506 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3443 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.348341 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.9/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.807167 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/003_system_library_path_in_sys_path.patch
+-rw-r--r--   0 rob        (501) staff       (20)      625 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.348568 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.807935 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/
+-rw-r--r--   0 rob        (501) staff       (20)     1856 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     1270 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/001_patch-svnversion.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3194 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.348800 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.808592 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/
+-rw-r--r--   0 rob        (501) staff       (20)     2333 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     3194 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.349019 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.809151 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/
+-rw-r--r--   0 rob        (501) staff       (20)     2333 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     3194 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.349255 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.809653 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/
+-rw-r--r--   0 rob        (501) staff       (20)     2333 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     3194 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.349463 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.810704 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/
+-rw-r--r--   0 rob        (501) staff       (20)     2225 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3358 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.349668 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.811394 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/
+-rw-r--r--   0 rob        (501) staff       (20)      524 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3317 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.349862 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.812075 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/
+-rw-r--r--   0 rob        (501) staff       (20)      524 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3317 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.350060 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.10.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.812740 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/
+-rw-r--r--   0 rob        (501) staff       (20)    18326 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0001-bpo-45350-Rerun-autoreconf-with-the-pkg-config-macro.patch
+-rw-r--r--   0 rob        (501) staff       (20)     2846 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0002-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.350256 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.11.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.812970 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.11.0/openssl-1.1.1q/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.11.0/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.350458 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.813804 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/
+-rw-r--r--   0 rob        (501) staff       (20)     1648 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/000_patch-setup.py.diff
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3457 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/010_ssl_no_ssl2_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.350656 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.814334 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3447 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.350845 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.814834 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3489 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.351041 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.815265 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3445 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.351231 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.815697 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3445 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.351429 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.819577 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3445 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.351637 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.820241 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3445 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.351833 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.820709 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.352023 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.821956 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.352216 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.822497 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.352415 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.3/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.825149 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.352608 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.825845 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.4/Python-3.3.4/
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.4/Python-3.3.4/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.352795 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.826129 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.5/Python-3.3.5/
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.5/Python-3.3.5/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.352980 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.826401 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.6/Python-3.3.6/
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.6/Python-3.3.6/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.353168 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.7/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.826705 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.7/Python-3.3.7/
+-rw-r--r--   0 rob        (501) staff       (20)     3503 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.7/Python-3.3.7/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.356145 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.826962 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.0/Python-3.4.0/
+-rw-r--r--   0 rob        (501) staff       (20)     2783 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.0/Python-3.4.0/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.356492 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.828331 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.1/Python-3.4.1/
+-rw-r--r--   0 rob        (501) staff       (20)     2783 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.1/Python-3.4.1/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.356794 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.828690 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.2/Python-3.4.2/
+-rw-r--r--   0 rob        (501) staff       (20)     2783 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.2/Python-3.4.2/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.357081 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.831752 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/
+-rw-r--r--   0 rob        (501) staff       (20)     1691 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0001-bpo-27987-pymalloc-align-by-16bytes-on-64bit-platfor.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1654 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0002-bpo-27987-align-PyGC_Head-to-alignof-long-double-GH-.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3137 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0003-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1009 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0004-Detect-arm64-in-configure.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1962 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0005-BPO-41100-Support-macOS-11-when-building-GH-21113.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1480 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0006-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)     5110 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0007-Port-ctypes-and-system-libffi-patch-for-arm64-macOS-.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3508 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0008-bpo-36231-Support-building-on-macOS-without-usr-incl.patch
+-rw-r--r--   0 rob        (501) staff       (20)      852 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0009-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.357364 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.831976 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.2/Python-3.5.2/
+-rw-r--r--   0 rob        (501) staff       (20)      957 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.2/Python-3.5.2/venv.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.357667 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.834944 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/
+-rw-r--r--   0 rob        (501) staff       (20)     1009 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0001-Detect-arm64-in-configure.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3478 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0002-bpo-36231-Support-building-on-macOS-without-usr-incl.patch
+-rw-r--r--   0 rob        (501) staff       (20)    10491 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0003-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch
+-rw-r--r--   0 rob        (501) staff       (20)    12468 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0004-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1962 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0005-BPO-41100-Support-macOS-11-when-building-GH-21113.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1480 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0006-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)      904 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0007-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3137 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0008-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1693 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0009-bpo-27987-pymalloc-align-by-16bytes-on-64bit-platfor.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1656 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0010-bpo-27987-align-PyGC_Head-to-alignof-long-double-GH-.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.357955 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.10/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.835167 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.10/Python-3.7.10/
+-rw-r--r--   0 rob        (501) staff       (20)     2846 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.10/Python-3.7.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.358230 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.11/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.835487 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.11/Python-3.7.11/
+-rw-r--r--   0 rob        (501) staff       (20)     2846 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.11/Python-3.7.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.358525 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.837427 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/
+-rw-r--r--   0 rob        (501) staff       (20)    12192 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1479 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)      904 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1461 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0004-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.358733 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.838440 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/
+-rw-r--r--   0 rob        (501) staff       (20)    12192 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1479 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)      904 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.358926 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.839410 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/
+-rw-r--r--   0 rob        (501) staff       (20)    12192 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1464 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)      904 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.359234 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.840777 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/
+-rw-r--r--   0 rob        (501) staff       (20)    12192 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1464 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)      904 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.841128 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/openssl-1.1.1q/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.359543 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.843047 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/
+-rw-r--r--   0 rob        (501) staff       (20)    12192 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1464 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)      904 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.843304 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/openssl-1.1.1q/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.359718 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.17/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.844160 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.17/Python-3.7.17/
+-rw-r--r--   0 rob        (501) staff       (20)    12192 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.17/Python-3.7.17/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+-rw-r--r--   0 rob        (501) staff       (20)     1464 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.17/Python-3.7.17/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+-rw-r--r--   0 rob        (501) staff       (20)      904 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.17/Python-3.7.17/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.359894 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.8/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.844628 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.8/Python-3.7.8/
+-rw-r--r--   0 rob        (501) staff       (20)     2846 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.8/Python-3.7.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.360081 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.9/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.844885 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.9/Python-3.7.9/
+-rw-r--r--   0 rob        (501) staff       (20)     2846 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.9/Python-3.7.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.360269 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.10/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.845130 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.10/Python-3.8.10/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.10/Python-3.8.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.360443 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.11/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.845589 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.11/Python-3.8.11/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.11/Python-3.8.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.360630 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.12/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.847893 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.12/Python-3.8.12/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.12/Python-3.8.12/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.360831 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.15/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.848295 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.15/openssl-1.1.1q/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.361057 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.16/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.848636 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.16/openssl-1.1.1q/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.361275 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.849722 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.4/Python-3.8.4/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.4/Python-3.8.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.361489 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.850107 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.5/Python-3.8.5/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.5/Python-3.8.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.361678 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.850503 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.6/Python-3.8.6/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.6/Python-3.8.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.361864 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.7/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.851570 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.7/Python-3.8.7/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.7/Python-3.8.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.362496 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.8/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.855216 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.8/Python-3.8.8/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.8/Python-3.8.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.362930 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.9/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.855973 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.9/Python-3.8.9/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.9/Python-3.8.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.363276 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.0/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.856366 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.0/Python-3.9.0/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.0/Python-3.9.0/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.363596 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.1/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.856628 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.1/Python-3.9.1/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.1/Python-3.9.1/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.363956 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.15/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.856859 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.15/openssl-1.1.1q/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.364390 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.16/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.857217 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.16/openssl-1.1.1q/
+-rw-r--r--   0 rob        (501) staff       (20)      264 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.364685 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.857538 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.2/Python-3.9.2/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.2/Python-3.9.2/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.364963 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.4/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.857872 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.4/Python-3.9.4/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.4/Python-3.9.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.365220 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.858114 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.5/Python-3.9.5/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.5/Python-3.9.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.365498 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.6/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.858423 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.6/Python-3.9.6/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.6/Python-3.9.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.365743 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.7/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.858840 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.7/Python-3.9.7/
+-rw-r--r--   0 rob        (501) staff       (20)     2836 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.7/Python-3.9.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.366000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/cinder-3.10-dev/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.859185 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/cinder-3.10-dev/Cinder-3.10-dev/
+-rw-r--r--   0 rob        (501) staff       (20)     1089 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/cinder-3.10-dev/Cinder-3.10-dev/001-disable-werror.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.366310 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/cinder-3.8-dev/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.859511 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/cinder-3.8-dev/Cinder-3.8-dev/
+-rw-r--r--   0 rob        (501) staff       (20)     1089 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/cinder-3.8-dev/Cinder-3.8-dev/001-disable-werror.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.366607 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.2/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.860325 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3489 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/010_ssl_no_ssl3.patch
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.366888 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.5/
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.860926 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/
+-rw-r--r--   0 rob        (501) staff       (20)     2045 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/002_readline63.patch
+-rw-r--r--   0 rob        (501) staff       (20)     3445 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/010_ssl_no_ssl3.patch
+-rw-r--r--   0 rob        (501) staff       (20)      372 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.5-src
+-rw-r--r--   0 rob        (501) staff       (20)     1052 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.6
+-rw-r--r--   0 rob        (501) staff       (20)     1102 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.7
+-rw-r--r--   0 rob        (501) staff       (20)     1102 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.8
+-rw-r--r--   0 rob        (501) staff       (20)     1102 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.9
+-rw-r--r--   0 rob        (501) staff       (20)     1710 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0
+-rw-r--r--   0 rob        (501) staff       (20)      410 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     1200 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     1200 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0.2
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0.2-src
+-rw-r--r--   0 rob        (501) staff       (20)     1974 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.1
+-rw-r--r--   0 rob        (501) staff       (20)      410 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2052 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.2
+-rw-r--r--   0 rob        (501) staff       (20)      410 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.2-src
+-rw-r--r--   0 rob        (501) staff       (20)     2082 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.2.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.2.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2052 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.3
+-rw-r--r--   0 rob        (501) staff       (20)      420 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.3-src
+-rw-r--r--   0 rob        (501) staff       (20)     2738 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.3.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2730 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.4.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2790 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.5.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.5.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2798 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.5.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.5.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2790 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.6.0
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.6.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     3017 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.6.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.6.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     3296 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-4.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-4.0.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     3174 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-4.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-4.0.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     3290 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.0.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2798 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.0.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.0.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     3356 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2858 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.1.1
+-rw-r--r--   0 rob        (501) staff       (20)      414 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.1.1-src
+-rw-r--r--   0 rob        (501) staff       (20)       37 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.3
+-rw-r--r--   0 rob        (501) staff       (20)       41 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.3-src
+-rw-r--r--   0 rob        (501) staff       (20)       39 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.3.1
+-rw-r--r--   0 rob        (501) staff       (20)       43 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.3.1-src
+-rw-r--r--   0 rob        (501) staff       (20)       37 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.4
+-rw-r--r--   0 rob        (501) staff       (20)       41 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.4-src
+-rw-r--r--   0 rob        (501) staff       (20)       39 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.4.1
+-rw-r--r--   0 rob        (501) staff       (20)       43 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.4.1-src
+-rw-r--r--   0 rob        (501) staff       (20)       39 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.6.0
+-rw-r--r--   0 rob        (501) staff       (20)       43 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.6.0-src
+-rw-r--r--   0 rob        (501) staff       (20)       39 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.7.0
+-rw-r--r--   0 rob        (501) staff       (20)       43 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.7.0-src
+-rw-r--r--   0 rob        (501) staff       (20)       39 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.7.1
+-rw-r--r--   0 rob        (501) staff       (20)       43 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.7.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     1681 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-c-jit-latest
+-rw-r--r--   0 rob        (501) staff       (20)      327 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-dev
+-rw-r--r--   0 rob        (501) staff       (20)      552 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-stm-2.3
+-rw-r--r--   0 rob        (501) staff       (20)      556 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-stm-2.5.1
+-rw-r--r--   0 rob        (501) staff       (20)     2760 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.3
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.3-src
+-rw-r--r--   0 rob        (501) staff       (20)     2889 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.3.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2879 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.4
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.4-src
+-rw-r--r--   0 rob        (501) staff       (20)     2891 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.4.1
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.4.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2883 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.6.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.6.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2586 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.7.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.7.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2590 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.7.1
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.7.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2474 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.10.0
+-rw-r--r--   0 rob        (501) staff       (20)      420 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.10.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2470 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.8.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.8.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2468 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.9.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.9.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2817 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-6.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-6.0.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2193 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.0.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2193 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.1.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2193 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.1.1
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.1.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2160 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.2.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.10
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.10-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.11
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.11-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.12
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.12-src
+-rw-r--r--   0 rob        (501) staff       (20)     2290 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.13
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.13-src
+-rw-r--r--   0 rob        (501) staff       (20)     2290 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.14
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.14-src
+-rw-r--r--   0 rob        (501) staff       (20)     2290 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.15
+-rw-r--r--   0 rob        (501) staff       (20)      608 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.15-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.2
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.2-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.3
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.3-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.4
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.4-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.5
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.5-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.6
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.6-src
+-rw-r--r--   0 rob        (501) staff       (20)     2512 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.8
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.8-src
+-rw-r--r--   0 rob        (501) staff       (20)     2357 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.9
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.9-src
+-rw-r--r--   0 rob        (501) staff       (20)     2756 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3-2.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      416 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3-2.3.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2808 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3-2.4.0
+-rw-r--r--   0 rob        (501) staff       (20)      416 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3-2.4.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2286 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.12
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.12-src
+-rw-r--r--   0 rob        (501) staff       (20)     2286 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.13
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.13-src
+-rw-r--r--   0 rob        (501) staff       (20)     2286 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.14
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.14-src
+-rw-r--r--   0 rob        (501) staff       (20)     2286 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.15
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.10-7.3.15-src
+-rw-r--r--   0 rob        (501) staff       (20)     2770 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1
+-rw-r--r--   0 rob        (501) staff       (20)      436 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2740 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.3-5.5-alpha
+-rw-r--r--   0 rob        (501) staff       (20)      426 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.3-5.5-alpha-src
+-rw-r--r--   0 rob        (501) staff       (20)     2737 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.10.0
+-rw-r--r--   0 rob        (501) staff       (20)      420 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.10.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2988 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.10.1
+-rw-r--r--   0 rob        (501) staff       (20)      420 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.10.1-src
+-rw-r--r--   0 rob        (501) staff       (20)      950 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.7-beta
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.7-beta-src
+-rw-r--r--   0 rob        (501) staff       (20)      954 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.7.1-beta
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.7.1-beta-src
+-rw-r--r--   0 rob        (501) staff       (20)      889 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.8.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.8.0-src
+-rw-r--r--   0 rob        (501) staff       (20)      887 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.9.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.9.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2768 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-6.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      418 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-6.0.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2199 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-7.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-7.0.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2183 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-c-jit-latest
+-rw-r--r--   0 rob        (501) staff       (20)     1909 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.0.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.0.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2209 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.1.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.1.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     2209 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.1.1
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.1.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     2174 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.2.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.2.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.0
+-rw-r--r--   0 rob        (501) staff       (20)      422 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.0-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.1-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.2
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.2-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.3
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.3-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.2
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.2-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.3
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.3-src
+-rw-r--r--   0 rob        (501) staff       (20)     1890 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.4
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.4-src
+-rw-r--r--   0 rob        (501) staff       (20)     1891 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.5
+-rw-r--r--   0 rob        (501) staff       (20)      412 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.5-src
+-rw-r--r--   0 rob        (501) staff       (20)     2175 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.6
+-rw-r--r--   0 rob        (501) staff       (20)      473 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.6-src
+-rw-r--r--   0 rob        (501) staff       (20)     2175 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.7
+-rw-r--r--   0 rob        (501) staff       (20)      511 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.7-src
+-rw-r--r--   0 rob        (501) staff       (20)     2512 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.8
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.8-src
+-rw-r--r--   0 rob        (501) staff       (20)     2357 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.9
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.9-src
+-rw-r--r--   0 rob        (501) staff       (20)     1734 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-c-jit-latest
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.10
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.10-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.11
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.11-src
+-rw-r--r--   0 rob        (501) staff       (20)     2171 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.6
+-rw-r--r--   0 rob        (501) staff       (20)      511 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.6-src
+-rw-r--r--   0 rob        (501) staff       (20)     2171 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.7
+-rw-r--r--   0 rob        (501) staff       (20)      511 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.7-src
+-rw-r--r--   0 rob        (501) staff       (20)     2512 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.8
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.8-src
+-rw-r--r--   0 rob        (501) staff       (20)     2357 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.9
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.9-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.10
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.10-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.11
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.11-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.12
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.12-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.13
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.13-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.14
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.14-src
+-rw-r--r--   0 rob        (501) staff       (20)     2285 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.15
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.15-src
+-rw-r--r--   0 rob        (501) staff       (20)     2512 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.8
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.8-src
+-rw-r--r--   0 rob        (501) staff       (20)     2357 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.9
+-rw-r--r--   0 rob        (501) staff       (20)      602 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.9-src
+-rw-r--r--   0 rob        (501) staff       (20)      638 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.2
+-rw-r--r--   0 rob        (501) staff       (20)      635 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3
+-rw-r--r--   0 rob        (501) staff       (20)      646 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.1
+-rw-r--r--   0 rob        (501) staff       (20)      643 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.2
+-rw-r--r--   0 rob        (501) staff       (20)      751 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.3
+-rw-r--r--   0 rob        (501) staff       (20)      843 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.4
+-rw-r--r--   0 rob        (501) staff       (20)      843 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.5
+-rw-r--r--   0 rob        (501) staff       (20)      534 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7-dev
+-rw-r--r--   0 rob        (501) staff       (20)      582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.10
+-rw-r--r--   0 rob        (501) staff       (20)      582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.11
+-rw-r--r--   0 rob        (501) staff       (20)      582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.12
+-rw-r--r--   0 rob        (501) staff       (20)      622 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.14
+-rw-r--r--   0 rob        (501) staff       (20)      604 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.16
+-rw-r--r--   0 rob        (501) staff       (20)      598 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.2
+-rw-r--r--   0 rob        (501) staff       (20)      598 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.3
+-rw-r--r--   0 rob        (501) staff       (20)      598 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.4
+-rw-r--r--   0 rob        (501) staff       (20)      598 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.5
+-rw-r--r--   0 rob        (501) staff       (20)      598 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.6
+-rw-r--r--   0 rob        (501) staff       (20)      582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.7
+-rw-r--r--   0 rob        (501) staff       (20)      582 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.8
+-rw-r--r--   0 rob        (501) staff       (20)      581 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.9
+-rw-r--r--   0 rob        (501) staff       (20)      941 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.2.2
+-rw-r--r--   0 rob        (501) staff       (20)      941 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.2.5
+-rw-r--r--   0 rob        (501) staff       (20)      581 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.3.5
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.3.7
+-rw-r--r--   0 rob        (501) staff       (20)      534 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.4-dev
+-rw-r--r--   0 rob        (501) staff       (20)      613 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.4.2
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.4.7
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.5.4
+-rw-r--r--   0 rob        (501) staff       (20)      603 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.7.5
+-rw-r--r--   0 rob        (501) staff       (20)      533 2024-04-01 12:00:36.000000 autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-dev
+-rw-r--r--   0 rob        (501) staff       (20)     1429 2021-04-23 03:34:41.000000 autovenv-0.3.1671337561/autovenv/util.py
+-rw-r--r--   0 rob        (501) staff       (20)    14293 2021-09-13 09:59:55.000000 autovenv-0.3.1671337561/autovenv/virtualenvs.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.863314 autovenv-0.3.1671337561/autovenv.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      609 2024-04-01 12:08:33.000000 autovenv-0.3.1671337561/autovenv.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)    72121 2024-04-01 12:08:33.000000 autovenv-0.3.1671337561/autovenv.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2024-04-01 12:08:33.000000 autovenv-0.3.1671337561/autovenv.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)       49 2024-04-01 12:08:33.000000 autovenv-0.3.1671337561/autovenv.egg-info/entry_points.txt
+-rw-r--r--   0 rob        (501) staff       (20)       26 2024-04-01 12:08:33.000000 autovenv-0.3.1671337561/autovenv.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)       15 2024-04-01 12:08:33.000000 autovenv-0.3.1671337561/autovenv.egg-info/top_level.txt
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.861777 autovenv-0.3.1671337561/scripts/
+-rwxr--r--   0 rob        (501) staff       (20)      713 2019-10-17 05:35:46.000000 autovenv-0.3.1671337561/scripts/autovenv-build
+-rw-r--r--   0 rob        (501) staff       (20)      107 2016-01-02 23:46:00.000000 autovenv-0.3.1671337561/scripts/autovenv-pythons-available
+-rw-r--r--   0 rob        (501) staff       (20)      118 2016-01-02 09:43:39.000000 autovenv-0.3.1671337561/scripts/autovenv.sh
+-rw-r--r--   0 rob        (501) staff       (20)       38 2024-04-01 12:08:33.864370 autovenv-0.3.1671337561/setup.cfg
+-rw-r--r--   0 rob        (501) staff       (20)     1103 2024-04-01 12:08:30.000000 autovenv-0.3.1671337561/setup.py
+drwxr-xr-x   0 rob        (501) staff       (20)        0 2024-04-01 12:08:33.862228 autovenv-0.3.1671337561/tests/
+-rw-r--r--   0 rob        (501) staff       (20)        0 2017-01-22 00:01:00.000000 autovenv-0.3.1671337561/tests/__init__.py
+-rwxr--r--   0 rob        (501) staff       (20)     3390 2021-04-23 03:26:00.000000 autovenv-0.3.1671337561/tests/test_autovenv.py
```

### Comparing `autovenv-0.3.1671337560/LICENSE` & `autovenv-0.3.1671337561/LICENSE`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/PKG-INFO` & `autovenv-0.3.1671337561/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: autovenv
-Version: 0.3.1671337560
+Version: 0.3.1671337561
 Summary: virtualenv with less hassle
 Home-page: http://autovenv.readthedocs.org
 Author: Robert Lechte
 Author-email: robertlechte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 License-File: LICENSE
+Requires-Dist: virtualenv
+Requires-Dist: appdirs
+Requires-Dist: pyyaml
 
 Virtual environments are great, but they can be a bit annoying to create, manage, and switch between. It gets even worse when multiple different python versions come into play. autovenv takes the annoyance away.
 
 Full documentation is at https://autovenv.readthedocs.org
```

### Comparing `autovenv-0.3.1671337560/README.rst` & `autovenv-0.3.1671337561/README.rst`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/command.py` & `autovenv-0.3.1671337561/autovenv/command.py`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/LICENSE` & `autovenv-0.3.1671337561/autovenv/python-build/LICENSE`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/autovenv-python-build` & `autovenv-0.3.1671337561/autovenv/python-build/autovenv-python-build`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 #
 
 PYTHON_BUILD_VERSION="20180424"
 
 OLDIFS="$IFS"
 
 set -E
-[ -n "$PYENV_DEBUG" ] && set -x
+[ -n "$PYENV_DEBUG" ] && {
+  export PS4='+(${BASH_SOURCE}:${LINENO}): ${FUNCNAME[0]:+${FUNCNAME[0]}(): }'
+  set -x
+}
 
 exec 3<&2 # preserve original stderr at fd 3
 
 
 lib() {
   parse_options() {
     OPTIONS=()
@@ -52,17 +55,22 @@
     declare -f "$FUNCNAME"
     echo "$FUNCNAME \"\$1\";"
     exit
   fi
 }
 lib "$1"
 
+READLINK=$(type -P readlink)
+if [ -z "$READLINK" ]; then
+  echo "pyenv: cannot find readlink - are you missing GNU coreutils?" >&2
+  exit 1
+fi
 
 resolve_link() {
-  $(type -P greadlink readlink | head -1) "$1"
+  $READLINK "$1"
 }
 
 abs_dirname() {
   local path="$1"
 
   # Use a subshell to avoid changing the current path
   (
@@ -98,27 +106,36 @@
     lsb_release -sir | xargs echo
   elif type -p sw_vers >/dev/null; then
     echo "OS X $(sw_vers -productVersion)"
   elif [ -r /etc/os-release ]; then
     source /etc/os-release
     echo "$NAME" $VERSION_ID
   else
-    local os="$(cat /etc/{centos,redhat,fedora,system}-release /etc/debian_version 2>/dev/null | head -1)"
+    local os="$(cat /etc/{centos,redhat,fedora,system}-release /etc/debian_version 2>/dev/null | head -n1)"
     echo "${os:-$(uname -sr)}"
   fi
 }
 
 is_mac() {
   [ "$(uname -s)" = "Darwin" ] || return 1
   [ $# -eq 0 ] || [ "$(osx_version)" "$@" ]
 }
 
 can_use_homebrew() {
-    [ -z "$PYTHON_BUILD_SKIP_HOMEBREW" ] || return 1
-    is_mac || return 1
+  [[ -n "$PYTHON_BUILD_USE_HOMEBREW" && -n "$PYTHON_BUILD_SKIP_HOMEBREW" ]] && {
+    echo "error: mutually exclusive environment variables PYTHON_BUILD_USE_HOMEBREW and PYTHON_BUILD_SKIP_HOMEBREW are set" >&3
+    exit 1
+  }
+  [[ -n "$PYTHON_BUILD_USE_HOMEBREW" ]] && return 0
+  [[ -n "$PYTHON_BUILD_SKIP_HOMEBREW" ]] && return 1
+  is_mac && return 0
+  # In Linux, if Pyenv itself is installed with Homebrew,
+  # we assume the user wants to take dependencies from there as well by default
+  command -v brew &>/dev/null && [[ $(abs_dirname "${BASH_SOURCE}") == "$(abs_dirname "$(brew --prefix 2>/dev/null ||true)")"/* ]] && return 0
+  return 1
 }
 
 #  9.1  -> 901
 # 10.9  -> 1009
 # 10.10 -> 1010
 osx_version() {
   local -a ver
@@ -229,17 +246,15 @@
   done
 
   pushd "$BUILD_PATH" >&4
   "fetch_${package_type}" "${fetch_args[@]}"
   make_package "${make_args[@]}"
   popd >&4
 
-  { echo "Installed ${package_name} to ${PREFIX_PATH}"
-    echo
-  } >&2
+  echo "Installed ${package_name} to ${PREFIX_PATH}" >&2
 }
 
 make_package() {
   local package_name="$1"
   shift
 
   pushd "$package_name" >&4
@@ -254,15 +269,15 @@
 
 compute_sha2() {
   local output
   if type shasum &>/dev/null; then
     output="$(shasum -a 256 -b)" || return 1
     echo "${output% *}"
   elif type openssl &>/dev/null; then
-    local openssl="$(command -v "$(brew --prefix openssl 2>/dev/null || true)"/bin/openssl openssl | head -1)"
+    local openssl="$(command -v "$(brew --prefix openssl 2>/dev/null || true)"/bin/openssl openssl | head -n1)"
     output="$("$openssl" dgst -sha256 2>/dev/null)" || return 1
     echo "${output##* }"
   elif type sha256sum &>/dev/null; then
     output="$(sha256sum -b)" || return 1
     echo "${output%% *}"
   else
     return 1
@@ -796,14 +811,15 @@
   local PACKAGE_MAKE_OPTS_ARRAY="${package_var_name}_MAKE_OPTS_ARRAY[@]"
   local PACKAGE_CFLAGS="${package_var_name}_CFLAGS"
 
   if [ "$package_var_name" = "PYTHON" ]; then
     use_homebrew || true
     use_tcltk || true
     use_homebrew_readline || use_freebsd_pkg || true
+    use_homebrew_ncurses || true
     if is_mac -ge 1014; then
       use_xcode_sdk_zlib || use_homebrew_zlib || true
     else
       use_homebrew_zlib || true
     fi
     use_dsymutil || true
   fi
@@ -811,18 +827,18 @@
   ( if [ "${CFLAGS+defined}" ] || [ "${!PACKAGE_CFLAGS+defined}" ]; then
       export CFLAGS="$CFLAGS ${!PACKAGE_CFLAGS}"
     fi
     if [ -z "$CC" ] && is_mac -ge 1010; then
       export CC=clang
     fi
     ${!PACKAGE_CONFIGURE:-./configure} --prefix="${!PACKAGE_PREFIX_PATH:-$PREFIX_PATH}" \
-      $CONFIGURE_OPTS ${!PACKAGE_CONFIGURE_OPTS} "${!PACKAGE_CONFIGURE_OPTS_ARRAY}" || return 1
+      "${!PACKAGE_CONFIGURE_OPTS_ARRAY}" $CONFIGURE_OPTS ${!PACKAGE_CONFIGURE_OPTS} || return 1
   ) >&4 2>&1
 
-  { "$MAKE" $MAKE_OPTS ${!PACKAGE_MAKE_OPTS} "${!PACKAGE_MAKE_OPTS_ARRAY}"
+  { "$MAKE" "${!PACKAGE_MAKE_OPTS_ARRAY}" $MAKE_OPTS ${!PACKAGE_MAKE_OPTS}
   } >&4 2>&1
 }
 
 build_package_standard_install() {
   local package_name="$1"
   local package_var_name="$(capitalize "${package_name%%-*}")"
 
@@ -865,15 +881,15 @@
   } >&4 2>&1
   fix_jython_shebangs
 }
 
 fix_jython_shebangs() {
   # Workaround for Jython 2.7+ (#458)
   for file in "${PREFIX_PATH}/bin"/*; do
-    case "$(head -1 "${file}")" in
+    case "$(head -n1 "${file}")" in
     "#!"*"/bin/jython" )
       sed -i.bak "1 s:.*:#\!${PREFIX_PATH}\/bin\/jython:" "${file}"
       ;;
     "#!"*"/bin/python2.7"* )
       sed -i.bak "1 s:.*:#\!\/usr\/bin\/env python:" "${file}"
       ;;
     esac
@@ -917,24 +933,30 @@
 }
 
 build_package_ironpython_builder() {
   xbuild Build.proj /t:Stage "/p:Mono=true;BaseConfiguration=Release" >&4 2>&1
   ( cd "Stage/Release/IronPython-"* && build_package_ironpython )
 }
 
+build_package_micropython_1_9() {
+  # supported version 1.9.3 and 1.9.4
+  build_package_micropython "with_axtls"
+}
+
 build_package_micropython() {
+  # supported version 1.10 and higher
   if [ "${MAKEOPTS+defined}" ]; then
     MAKE_OPTS="$MAKEOPTS"
   elif [ -z "${MAKE_OPTS+defined}" ]; then
     MAKE_OPTS="-j $(num_cpu_cores)"
   fi
   { cd mpy-cross
     "$MAKE" $MAKE_OPTS
     cd ../ports/unix
-    "$MAKE" $MAKE_OPTS axtls
+    [ "$1" = "with_axtls" ] && "$MAKE" $MAKE_OPTS axtls
     "$MAKE" $MAKE_OPTS CFLAGS_EXTRA="-DMICROPY_PY_SYS_PATH_DEFAULT='\".frozen:${PREFIX_PATH}/lib/micropython\"' $CFLAGS_EXTRA"
     "$MAKE" install $MAKE_INSTALL_OPTS PREFIX="${PREFIX_PATH}"
     ln -fs micropython "${PREFIX_PATH}/bin/python"
     mkdir -p "${PREFIX_PATH}/lib/micropython"
   }>&4 2>&1
 }
 
@@ -1142,15 +1164,15 @@
 
 fix_directory_permissions() {
   # Ensure installed directories are not world-writable
   find "$PREFIX_PATH" -type d \( -perm -020 -o -perm -002 \) -exec chmod go-w {} \;
 }
 
 require_java7() {
-  local version="$(java -version 2>&1 | grep '\(java\|openjdk\) version' | head -1)"
+  local version="$(java -version 2>&1 | grep '\(java\|openjdk\) version' | head -n1)"
   if [[ $version != *[789]* ]]; then
     colorize 1 "ERROR" >&3
     echo ": Java 7 required. Please install a 1.7-compatible JRE." >&3
     return 1
   fi
 }
 
@@ -1197,15 +1219,15 @@
       fi
     } >&3
     return 1
   fi
 
   export CC="$gcc"
   if is_mac -ge 1010; then
-    export MACOSX_DEPLOYMENT_TARGET=10.9
+    export MACOSX_DEPLOYMENT_TARGET=${MACOSX_DEPLOYMENT_TARGET:-10.9}
   fi
 }
 
 locate_gcc() {
   local gcc gccs
   IFS=: gccs=($(gccs_in_path))
   IFS="$OLDIFS"
@@ -1375,67 +1397,83 @@
         fi
       done
     fi
   done
   return 1
 }
 
+# `python-config` ignores LDFLAGS envvar. Adding to LIBS is the only way to add extra stuff
+# to `python-config --ldflags` output
+append_ldflags_libs() {
+  local args="$1"
+  export LDFLAGS="${LDFLAGS:+$LDFLAGS }$args"
+  export LIBS="${LIBS:+${LIBS% } }$args"
+}
+prepend_ldflags_libs() {
+  local args="$1"
+  export LDFLAGS="$args${LDFLAGS:+ $LDFLAGS}"
+  export LIBS="$args${LIBS:+ $LIBS}"
+}
+
 use_homebrew() {
   can_use_homebrew || return 1
   # unless Homebrew is at the default /usr/local, need to add its paths to
   # compiler search to be able to use non-keg-only deps from there
   if command -v brew &>/dev/null; then
     local brew_prefix="$(brew --prefix 2>/dev/null || true)"
     # /usr/local/lib:/usr/lib is the default library search path
     if [[ -n $brew_prefix && $brew_prefix != "/usr" && $brew_prefix != "/usr/local" ]]; then
-      export CPPFLAGS="${CPPFLAGS:+${CPPFLAGS% } }-I${brew_prefix}/include"
-      export LDFLAGS="${LDFLAGS:+${LDFLAGS% } }-L${brew_prefix}/lib -Wl,-rpath,${brew_prefix}/lib"
-      # `python-config` ignores LDFLAGS envvar. Adding to LIBS is the only way to add extra stuff
-      # to `python-config --ldflags` output
-      export LIBS="${LIBS:+${LIBS% } }-L${brew_prefix}/lib -Wl,-rpath,${brew_prefix}/lib"
+      export CPPFLAGS="${CPPFLAGS:+$CPPFLAGS }-I${brew_prefix}/include"
+      append_ldflags_libs "-L${brew_prefix}/lib -Wl,-rpath,${brew_prefix}/lib"
     fi
   fi
 }
 
 needs_yaml() {
   ! configured_with_package_dir "python" "yaml.h" &&
   ! use_homebrew_yaml
 }
 
 use_homebrew_yaml() {
   can_use_homebrew || return 1
   local libdir="$(brew --prefix libyaml 2>/dev/null || true)"
   if [ -d "$libdir" ]; then
     echo "python-build: use libyaml from homebrew"
-    export CPPFLAGS="-I$libdir/include ${CPPFLAGS}"
-    export LDFLAGS="-L$libdir/lib ${LDFLAGS}"
+    export CPPFLAGS="-I$libdir/include${CPPFLAGS:+ $CPPFLAGS}"
+    export LDFLAGS="-L$libdir/lib${LDFLAGS:+ ${LDFLAGS% }}"
   else
     return 1
   fi
 }
 
 use_freebsd_pkg() {
   # check if FreeBSD
   if [ "FreeBSD" = "$(uname -s)" ]; then
     # use openssl if installed from Ports Collection
-    if [ -f /usr/local/include/openssl/ssl.h ]; then
-      package_option ruby configure --with-openssl-dir="/usr/local"
+    if pkg info -e openssl; then
+      package_option python configure --with-openssl="/usr/local"
     fi
 
     # check if 11-R or later
     release="$(uname -r)"
     if [ "${release%%.*}" -ge 11 ]; then
-      # prefers readline to compile most of ruby versions
-      if pkg info -e readline > /dev/null; then
-        # use readline from Ports Collection
-        package_option ruby configure --with-readline-dir="/usr/local"
-      elif pkg info -e libedit > /dev/null; then
-        # use libedit from Ports Collection
-        package_option ruby configure --enable-libedit
-        package_option ruby configure --with-libedit-dir="/usr/local"
+      # Use packages from Ports Collection.
+      #
+      # Unlike Linux, BSD's cc does not look in /usr/local by default
+      # where Ports-installed packages are, but they are available via pkg-config.
+      # Surprisingly, CPython's Configure only uses pkg-config
+      # to locate some of the dependencies and not others.
+      # Here we detect those that are (as of this writing) known
+      # to not be searched via pkg-config.
+      #
+      # XXX: As a side effect, this would pick up any other libs from Ports
+      # that are searched via compiler
+      if pkg info -e readline || pkg info -e sqlite3; then
+        export CPPFLAGS="${CPPFLAGS:+$CPPFLAGS }-I/usr/local/include"
+        export LDFLAGS="${LDFLAGS:+$LDFLAGS }-L/usr/local/lib -Wl,-rpath,/usr/local/lib"
       fi
     fi
   fi
 }
 
 has_broken_mac_readline() {
   # Mac OS X 10.4 has broken readline.
@@ -1447,35 +1485,53 @@
 
 use_homebrew_readline() {
   can_use_homebrew || return 1
   if ! configured_with_package_dir "python" "readline/rlconf.h"; then
     local libdir="$(brew --prefix readline 2>/dev/null || true)"
     if [ -d "$libdir" ]; then
       echo "python-build: use readline from homebrew"
-      export CPPFLAGS="-I$libdir/include ${CPPFLAGS}"
-      export LDFLAGS="-L$libdir/lib ${LDFLAGS}"
+      export CPPFLAGS="-I$libdir/include${CPPFLAGS:+ $CPPFLAGS}"
+      export LDFLAGS="-L$libdir/lib${LDFLAGS:+ $LDFLAGS}"
     else
       return 1
     fi
   fi
 }
 
+use_homebrew_ncurses() {
+  can_use_homebrew || return 1
+  local libdir="$(brew --prefix ncurses 2>/dev/null || true)"
+  if [ -d "$libdir" ]; then
+    echo "python-build: use ncurses from homebrew"
+    export CPPFLAGS="-I$libdir/include${CPPFLAGS:+ $CPPFLAGS}"
+    export LDFLAGS="-L$libdir/lib${LDFLAGS:+ $LDFLAGS}"
+  else
+    return 1
+  fi
+}
+
 prefer_openssl11() {
   # Allow overriding the preference of OpenSSL version per definition basis (#1302, #1325, #1326)
   PYTHON_BUILD_HOMEBREW_OPENSSL_FORMULA="${PYTHON_BUILD_HOMEBREW_OPENSSL_FORMULA:-openssl@1.1 openssl}"
   export PYTHON_BUILD_HOMEBREW_OPENSSL_FORMULA
 }
 
+prefer_openssl3() {
+  # Allow overriding the preference of OpenSSL version per definition basis (#1302, #1325, #1326)
+  PYTHON_BUILD_HOMEBREW_OPENSSL_FORMULA="${PYTHON_BUILD_HOMEBREW_OPENSSL_FORMULA:-openssl@3 openssl@1.1 openssl}"
+  export PYTHON_BUILD_HOMEBREW_OPENSSL_FORMULA
+}
+
 build_package_mac_readline() {
   # Install to a subdirectory since we don't want shims for bin/readline.
   READLINE_PREFIX_PATH="${PREFIX_PATH}/readline"
 
   # Tell Python to use this readline for its extension.
-  export CPPFLAGS="-I${READLINE_PREFIX_PATH}/include ${CPPFLAGS}"
-  export LDFLAGS="-L${READLINE_PREFIX_PATH}/lib ${LDFLAGS}"
+  export CPPFLAGS="-I${READLINE_PREFIX_PATH}/include${CPPFLAGS:+ $CPPFLAGS}"
+  export LDFLAGS="-L${READLINE_PREFIX_PATH}/lib${LDFLAGS:+ $LDFLAGS}"
 
   # Make sure pkg-config finds our build first.
   export PKG_CONFIG_PATH="${READLINE_PREFIX_PATH}/lib/pkgconfig${PKG_CONFIG_PATH:+:$PKG_CONFIG_PATH}"
 
   build_package_standard "$@"
 }
 
@@ -1494,16 +1550,16 @@
     if [ -d "$ssldir" ]; then
       echo "python-build: use ${openssl} from homebrew"
       if [[ -n "${PYTHON_BUILD_CONFIGURE_WITH_OPENSSL:-}" ]]; then
         # configure script of newer CPython versions support `--with-openssl`
         # https://bugs.python.org/issue21541
         package_option python configure --with-openssl="${ssldir}"
       else
-        export CPPFLAGS="-I$ssldir/include ${CPPFLAGS}"
-        export LDFLAGS="-L$ssldir/lib ${LDFLAGS}"
+        export CPPFLAGS="-I$ssldir/include ${CPPFLAGS:+ $CPPFLAGS}"
+        export LDFLAGS="-L$ssldir/lib${LDFLAGS:+ $LDFLAGS}"
       fi
       export PKG_CONFIG_PATH="$ssldir/lib/pkgconfig/:${PKG_CONFIG_PATH}"
       return
     fi
   done
   return 1
 }
@@ -1517,16 +1573,16 @@
 
   # Tell Python to use this openssl for its extension.
   if [[ -n "${PYTHON_BUILD_CONFIGURE_WITH_OPENSSL:-}" ]]; then
     # configure script of newer CPython versions support `--with-openssl`
     # https://bugs.python.org/issue21541
     package_option python configure --with-openssl="${OPENSSL_PREFIX_PATH}"
   else
-    export CPPFLAGS="-I${OPENSSL_PREFIX_PATH}/include ${CPPFLAGS}"
-    export LDFLAGS="-L${OPENSSL_PREFIX_PATH}/lib ${LDFLAGS}"
+    export CPPFLAGS="-I${OPENSSL_PREFIX_PATH}/include ${CPPFLAGS:+ $CPPFLAGS}"
+    export LDFLAGS="-L${OPENSSL_PREFIX_PATH}/lib${LDFLAGS:+ $LDFLAGS}"
   fi
 
   # Make sure pkg-config finds our build first.
   export PKG_CONFIG_PATH="${OPENSSL_PREFIX_PATH}/lib/pkgconfig${PKG_CONFIG_PATH:+:$PKG_CONFIG_PATH}"
 
   # Hint OpenSSL that we prefer a 64-bit build.
   export KERNEL_BITS="64"
@@ -1579,15 +1635,15 @@
         failed.map { |lib| packages.fetch(manager)[lib] }.join(" ")
       ] unless manager.empty?
       $stderr.puts "Configure options used:"
       require "rbconfig"; require "shellwords"
       RbConfig::CONFIG.fetch("configure_args").shellsplit.each { |arg| $stderr.puts "  #{arg}" }
       exit 1
     end
-  ' "$(basename "$(type -P yum apt-get | head -1)")" >&4 2>&1
+  ' "$(basename "$(type -P yum apt-get | head -n1)")" >&4 2>&1
 }
 
 use_homebrew_zlib() {
   can_use_homebrew || return 1
   local brew_zlib="$(brew --prefix zlib 2>/dev/null || true)"
   if [ -d "$brew_zlib" ]; then
     echo "python-build: use zlib from homebrew"
@@ -1597,31 +1653,42 @@
 
 use_xcode_sdk_zlib() {
   # If a custom compiler is used, including XCode SDK will likely break it
   [[ "${CC:-clang}" != "clang" || "$(command -v clang 2>/dev/null || true)" != "/usr/bin/clang" ]] && return 1
   local xc_sdk_path="$(xcrun --show-sdk-path 2>/dev/null || true)"
   if [ -d "$xc_sdk_path" ]; then
     echo "python-build: use zlib from xcode sdk"
-    export CFLAGS="-I${xc_sdk_path}/usr/include ${CFLAGS}"
+    # Even though SDK's compiler uses the SDK dirs implicitly,
+    # CPython's setup.py has to have nonstandard paths specified explicitly
+    # to search for zlib.h in them
+    export CPPFLAGS="${CPPFLAGS:+$CPPFLAGS }-I${xc_sdk_path}/usr/include"
     if is_mac -ge 1100; then
-      export LDFLAGS="${LDFLAGS} -L${xc_sdk_path}/usr/lib"
+      export LDFLAGS="${LDFLAGS:+$LDFLAGS }-L${xc_sdk_path}/usr/lib"
     fi
   fi
 }
 
 use_homebrew_tcltk() {
   can_use_homebrew || return 1
   # get the version from the folder that homebrew versions
   local tcltk_libdir="$(brew --prefix tcl-tk 2>/dev/null || true)"
   if [ -d "$tcltk_libdir" ]; then
     echo "python-build: use tcl-tk from homebrew"
     if [[ -z "$PYTHON_BUILD_TCLTK_USE_PKGCONFIG" ]]; then
       local tcltk_version="$(sh -c '. '"$tcltk_libdir"'/lib/tclConfig.sh; echo $TCL_VERSION')"
       package_option python configure --with-tcltk-libs="-L$tcltk_libdir/lib -ltcl$tcltk_version -ltk$tcltk_version"
-      package_option python configure --with-tcltk-includes="-I$tcltk_libdir/include"
+      # In Homebrew Tcl/Tk 8.6.13, headers have been moved to the 'tcl-tk' subdir.
+      # We're not using tclConfig.sh here 'cuz it produces the version-specific path to <brew prefix>/Cellar
+      # and we'd rather have rpath set to <brew prefix>/opt/<...> to allow micro release upgrades without rebuilding
+      # XXX: do use tclConfig.sh and translate the paths if more path shenanigans appear in later releases
+      if [ -d "$tcltk_libdir/include/tcl-tk" ]; then
+        package_option python configure --with-tcltk-includes="-I$tcltk_libdir/include/tcl-tk"
+      else
+        package_option python configure --with-tcltk-includes="-I$tcltk_libdir/include"
+      fi
     fi
     export PKG_CONFIG_PATH="${tcltk_libdir}/lib/pkgconfig${PKG_CONFIG_PATH:+:$PKG_CONFIG_PATH}"
   fi
 }
 
 # FIXME: this function is a workaround for #1125
 # once fixed, it should be removed.
@@ -1698,15 +1765,15 @@
     package_option python configure --enable-shared
 }
 
 build_package_auto_tcltk() {
   if is_mac && [ ! -d /usr/include/X11 ]; then
     if [ -d /opt/X11/include ]; then
       if [[ "$CPPFLAGS" != *-I/opt/X11/include* ]]; then
-        export CPPFLAGS="-I/opt/X11/include $CPPFLAGS"
+        export CPPFLAGS="-I/opt/X11/include${CPPFLAGS:+ $CPPFLAGS}"
       fi
     else
       package_option python configure --without-tk
     fi
   fi
 }
 
@@ -1734,17 +1801,17 @@
   local striplevel=0
   grep -q '^diff --git a/' "$patchfile" && striplevel=1
   patch -p$striplevel --force -i "$patchfile"
 }
 
 
 build_package_symlink_version_suffix() {
-  if [[ "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" == *"--enable-framework"* ]]; then
+  if [[ "${PYTHON_CONFIGURE_OPTS_ARRAY[*]} $CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" == *"--enable-framework"* ]]; then
     if [ -e "${PREFIX_PATH}/bin" ]; then
-      # Always create `bin` as symlink to framework path if the version was built with `--enable-frameowrk` (#590)
+      # Always create `bin` as symlink to framework path if the version was built with `--enable-framework` (#590)
       rm -rf "${PREFIX_PATH}/bin.orig"
       mv -f "${PREFIX_PATH}/bin" "${PREFIX_PATH}/bin.orig"
     fi
     # Only symlinks are installed in ${PREFIX_PATH}/bin
     ln -fs "${PREFIX_PATH}/Library/Frameworks/Python.framework/Versions/Current/bin" "${PREFIX_PATH}/bin"
   fi
 
@@ -1790,24 +1857,24 @@
       echo "https://github.com/pyenv/pyenv/issues"
       return 1
     } >&3
   fi
 }
 
 try_python_module() {
-  if ! "$PYTHON_BIN" -c "import $1" 1>/dev/null 2>&1; then
+  if ! "$PYTHON_BIN" -c "import $1"; then
     { colorize 1 "WARNING"
       echo ": The Python $1 extension was not compiled${3:+ $3}. Missing the ${2:-$1}?"
       return 0
     } >&3
   fi
 }
 
 verify_python_module() {
-  if ! "$PYTHON_BIN" -c "import $1" 1>/dev/null 2>&1; then
+  if ! "$PYTHON_BIN" -c "import $1"; then
     { colorize 1 "ERROR"
       echo ": The Python $1 extension was not compiled. Missing the ${2:-$1}?"
       echo
       echo "Please consult to the Wiki page to fix the problem."
       echo "https://github.com/pyenv/pyenv/wiki/Common-build-problems"
       echo
       return 1
@@ -1945,14 +2012,19 @@
 }
 
 # Post-install check for Python 3.12.x
 build_package_verify_py312() {
   build_package_verify_py311 "$1" "${2:-3.12}"
 }
 
+# Post-install check for Python 3.13.x
+build_package_verify_py313() {
+  build_package_verify_py312 "$1" "${2:-3.13}"
+}
+
 # Post-install check for Python 3.x rolling release scripts
 # XXX: Will need splitting into project-specific ones if there emerge
 # multiple rolling-release scripts with different checks needed
 build_package_verify_py3_latest() {
   build_package_verify_py311 "$1" "3"
 }
 
@@ -2000,22 +2072,31 @@
   "${PYTHON_BIN}" -s "${get_pip}" ${GET_PIP_OPTS} 1>&4 2>&1 || {
     echo "error: failed to install pip via get-pip.py" >&2
     return 1
   }
   build_package_symlink_version_suffix
 }
 
+# Pip <21 (in 2.7 and derivatives like PyPy-2.7) doesn't support -I
+build_package_ensurepip_lt21() {
+  build_package_ensurepip lt21
+}
+
 build_package_ensurepip() {
+  local mode="$1"
   local ensurepip_opts
   # Install as `--altinstall` if the Python is installed as `altinstall` (#255)
   if [[ "$PYTHON_MAKE_INSTALL_TARGET" == *"altinstall"* ]]; then
     ensurepip_opts="--altinstall"
   fi
+  local python_opts="-I"
+  if [[ $mode == "lt21" ]]; then python_opts="-s"; fi
+  
   # FIXME: `--altinstall` with `get-pip.py`
-  "$PYTHON_BIN" -s -m ensurepip ${ensurepip_opts} 1>/dev/null 2>&1 || build_package_get_pip "$@" || return 1
+  "$PYTHON_BIN" $python_opts -m ensurepip ${ensurepip_opts} 1>/dev/null 2>&1 || build_package_get_pip "$@" || return 1
   build_package_symlink_version_suffix
 }
 
 version() {
   local git_revision
   # Read the revision from git if the remote points to "python-build" repository
   if GIT_DIR="$PYTHON_BUILD_INSTALL_PREFIX/../../.git" git remote -v 2>/dev/null | grep -q /pyenv; then
@@ -2190,34 +2271,39 @@
 WGET_OPTS="${PYTHON_BUILD_WGET_OPTS} ${IPV4+--inet4-only} ${IPV6+--inet6-only}"
 
 # Add an option to build a debug version of Python (#11)
 if [ -n "$DEBUG" ]; then
   package_option python configure --with-pydebug
 fi
 
+if [[ "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" != *"--enable-framework"* && "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" != *"--disable-shared"* ]]; then
+  package_option python configure --enable-shared
+fi
+
 # python-build: Specify `--libdir` on configure to fix build on openSUSE (#36)
 package_option python configure --libdir="${PREFIX_PATH}/lib"
 
 # python-build: Set `RPATH` if `--enable-shared` was given (#65, #66, #82)
-if [[ "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" == *"--enable-shared"* ]]; then
+if [[ "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS ${PYTHON_CONFIGURE_OPTS_ARRAY[@]}" == *"--enable-shared"* ]]; then
   # The ld on Darwin embeds the full paths to each dylib by default
-  if [[ "$LDFLAGS" != *"-rpath="* ]] && ! is_mac; then
-    export LDFLAGS="-Wl,-rpath=${PREFIX_PATH}/lib ${LDFLAGS}"
+  if [[ "$LDFLAGS" != *"-rpath="* ]] ; then
+    prepend_ldflags_libs "-Wl,-rpath,${PREFIX_PATH}/lib"
   fi
 fi
 
 # python-build: Set `RPATH` if --shared` was given for PyPy (#244)
 if [[ "$PYPY_OPTS" == *"--shared"* ]]; then
-  export LDFLAGS="-Wl,-rpath=${PREFIX_PATH}/lib ${LDFLAGS}"
+  prepend_ldflags_libs "-Wl,-rpath=${PREFIX_PATH}/lib"
 fi
 
 # Add support for framework installation (`--enable-framework`) of CPython (#55, #99)
+shopt -s extglob
 if [[ "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" == *"--enable-framework"* ]]; then
   if ! is_mac; then
-    echo "python-build: framework installation is not supported." >&2
+    echo "python-build: framework installation is not supported outside of MacOS." >&2
     exit 1
   fi
   create_framework_dirs() {
     local version="$(echo "$1" | sed -E 's/^[^0-9]*([0-9]+\.[0-9]+).*$/\1/')"
     mkdir -p "${PREFIX_PATH}/Library/Frameworks/Python.framework/Versions/${version}"
     ( cd "${PREFIX_PATH}/Library/Frameworks/Python.framework/Versions" && ln -fs "${version}" "Current")
     local path
@@ -2225,32 +2311,47 @@
       mkdir -p "${PREFIX_PATH}/Library/Frameworks/Python.framework/Versions/Current/${path}"
       ln -fs "${PREFIX_PATH}/Library/Frameworks/Python.framework/Versions/Current/${path}" "${PREFIX_PATH}/${path}"
     done
   }
   create_framework_dirs "${DEFINITION_PATH##*/}"
   # the `/Library/Frameworks` suffix makes CPython build install apps under prefix rather than into /Applications (#1003)
   package_option python configure --enable-framework="${PREFIX_PATH}/Library/Frameworks"
+  
+  #FIXME: doesn't properly handle paths with spaces. Fix by parsing *OPTS into arrays.
+  CONFIGURE_OPTS="${CONFIGURE_OPTS//--enable-framework?(=*([^ ]))?( )/}";
+  CONFIGURE_OPTS="${CONFIGURE_OPTS% }"
+  PYTHON_CONFIGURE_OPTS="${PYTHON_CONFIGURE_OPTS//--enable-framework?(=*([^ ]))?( )/}";
+  PYTHON_CONFIGURE_OPTS="${PYTHON_CONFIGURE_OPTS% }"
 fi
+shopt -u extglob
 
 # Build against universal SDK
+shopt -s extglob
 if [[ "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" == *"--enable-universalsdk"* ]]; then
   if ! is_mac; then
-    echo "python-build: universal installation is not supported." >&2
+    echo "python-build: universal installation is not supported outside of MacOS." >&2
     exit 1
   fi
   package_option python configure --enable-universalsdk=/
+  #FIXME: doesn't properly handle paths with spaces. Fix by parsing *OPTS into arrays.
+  CONFIGURE_OPTS="${CONFIGURE_OPTS//--enable-universalsdk?(=*([^ ]))?( )/}"
+  CONFIGURE_OPTS="${CONFIGURE_OPTS% }"
+  PYTHON_CONFIGURE_OPTS="${PYTHON_CONFIGURE_OPTS//--enable-universalsdk?(=*([^ ]))?( )/}"
+  PYTHON_CONFIGURE_OPTS="${PYTHON_CONFIGURE_OPTS% }"
+
   if [[ "$CONFIGURE_OPTS $PYTHON_CONFIGURE_OPTS" != *"--with-universal-archs"* ]]; then
     # in CPython's configure.ac, --with-universal-archs defaults to 'intel' which means i386 + x86_64
     # since 2.7.5 and 3.3.0 -- i.e. in all non-EOL versions
     # Apple Silicon cannot build these, in it, it rather makes sense to default to Universal2 binaries
     if [[ $(arch) == "arm64" ]]; then
       package_option python configure --with-universal-archs=universal2
     fi
   fi
 fi
+shopt -u extglob
 
 # Compile with `--enable-unicode=ucs4` by default (#257)
 if [[ "$PYTHON_CONFIGURE_OPTS" != *"--enable-unicode="* ]]; then
   if ! is_mac; then
     # Skip specifying `--enable-unicode` for CPython 3.3+ (#912)
     case "${DEFINITION_PATH##*/}" in
     "2."* | \
@@ -2293,30 +2394,30 @@
     unset PIP_VERSION
   else
     # Use custom get-pip URL based on the target version (#1127)
     case "${DEFINITION_PATH##*/}" in
     2.6 | 2.6.* )
       GET_PIP_URL="https://bootstrap.pypa.io/pip/2.6/get-pip.py"
       ;;
-    2.7 | 2.7.* )
+    2.7 | 2.7.* | pypy2.7 | pypy2.7-* )
       GET_PIP_URL="https://bootstrap.pypa.io/pip/2.7/get-pip.py"
       ;;
     3.2 | 3.2.* )
       GET_PIP_URL="https://bootstrap.pypa.io/pip/3.2/get-pip.py"
       ;;
     3.3 | 3.3.* )
       GET_PIP_URL="https://bootstrap.pypa.io/pip/3.3/get-pip.py"
       ;;
     3.4 | 3.4.* )
       GET_PIP_URL="https://bootstrap.pypa.io/pip/3.4/get-pip.py"
       ;;
-    3.5 | 3.5.* )
+    3.5 | 3.5.* | pypy3.5 | pypy3.5-* )
       GET_PIP_URL="https://bootstrap.pypa.io/pip/3.5/get-pip.py"
       ;;
-    3.6 | 3.6.* )
+    3.6 | 3.6.* | pypy3.6 | pypy3.6-* )
       GET_PIP_URL="https://bootstrap.pypa.io/pip/3.6/get-pip.py"
       ;;
     * )
       GET_PIP_URL="https://bootstrap.pypa.io/get-pip.py"
       ;;
     esac
   fi
@@ -2369,16 +2470,16 @@
 exec 4<> "$LOG_PATH" # open the log file at fd 4
 if [ -n "$VERBOSE" ]; then
   tail -f "$LOG_PATH" &
   TAIL_PID=$!
   trap "kill $TAIL_PID" SIGINT SIGTERM EXIT
 fi
 
-export LDFLAGS="-L${PREFIX_PATH}/lib ${LDFLAGS}"
-export CPPFLAGS="-I${PREFIX_PATH}/include ${CPPFLAGS}"
+prepend_ldflags_libs "-L${PREFIX_PATH}/lib"
+export CPPFLAGS="-I${PREFIX_PATH}/include${CPPFLAGS:+ $CPPFLAGS}"
 
 unset PYTHONHOME
 unset PYTHONPATH
 
 trap build_failed ERR
 mkdir -p "$BUILD_PATH"
 source "$DEFINITION_PATH"
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.1.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.1.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.2.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.2.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.3.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.3.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.4.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.4.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.5.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.5.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.6.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.6.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.13` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.13`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.15` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.15`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.16` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.16`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.17` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.17`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.18` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.1`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-export PYTHON_BUILD_HOMEBREW_OPENSSL_FORMULA="openssl@1.1 openssl@1.0 openssl"
-install_package "openssl-1.0.2q" "https://www.openssl.org/source/old/1.0.2/openssl-1.0.2q.tar.gz#5744cfcbcec2b1b48629f7354203bc1e5e9b5466998bbccc5b5fcde3b18eb684" mac_openssl --if has_broken_mac_openssl
+prefer_openssl11
+export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+install_package "openssl-1.1.0j" "https://www.openssl.org/source/old/1.1.0/openssl-1.1.0j.tar.gz#31bec6c203ce1a8e93d5994f4ed304c63ccf07676118b6634edded12ad1b3246" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-2.7.18" "https://www.python.org/ftp/python/2.7.18/Python-2.7.18.tar.xz#b62c0e7937551d0cc02b8fd5cb0f544f9405bafc9a54d3808ed4594812edef43" standard verify_py27 copy_python_gdb ensurepip
+  install_package "Python-3.7.1" "https://www.python.org/ftp/python/3.7.1/Python-3.7.1.tar.xz#fa7e2b8e8c9402f192ad56dc4f814089d1c4466c97d780f5e5acc02c04243d6d" standard verify_py37 copy_python_gdb ensurepip
 else
-  install_package "Python-2.7.18" "https://www.python.org/ftp/python/2.7.18/Python-2.7.18.tgz#da3080e3b488f648a3d7a4560ddee895284c3380b11d6de75edb986526b9a814" standard verify_py27 copy_python_gdb ensurepip
+  install_package "Python-3.7.1" "https://www.python.org/ftp/python/3.7.1/Python-3.7.1.tgz#36c1b81ac29d0f8341f727ef40864d99d8206897be96be73dc34d4739c9c9f06" standard verify_py37 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/2.7.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/2.7.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.1.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.1.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.10.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.11-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.11.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.11.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.11.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.12-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.7`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-export PYTHON_BUILD_TCLTK_USE_PKGCONFIG=1
-export PYTHON_BUILD_CONFIGURE_WITH_DSYMUTIL=1
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
-install_git "Python-3.12-dev" "https://github.com/python/cpython" main standard verify_py312 copy_python_gdb ensurepip
+if has_tar_xz_support; then
+  install_package "Python-3.8.7" "https://www.python.org/ftp/python/3.8.7/Python-3.8.7.tar.xz#ddcc1df16bb5b87aa42ec5d20a5b902f2d088caa269b28e01590f97a798ec50a" standard verify_py38 copy_python_gdb ensurepip
+else
+  install_package "Python-3.8.7" "https://www.python.org/ftp/python/3.8.7/Python-3.8.7.tgz#20e5a04262f0af2eb9c19240d7ec368f385788bba2d8dfba7e74b20bab4d2bac" standard verify_py38 copy_python_gdb ensurepip
+fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.12.0a3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.10.10`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1s" "https://www.openssl.org/source/openssl-1.1.1s.tar.gz#c5ac01e760ee6ff0dab61d6b2bbd30146724d063eb322180c6f18a6f74e4b6aa" mac_openssl --if has_broken_mac_openssl
-install_package "readline-8.2" "https://ftpmirror.gnu.org/readline/readline-8.2.tar.gz#3feb7171f16a84ee82ca18a36d7b9be109a52c04f492a053331d7d1095007c35" mac_readline --if has_broken_mac_readline
+install_package "openssl-1.1.1o" "https://www.openssl.org/source/openssl-1.1.1o.tar.gz#9384a2b0570dd80358841464677115df785edb941c71211f75076d72fe6b438f" mac_openssl --if has_broken_mac_openssl
+install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-    install_package "Python-3.12.0a3" "https://www.python.org/ftp/python/3.12.0/Python-3.12.0a3.tar.xz#1b64b3075e0a9241974e580e09b09c9117a1c4e2be698039201ef1d8a73453d1" standard verify_py312 copy_python_gdb ensurepip
+    install_package "Python-3.10.10" "https://www.python.org/ftp/python/3.10.10/Python-3.10.10.tar.xz#0419e9085bf51b7a672009b3f50dbf1859acdf18ba725d0ec19aa5c8503f0ea3" standard verify_py310 copy_python_gdb ensurepip
 else
-    install_package "Python-3.12.0a3" "https://www.python.org/ftp/python/3.12.0/Python-3.12.0a3.tgz#fd414e6b6520171f5cefc5cba1067265187a322417f7bdec8d024db7fc8fbe96" standard verify_py312 copy_python_gdb ensurepip
+    install_package "Python-3.10.10" "https://www.python.org/ftp/python/3.10.10/Python-3.10.10.tgz#fba64559dde21ebdc953e4565e731573bb61159de8e4d4cedee70fb1196f610d" standard verify_py310 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.2.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.2.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.3.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.3.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.4.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.4.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.5.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.5.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.13` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.13`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.15` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.15`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.6.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.6.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.7`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
 install_package "openssl-1.1.0j" "https://www.openssl.org/source/old/1.1.0/openssl-1.1.0j.tar.gz#31bec6c203ce1a8e93d5994f4ed304c63ccf07676118b6634edded12ad1b3246" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.7.1" "https://www.python.org/ftp/python/3.7.1/Python-3.7.1.tar.xz#fa7e2b8e8c9402f192ad56dc4f814089d1c4466c97d780f5e5acc02c04243d6d" standard verify_py37 copy_python_gdb ensurepip
+  install_package "Python-3.7.7" "https://www.python.org/ftp/python/3.7.7/Python-3.7.7.tar.xz#06a0a9f1bf0d8cd1e4121194d666c4e28ddae4dd54346de6c343206599f02136" standard verify_py37 copy_python_gdb ensurepip
 else
-  install_package "Python-3.7.1" "https://www.python.org/ftp/python/3.7.1/Python-3.7.1.tgz#36c1b81ac29d0f8341f727ef40864d99d8206897be96be73dc34d4739c9c9f06" standard verify_py37 copy_python_gdb ensurepip
+  install_package "Python-3.7.7" "https://www.python.org/ftp/python/3.7.7/Python-3.7.7.tgz#8c8be91cd2648a1a0c251f04ea0bb4c2a5570feb9c45eaaa2241c785585b475a" standard verify_py37 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.13` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.13`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.15` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.15`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.16` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.16`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.3`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
 install_package "openssl-1.1.0j" "https://www.openssl.org/source/old/1.1.0/openssl-1.1.0j.tar.gz#31bec6c203ce1a8e93d5994f4ed304c63ccf07676118b6634edded12ad1b3246" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.7.7" "https://www.python.org/ftp/python/3.7.7/Python-3.7.7.tar.xz#06a0a9f1bf0d8cd1e4121194d666c4e28ddae4dd54346de6c343206599f02136" standard verify_py37 copy_python_gdb ensurepip
+  install_package "Python-3.8.3" "https://www.python.org/ftp/python/3.8.3/Python-3.8.3.tar.xz#dfab5ec723c218082fe3d5d7ae17ecbdebffa9a1aea4d64aa3a2ecdd2e795864" standard verify_py38 copy_python_gdb ensurepip
 else
-  install_package "Python-3.7.7" "https://www.python.org/ftp/python/3.7.7/Python-3.7.7.tgz#8c8be91cd2648a1a0c251f04ea0bb4c2a5570feb9c45eaaa2241c785585b475a" standard verify_py37 copy_python_gdb ensurepip
+  install_package "Python-3.8.3" "https://www.python.org/ftp/python/3.8.3/Python-3.8.3.tgz#6af6d4d2e010f9655518d0fc6738c7ff7069f10a4d2fbd55509e467f092a8b90" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.7.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.7.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.10`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.8.10" "https://www.python.org/ftp/python/3.8.10/Python-3.8.10.tar.xz#6af24a66093dd840bcccf371d4044a3027e655cf24591ce26e48022bc79219d9" standard verify_py38 copy_python_gdb ensurepip
 else
   install_package "Python-3.8.10" "https://www.python.org/ftp/python/3.8.10/Python-3.8.10.tgz#b37ac74d2cbad2590e7cd0dd2b3826c29afe89a734090a87bf8c03c45066cb65" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.11`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.8.11" "https://www.python.org/ftp/python/3.8.11/Python-3.8.11.tar.xz#fb1a1114ebfe9e97199603c6083e20b236a0e007a2c51f29283ffb50c1420fb2" standard verify_py38 copy_python_gdb ensurepip
 else
   install_package "Python-3.8.11" "https://www.python.org/ftp/python/3.8.11/Python-3.8.11.tgz#b77464ea80cec14581b86aeb7fb2ff02830e0abc7bcdc752b7b4bdfcd8f3e393" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.12`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.8.12" "https://www.python.org/ftp/python/3.8.12/Python-3.8.12.tar.xz#b1d3a76420375343b5e8a22fceb1ac65b77193e9ed27146524f0a9db058728ea" standard verify_py38 copy_python_gdb ensurepip
 else
   install_package "Python-3.8.12" "https://www.python.org/ftp/python/3.8.12/Python-3.8.12.tgz#316aa33f3b7707d041e73f246efedb297a70898c4b91f127f66dc8d80c596f1a" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.13` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.13`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1n" "https://www.openssl.org/source/openssl-1.1.1n.tar.gz#40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.8.13" "https://www.python.org/ftp/python/3.8.13/Python-3.8.13.tar.xz#6f309077012040aa39fe8f0c61db8c0fa1c45136763299d375c9e5756f09cf57" standard verify_py38 copy_python_gdb ensurepip
 else
   install_package "Python-3.8.13" "https://www.python.org/ftp/python/3.8.13/Python-3.8.13.tgz#903b92d76354366b1d9c4434d0c81643345cef87c1600adfa36095d7b00eede4" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.14`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1n" "https://www.openssl.org/source/openssl-1.1.1n.tar.gz#40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.8.14" "https://www.python.org/ftp/python/3.8.14/Python-3.8.14.tar.xz#5d77e278271ba803e9909a41a4f3baca006181c93ada682a5e5fe8dc4a24c5f3" standard verify_py38 copy_python_gdb ensurepip
 else
   install_package "Python-3.8.14" "https://www.python.org/ftp/python/3.8.14/Python-3.8.14.tgz#41f959c480c59211feb55d5a28851a56c7e22d02ef91035606ebb21011723c31" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.15` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.15`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1q" "https://www.openssl.org/source/openssl-1.1.1q.tar.gz#d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.8.15" "https://www.python.org/ftp/python/3.8.15/Python-3.8.15.tar.xz#5114fc7918a2a5e20eb5aac696b30c36f412c6ef24b13f5c9eb9e056982d9550" standard verify_py38 copy_python_gdb ensurepip
 else
   install_package "Python-3.8.15" "https://www.python.org/ftp/python/3.8.15/Python-3.8.15.tgz#924d46999df82aa2eaa1de5ca51d6800ffb56b4bf52486a28f40634e3362abc4" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.16` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.16`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1q" "https://www.openssl.org/source/openssl-1.1.1q.tar.gz#d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.8.16" "https://www.python.org/ftp/python/3.8.16/Python-3.8.16.tar.xz#d85dbb3774132473d8081dcb158f34a10ccad7a90b96c7e50ea4bb61f5ce4562" standard verify_py38 copy_python_gdb ensurepip
 else
   install_package "Python-3.8.16" "https://www.python.org/ftp/python/3.8.16/Python-3.8.16.tgz#71ca9d935637ed2feb59e90a368361dc91eca472a90acb1d344a2e8178ccaf10" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.9`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.0j" "https://www.openssl.org/source/old/1.1.0/openssl-1.1.0j.tar.gz#31bec6c203ce1a8e93d5994f4ed304c63ccf07676118b6634edded12ad1b3246" mac_openssl --if has_broken_mac_openssl
+install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.8.3" "https://www.python.org/ftp/python/3.8.3/Python-3.8.3.tar.xz#dfab5ec723c218082fe3d5d7ae17ecbdebffa9a1aea4d64aa3a2ecdd2e795864" standard verify_py38 copy_python_gdb ensurepip
+  install_package "Python-3.8.9" "https://www.python.org/ftp/python/3.8.9/Python-3.8.9.tar.xz#5e391f3ec45da2954419cab0beaefd8be38895ea5ce33577c3ec14940c4b9572" standard verify_py38 copy_python_gdb ensurepip
 else
-  install_package "Python-3.8.3" "https://www.python.org/ftp/python/3.8.3/Python-3.8.3.tgz#6af6d4d2e010f9655518d0fc6738c7ff7069f10a4d2fbd55509e467f092a8b90" standard verify_py38 copy_python_gdb ensurepip
+  install_package "Python-3.8.9" "https://www.python.org/ftp/python/3.8.9/Python-3.8.9.tgz#9779ec1df000bf86914cdd40860b88da56c1e61db59d37784beca14a259ac9e9" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.7`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
-install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
+install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.8.7" "https://www.python.org/ftp/python/3.8.7/Python-3.8.7.tar.xz#ddcc1df16bb5b87aa42ec5d20a5b902f2d088caa269b28e01590f97a798ec50a" standard verify_py38 copy_python_gdb ensurepip
+  install_package "Python-3.9.7" "https://www.python.org/ftp/python/3.9.7/Python-3.9.7.tar.xz#f8145616e68c00041d1a6399b76387390388f8359581abc24432bb969b5e3c57" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.8.7" "https://www.python.org/ftp/python/3.8.7/Python-3.8.7.tgz#20e5a04262f0af2eb9c19240d7ec368f385788bba2d8dfba7e74b20bab4d2bac" standard verify_py38 copy_python_gdb ensurepip
+  install_package "Python-3.9.7" "https://www.python.org/ftp/python/3.9.7/Python-3.9.7.tgz#a838d3f9360d157040142b715db34f0218e535333696a5569dc6f854604eb9d1" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.8.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.1`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.8.9" "https://www.python.org/ftp/python/3.8.9/Python-3.8.9.tar.xz#5e391f3ec45da2954419cab0beaefd8be38895ea5ce33577c3ec14940c4b9572" standard verify_py38 copy_python_gdb ensurepip
+    install_package "Python-3.9.1" "https://www.python.org/ftp/python/3.9.1/Python-3.9.1.tar.xz#991c3f8ac97992f3d308fefeb03a64db462574eadbff34ce8bc5bb583d9903ff" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.8.9" "https://www.python.org/ftp/python/3.8.9/Python-3.8.9.tgz#9779ec1df000bf86914cdd40860b88da56c1e61db59d37784beca14a259ac9e9" standard verify_py38 copy_python_gdb ensurepip
+    install_package "Python-3.9.1" "https://www.python.org/ftp/python/3.9.1/Python-3.9.1.tgz#29cb91ba038346da0bd9ab84a0a55a845d872c341a4da6879f462e94c741f117" standard verify_py39 copy_python_gdb ensurepip
 fi
+
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
+install_package "openssl-1.1.1i" "https://www.openssl.org/source/old/1.1.1/openssl-1.1.1i.tar.gz#e8be6a35fe41d10603c3cc635e93289ed00bf34b79671a3a4de64fcee00d5242" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-    install_package "Python-3.9.1" "https://www.python.org/ftp/python/3.9.1/Python-3.9.1.tar.xz#991c3f8ac97992f3d308fefeb03a64db462574eadbff34ce8bc5bb583d9903ff" standard verify_py39 copy_python_gdb ensurepip
+    install_package "Python-3.9.2" "https://www.python.org/ftp/python/3.9.2/Python-3.9.2.tar.xz#3c2034c54f811448f516668dce09d24008a0716c3a794dd8639b5388cbde247d" standard verify_py39 copy_python_gdb ensurepip
 else
-    install_package "Python-3.9.1" "https://www.python.org/ftp/python/3.9.1/Python-3.9.1.tgz#29cb91ba038346da0bd9ab84a0a55a845d872c341a4da6879f462e94c741f117" standard verify_py39 copy_python_gdb ensurepip
+    install_package "Python-3.9.2" "https://www.python.org/ftp/python/3.9.2/Python-3.9.2.tgz#7899e8a6f7946748830d66739f2d8f2b30214dad956e56b9ba216b3de5581519" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.8`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1l" "https://www.openssl.org/source/openssl-1.1.1l.tar.gz#0b7a3e5e59c34827fe0c3a74b7ec8baef302b98fa80088d7f9153aa16fa76bd1" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.10" "https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz#0a8fbfb5287ebc3a13e9baf3d54e08fa06778ffeccf6311aef821bb3a6586cc8" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.8" "https://www.python.org/ftp/python/3.9.8/Python-3.9.8.tar.xz#675ce09bf23c09836bf1969b744b1ea4c1a18c32788626632525f08444ebad5c" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.10" "https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tgz#1aa9c0702edbae8f6a2c95f70a49da8420aaa76b7889d3419c186bfc8c0e571e" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.8" "https://www.python.org/ftp/python/3.9.8/Python-3.9.8.tgz#7447fb8bb270942d620dd24faa7814b1383b61fa99029a240025fd81c1db8283" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.12`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1n" "https://www.openssl.org/source/openssl-1.1.1n.tar.gz#40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.11" "https://www.python.org/ftp/python/3.9.11/Python-3.9.11.tar.xz#66767a35309d724f370df9e503c172b4ee444f49d62b98bc4eca725123e26c49" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.12" "https://www.python.org/ftp/python/3.9.12/Python-3.9.12.tar.xz#2cd94b20670e4159c6d9ab57f91dbf255b97d8c1a1451d1c35f4ec1968adf971" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.11" "https://www.python.org/ftp/python/3.9.11/Python-3.9.11.tgz#3442400072f582ac2f0df30895558f08883b416c8c7877ea55d40d00d8a93112" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.12" "https://www.python.org/ftp/python/3.9.12/Python-3.9.12.tgz#70e08462ebf265012bd2be88a63d2149d880c73e53f1712b7bbbe93750560ae8" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.15`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1n" "https://www.openssl.org/source/openssl-1.1.1n.tar.gz#40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a" mac_openssl --if has_broken_mac_openssl
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
+install_package "openssl-1.1.1q" "https://www.openssl.org/source/openssl-1.1.1q.tar.gz#d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.12" "https://www.python.org/ftp/python/3.9.12/Python-3.9.12.tar.xz#2cd94b20670e4159c6d9ab57f91dbf255b97d8c1a1451d1c35f4ec1968adf971" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.15" "https://www.python.org/ftp/python/3.9.15/Python-3.9.15.tar.xz#12daff6809528d9f6154216950423c9e30f0e47336cb57c6aa0b4387dd5eb4b2" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.12" "https://www.python.org/ftp/python/3.9.12/Python-3.9.12.tgz#70e08462ebf265012bd2be88a63d2149d880c73e53f1712b7bbbe93750560ae8" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.15" "https://www.python.org/ftp/python/3.9.15/Python-3.9.15.tgz#48d1ccb29d5fbaf1fb8f912271d09f7450e426d4dfe95978ef6aaada70ece4d8" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.13` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.8.17`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1n" "https://www.openssl.org/source/openssl-1.1.1n.tar.gz#40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a" mac_openssl --if has_broken_mac_openssl
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
+install_package "openssl-1.1.1u" "https://www.openssl.org/source/openssl-1.1.1u.tar.gz#e2f8d84b523eecd06c7be7626830370300fbcc15386bf5142d72758f6963ebc6" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.13" "https://www.python.org/ftp/python/3.9.13/Python-3.9.13.tar.xz#125b0c598f1e15d2aa65406e83f792df7d171cdf38c16803b149994316a3080f" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.8.17" "https://www.python.org/ftp/python/3.8.17/Python-3.8.17.tar.xz#2e54b0c68191f16552f6de2e97a2396540572a219f6bbb28591a137cecc490a9" standard verify_py38 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.13" "https://www.python.org/ftp/python/3.9.13/Python-3.9.13.tgz#829b0d26072a44689a6b0810f5b4a3933ee2a0b8a4bfc99d7c5893ffd4f97c44" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.8.17" "https://www.python.org/ftp/python/3.8.17/Python-3.8.17.tgz#def428fa6cf61b66bcde72e3d9f7d07d33b2e4226f04f9d6fce8384c055113ae" standard verify_py38 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.14`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1n" "https://www.openssl.org/source/openssl-1.1.1n.tar.gz#40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.9.14" "https://www.python.org/ftp/python/3.9.14/Python-3.9.14.tar.xz#651304d216c8203fe0adf1a80af472d8e92c3b0e0a7892222ae4d9f3ae4debcf" standard verify_py39 copy_python_gdb ensurepip
 else
   install_package "Python-3.9.14" "https://www.python.org/ftp/python/3.9.14/Python-3.9.14.tgz#9201836e2c16361b2b7408680502393737d44f227333fe2e5729c7d5f6041675" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.15` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.16`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1q" "https://www.openssl.org/source/openssl-1.1.1q.tar.gz#d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.15" "https://www.python.org/ftp/python/3.9.15/Python-3.9.15.tar.xz#12daff6809528d9f6154216950423c9e30f0e47336cb57c6aa0b4387dd5eb4b2" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.16" "https://www.python.org/ftp/python/3.9.16/Python-3.9.16.tar.xz#22dddc099246dd2760665561e8adb7394ea0cc43a72684c6480f9380f7786439" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.15" "https://www.python.org/ftp/python/3.9.15/Python-3.9.15.tgz#48d1ccb29d5fbaf1fb8f912271d09f7450e426d4dfe95978ef6aaada70ece4d8" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.16" "https://www.python.org/ftp/python/3.9.16/Python-3.9.16.tgz#1ad539e9dbd2b42df714b69726e0693bc6b9d2d2c8e91c2e43204026605140c5" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.16` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.11`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1q" "https://www.openssl.org/source/openssl-1.1.1q.tar.gz#d7939ce614029cdff0b6c20f0e2e5703158a489a72b2507b8bd51bf8c8fd10ca" mac_openssl --if has_broken_mac_openssl
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
+install_package "openssl-1.1.1n" "https://www.openssl.org/source/openssl-1.1.1n.tar.gz#40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.16" "https://www.python.org/ftp/python/3.9.16/Python-3.9.16.tar.xz#22dddc099246dd2760665561e8adb7394ea0cc43a72684c6480f9380f7786439" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.11" "https://www.python.org/ftp/python/3.9.11/Python-3.9.11.tar.xz#66767a35309d724f370df9e503c172b4ee444f49d62b98bc4eca725123e26c49" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.16" "https://www.python.org/ftp/python/3.9.16/Python-3.9.16.tgz#1ad539e9dbd2b42df714b69726e0693bc6b9d2d2c8e91c2e43204026605140c5" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.11" "https://www.python.org/ftp/python/3.9.11/Python-3.9.11.tgz#3442400072f582ac2f0df30895558f08883b416c8c7877ea55d40d00d8a93112" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.12.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-prefer_openssl11
+prefer_openssl3
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1i" "https://www.openssl.org/source/old/1.1.1/openssl-1.1.1i.tar.gz#e8be6a35fe41d10603c3cc635e93289ed00bf34b79671a3a4de64fcee00d5242" mac_openssl --if has_broken_mac_openssl
-install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
+install_package "openssl-3.2.1" "https://www.openssl.org/source/openssl-3.2.1.tar.gz#83c7329fe52c850677d75e5d0b0ca245309b97e8ecbcfdc1dfdc4ab9fac35b39" mac_openssl --if has_broken_mac_openssl
+install_package "readline-8.2" "https://ftpmirror.gnu.org/readline/readline-8.2.tar.gz#3feb7171f16a84ee82ca18a36d7b9be109a52c04f492a053331d7d1095007c35" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-    install_package "Python-3.9.2" "https://www.python.org/ftp/python/3.9.2/Python-3.9.2.tar.xz#3c2034c54f811448f516668dce09d24008a0716c3a794dd8639b5388cbde247d" standard verify_py39 copy_python_gdb ensurepip
+    install_package "Python-3.12.2" "https://www.python.org/ftp/python/3.12.2/Python-3.12.2.tar.xz#be28112dac813d2053545c14bf13a16401a21877f1a69eb6ea5d84c4a0f3d870" standard verify_py312 copy_python_gdb ensurepip
 else
-    install_package "Python-3.9.2" "https://www.python.org/ftp/python/3.9.2/Python-3.9.2.tgz#7899e8a6f7946748830d66739f2d8f2b30214dad956e56b9ba216b3de5581519" standard verify_py39 copy_python_gdb ensurepip
+    install_package "Python-3.12.2" "https://www.python.org/ftp/python/3.12.2/Python-3.12.2.tgz#a7c4f6a9dc423d8c328003254ab0c9338b83037bd787d680826a5bf84308116e" standard verify_py312 copy_python_gdb ensurepip
 fi
-
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.5`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.0" "https://ftpmirror.gnu.org/readline/readline-8.0.tar.gz#e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
     install_package "Python-3.9.5" "https://www.python.org/ftp/python/3.9.5/Python-3.9.5.tar.xz#0c5a140665436ec3dbfbb79e2dfb6d192655f26ef4a29aeffcb6d1820d716d83" standard verify_py39 copy_python_gdb ensurepip
 else
     install_package "Python-3.9.5" "https://www.python.org/ftp/python/3.9.5/Python-3.9.5.tgz#e0fbd5b6e1ee242524430dee3c91baf4cbbaba4a72dd1674b90fda87b713c7ab" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.6`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
   install_package "Python-3.9.6" "https://www.python.org/ftp/python/3.9.6/Python-3.9.6.tar.xz#397920af33efc5b97f2e0b57e91923512ef89fc5b3c1d21dbfc8c4828ce0108a" standard verify_py39 copy_python_gdb ensurepip
 else
   install_package "Python-3.9.6" "https://www.python.org/ftp/python/3.9.6/Python-3.9.6.tgz#d0a35182e19e416fc8eae25a3dcd4d02d4997333e4ad1f2eee6010aadc3fe866" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.12.0`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-prefer_openssl11
+prefer_openssl3
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1k" "https://www.openssl.org/source/openssl-1.1.1k.tar.gz#892a0875b9872acd04a9fde79b1f943075d5ea162415de3047c327df33fbaee5" mac_openssl --if has_broken_mac_openssl
-install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
+install_package "openssl-3.1.2" "https://www.openssl.org/source/openssl-3.1.2.tar.gz#a0ce69b8b97ea6a35b96875235aa453b966ba3cba8af2de23657d8b6767d6539" mac_openssl --if has_broken_mac_openssl
+install_package "readline-8.2" "https://ftpmirror.gnu.org/readline/readline-8.2.tar.gz#3feb7171f16a84ee82ca18a36d7b9be109a52c04f492a053331d7d1095007c35" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.7" "https://www.python.org/ftp/python/3.9.7/Python-3.9.7.tar.xz#f8145616e68c00041d1a6399b76387390388f8359581abc24432bb969b5e3c57" standard verify_py39 copy_python_gdb ensurepip
+    install_package "Python-3.12.0" "https://www.python.org/ftp/python/3.12.0/Python-3.12.0.tar.xz#795c34f44df45a0e9b9710c8c71c15c671871524cd412ca14def212e8ccb155d" standard verify_py312 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.7" "https://www.python.org/ftp/python/3.9.7/Python-3.9.7.tgz#a838d3f9360d157040142b715db34f0218e535333696a5569dc6f854604eb9d1" standard verify_py39 copy_python_gdb ensurepip
+    install_package "Python-3.12.0" "https://www.python.org/ftp/python/3.12.0/Python-3.12.0.tgz#51412956d24a1ef7c97f1cb5f70e185c13e3de1f50d131c0aac6338080687afb" standard verify_py312 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.9`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
 install_package "openssl-1.1.1l" "https://www.openssl.org/source/openssl-1.1.1l.tar.gz#0b7a3e5e59c34827fe0c3a74b7ec8baef302b98fa80088d7f9153aa16fa76bd1" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.8" "https://www.python.org/ftp/python/3.9.8/Python-3.9.8.tar.xz#675ce09bf23c09836bf1969b744b1ea4c1a18c32788626632525f08444ebad5c" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.9" "https://www.python.org/ftp/python/3.9.9/Python-3.9.9.tar.xz#06828c04a573c073a4e51c4292a27c1be4ae26621c3edc7cf9318418ce3b6d27" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.8" "https://www.python.org/ftp/python/3.9.8/Python-3.9.8.tgz#7447fb8bb270942d620dd24faa7814b1383b61fa99029a240025fd81c1db8283" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.9" "https://www.python.org/ftp/python/3.9.9/Python-3.9.9.tgz#2cc7b67c1f3f66c571acc42479cdf691d8ed6b47bee12c9b68430413a17a44ea" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/3.9.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/3.9.17`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 prefer_openssl11
 export PYTHON_BUILD_CONFIGURE_WITH_OPENSSL=1
-install_package "openssl-1.1.1l" "https://www.openssl.org/source/openssl-1.1.1l.tar.gz#0b7a3e5e59c34827fe0c3a74b7ec8baef302b98fa80088d7f9153aa16fa76bd1" mac_openssl --if has_broken_mac_openssl
+# Avoid a compilation error when linking against OpenSSL built with SSLv3 support (fixed in 3.10.0) (#2181)
+export PYTHON_CFLAGS="-DOPENSSL_NO_SSL3${PYTHON_CFLAGS:+ $PYTHON_CFLAGS}"
+
+install_package "openssl-1.1.1u" "https://www.openssl.org/source/openssl-1.1.1u.tar.gz#e2f8d84b523eecd06c7be7626830370300fbcc15386bf5142d72758f6963ebc6" mac_openssl --if has_broken_mac_openssl
 install_package "readline-8.1" "https://ftpmirror.gnu.org/readline/readline-8.1.tar.gz#f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02" mac_readline --if has_broken_mac_readline
 if has_tar_xz_support; then
-  install_package "Python-3.9.9" "https://www.python.org/ftp/python/3.9.9/Python-3.9.9.tar.xz#06828c04a573c073a4e51c4292a27c1be4ae26621c3edc7cf9318418ce3b6d27" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.17" "https://www.python.org/ftp/python/3.9.17/Python-3.9.17.tar.xz#30ce057c44f283f8ed93606ccbdb8d51dd526bdc4c62cce5e0dc217bfa3e8cee" standard verify_py39 copy_python_gdb ensurepip
 else
-  install_package "Python-3.9.9" "https://www.python.org/ftp/python/3.9.9/Python-3.9.9.tgz#2cc7b67c1f3f66c571acc42479cdf691d8ed6b47bee12c9b68430413a17a44ea" standard verify_py39 copy_python_gdb ensurepip
+  install_package "Python-3.9.17" "https://www.python.org/ftp/python/3.9.17/Python-3.9.17.tgz#8ead58f669f7e19d777c3556b62fae29a81d7f06a7122ff9bc57f7dd82d7e014" standard verify_py39 copy_python_gdb ensurepip
 fi
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/activepython-2.7.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/activepython-2.7.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/activepython-3.5.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/activepython-3.5.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/activepython-3.6.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/activepython-3.6.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.5.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.5.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.6.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.6.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.6.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.6.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.7.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.7.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.8.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.8.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.9.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.9.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.9.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.9.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-1.9.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-1.9.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda-2.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda-2.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2.4.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2.4.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2.5.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2.5.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2018.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2018.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2019.03` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2019.03`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2019.07` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2019.07`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-2019.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-2019.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.1.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.1.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-4.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-4.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda2-5.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda2-5.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.4.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.4.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2.5.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2.5.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2018.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2018.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2019.03` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2019.03`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2019.07` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2019.07`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2019.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2019.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2020.02` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2020.02`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2020.07` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2020.07`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2020.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2020.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2021.04` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2021.04`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2021.05` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2021.05`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2021.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2021.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-2022.05` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-2022.05`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.1.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.1.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-4.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-4.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/anaconda3-5.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/anaconda3-5.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpy-22.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpy-22.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-20.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-20.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-20.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-20.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-20.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-20.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-21.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-21.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-22.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-22.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-22.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-22.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/graalpython-22.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/graalpython-22.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.5.4-rc1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.5.4-rc1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.7.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.7.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.7.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.7.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/jython-2.7.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/jython-2.7.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-22.9.0-2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-22.9.0-2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-4.10.1-4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.1-4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-4.10.1-5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.1-5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-4.10.3-10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-4.10.3-10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/mambaforge-pypy3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/mambaforge-pypy3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-2.2.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-2.2.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.0.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.0.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.0.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.0.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.10.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.10.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.16.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.16.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.4.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.4.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.7.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.7.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.8.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.8.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda-3.9.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda-3.9.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-2.7-4.8.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-2.7-4.8.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-3.18.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-3.18.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-3.19.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-3.19.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.0.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.0.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.1.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.1.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.21` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.21`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.27` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.27`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.30` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.30`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.3.31` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.3.31`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.4.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.4.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.5.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.5.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.6.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.6.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.7.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.7.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-4.7.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-4.7.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda2-latest` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda2-latest`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-2.2.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-2.2.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.0.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.0.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.0.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.0.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.10.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.10.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.16.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.16.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.18.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.18.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.19.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.19.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.4.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.4.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.10.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.11.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.11.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.12.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.12.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.8.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7-4.9.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7-4.9.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.7.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.7.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.10.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.11.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.11.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.12.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.12.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.8.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8-4.9.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8-4.9.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.8.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.8.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.10.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.11.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.11.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.12.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.12.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9-4.9.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9-4.9.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-3.9.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-3.9.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.0.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.0.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.1.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.1.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.2.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.2.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.21` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.21`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.27` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.27`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.30` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.30`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.3.31` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.3.31`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.4.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.4.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.5.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.5.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.6.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.6.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.7.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.7.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-4.7.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-4.7.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniconda3-latest` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniconda3-latest`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge-pypy3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge-pypy3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-22.9.0-2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-22.9.0-2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.1-1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.1-1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.1-3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.1-3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.1-5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.1-5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.10.3-10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.10.3-10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-4.9.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-4.9.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/miniforge3-latest` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/miniforge3-latest`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/nogil-3.9.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/nogil-3.9.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.1.3/Python-2.1.3/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.1.3/Python-2.1.3/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.2.3/Python-2.2.3/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.2.3/Python-2.2.3/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/001_fortify_crash_workaround.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.3.7/Python-2.3.7/001_fortify_crash_workaround.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/001_fortify_crash_workaround.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/001_fortify_crash_workaround.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/002_patch-posixmodule.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.0/Python-2.4/002_patch-posixmodule.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/001_fortify_crash_workaround.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/001_fortify_crash_workaround.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/002_patch-posixmodule.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.1/Python-2.4.1/002_patch-posixmodule.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/001_fortify_crash_workaround.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/001_fortify_crash_workaround.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/002_patch-posixmodule.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.2/Python-2.4.2/002_patch-posixmodule.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/001_fortify_crash_workaround.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/001_fortify_crash_workaround.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/002_patch-posixmodule.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.3/Python-2.4.3/002_patch-posixmodule.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/001_patch-posixmodule.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.4/Python-2.4.4/001_patch-posixmodule.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/001_patch-posixmodule.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.5/Python-2.4.5/001_patch-posixmodule.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/001_patch-posixmodule.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.4.6/Python-2.4.6/001_patch-posixmodule.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/002_darwin_c_source.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/002_darwin_c_source.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/003_osx_lp64.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/003_osx_lp64.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/004_osx_libffi.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/004_osx_libffi.patch`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 +	FFI_BAD_TYPEDEF - One of the ffi_type objects that ffi_prep_cif
 +		came across is bad.
 +
 +
 +Before making the call, the VALUES vector should be initialized 
 +with pointers to the appropriate argument values.
 +
-+To call the the function using the initialized ffi_cif, use the
++To call the function using the initialized ffi_cif, use the
 +ffi_call function:
 +
 +void ffi_call(ffi_cif *cif, void *fn, void *rvalue, void **avalues);
 +
 +	CIF is a pointer to the ffi_cif initialized specifically
 +		for this function.
 +
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/005_osx_failed_modules.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.0/Python-2.5/005_osx_failed_modules.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/002_darwin_c_source.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/002_darwin_c_source.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/003_osx_lp64.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/003_osx_lp64.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/004_osx_libffi.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/004_osx_libffi.patch`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 +	FFI_BAD_TYPEDEF - One of the ffi_type objects that ffi_prep_cif
 +		came across is bad.
 +
 +
 +Before making the call, the VALUES vector should be initialized 
 +with pointers to the appropriate argument values.
 +
-+To call the the function using the initialized ffi_cif, use the
++To call the function using the initialized ffi_cif, use the
 +ffi_call function:
 +
 +void ffi_call(ffi_cif *cif, void *fn, void *rvalue, void **avalues);
 +
 +	CIF is a pointer to the ffi_cif initialized specifically
 +		for this function.
 +
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/005_osx_failed_modules.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.1/Python-2.5.1/005_osx_failed_modules.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/002_darwin_c_source.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/002_darwin_c_source.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/003_osx_lp64.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/003_osx_lp64.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/004_osx_libffi.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/004_osx_libffi.patch`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 +	FFI_BAD_TYPEDEF - One of the ffi_type objects that ffi_prep_cif
 +		came across is bad.
 +
 +
 +Before making the call, the VALUES vector should be initialized 
 +with pointers to the appropriate argument values.
 +
-+To call the the function using the initialized ffi_cif, use the
++To call the function using the initialized ffi_cif, use the
 +ffi_call function:
 +
 +void ffi_call(ffi_cif *cif, void *fn, void *rvalue, void **avalues);
 +
 +	CIF is a pointer to the ffi_cif initialized specifically
 +		for this function.
 +
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/005_osx_failed_modules.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.2/Python-2.5.2/005_osx_failed_modules.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/002_darwin_c_source.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/002_darwin_c_source.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/003_osx_lp64.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/003_osx_lp64.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/004_osx_libffi.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/004_osx_libffi.patch`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 +	FFI_BAD_TYPEDEF - One of the ffi_type objects that ffi_prep_cif
 +		came across is bad.
 +
 +
 +Before making the call, the VALUES vector should be initialized 
 +with pointers to the appropriate argument values.
 +
-+To call the the function using the initialized ffi_cif, use the
++To call the function using the initialized ffi_cif, use the
 +ffi_call function:
 +
 +void ffi_call(ffi_cif *cif, void *fn, void *rvalue, void **avalues);
 +
 +	CIF is a pointer to the ffi_cif initialized specifically
 +		for this function.
 +
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/005_osx_failed_modules.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.3/Python-2.5.3/005_osx_failed_modules.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/002_darwin_c_source.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/002_darwin_c_source.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/003_osx_lp64.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/003_osx_lp64.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/004_osx_libffi.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/004_osx_libffi.patch`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 +	FFI_BAD_TYPEDEF - One of the ffi_type objects that ffi_prep_cif
 +		came across is bad.
 +
 +
 +Before making the call, the VALUES vector should be initialized 
 +with pointers to the appropriate argument values.
 +
-+To call the the function using the initialized ffi_cif, use the
++To call the function using the initialized ffi_cif, use the
 +ffi_call function:
 +
 +void ffi_call(ffi_cif *cif, void *fn, void *rvalue, void **avalues);
 +
 +	CIF is a pointer to the ffi_cif initialized specifically
 +		for this function.
 +
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/005_osx_failed_modules.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.4/Python-2.5.4/005_osx_failed_modules.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/002_darwin_c_source.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/002_darwin_c_source.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/003_osx_lp64.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/003_osx_lp64.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/004_osx_libffi.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/004_osx_libffi.patch`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 +	FFI_BAD_TYPEDEF - One of the ffi_type objects that ffi_prep_cif
 +		came across is bad.
 +
 +
 +Before making the call, the VALUES vector should be initialized 
 +with pointers to the appropriate argument values.
 +
-+To call the the function using the initialized ffi_cif, use the
++To call the function using the initialized ffi_cif, use the
 +ffi_call function:
 +
 +void ffi_call(ffi_cif *cif, void *fn, void *rvalue, void **avalues);
 +
 +	CIF is a pointer to the ffi_cif initialized specifically
 +		for this function.
 +
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/005_osx_failed_modules.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.5/Python-2.5.5/005_osx_failed_modules.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/002_darwin_c_source.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/002_darwin_c_source.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/003_osx_lp64.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/003_osx_lp64.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/004_osx_libffi.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/004_osx_libffi.patch`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 +	FFI_BAD_TYPEDEF - One of the ffi_type objects that ffi_prep_cif
 +		came across is bad.
 +
 +
 +Before making the call, the VALUES vector should be initialized 
 +with pointers to the appropriate argument values.
 +
-+To call the the function using the initialized ffi_cif, use the
++To call the function using the initialized ffi_cif, use the
 +ffi_call function:
 +
 +void ffi_call(ffi_cif *cif, void *fn, void *rvalue, void **avalues);
 +
 +	CIF is a pointer to the ffi_cif initialized specifically
 +		for this function.
 +
```

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/005_osx_failed_modules.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.5.6/Python-2.5.6/005_osx_failed_modules.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.0/Python-2.6/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.1/Python-2.6.1/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.2/Python-2.6.2/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.3/Python-2.6.3/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.4/Python-2.6.4/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.5/Python-2.6.5/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.6/Python-2.6.6/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.7/Python-2.6.7/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.8/Python-2.6.8/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/001_remove_systemstubs.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/001_remove_systemstubs.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/003_tk86.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/003_tk86.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.6.9/Python-2.6.9/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.0/Python-2.7/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.1/Python-2.7.1/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.10/Python-2.7.10/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.10/Python-2.7.10/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0001-Detect-arm64-in-configure.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0001-Detect-arm64-in-configure.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0002-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0002-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0003-Support-arm64-in-Mac-Tools-pythonw.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0003-Support-arm64-in-Mac-Tools-pythonw.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0004-Use-system-libffi-for-Mac-OS-10.15-and-up.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0004-Use-system-libffi-for-Mac-OS-10.15-and-up.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0005-ctypes-use-the-correct-ABI-for-variadic-functions.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0005-ctypes-use-the-correct-ABI-for-variadic-functions.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0006-ctypes-probe-libffi-for-ffi_closure_alloc-and-ffi_pr.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0006-ctypes-probe-libffi-for-ffi_closure_alloc-and-ffi_pr.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0007-Remove-QuickTime-from-link-args.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.18/Python-2.7.18/0007-Remove-QuickTime-from-link-args.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.2/Python-2.7.2/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.3/Python-2.7.3/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.4/Python-2.7.4/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.5/Python-2.7.5/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/012_fix_bundle_loader_for_new_osx.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.6/Python-2.7.6/012_fix_bundle_loader_for_new_osx.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.7/Python-2.7.7/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.8/Python-2.7.8/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/003_system_library_path_in_sys_path.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/003_system_library_path_in_sys_path.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/2.7.9/Python-2.7.9/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/001_patch-svnversion.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/001_patch-svnversion.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.0.1/Python-3.0.1/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.0/Python-3.1/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.1/Python-3.1.1/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.2/Python-3.1.2/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.3/Python-3.1.3/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.4/Python-3.1.4/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.1.5/Python-3.1.5/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0001-bpo-45350-Rerun-autoreconf-with-the-pkg-config-macro.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0001-bpo-45350-Rerun-autoreconf-with-the-pkg-config-macro.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0002-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.10.0/Python-3.10.0/0002-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/000_patch-setup.py.diff` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/000_patch-setup.py.diff`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/010_ssl_no_ssl2_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.0/Python-3.2/010_ssl_no_ssl2_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.1/Python-3.2.1/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.2/Python-3.2.2/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.3/Python-3.2.3/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.4/Python-3.2.4/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.5/Python-3.2.5/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.2.6/Python-3.2.6/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.0/Python-3.3.0/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.1/Python-3.3.1/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.2/Python-3.3.2/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.3/Python-3.3.3/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.4/Python-3.3.4/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.4/Python-3.3.4/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.5/Python-3.3.5/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.5/Python-3.3.5/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.6/Python-3.3.6/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.6/Python-3.3.6/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.3.7/Python-3.3.7/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.3.7/Python-3.3.7/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.0/Python-3.4.0/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.0/Python-3.4.0/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.1/Python-3.4.1/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.1/Python-3.4.1/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.4.2/Python-3.4.2/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.4.2/Python-3.4.2/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.5.2/Python-3.5.2/venv.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.2/Python-3.5.2/venv.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0001-Detect-arm64-in-configure.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0004-Detect-arm64-in-configure.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0002-bpo-36231-Support-building-on-macOS-without-usr-incl.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0002-bpo-36231-Support-building-on-macOS-without-usr-incl.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0003-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0003-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0004-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0004-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0005-BPO-41100-Support-macOS-11-when-building-GH-21113.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0005-BPO-41100-Support-macOS-11-when-building-GH-21113.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0006-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0006-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0007-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0007-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0008-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0003-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.10/Python-3.7.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.10/Python-3.7.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.11/Python-3.7.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.11/Python-3.7.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0004-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0004-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.14/Python-3.7.14/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.8/Python-3.7.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.8/Python-3.7.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.7.9/Python-3.7.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.7.9/Python-3.7.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.10/Python-3.8.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.10/Python-3.8.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.11/Python-3.8.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.11/Python-3.8.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.12/Python-3.8.12/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.12/Python-3.8.12/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.4/Python-3.8.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.4/Python-3.8.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.5/Python-3.8.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.5/Python-3.8.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.6/Python-3.8.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.6/Python-3.8.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.7/Python-3.8.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.7/Python-3.8.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.8/Python-3.8.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.8/Python-3.8.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.8.9/Python-3.8.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.8.9/Python-3.8.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.0/Python-3.9.0/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.0/Python-3.9.0/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.1/Python-3.9.1/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.1/Python-3.9.1/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.2/Python-3.9.2/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.2/Python-3.9.2/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.4/Python-3.9.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.4/Python-3.9.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.5/Python-3.9.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.5/Python-3.9.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.6/Python-3.9.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.6/Python-3.9.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/3.9.7/Python-3.9.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/3.9.7/Python-3.9.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/002_readline63.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/002_readline63.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/010_ssl_no_ssl3.patch` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/010_ssl_no_ssl3.patch`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-1.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-1.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.0.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.0.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.2.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.2.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.5.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.5.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.6.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.6.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-2.6.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-2.6.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-4.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-4.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-4.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-4.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.0.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.0.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-5.1.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-5.1.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-c-jit-latest` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-c-jit-latest`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-stm-2.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-stm-2.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy-stm-2.5.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy-stm-2.5.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.4.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.4.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.6.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.6.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.7.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.7.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2-5.7.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2-5.7.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.10.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.10.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.8.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.8.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-5.9.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-5.9.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-6.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-6.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.1.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.1.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.10-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.10-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.8-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.8-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy2.7-7.3.9-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy2.7-7.3.9-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3-2.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3-2.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3-2.4.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3-2.4.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.3-5.5-alpha` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.3-5.5-alpha`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.10.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.10.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.10.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.10.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.7-beta` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.7-beta`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.7.1-beta` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.7.1-beta`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.8.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.8.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-5.9.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-5.9.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-6.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-6.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-7.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-7.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.5-c-jit-latest` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.5-c-jit-latest`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.0.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.0.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.1.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.1.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.1.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.1.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.2.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.2.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.0` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.0`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.6-7.3.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.6-7.3.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.8-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.8-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-7.3.9-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-7.3.9-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.7-c-jit-latest` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.7-c-jit-latest`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.10-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.10-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.8-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.8-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.8-7.3.9-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.8-7.3.9-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.10-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.10-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.8-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.8-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pypy3.9-7.3.9-src` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pypy3.9-7.3.9-src`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.1` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.1`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/pyston-2.3.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/pyston-2.3.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.10` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.10`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.11` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.11`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.12` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.12`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.14` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.14`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.16` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.16`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.3` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.3`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.6` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.6`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.8` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.8`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-2.7.9` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-2.7.9`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.2.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.2.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.2.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.2.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.3.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.3.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.3.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.3.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.4-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.4-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.4.2` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.4.2`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.4.7` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.4.7`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.5.4` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.5.4`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-3.7.5` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-3.7.5`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/python-build/share/python-build/stackless-dev` & `autovenv-0.3.1671337561/autovenv/python-build/share/python-build/stackless-dev`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/util.py` & `autovenv-0.3.1671337561/autovenv/util.py`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv/virtualenvs.py` & `autovenv-0.3.1671337561/autovenv/virtualenvs.py`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/autovenv.egg-info/PKG-INFO` & `autovenv-0.3.1671337561/autovenv.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: autovenv
-Version: 0.3.1671337560
+Version: 0.3.1671337561
 Summary: virtualenv with less hassle
 Home-page: http://autovenv.readthedocs.org
 Author: Robert Lechte
 Author-email: robertlechte@gmail.com
 Classifier: Development Status :: 3 - Alpha
 License-File: LICENSE
+Requires-Dist: virtualenv
+Requires-Dist: appdirs
+Requires-Dist: pyyaml
 
 Virtual environments are great, but they can be a bit annoying to create, manage, and switch between. It gets even worse when multiple different python versions come into play. autovenv takes the annoyance away.
 
 Full documentation is at https://autovenv.readthedocs.org
```

### Comparing `autovenv-0.3.1671337560/autovenv.egg-info/SOURCES.txt` & `autovenv-0.3.1671337561/autovenv.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -67,27 +67,43 @@
 autovenv/python-build/share/python-build/3.1.2
 autovenv/python-build/share/python-build/3.1.3
 autovenv/python-build/share/python-build/3.1.4
 autovenv/python-build/share/python-build/3.1.5
 autovenv/python-build/share/python-build/3.10-dev
 autovenv/python-build/share/python-build/3.10.0
 autovenv/python-build/share/python-build/3.10.1
+autovenv/python-build/share/python-build/3.10.10
+autovenv/python-build/share/python-build/3.10.11
+autovenv/python-build/share/python-build/3.10.12
+autovenv/python-build/share/python-build/3.10.13
+autovenv/python-build/share/python-build/3.10.14
 autovenv/python-build/share/python-build/3.10.2
 autovenv/python-build/share/python-build/3.10.3
 autovenv/python-build/share/python-build/3.10.4
 autovenv/python-build/share/python-build/3.10.5
 autovenv/python-build/share/python-build/3.10.6
 autovenv/python-build/share/python-build/3.10.7
 autovenv/python-build/share/python-build/3.10.8
 autovenv/python-build/share/python-build/3.10.9
 autovenv/python-build/share/python-build/3.11-dev
 autovenv/python-build/share/python-build/3.11.0
 autovenv/python-build/share/python-build/3.11.1
+autovenv/python-build/share/python-build/3.11.2
+autovenv/python-build/share/python-build/3.11.3
+autovenv/python-build/share/python-build/3.11.4
+autovenv/python-build/share/python-build/3.11.5
+autovenv/python-build/share/python-build/3.11.6
+autovenv/python-build/share/python-build/3.11.7
+autovenv/python-build/share/python-build/3.11.8
 autovenv/python-build/share/python-build/3.12-dev
-autovenv/python-build/share/python-build/3.12.0a3
+autovenv/python-build/share/python-build/3.12.0
+autovenv/python-build/share/python-build/3.12.1
+autovenv/python-build/share/python-build/3.12.2
+autovenv/python-build/share/python-build/3.13-dev
+autovenv/python-build/share/python-build/3.13.0a5
 autovenv/python-build/share/python-build/3.2.0
 autovenv/python-build/share/python-build/3.2.1
 autovenv/python-build/share/python-build/3.2.2
 autovenv/python-build/share/python-build/3.2.3
 autovenv/python-build/share/python-build/3.2.4
 autovenv/python-build/share/python-build/3.2.5
 autovenv/python-build/share/python-build/3.2.6
@@ -146,14 +162,15 @@
 autovenv/python-build/share/python-build/3.7.10
 autovenv/python-build/share/python-build/3.7.11
 autovenv/python-build/share/python-build/3.7.12
 autovenv/python-build/share/python-build/3.7.13
 autovenv/python-build/share/python-build/3.7.14
 autovenv/python-build/share/python-build/3.7.15
 autovenv/python-build/share/python-build/3.7.16
+autovenv/python-build/share/python-build/3.7.17
 autovenv/python-build/share/python-build/3.7.2
 autovenv/python-build/share/python-build/3.7.3
 autovenv/python-build/share/python-build/3.7.4
 autovenv/python-build/share/python-build/3.7.5
 autovenv/python-build/share/python-build/3.7.6
 autovenv/python-build/share/python-build/3.7.7
 autovenv/python-build/share/python-build/3.7.8
@@ -164,14 +181,17 @@
 autovenv/python-build/share/python-build/3.8.10
 autovenv/python-build/share/python-build/3.8.11
 autovenv/python-build/share/python-build/3.8.12
 autovenv/python-build/share/python-build/3.8.13
 autovenv/python-build/share/python-build/3.8.14
 autovenv/python-build/share/python-build/3.8.15
 autovenv/python-build/share/python-build/3.8.16
+autovenv/python-build/share/python-build/3.8.17
+autovenv/python-build/share/python-build/3.8.18
+autovenv/python-build/share/python-build/3.8.19
 autovenv/python-build/share/python-build/3.8.2
 autovenv/python-build/share/python-build/3.8.3
 autovenv/python-build/share/python-build/3.8.4
 autovenv/python-build/share/python-build/3.8.5
 autovenv/python-build/share/python-build/3.8.6
 autovenv/python-build/share/python-build/3.8.7
 autovenv/python-build/share/python-build/3.8.8
@@ -182,14 +202,17 @@
 autovenv/python-build/share/python-build/3.9.10
 autovenv/python-build/share/python-build/3.9.11
 autovenv/python-build/share/python-build/3.9.12
 autovenv/python-build/share/python-build/3.9.13
 autovenv/python-build/share/python-build/3.9.14
 autovenv/python-build/share/python-build/3.9.15
 autovenv/python-build/share/python-build/3.9.16
+autovenv/python-build/share/python-build/3.9.17
+autovenv/python-build/share/python-build/3.9.18
+autovenv/python-build/share/python-build/3.9.19
 autovenv/python-build/share/python-build/3.9.2
 autovenv/python-build/share/python-build/3.9.4
 autovenv/python-build/share/python-build/3.9.5
 autovenv/python-build/share/python-build/3.9.6
 autovenv/python-build/share/python-build/3.9.7
 autovenv/python-build/share/python-build/3.9.8
 autovenv/python-build/share/python-build/3.9.9
@@ -248,29 +271,45 @@
 autovenv/python-build/share/python-build/anaconda3-2020.02
 autovenv/python-build/share/python-build/anaconda3-2020.07
 autovenv/python-build/share/python-build/anaconda3-2020.11
 autovenv/python-build/share/python-build/anaconda3-2021.04
 autovenv/python-build/share/python-build/anaconda3-2021.05
 autovenv/python-build/share/python-build/anaconda3-2021.11
 autovenv/python-build/share/python-build/anaconda3-2022.05
+autovenv/python-build/share/python-build/anaconda3-2022.10
+autovenv/python-build/share/python-build/anaconda3-2023.03
+autovenv/python-build/share/python-build/anaconda3-2023.03-0
+autovenv/python-build/share/python-build/anaconda3-2023.03-1
+autovenv/python-build/share/python-build/anaconda3-2023.07-0
+autovenv/python-build/share/python-build/anaconda3-2023.07-1
+autovenv/python-build/share/python-build/anaconda3-2023.07-2
+autovenv/python-build/share/python-build/anaconda3-2023.09-0
 autovenv/python-build/share/python-build/anaconda3-4.0.0
 autovenv/python-build/share/python-build/anaconda3-4.1.0
 autovenv/python-build/share/python-build/anaconda3-4.1.1
 autovenv/python-build/share/python-build/anaconda3-4.2.0
 autovenv/python-build/share/python-build/anaconda3-4.3.0
 autovenv/python-build/share/python-build/anaconda3-4.3.1
 autovenv/python-build/share/python-build/anaconda3-4.4.0
 autovenv/python-build/share/python-build/anaconda3-5.0.0
 autovenv/python-build/share/python-build/anaconda3-5.0.1
 autovenv/python-build/share/python-build/anaconda3-5.1.0
 autovenv/python-build/share/python-build/anaconda3-5.2.0
 autovenv/python-build/share/python-build/anaconda3-5.3.0
 autovenv/python-build/share/python-build/anaconda3-5.3.1
+autovenv/python-build/share/python-build/cinder-3.10-dev
 autovenv/python-build/share/python-build/cinder-3.8-dev
 autovenv/python-build/share/python-build/graalpy-22.3.0
+autovenv/python-build/share/python-build/graalpy-23.0.0
+autovenv/python-build/share/python-build/graalpy-23.1.0
+autovenv/python-build/share/python-build/graalpy-23.1.2
+autovenv/python-build/share/python-build/graalpy-24.0.0
+autovenv/python-build/share/python-build/graalpy-community-23.1.0
+autovenv/python-build/share/python-build/graalpy-community-23.1.2
+autovenv/python-build/share/python-build/graalpy-community-24.0.0
 autovenv/python-build/share/python-build/graalpython-20.1.0
 autovenv/python-build/share/python-build/graalpython-20.2.0
 autovenv/python-build/share/python-build/graalpython-20.3.0
 autovenv/python-build/share/python-build/graalpython-21.0.0
 autovenv/python-build/share/python-build/graalpython-21.1.0
 autovenv/python-build/share/python-build/graalpython-21.2.0
 autovenv/python-build/share/python-build/graalpython-21.3.0
@@ -287,31 +326,73 @@
 autovenv/python-build/share/python-build/jython-2.5.1
 autovenv/python-build/share/python-build/jython-2.5.2
 autovenv/python-build/share/python-build/jython-2.5.3
 autovenv/python-build/share/python-build/jython-2.5.4-rc1
 autovenv/python-build/share/python-build/jython-2.7.0
 autovenv/python-build/share/python-build/jython-2.7.1
 autovenv/python-build/share/python-build/jython-2.7.2
+autovenv/python-build/share/python-build/jython-2.7.3
 autovenv/python-build/share/python-build/jython-dev
 autovenv/python-build/share/python-build/mambaforge
+autovenv/python-build/share/python-build/mambaforge-22.11.1-3
+autovenv/python-build/share/python-build/mambaforge-22.11.1-4
+autovenv/python-build/share/python-build/mambaforge-22.9.0-0
+autovenv/python-build/share/python-build/mambaforge-22.9.0-1
 autovenv/python-build/share/python-build/mambaforge-22.9.0-2
+autovenv/python-build/share/python-build/mambaforge-22.9.0-3
+autovenv/python-build/share/python-build/mambaforge-23.1.0-0
+autovenv/python-build/share/python-build/mambaforge-23.1.0-1
+autovenv/python-build/share/python-build/mambaforge-23.1.0-2
+autovenv/python-build/share/python-build/mambaforge-23.1.0-3
+autovenv/python-build/share/python-build/mambaforge-23.1.0-4
+autovenv/python-build/share/python-build/mambaforge-23.10.0-0
+autovenv/python-build/share/python-build/mambaforge-23.11.0-0
+autovenv/python-build/share/python-build/mambaforge-23.3.0-0
+autovenv/python-build/share/python-build/mambaforge-23.3.1-0
+autovenv/python-build/share/python-build/mambaforge-23.3.1-1
 autovenv/python-build/share/python-build/mambaforge-4.10.1-4
 autovenv/python-build/share/python-build/mambaforge-4.10.1-5
+autovenv/python-build/share/python-build/mambaforge-4.10.2-0
+autovenv/python-build/share/python-build/mambaforge-4.10.3-0
+autovenv/python-build/share/python-build/mambaforge-4.10.3-1
 autovenv/python-build/share/python-build/mambaforge-4.10.3-10
+autovenv/python-build/share/python-build/mambaforge-4.10.3-2
+autovenv/python-build/share/python-build/mambaforge-4.10.3-3
+autovenv/python-build/share/python-build/mambaforge-4.10.3-4
+autovenv/python-build/share/python-build/mambaforge-4.10.3-5
+autovenv/python-build/share/python-build/mambaforge-4.10.3-6
+autovenv/python-build/share/python-build/mambaforge-4.10.3-7
+autovenv/python-build/share/python-build/mambaforge-4.10.3-8
+autovenv/python-build/share/python-build/mambaforge-4.10.3-9
+autovenv/python-build/share/python-build/mambaforge-4.11.0-0
+autovenv/python-build/share/python-build/mambaforge-4.11.0-1
+autovenv/python-build/share/python-build/mambaforge-4.11.0-2
+autovenv/python-build/share/python-build/mambaforge-4.11.0-3
+autovenv/python-build/share/python-build/mambaforge-4.11.0-4
+autovenv/python-build/share/python-build/mambaforge-4.12.0-0
+autovenv/python-build/share/python-build/mambaforge-4.12.0-1
+autovenv/python-build/share/python-build/mambaforge-4.12.0-2
+autovenv/python-build/share/python-build/mambaforge-4.12.0-3
+autovenv/python-build/share/python-build/mambaforge-4.13.0-1
+autovenv/python-build/share/python-build/mambaforge-4.14.0-0
+autovenv/python-build/share/python-build/mambaforge-4.14.0-1
+autovenv/python-build/share/python-build/mambaforge-4.14.0-2
 autovenv/python-build/share/python-build/mambaforge-pypy3
 autovenv/python-build/share/python-build/micropython-1.10
 autovenv/python-build/share/python-build/micropython-1.11
 autovenv/python-build/share/python-build/micropython-1.12
 autovenv/python-build/share/python-build/micropython-1.13
 autovenv/python-build/share/python-build/micropython-1.14
 autovenv/python-build/share/python-build/micropython-1.15
 autovenv/python-build/share/python-build/micropython-1.16
 autovenv/python-build/share/python-build/micropython-1.17
 autovenv/python-build/share/python-build/micropython-1.18
 autovenv/python-build/share/python-build/micropython-1.19.1
+autovenv/python-build/share/python-build/micropython-1.20.0
+autovenv/python-build/share/python-build/micropython-1.21.0
 autovenv/python-build/share/python-build/micropython-1.9.3
 autovenv/python-build/share/python-build/micropython-1.9.4
 autovenv/python-build/share/python-build/micropython-dev
 autovenv/python-build/share/python-build/miniconda-2.2.2
 autovenv/python-build/share/python-build/miniconda-3.0.0
 autovenv/python-build/share/python-build/miniconda-3.0.4
 autovenv/python-build/share/python-build/miniconda-3.0.5
@@ -343,36 +424,79 @@
 autovenv/python-build/share/python-build/miniconda2-4.7.10
 autovenv/python-build/share/python-build/miniconda2-4.7.12
 autovenv/python-build/share/python-build/miniconda2-latest
 autovenv/python-build/share/python-build/miniconda3-2.2.2
 autovenv/python-build/share/python-build/miniconda3-3.0.0
 autovenv/python-build/share/python-build/miniconda3-3.0.4
 autovenv/python-build/share/python-build/miniconda3-3.0.5
+autovenv/python-build/share/python-build/miniconda3-3.10-22.11.1-1
+autovenv/python-build/share/python-build/miniconda3-3.10-23.1.0-1
+autovenv/python-build/share/python-build/miniconda3-3.10-23.10.0-1
+autovenv/python-build/share/python-build/miniconda3-3.10-23.11.0-1
+autovenv/python-build/share/python-build/miniconda3-3.10-23.11.0-2
+autovenv/python-build/share/python-build/miniconda3-3.10-23.3.1-0
+autovenv/python-build/share/python-build/miniconda3-3.10-23.5.0-3
+autovenv/python-build/share/python-build/miniconda3-3.10-23.5.1-0
+autovenv/python-build/share/python-build/miniconda3-3.10-23.5.2-0
+autovenv/python-build/share/python-build/miniconda3-3.10-23.9.0-0
+autovenv/python-build/share/python-build/miniconda3-3.10-24.1.2-0
 autovenv/python-build/share/python-build/miniconda3-3.10.1
+autovenv/python-build/share/python-build/miniconda3-3.11-23.10.0-1
+autovenv/python-build/share/python-build/miniconda3-3.11-23.11.0-1
+autovenv/python-build/share/python-build/miniconda3-3.11-23.11.0-2
+autovenv/python-build/share/python-build/miniconda3-3.11-23.5.0-3
+autovenv/python-build/share/python-build/miniconda3-3.11-23.5.1-0
+autovenv/python-build/share/python-build/miniconda3-3.11-23.5.2-0
+autovenv/python-build/share/python-build/miniconda3-3.11-23.9.0-0
+autovenv/python-build/share/python-build/miniconda3-3.11-24.1.2-0
+autovenv/python-build/share/python-build/miniconda3-3.12-24.1.2-0
 autovenv/python-build/share/python-build/miniconda3-3.16.0
 autovenv/python-build/share/python-build/miniconda3-3.18.3
 autovenv/python-build/share/python-build/miniconda3-3.19.0
 autovenv/python-build/share/python-build/miniconda3-3.3.0
 autovenv/python-build/share/python-build/miniconda3-3.4.2
+autovenv/python-build/share/python-build/miniconda3-3.7-22.11.1-1
+autovenv/python-build/share/python-build/miniconda3-3.7-23.1.0-1
 autovenv/python-build/share/python-build/miniconda3-3.7-4.10.1
 autovenv/python-build/share/python-build/miniconda3-3.7-4.10.3
 autovenv/python-build/share/python-build/miniconda3-3.7-4.11.0
 autovenv/python-build/share/python-build/miniconda3-3.7-4.12.0
 autovenv/python-build/share/python-build/miniconda3-3.7-4.8.2
 autovenv/python-build/share/python-build/miniconda3-3.7-4.8.3
 autovenv/python-build/share/python-build/miniconda3-3.7-4.9.2
 autovenv/python-build/share/python-build/miniconda3-3.7.0
+autovenv/python-build/share/python-build/miniconda3-3.8-22.11.1-1
+autovenv/python-build/share/python-build/miniconda3-3.8-23.1.0-1
+autovenv/python-build/share/python-build/miniconda3-3.8-23.10.0-1
+autovenv/python-build/share/python-build/miniconda3-3.8-23.11.0-1
+autovenv/python-build/share/python-build/miniconda3-3.8-23.11.0-2
+autovenv/python-build/share/python-build/miniconda3-3.8-23.3.1-0
+autovenv/python-build/share/python-build/miniconda3-3.8-23.5.0-3
+autovenv/python-build/share/python-build/miniconda3-3.8-23.5.1-0
+autovenv/python-build/share/python-build/miniconda3-3.8-23.5.2-0
+autovenv/python-build/share/python-build/miniconda3-3.8-23.9.0-0
 autovenv/python-build/share/python-build/miniconda3-3.8-4.10.1
 autovenv/python-build/share/python-build/miniconda3-3.8-4.10.3
 autovenv/python-build/share/python-build/miniconda3-3.8-4.11.0
 autovenv/python-build/share/python-build/miniconda3-3.8-4.12.0
 autovenv/python-build/share/python-build/miniconda3-3.8-4.8.2
 autovenv/python-build/share/python-build/miniconda3-3.8-4.8.3
 autovenv/python-build/share/python-build/miniconda3-3.8-4.9.2
 autovenv/python-build/share/python-build/miniconda3-3.8.3
+autovenv/python-build/share/python-build/miniconda3-3.9-22.11.1-1
+autovenv/python-build/share/python-build/miniconda3-3.9-23.1.0-1
+autovenv/python-build/share/python-build/miniconda3-3.9-23.10.0-1
+autovenv/python-build/share/python-build/miniconda3-3.9-23.11.0-1
+autovenv/python-build/share/python-build/miniconda3-3.9-23.11.0-2
+autovenv/python-build/share/python-build/miniconda3-3.9-23.3.1-0
+autovenv/python-build/share/python-build/miniconda3-3.9-23.5.0-3
+autovenv/python-build/share/python-build/miniconda3-3.9-23.5.1-0
+autovenv/python-build/share/python-build/miniconda3-3.9-23.5.2-0
+autovenv/python-build/share/python-build/miniconda3-3.9-23.9.0-0
+autovenv/python-build/share/python-build/miniconda3-3.9-24.1.2-0
 autovenv/python-build/share/python-build/miniconda3-3.9-4.10.1
 autovenv/python-build/share/python-build/miniconda3-3.9-4.10.3
 autovenv/python-build/share/python-build/miniconda3-3.9-4.11.0
 autovenv/python-build/share/python-build/miniconda3-3.9-4.12.0
 autovenv/python-build/share/python-build/miniconda3-3.9-4.9.2
 autovenv/python-build/share/python-build/miniconda3-3.9.1
 autovenv/python-build/share/python-build/miniconda3-4.0.5
@@ -390,23 +514,64 @@
 autovenv/python-build/share/python-build/miniconda3-4.5.12
 autovenv/python-build/share/python-build/miniconda3-4.5.4
 autovenv/python-build/share/python-build/miniconda3-4.6.14
 autovenv/python-build/share/python-build/miniconda3-4.7.10
 autovenv/python-build/share/python-build/miniconda3-4.7.12
 autovenv/python-build/share/python-build/miniconda3-latest
 autovenv/python-build/share/python-build/miniforge-pypy3
+autovenv/python-build/share/python-build/miniforge3-22.11.1-3
+autovenv/python-build/share/python-build/miniforge3-22.11.1-4
+autovenv/python-build/share/python-build/miniforge3-22.9.0-0
+autovenv/python-build/share/python-build/miniforge3-22.9.0-1
 autovenv/python-build/share/python-build/miniforge3-22.9.0-2
+autovenv/python-build/share/python-build/miniforge3-22.9.0-3
+autovenv/python-build/share/python-build/miniforge3-23.1.0-0
+autovenv/python-build/share/python-build/miniforge3-23.1.0-1
+autovenv/python-build/share/python-build/miniforge3-23.1.0-2
+autovenv/python-build/share/python-build/miniforge3-23.1.0-3
+autovenv/python-build/share/python-build/miniforge3-23.1.0-4
+autovenv/python-build/share/python-build/miniforge3-23.10.0-0
+autovenv/python-build/share/python-build/miniforge3-23.11.0-0
+autovenv/python-build/share/python-build/miniforge3-23.3.0-0
+autovenv/python-build/share/python-build/miniforge3-23.3.1-0
+autovenv/python-build/share/python-build/miniforge3-23.3.1-1
 autovenv/python-build/share/python-build/miniforge3-4.10
 autovenv/python-build/share/python-build/miniforge3-4.10.1-1
 autovenv/python-build/share/python-build/miniforge3-4.10.1-3
 autovenv/python-build/share/python-build/miniforge3-4.10.1-5
+autovenv/python-build/share/python-build/miniforge3-4.10.2-0
+autovenv/python-build/share/python-build/miniforge3-4.10.3-0
+autovenv/python-build/share/python-build/miniforge3-4.10.3-1
 autovenv/python-build/share/python-build/miniforge3-4.10.3-10
+autovenv/python-build/share/python-build/miniforge3-4.10.3-2
+autovenv/python-build/share/python-build/miniforge3-4.10.3-3
+autovenv/python-build/share/python-build/miniforge3-4.10.3-4
+autovenv/python-build/share/python-build/miniforge3-4.10.3-5
+autovenv/python-build/share/python-build/miniforge3-4.10.3-6
+autovenv/python-build/share/python-build/miniforge3-4.10.3-7
+autovenv/python-build/share/python-build/miniforge3-4.10.3-8
+autovenv/python-build/share/python-build/miniforge3-4.10.3-9
+autovenv/python-build/share/python-build/miniforge3-4.11.0-0
+autovenv/python-build/share/python-build/miniforge3-4.11.0-1
+autovenv/python-build/share/python-build/miniforge3-4.11.0-2
+autovenv/python-build/share/python-build/miniforge3-4.11.0-3
+autovenv/python-build/share/python-build/miniforge3-4.11.0-4
+autovenv/python-build/share/python-build/miniforge3-4.12.0-0
+autovenv/python-build/share/python-build/miniforge3-4.12.0-1
+autovenv/python-build/share/python-build/miniforge3-4.12.0-2
+autovenv/python-build/share/python-build/miniforge3-4.12.0-3
+autovenv/python-build/share/python-build/miniforge3-4.13.0-0
+autovenv/python-build/share/python-build/miniforge3-4.13.0-1
+autovenv/python-build/share/python-build/miniforge3-4.14.0-0
+autovenv/python-build/share/python-build/miniforge3-4.14.0-1
+autovenv/python-build/share/python-build/miniforge3-4.14.0-2
 autovenv/python-build/share/python-build/miniforge3-4.9.2
 autovenv/python-build/share/python-build/miniforge3-latest
 autovenv/python-build/share/python-build/nogil-3.9.10
+autovenv/python-build/share/python-build/nogil-3.9.10-1
 autovenv/python-build/share/python-build/pypy-1.5-src
 autovenv/python-build/share/python-build/pypy-1.6
 autovenv/python-build/share/python-build/pypy-1.7
 autovenv/python-build/share/python-build/pypy-1.8
 autovenv/python-build/share/python-build/pypy-1.9
 autovenv/python-build/share/python-build/pypy-2.0
 autovenv/python-build/share/python-build/pypy-2.0-src
@@ -496,14 +661,24 @@
 autovenv/python-build/share/python-build/pypy2.7-7.2.0-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.0
 autovenv/python-build/share/python-build/pypy2.7-7.3.0-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.1
 autovenv/python-build/share/python-build/pypy2.7-7.3.1-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.10
 autovenv/python-build/share/python-build/pypy2.7-7.3.10-src
+autovenv/python-build/share/python-build/pypy2.7-7.3.11
+autovenv/python-build/share/python-build/pypy2.7-7.3.11-src
+autovenv/python-build/share/python-build/pypy2.7-7.3.12
+autovenv/python-build/share/python-build/pypy2.7-7.3.12-src
+autovenv/python-build/share/python-build/pypy2.7-7.3.13
+autovenv/python-build/share/python-build/pypy2.7-7.3.13-src
+autovenv/python-build/share/python-build/pypy2.7-7.3.14
+autovenv/python-build/share/python-build/pypy2.7-7.3.14-src
+autovenv/python-build/share/python-build/pypy2.7-7.3.15
+autovenv/python-build/share/python-build/pypy2.7-7.3.15-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.2
 autovenv/python-build/share/python-build/pypy2.7-7.3.2-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.3
 autovenv/python-build/share/python-build/pypy2.7-7.3.3-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.4
 autovenv/python-build/share/python-build/pypy2.7-7.3.4-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.5
@@ -514,14 +689,22 @@
 autovenv/python-build/share/python-build/pypy2.7-7.3.8-src
 autovenv/python-build/share/python-build/pypy2.7-7.3.9
 autovenv/python-build/share/python-build/pypy2.7-7.3.9-src
 autovenv/python-build/share/python-build/pypy3-2.3.1
 autovenv/python-build/share/python-build/pypy3-2.3.1-src
 autovenv/python-build/share/python-build/pypy3-2.4.0
 autovenv/python-build/share/python-build/pypy3-2.4.0-src
+autovenv/python-build/share/python-build/pypy3.10-7.3.12
+autovenv/python-build/share/python-build/pypy3.10-7.3.12-src
+autovenv/python-build/share/python-build/pypy3.10-7.3.13
+autovenv/python-build/share/python-build/pypy3.10-7.3.13-src
+autovenv/python-build/share/python-build/pypy3.10-7.3.14
+autovenv/python-build/share/python-build/pypy3.10-7.3.14-src
+autovenv/python-build/share/python-build/pypy3.10-7.3.15
+autovenv/python-build/share/python-build/pypy3.10-7.3.15-src
 autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1
 autovenv/python-build/share/python-build/pypy3.3-5.2-alpha1-src
 autovenv/python-build/share/python-build/pypy3.3-5.5-alpha
 autovenv/python-build/share/python-build/pypy3.3-5.5-alpha-src
 autovenv/python-build/share/python-build/pypy3.5-5.10.0
 autovenv/python-build/share/python-build/pypy3.5-5.10.0-src
 autovenv/python-build/share/python-build/pypy3.5-5.10.1
@@ -570,24 +753,36 @@
 autovenv/python-build/share/python-build/pypy3.7-7.3.8
 autovenv/python-build/share/python-build/pypy3.7-7.3.8-src
 autovenv/python-build/share/python-build/pypy3.7-7.3.9
 autovenv/python-build/share/python-build/pypy3.7-7.3.9-src
 autovenv/python-build/share/python-build/pypy3.7-c-jit-latest
 autovenv/python-build/share/python-build/pypy3.8-7.3.10
 autovenv/python-build/share/python-build/pypy3.8-7.3.10-src
+autovenv/python-build/share/python-build/pypy3.8-7.3.11
+autovenv/python-build/share/python-build/pypy3.8-7.3.11-src
 autovenv/python-build/share/python-build/pypy3.8-7.3.6
 autovenv/python-build/share/python-build/pypy3.8-7.3.6-src
 autovenv/python-build/share/python-build/pypy3.8-7.3.7
 autovenv/python-build/share/python-build/pypy3.8-7.3.7-src
 autovenv/python-build/share/python-build/pypy3.8-7.3.8
 autovenv/python-build/share/python-build/pypy3.8-7.3.8-src
 autovenv/python-build/share/python-build/pypy3.8-7.3.9
 autovenv/python-build/share/python-build/pypy3.8-7.3.9-src
 autovenv/python-build/share/python-build/pypy3.9-7.3.10
 autovenv/python-build/share/python-build/pypy3.9-7.3.10-src
+autovenv/python-build/share/python-build/pypy3.9-7.3.11
+autovenv/python-build/share/python-build/pypy3.9-7.3.11-src
+autovenv/python-build/share/python-build/pypy3.9-7.3.12
+autovenv/python-build/share/python-build/pypy3.9-7.3.12-src
+autovenv/python-build/share/python-build/pypy3.9-7.3.13
+autovenv/python-build/share/python-build/pypy3.9-7.3.13-src
+autovenv/python-build/share/python-build/pypy3.9-7.3.14
+autovenv/python-build/share/python-build/pypy3.9-7.3.14-src
+autovenv/python-build/share/python-build/pypy3.9-7.3.15
+autovenv/python-build/share/python-build/pypy3.9-7.3.15-src
 autovenv/python-build/share/python-build/pypy3.9-7.3.8
 autovenv/python-build/share/python-build/pypy3.9-7.3.8-src
 autovenv/python-build/share/python-build/pypy3.9-7.3.9
 autovenv/python-build/share/python-build/pypy3.9-7.3.9-src
 autovenv/python-build/share/python-build/pyston-2.2
 autovenv/python-build/share/python-build/pyston-2.3
 autovenv/python-build/share/python-build/pyston-2.3.1
@@ -807,23 +1002,34 @@
 autovenv/python-build/share/python-build/patches/3.3.4/Python-3.3.4/010_ssl_no_ssl3.patch
 autovenv/python-build/share/python-build/patches/3.3.5/Python-3.3.5/010_ssl_no_ssl3.patch
 autovenv/python-build/share/python-build/patches/3.3.6/Python-3.3.6/010_ssl_no_ssl3.patch
 autovenv/python-build/share/python-build/patches/3.3.7/Python-3.3.7/010_ssl_no_ssl3.patch
 autovenv/python-build/share/python-build/patches/3.4.0/Python-3.4.0/010_ssl_no_ssl3.patch
 autovenv/python-build/share/python-build/patches/3.4.1/Python-3.4.1/010_ssl_no_ssl3.patch
 autovenv/python-build/share/python-build/patches/3.4.2/Python-3.4.2/010_ssl_no_ssl3.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0001-bpo-27987-pymalloc-align-by-16bytes-on-64bit-platfor.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0002-bpo-27987-align-PyGC_Head-to-alignof-long-double-GH-.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0003-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0004-Detect-arm64-in-configure.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0005-BPO-41100-Support-macOS-11-when-building-GH-21113.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0006-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0007-Port-ctypes-and-system-libffi-patch-for-arm64-macOS-.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0008-bpo-36231-Support-building-on-macOS-without-usr-incl.patch
+autovenv/python-build/share/python-build/patches/3.5.10/Python-3.5.10/0009-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
 autovenv/python-build/share/python-build/patches/3.5.2/Python-3.5.2/venv.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0001-Detect-arm64-in-configure.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0002-bpo-36231-Support-building-on-macOS-without-usr-incl.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0003-Fix-macOS-_tkinter-use-of-Tck-Tk-in-Library-Framewor.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0004-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0005-BPO-41100-Support-macOS-11-when-building-GH-21113.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0006-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0007-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
 autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0008-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0009-bpo-27987-pymalloc-align-by-16bytes-on-64bit-platfor.patch
+autovenv/python-build/share/python-build/patches/3.6.15/Python-3.6.15/0010-bpo-27987-align-PyGC_Head-to-alignof-long-double-GH-.patch
 autovenv/python-build/share/python-build/patches/3.7.10/Python-3.7.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.7.11/Python-3.7.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
 autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
 autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
 autovenv/python-build/share/python-build/patches/3.7.12/Python-3.7.12/0004-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.7.13/Python-3.7.13/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
@@ -836,14 +1042,17 @@
 autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
 autovenv/python-build/share/python-build/patches/3.7.15/Python-3.7.15/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
 autovenv/python-build/share/python-build/patches/3.7.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
 autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
 autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
 autovenv/python-build/share/python-build/patches/3.7.16/Python-3.7.16/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
 autovenv/python-build/share/python-build/patches/3.7.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
+autovenv/python-build/share/python-build/patches/3.7.17/Python-3.7.17/0001-Port-ctypes-and-system-libffi-patches-for-arm64-macO.patch
+autovenv/python-build/share/python-build/patches/3.7.17/Python-3.7.17/0002-bpo-41100-fix-_decimal-for-arm64-Mac-OS-GH-21228.patch
+autovenv/python-build/share/python-build/patches/3.7.17/Python-3.7.17/0003-bpo-42351-Avoid-error-when-opening-header-with-non-U.patch
 autovenv/python-build/share/python-build/patches/3.7.8/Python-3.7.8/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.7.9/Python-3.7.9/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.8.10/Python-3.8.10/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.8.11/Python-3.8.11/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.8.12/Python-3.8.12/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.8.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
 autovenv/python-build/share/python-build/patches/3.8.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
@@ -858,14 +1067,16 @@
 autovenv/python-build/share/python-build/patches/3.9.15/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
 autovenv/python-build/share/python-build/patches/3.9.16/openssl-1.1.1q/openssl_1.1.1q_fix_c_include.patch
 autovenv/python-build/share/python-build/patches/3.9.2/Python-3.9.2/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.9.4/Python-3.9.4/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.9.5/Python-3.9.5/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.9.6/Python-3.9.6/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
 autovenv/python-build/share/python-build/patches/3.9.7/Python-3.9.7/0001-bpo-45405-Prevent-internal-configure-error-when-runn.patch
+autovenv/python-build/share/python-build/patches/cinder-3.10-dev/Cinder-3.10-dev/001-disable-werror.patch
+autovenv/python-build/share/python-build/patches/cinder-3.8-dev/Cinder-3.8-dev/001-disable-werror.patch
 autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/002_readline63.patch
 autovenv/python-build/share/python-build/patches/stackless-3.2.2/stackless-322-export/010_ssl_no_ssl3.patch
 autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/002_readline63.patch
 autovenv/python-build/share/python-build/patches/stackless-3.2.5/stackless-325-export/010_ssl_no_ssl3.patch
 scripts/autovenv-build
 scripts/autovenv-pythons-available
 scripts/autovenv.sh
```

### Comparing `autovenv-0.3.1671337560/scripts/autovenv-build` & `autovenv-0.3.1671337561/scripts/autovenv-build`

 * *Files identical despite different names*

### Comparing `autovenv-0.3.1671337560/setup.py` & `autovenv-0.3.1671337561/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from setuptools import setup, find_packages
 
 setup(
     name="autovenv",
-    version="0.3.1671337560",
+    version="0.3.1671337561",
     description="virtualenv with less hassle",
     url="http://autovenv.readthedocs.org",
     long_description="Virtual environments are great, but they can be a bit annoying to create, manage, and switch between. It gets even worse when multiple different python versions come into play. autovenv takes the annoyance away.\n\nFull documentation is at https://autovenv.readthedocs.org",
     author="Robert Lechte",
     author_email="robertlechte@gmail.com",
     install_requires=["virtualenv", "appdirs", "pyyaml"],
     packages=find_packages(),
```

### Comparing `autovenv-0.3.1671337560/tests/test_autovenv.py` & `autovenv-0.3.1671337561/tests/test_autovenv.py`

 * *Files identical despite different names*

