# Comparing `tmp/hw2latex-0.1.2.tar.gz` & `tmp/hw2latex-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hw2latex-0.1.2.tar", max compression
+gzip compressed data, was "hw2latex-0.1.3.tar", max compression
```

## Comparing `hw2latex-0.1.2.tar` & `hw2latex-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-31 09:50:35.051839 hw2latex-0.1.2/hw2latex/__init__.py
--rw-r--r--   0        0        0      977 2024-03-31 10:53:38.943835 hw2latex-0.1.2/hw2latex/hw2latex.py
--rw-r--r--   0        0        0      312 2024-03-31 10:54:37.452961 hw2latex-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       31 2024-03-31 09:53:53.735976 hw2latex-0.1.2/README.md
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 hw2latex-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-31 09:50:35.051839 hw2latex-0.1.3/hw2latex/__init__.py
+-rw-r--r--   0        0        0     1322 2024-04-01 11:55:14.958135 hw2latex-0.1.3/hw2latex/hw2latex.py
+-rw-r--r--   0        0        0      312 2024-04-01 12:07:31.672714 hw2latex-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-03-31 09:53:53.735976 hw2latex-0.1.3/README.md
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 hw2latex-0.1.3/PKG-INFO
```

