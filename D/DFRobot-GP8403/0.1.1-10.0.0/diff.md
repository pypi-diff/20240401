# Comparing `tmp/DFRobot_GP8403-0.1.1.tar.gz` & `tmp/DFRobot_GP8403-10.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFRobot_GP8403-0.1.1.tar", last modified: Sat Mar  2 15:29:38 2024, max compression
+gzip compressed data, was "DFRobot_GP8403-10.0.0.tar", last modified: Mon Apr  1 18:31:00 2024, max compression
```

## Comparing `DFRobot_GP8403-0.1.1.tar` & `DFRobot_GP8403-10.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:29:38.627242 DFRobot_GP8403-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:29:38.627242 DFRobot_GP8403-0.1.1/DFRobot/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15603 2024-03-02 15:29:28.000000 DFRobot_GP8403-0.1.1/DFRobot/DAC.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-02 15:29:28.000000 DFRobot_GP8403-0.1.1/DFRobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:29:38.627242 DFRobot_GP8403-0.1.1/DFRobot_GP8403.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-02 15:29:38.000000 DFRobot_GP8403-0.1.1/DFRobot_GP8403.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-02 15:29:38.000000 DFRobot_GP8403-0.1.1/DFRobot_GP8403.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 15:29:38.000000 DFRobot_GP8403-0.1.1/DFRobot_GP8403.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-02 15:29:38.000000 DFRobot_GP8403-0.1.1/DFRobot_GP8403.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-02 15:29:38.000000 DFRobot_GP8403-0.1.1/DFRobot_GP8403.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-02 15:29:28.000000 DFRobot_GP8403-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-02 15:29:38.627242 DFRobot_GP8403-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-02 15:29:28.000000 DFRobot_GP8403-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-02 15:29:28.000000 DFRobot_GP8403-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 15:29:38.627242 DFRobot_GP8403-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-02 15:29:28.000000 DFRobot_GP8403-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:31:00.009605 DFRobot_GP8403-10.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:31:00.005605 DFRobot_GP8403-10.0.0/DFRobot/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15603 2024-04-01 18:30:50.000000 DFRobot_GP8403-10.0.0/DFRobot/DAC.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 18:30:50.000000 DFRobot_GP8403-10.0.0/DFRobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:31:00.005605 DFRobot_GP8403-10.0.0/DFRobot_GP8403.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-01 18:30:59.000000 DFRobot_GP8403-10.0.0/DFRobot_GP8403.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 18:30:59.000000 DFRobot_GP8403-10.0.0/DFRobot_GP8403.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:30:59.000000 DFRobot_GP8403-10.0.0/DFRobot_GP8403.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 18:30:59.000000 DFRobot_GP8403-10.0.0/DFRobot_GP8403.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 18:30:59.000000 DFRobot_GP8403-10.0.0/DFRobot_GP8403.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 18:30:50.000000 DFRobot_GP8403-10.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-01 18:31:00.009605 DFRobot_GP8403-10.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 18:30:50.000000 DFRobot_GP8403-10.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 18:30:50.000000 DFRobot_GP8403-10.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:31:00.009605 DFRobot_GP8403-10.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-01 18:30:50.000000 DFRobot_GP8403-10.0.0/setup.py
```

### Comparing `DFRobot_GP8403-0.1.1/DFRobot/DAC.py` & `DFRobot_GP8403-10.0.0/DFRobot/DAC.py`

 * *Files identical despite different names*

### Comparing `DFRobot_GP8403-0.1.1/LICENSE` & `DFRobot_GP8403-10.0.0/LICENSE`

 * *Files identical despite different names*

