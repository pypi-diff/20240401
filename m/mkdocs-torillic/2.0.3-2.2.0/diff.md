# Comparing `tmp/mkdocs-torillic-2.0.3.tar.gz` & `tmp/mkdocs-torillic-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-torillic-2.0.3.tar", last modified: Sun Mar 31 20:00:28 2024, max compression
+gzip compressed data, was "mkdocs-torillic-2.2.0.tar", last modified: Mon Apr  1 13:32:30 2024, max compression
```

## Comparing `mkdocs-torillic-2.0.3.tar` & `mkdocs-torillic-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 20:00:28.961000 mkdocs-torillic-2.0.3/
--rw-rw-rw-   0        0        0      117 2024-03-31 20:00:28.922000 mkdocs-torillic-2.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-31 20:00:28.898000 mkdocs-torillic-2.0.3/mkdocs_torillic.egg-info/
--rw-rw-rw-   0        0        0      117 2024-03-31 20:00:28.000000 mkdocs-torillic-2.0.3/mkdocs_torillic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-03-31 20:00:28.000000 mkdocs-torillic-2.0.3/mkdocs_torillic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 20:00:28.000000 mkdocs-torillic-2.0.3/mkdocs_torillic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-03-31 20:00:28.000000 mkdocs-torillic-2.0.3/mkdocs_torillic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-03-31 20:00:28.000000 mkdocs-torillic-2.0.3/mkdocs_torillic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      198 2024-03-30 19:19:26.000000 mkdocs-torillic-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 20:00:28.952000 mkdocs-torillic-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-31 20:00:28.848000 mkdocs-torillic-2.0.3/torillic/
--rw-rw-rw-   0        0        0        0 2024-03-28 20:52:08.000000 mkdocs-torillic-2.0.3/torillic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.821000 mkdocs-torillic-2.2.0/
+-rw-rw-rw-   0        0        0      364 2024-04-01 13:32:30.808000 mkdocs-torillic-2.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.248000 mkdocs-torillic-2.2.0/mkdocs_torillic/
+-rw-rw-rw-   0        0        0        0 2024-04-01 13:30:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.322000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.349000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.460000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/
+-rw-rw-rw-   0        0        0     4195 2024-04-01 13:30:48.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/attrib.json
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.537000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/coins/
+-rw-rw-rw-   0        0        0      932 2024-04-01 13:30:48.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/coins/copper.png
+-rw-rw-rw-   0        0        0     1027 2024-04-01 13:30:48.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/coins/electrum.png
+-rw-rw-rw-   0        0        0      902 2024-04-01 13:30:48.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/coins/gold.png
+-rw-rw-rw-   0        0        0     1024 2024-04-01 13:30:48.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/coins/platinum.png
+-rw-rw-rw-   0        0        0      929 2024-04-01 13:30:48.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/coins/silver.png
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.205000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.622000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/
+-rw-rw-rw-   0        0        0   258792 2024-04-01 13:30:48.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-Bold.ttf
+-rw-rw-rw-   0        0        0   257292 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   254808 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-Italic.ttf
+-rw-rw-rw-   0        0        0   256112 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/Alegreya/Alegreya-Regular.ttf
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.711000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/
+-rw-rw-rw-   0        0        0   112116 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-Bold.ttf
+-rw-rw-rw-   0        0        0   114268 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   109440 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-Italic.ttf
+-rw-rw-rw-   0        0        0   106512 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/CrimsonText/CrimsonText-Regular.ttf
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.788000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/
+-rw-rw-rw-   0        0        0   120316 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-Bold.ttf
+-rw-rw-rw-   0        0        0   101956 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   102004 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-Italic.ttf
+-rw-rw-rw-   0        0        0   120456 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/fonts/SourceCodePro/SourceCodePro-Regular.ttf
+-rw-rw-rw-   0        0        0   291485 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/paper-texture.png
+-rw-rw-rw-   0        0        0   129962 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/splash.png
+-rw-rw-rw-   0        0        0  4661906 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/assets/torillic-bg.jpg
+-rw-rw-rw-   0        0        0     9659 2024-04-01 13:30:49.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic/torillic.css
+-rw-rw-rw-   0        0        0      142 2024-04-01 13:30:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/css/torillic.css
+-rw-rw-rw-   0        0        0     1173 2024-04-01 13:30:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/main.html
+-rw-rw-rw-   0        0        0       14 2024-04-01 13:30:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic/mkdocs_theme.yml
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:30.803000 mkdocs-torillic-2.2.0/mkdocs_torillic.egg-info/
+-rw-rw-rw-   0        0        0      364 2024-04-01 13:32:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1804 2024-04-01 13:32:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 13:32:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-01 13:32:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-01 13:32:30.000000 mkdocs-torillic-2.2.0/mkdocs_torillic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      599 2024-04-01 13:31:49.000000 mkdocs-torillic-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 13:32:30.819000 mkdocs-torillic-2.2.0/setup.cfg
```

