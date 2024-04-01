# Comparing `tmp/CustomChat-1.0.3.tar.gz` & `tmp/CustomChat-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomChat-1.0.3.tar", last modified: Sun Mar 31 21:49:31 2024, max compression
+gzip compressed data, was "CustomChat-1.0.4.tar", last modified: Mon Apr  1 21:57:40 2024, max compression
```

## Comparing `CustomChat-1.0.3.tar` & `CustomChat-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-03-31 21:49:31.165537 CustomChat-1.0.3/
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-03-31 21:49:31.165537 CustomChat-1.0.3/CustomChat.egg-info/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       76 2024-03-31 21:49:31.000000 CustomChat-1.0.3/CustomChat.egg-info/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      195 2024-03-31 21:49:31.000000 CustomChat-1.0.3/CustomChat.egg-info/SOURCES.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-03-31 21:49:31.000000 CustomChat-1.0.3/CustomChat.egg-info/dependency_links.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-03-31 21:49:31.000000 CustomChat-1.0.3/CustomChat.egg-info/requires.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-03-31 21:49:31.000000 CustomChat-1.0.3/CustomChat.egg-info/top_level.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     1186 2024-03-09 18:39:04.000000 CustomChat-1.0.3/LICENSE
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       76 2024-03-31 21:49:31.165537 CustomChat-1.0.3/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     2484 2024-03-16 14:25:48.000000 CustomChat-1.0.3/README.md
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-03-31 21:49:31.165537 CustomChat-1.0.3/setup.cfg
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      203 2024-03-31 21:48:45.000000 CustomChat-1.0.3/setup.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 21:57:40.124383 CustomChat-1.0.4/
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 21:57:40.124383 CustomChat-1.0.4/CustomChat/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       80 2024-03-31 21:26:32.000000 CustomChat-1.0.4/CustomChat/__init__.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)    30996 2024-03-31 21:39:42.000000 CustomChat-1.0.4/CustomChat/app.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      189 2024-03-02 23:52:49.000000 CustomChat-1.0.4/CustomChat/configuration.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      940 2024-03-31 21:36:42.000000 CustomChat-1.0.4/CustomChat/main.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:30.000000 CustomChat-1.0.4/CustomChat/new_com.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:13.000000 CustomChat-1.0.4/CustomChat/new_words.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 21:57:40.124383 CustomChat-1.0.4/CustomChat.egg-info/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2963 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      321 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/SOURCES.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/dependency_links.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/requires.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/top_level.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2963 2024-04-01 21:57:40.124383 CustomChat-1.0.4/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2456 2024-03-31 22:00:54.000000 CustomChat-1.0.4/README.md
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-01 21:57:40.124383 CustomChat-1.0.4/setup.cfg
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      808 2024-04-01 21:57:29.000000 CustomChat-1.0.4/setup.py
```

### Comparing `CustomChat-1.0.3/README.md` & `CustomChat-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 CustomChat is an easily customizable AI chatbot powered by Jimbot AI. Whether you're running it on an online compiler or locally, CustomChat empowers you to tailor it to your specific needs.
 
 ## Installation
 
 To install CustomChat, follow these steps:
 
-1. Download the zip file from the latest release and unzip it.
-
-2. Navigate to the CustomChat directory:
-   <pre><code>cd CustomChat</code></pre>
+1. Download the package with pip:
+   <pre><code>pip install CustomChat</code></pre>
    
-3. Run the code:
-   <pre><code>python3 main.py</code></pre>
+3. Run the code with python:
+   <pre><code>import CustomChat
+   CustomChat.run()</code></pre>
 
    This will start CustomChat and you can begin customizing it for your needs.
 
 ### Requirements
 
 CustomChat requires the following Python libraries:
 - `bs4` (Beautiful Soup): For web scraping capabilities.
```

