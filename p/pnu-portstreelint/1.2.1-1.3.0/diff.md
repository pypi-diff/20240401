# Comparing `tmp/pnu-portstreelint-1.2.1.tar.gz` & `tmp/pnu-portstreelint-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnu-portstreelint-1.2.1.tar", last modified: Sat Mar 23 15:04:26 2024, max compression
+gzip compressed data, was "pnu-portstreelint-1.3.0.tar", last modified: Mon Apr  1 17:02:27 2024, max compression
```

## Comparing `pnu-portstreelint-1.2.1.tar` & `pnu-portstreelint-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-03-23 15:04:26.902503 pnu-portstreelint-1.2.1/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2024-03-01 21:23:12.000000 pnu-portstreelint-1.2.1/License
--rw-r--r--   0 hubert    (1001) hubert    (1001)    10178 2024-03-23 15:04:26.902470 pnu-portstreelint-1.2.1/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     8943 2024-03-23 08:34:48.000000 pnu-portstreelint-1.2.1/README.md
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-03-23 15:04:26.897386 pnu-portstreelint-1.2.1/man/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     3147 2024-03-23 15:04:24.000000 pnu-portstreelint-1.2.1/man/portstreelint.8.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-17 21:50:43.000000 pnu-portstreelint-1.2.1/pyproject.toml
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1437 2024-03-23 15:04:26.903290 pnu-portstreelint-1.2.1/setup.cfg
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-03-23 15:04:26.896419 pnu-portstreelint-1.2.1/src/
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-03-23 15:04:26.902176 pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/
--rw-r--r--   0 hubert    (1001) hubert    (1001)    10178 2024-03-23 15:04:26.000000 pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1030 2024-03-23 15:04:26.000000 pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/SOURCES.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-03-23 15:04:26.000000 pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/dependency_links.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)      106 2024-03-23 15:04:26.000000 pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/entry_points.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       35 2024-03-23 15:04:26.000000 pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/requires.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       14 2024-03-23 15:04:26.000000 pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/top_level.txt
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-03-23 15:04:26.901968 pnu-portstreelint-1.2.1/src/portstreelint/
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-01 21:22:20.000000 pnu-portstreelint-1.2.1/src/portstreelint/__init__.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3225 2024-03-03 22:42:02.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_categories.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2407 2024-03-03 22:42:08.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_comment.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3151 2024-03-23 14:55:09.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_description_file.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1516 2024-03-03 22:42:21.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_installation_prefix.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1400 2024-03-03 22:42:27.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_maintainer.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4102 2024-03-03 22:42:32.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_marks.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1859 2024-03-23 14:49:40.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_plist.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      976 2024-03-23 13:58:54.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_port_path.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1052 2024-03-03 22:42:50.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_unchanging_ports.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     5358 2024-03-19 23:07:48.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_vulnerabilities.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7125 2024-03-03 22:43:01.000000 pnu-portstreelint-1.2.1/src/portstreelint/check_www_site.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2008 2024-03-03 22:38:49.000000 pnu-portstreelint-1.2.1/src/portstreelint/library.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4914 2024-03-23 12:19:17.000000 pnu-portstreelint-1.2.1/src/portstreelint/load_data.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)    13639 2024-03-23 14:19:06.000000 pnu-portstreelint-1.2.1/src/portstreelint/main.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1005 2024-03-03 22:54:02.000000 pnu-portstreelint-1.2.1/src/portstreelint/show_categories.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      987 2024-03-03 22:54:09.000000 pnu-portstreelint-1.2.1/src/portstreelint/show_maintainers.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1757 2024-03-19 23:09:14.000000 pnu-portstreelint-1.2.1/src/portstreelint/show_notifications.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3940 2024-03-19 23:09:21.000000 pnu-portstreelint-1.2.1/src/portstreelint/show_summary.py
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.841448 pnu-portstreelint-1.3.0/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2024-03-01 21:23:12.000000 pnu-portstreelint-1.3.0/License
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    11057 2024-04-01 17:02:27.841415 pnu-portstreelint-1.3.0/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     9822 2024-04-01 16:50:17.000000 pnu-portstreelint-1.3.0/README.md
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.836460 pnu-portstreelint-1.3.0/man/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     3415 2024-04-01 17:02:25.000000 pnu-portstreelint-1.3.0/man/portstreelint.8.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-17 21:50:43.000000 pnu-portstreelint-1.3.0/pyproject.toml
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1437 2024-04-01 17:02:27.842247 pnu-portstreelint-1.3.0/setup.cfg
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.817598 pnu-portstreelint-1.3.0/src/
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.841129 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    11057 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1063 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/SOURCES.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/dependency_links.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)      106 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/entry_points.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       35 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/requires.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       14 2024-04-01 17:02:27.000000 pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/top_level.txt
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-01 17:02:27.840932 pnu-portstreelint-1.3.0/src/portstreelint/
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-01 21:22:20.000000 pnu-portstreelint-1.3.0/src/portstreelint/__init__.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3225 2024-04-01 14:27:16.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_categories.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2407 2024-04-01 14:27:25.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_comment.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3151 2024-04-01 14:27:31.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_description_file.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1516 2024-04-01 14:27:38.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_installation_prefix.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1400 2024-04-01 14:27:44.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_maintainer.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4102 2024-04-01 14:27:52.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_marks.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1859 2024-04-01 14:28:00.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_plist.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      976 2024-04-01 14:28:06.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_port_path.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1052 2024-04-01 14:28:12.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_unchanging_ports.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     5597 2024-04-01 14:28:20.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_vulnerabilities.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7125 2024-04-01 14:29:09.000000 pnu-portstreelint-1.3.0/src/portstreelint/check_www_site.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2008 2024-03-03 22:38:49.000000 pnu-portstreelint-1.3.0/src/portstreelint/library.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7540 2024-04-01 14:11:53.000000 pnu-portstreelint-1.3.0/src/portstreelint/load_config.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4914 2024-04-01 14:29:36.000000 pnu-portstreelint-1.3.0/src/portstreelint/load_data.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    15801 2024-04-01 16:28:57.000000 pnu-portstreelint-1.3.0/src/portstreelint/main.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1005 2024-03-03 22:54:02.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_categories.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      987 2024-03-03 22:54:09.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_maintainers.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1757 2024-04-01 14:30:49.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_notifications.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3940 2024-04-01 14:30:57.000000 pnu-portstreelint-1.3.0/src/portstreelint/show_summary.py
```

### Comparing `pnu-portstreelint-1.2.1/License` & `pnu-portstreelint-1.3.0/License`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/PKG-INFO` & `pnu-portstreelint-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-portstreelint
-Version: 1.2.1
+Version: 1.3.0
 Summary: FreeBSD ports tree lint
 Home-page: https://github.com/HubTou/portstreelint/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/portstreelint/issues
 Keywords: pnu-project
@@ -47,20 +47,22 @@
 # PortsTreeLint(8)
 
 ## NAME
 portstreelint - FreeBSD ports tree lint
 
 ## SYNOPSIS
 **portstreelint**
-\[--tree|-t DIR\]
+\[--nocfg|-n\]
+\[--gencfg|-g FILE\]
 \[--show-cat|-C\]
 \[--show-mnt|-M\]
 \[--cat|-c LIST\]
 \[--mnt|-m LIST\]
 \[--port|-p LIST\]
+\[--tree|-t DIR\]
 \[--plist NUM\]
 \[--broken NUM\]
 \[--deprecated NUM\]
 \[--forbidden NUM\]
 \[--unchanged NUM\]
 \[--check-host|-h\]
 \[--check-url|-u\]
@@ -129,31 +131,43 @@
 * Makefile:PORTVERSION and Makefile:DISTVERSION used simultaneously
 * VuXML vulnerabilities for the current port versions (warning)
 
 It's possible to change the default values for PLIST_FILES abuse,
 BROKEN_since, DEPRECATED_since, FORBIDDEN_since and Unchanged_since
 with the *--plist*, *--broken*, *--deprecated*, *--forbidden* and
 *--unchanged* options, followed by a number of files for the first
-one and a number of days for the others.
+one and a number of days for the others. And you can select a port
+tree in a location other than */usr/ports* with the *--tree|-t*
+option.
 
 Finally, there's a *--output|-o* option to generate a CSV delimited
 file with the per-maintainer findings to a specified filename. This
 allows for automated processing of the results, such as, for example,
 sending warning emails, storing results and displaying only diffs
 since previous run...
 
+For convenience, you can put your favourite options in a
+configuration file, which will be read before processing the
+environment and the command line, unless you use the *--nocfg|-n*
+option. You can generate a default configuration file with the
+*--gencfg|-g* option followed by a filename. This file also offers
+full control over the checks to perform, and a way to discard
+false-positive vulnerabilities.
+
 ### OPTIONS
 Options | Use
 ------- | ---
---tree\|-t DIR|Ports directory (default=/usr/ports)
+--nocfg\|-n|Don't use the configuration file
+--gencfg\|-g FILE|Generate a default configuration file in FILE
 --show-cat\|-C|Show categories with ports count
 --show-mnt\|-M|Show maintainers with ports count
 --cat\|-c LIST|Select only the comma-separated categories in LIST
 --mnt\|-m LIST|Select only the comma-separated maintainers in LIST
 --port\|-p LIST|Select only the comma-separated ports in LIST
+--tree\|-t DIR|Set ports directory (default=/usr/ports)
 --plist NUM|Set PLIST_FILES abuse to NUM files
 --broken NUM|Set BROKEN since to NUM days
 --deprecated NUM|Set DEPRECATED since to NUM days
 --forbidden NUM|Set FORBIDDEN since to NUM days
 --unchanged NUM|Set Unchanged since to NUM days
 --check-host\|-h|Enable checking hostname resolution (long!)
 --check-url\|-u|Enable checking URL (very long!)
@@ -167,24 +181,28 @@
 ## ENVIRONMENT
 The *PTLINT_DEBUG* environment variable can be set to any value to enable debug mode.
 
 If the system's *PORTSDIR* environment variable is set, it'll be used instead of the
 default "/usr/ports". But the *--tree|-t DIR* option will still override it.
 
 ## FILES
-The whole port tree under /usr/ports, or the location indicated by the *PORTSDIR*
+The whole port tree under */usr/ports*, or the location indicated by the *PORTSDIR*
 environment variable, or the *--tree|-t* argument:
 - as root, if you have installed portsnap, update to the last version with "portsnap fetch update"
 - or, if you have installed git, clone the latest repository with "git clone https://git.FreeBSD.org/ports.git /usr/ports"
 
 [/usr/ports/INDEX-xx](https://wiki.freebsd.org/Ports/INDEX)
-where xx is the major version of FreeBSD that you are using (as I write this xx=14).
+: where xx is the major version of FreeBSD that you are using (as I write this xx=14).
 - as root, get the last version with "cd /usr/ports ; make fetchindex"
 - or rebuild it from your port tree with "cd /usr/ports ; make index"
 
+${HOME}/.ptlint
+: an [INI-style](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure) configuration file.
+- Generate a default one with the *--gencfg|-g* option and tweak it to your taste.
+
 ## EXIT STATUS
 The **portstreelint** utility exits 0 on success, and >0 if an error occurs.
 
 ## EXAMPLES
 To analyze the full port tree in the background, do:
 ```Shell
 $ nohup portstreelint --info -hu > stdout.txt 2> stderr.txt &
```

### Comparing `pnu-portstreelint-1.2.1/README.md` & `pnu-portstreelint-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 # PortsTreeLint(8)
 
 ## NAME
 portstreelint - FreeBSD ports tree lint
 
 ## SYNOPSIS
 **portstreelint**
-\[--tree|-t DIR\]
+\[--nocfg|-n\]
+\[--gencfg|-g FILE\]
 \[--show-cat|-C\]
 \[--show-mnt|-M\]
 \[--cat|-c LIST\]
 \[--mnt|-m LIST\]
 \[--port|-p LIST\]
+\[--tree|-t DIR\]
 \[--plist NUM\]
 \[--broken NUM\]
 \[--deprecated NUM\]
 \[--forbidden NUM\]
 \[--unchanged NUM\]
 \[--check-host|-h\]
 \[--check-url|-u\]
@@ -97,31 +99,43 @@
 * Makefile:PORTVERSION and Makefile:DISTVERSION used simultaneously
 * VuXML vulnerabilities for the current port versions (warning)
 
 It's possible to change the default values for PLIST_FILES abuse,
 BROKEN_since, DEPRECATED_since, FORBIDDEN_since and Unchanged_since
 with the *--plist*, *--broken*, *--deprecated*, *--forbidden* and
 *--unchanged* options, followed by a number of files for the first
-one and a number of days for the others.
+one and a number of days for the others. And you can select a port
+tree in a location other than */usr/ports* with the *--tree|-t*
+option.
 
 Finally, there's a *--output|-o* option to generate a CSV delimited
 file with the per-maintainer findings to a specified filename. This
 allows for automated processing of the results, such as, for example,
 sending warning emails, storing results and displaying only diffs
 since previous run...
 
+For convenience, you can put your favourite options in a
+configuration file, which will be read before processing the
+environment and the command line, unless you use the *--nocfg|-n*
+option. You can generate a default configuration file with the
+*--gencfg|-g* option followed by a filename. This file also offers
+full control over the checks to perform, and a way to discard
+false-positive vulnerabilities.
+
 ### OPTIONS
 Options | Use
 ------- | ---
---tree\|-t DIR|Ports directory (default=/usr/ports)
+--nocfg\|-n|Don't use the configuration file
+--gencfg\|-g FILE|Generate a default configuration file in FILE
 --show-cat\|-C|Show categories with ports count
 --show-mnt\|-M|Show maintainers with ports count
 --cat\|-c LIST|Select only the comma-separated categories in LIST
 --mnt\|-m LIST|Select only the comma-separated maintainers in LIST
 --port\|-p LIST|Select only the comma-separated ports in LIST
+--tree\|-t DIR|Set ports directory (default=/usr/ports)
 --plist NUM|Set PLIST_FILES abuse to NUM files
 --broken NUM|Set BROKEN since to NUM days
 --deprecated NUM|Set DEPRECATED since to NUM days
 --forbidden NUM|Set FORBIDDEN since to NUM days
 --unchanged NUM|Set Unchanged since to NUM days
 --check-host\|-h|Enable checking hostname resolution (long!)
 --check-url\|-u|Enable checking URL (very long!)
@@ -135,24 +149,28 @@
 ## ENVIRONMENT
 The *PTLINT_DEBUG* environment variable can be set to any value to enable debug mode.
 
 If the system's *PORTSDIR* environment variable is set, it'll be used instead of the
 default "/usr/ports". But the *--tree|-t DIR* option will still override it.
 
 ## FILES
-The whole port tree under /usr/ports, or the location indicated by the *PORTSDIR*
+The whole port tree under */usr/ports*, or the location indicated by the *PORTSDIR*
 environment variable, or the *--tree|-t* argument:
 - as root, if you have installed portsnap, update to the last version with "portsnap fetch update"
 - or, if you have installed git, clone the latest repository with "git clone https://git.FreeBSD.org/ports.git /usr/ports"
 
 [/usr/ports/INDEX-xx](https://wiki.freebsd.org/Ports/INDEX)
-where xx is the major version of FreeBSD that you are using (as I write this xx=14).
+: where xx is the major version of FreeBSD that you are using (as I write this xx=14).
 - as root, get the last version with "cd /usr/ports ; make fetchindex"
 - or rebuild it from your port tree with "cd /usr/ports ; make index"
 
+${HOME}/.ptlint
+: an [INI-style](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure) configuration file.
+- Generate a default one with the *--gencfg|-g* option and tweak it to your taste.
+
 ## EXIT STATUS
 The **portstreelint** utility exits 0 on success, and >0 if an error occurs.
 
 ## EXAMPLES
 To analyze the full port tree in the background, do:
 ```Shell
 $ nohup portstreelint --info -hu > stdout.txt 2> stderr.txt &
```

### Comparing `pnu-portstreelint-1.2.1/setup.cfg` & `pnu-portstreelint-1.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pnu-portstreelint
 description = FreeBSD ports tree lint
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 1.2.1
+version = 1.3.0
 license = BSD 3-Clause License
 license_files = License
 author = Hubert Tournier
 author_email = hubert.tournier@gmail.com
 url = https://github.com/HubTou/portstreelint/
 project_urls = 
 	Bug Tracker = https://github.com/HubTou/portstreelint/issues
```

### Comparing `pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/PKG-INFO` & `pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-portstreelint
-Version: 1.2.1
+Version: 1.3.0
 Summary: FreeBSD ports tree lint
 Home-page: https://github.com/HubTou/portstreelint/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/portstreelint/issues
 Keywords: pnu-project
@@ -47,20 +47,22 @@
 # PortsTreeLint(8)
 
 ## NAME
 portstreelint - FreeBSD ports tree lint
 
 ## SYNOPSIS
 **portstreelint**
-\[--tree|-t DIR\]
+\[--nocfg|-n\]
+\[--gencfg|-g FILE\]
 \[--show-cat|-C\]
 \[--show-mnt|-M\]
 \[--cat|-c LIST\]
 \[--mnt|-m LIST\]
 \[--port|-p LIST\]
+\[--tree|-t DIR\]
 \[--plist NUM\]
 \[--broken NUM\]
 \[--deprecated NUM\]
 \[--forbidden NUM\]
 \[--unchanged NUM\]
 \[--check-host|-h\]
 \[--check-url|-u\]
@@ -129,31 +131,43 @@
 * Makefile:PORTVERSION and Makefile:DISTVERSION used simultaneously
 * VuXML vulnerabilities for the current port versions (warning)
 
 It's possible to change the default values for PLIST_FILES abuse,
 BROKEN_since, DEPRECATED_since, FORBIDDEN_since and Unchanged_since
 with the *--plist*, *--broken*, *--deprecated*, *--forbidden* and
 *--unchanged* options, followed by a number of files for the first
-one and a number of days for the others.
+one and a number of days for the others. And you can select a port
+tree in a location other than */usr/ports* with the *--tree|-t*
+option.
 
 Finally, there's a *--output|-o* option to generate a CSV delimited
 file with the per-maintainer findings to a specified filename. This
 allows for automated processing of the results, such as, for example,
 sending warning emails, storing results and displaying only diffs
 since previous run...
 
+For convenience, you can put your favourite options in a
+configuration file, which will be read before processing the
+environment and the command line, unless you use the *--nocfg|-n*
+option. You can generate a default configuration file with the
+*--gencfg|-g* option followed by a filename. This file also offers
+full control over the checks to perform, and a way to discard
+false-positive vulnerabilities.
+
 ### OPTIONS
 Options | Use
 ------- | ---
---tree\|-t DIR|Ports directory (default=/usr/ports)
+--nocfg\|-n|Don't use the configuration file
+--gencfg\|-g FILE|Generate a default configuration file in FILE
 --show-cat\|-C|Show categories with ports count
 --show-mnt\|-M|Show maintainers with ports count
 --cat\|-c LIST|Select only the comma-separated categories in LIST
 --mnt\|-m LIST|Select only the comma-separated maintainers in LIST
 --port\|-p LIST|Select only the comma-separated ports in LIST
+--tree\|-t DIR|Set ports directory (default=/usr/ports)
 --plist NUM|Set PLIST_FILES abuse to NUM files
 --broken NUM|Set BROKEN since to NUM days
 --deprecated NUM|Set DEPRECATED since to NUM days
 --forbidden NUM|Set FORBIDDEN since to NUM days
 --unchanged NUM|Set Unchanged since to NUM days
 --check-host\|-h|Enable checking hostname resolution (long!)
 --check-url\|-u|Enable checking URL (very long!)
@@ -167,24 +181,28 @@
 ## ENVIRONMENT
 The *PTLINT_DEBUG* environment variable can be set to any value to enable debug mode.
 
 If the system's *PORTSDIR* environment variable is set, it'll be used instead of the
 default "/usr/ports". But the *--tree|-t DIR* option will still override it.
 
 ## FILES
-The whole port tree under /usr/ports, or the location indicated by the *PORTSDIR*
+The whole port tree under */usr/ports*, or the location indicated by the *PORTSDIR*
 environment variable, or the *--tree|-t* argument:
 - as root, if you have installed portsnap, update to the last version with "portsnap fetch update"
 - or, if you have installed git, clone the latest repository with "git clone https://git.FreeBSD.org/ports.git /usr/ports"
 
 [/usr/ports/INDEX-xx](https://wiki.freebsd.org/Ports/INDEX)
-where xx is the major version of FreeBSD that you are using (as I write this xx=14).
+: where xx is the major version of FreeBSD that you are using (as I write this xx=14).
 - as root, get the last version with "cd /usr/ports ; make fetchindex"
 - or rebuild it from your port tree with "cd /usr/ports ; make index"
 
+${HOME}/.ptlint
+: an [INI-style](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure) configuration file.
+- Generate a default one with the *--gencfg|-g* option and tweak it to your taste.
+
 ## EXIT STATUS
 The **portstreelint** utility exits 0 on success, and >0 if an error occurs.
 
 ## EXAMPLES
 To analyze the full port tree in the background, do:
 ```Shell
 $ nohup portstreelint --info -hu > stdout.txt 2> stderr.txt &
```

### Comparing `pnu-portstreelint-1.2.1/src/pnu_portstreelint.egg-info/SOURCES.txt` & `pnu-portstreelint-1.3.0/src/pnu_portstreelint.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,13 +18,14 @@
 src/portstreelint/check_marks.py
 src/portstreelint/check_plist.py
 src/portstreelint/check_port_path.py
 src/portstreelint/check_unchanging_ports.py
 src/portstreelint/check_vulnerabilities.py
 src/portstreelint/check_www_site.py
 src/portstreelint/library.py
+src/portstreelint/load_config.py
 src/portstreelint/load_data.py
 src/portstreelint/main.py
 src/portstreelint/show_categories.py
 src/portstreelint/show_maintainers.py
 src/portstreelint/show_notifications.py
 src/portstreelint/show_summary.py
```

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_categories.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_categories.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_comment.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_comment.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_description_file.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_description_file.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_installation_prefix.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_installation_prefix.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_maintainer.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_maintainer.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_marks.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_marks.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_plist.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_plist.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_port_path.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_port_path.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_unchanging_ports.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_unchanging_ports.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_vulnerabilities.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_vulnerabilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     logging.debug("  PORTEPOCH=%s", portepoch)
     logging.debug("  DISTVERSIONPREFIX=%s", distversionprefix)
     logging.debug("  DISTVERSION=%s", distversion)
     logging.debug("  DISTVERSIONSUFFIX=%s", distversionsuffix)
 
 
 ####################################################################################################
-def check_vulnerabilities(ports):
+def check_vulnerabilities(ports, excluded_vulnerabilities):
     """ Checks if the port has vulnerabilities reported in VuXML """
     vulns = vuxml.load_vuxml()
     logging.info("Loaded %d vulnerabilities from the FreeBSD VuXML files", len(vulns))
 
     for name, port in ports.items():
         portname = ""
         if "PORTNAME" in port:
@@ -123,14 +123,19 @@
         try:
             vids = vuxml.search_vulns_by_package(vulns, portname, version)
         except Exception as error:
             logging.warning('Encountered "%s" while searching vulnerabilities for port %s. Skipping vulnerability check', error, name)
             counters["Skipped vulnerability checks"] += 1
             continue
 
+        for vid in excluded_vulnerabilities:
+            if vid in vids:
+                vids.remove(vid)
+                logging.debug("Discarded false-positive VuXML vulnerability '%s' for port %s", vid, name)
+
         for vid in vids:
             logging.warning("Found VuXML vulnerability '%s' for port %s", vid, name)
             if not "FORBIDDEN" in port:
                 logging.debug("Vulnerable port not marked as FORBIDDEN for port %s", name)
 
         if vids:
             counters["Vulnerable port version"] += 1
```

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/check_www_site.py` & `pnu-portstreelint-1.3.0/src/portstreelint/check_www_site.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import socket
 import urllib.request
 
 from .library import counters, notify_maintainer
 
 # Headers and timeout delay for HTTP(S) requests:
 HTTP_HEADERS = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:123.0) Gecko/20100101 Firefox/123.0",
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:124.0) Gecko/20100101 Firefox/124.0",
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
     "Accept-Language": "en;q=1.0, en-US;q=0.8, *;q=0.5",
     "Accept-Encoding": "identity",
     "Connection": "keep-alive",
 }
 CONNECTION_TIMEOUT = 10 # seconds
```

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/library.py` & `pnu-portstreelint-1.3.0/src/portstreelint/library.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/load_data.py` & `pnu-portstreelint-1.3.0/src/portstreelint/load_data.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/main.py` & `pnu-portstreelint-1.3.0/src/portstreelint/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import logging
 import os
 import sys
 
 import libpnu
 
 from .load_data import load_freebsd_ports_dict, filter_ports, update_with_makefiles
+from .load_config import generate_config, load_config
 from .check_port_path import check_port_path
 from .check_installation_prefix import check_installation_prefix
 from .check_comment import check_comment
 from .check_description_file import check_description_file
 from .check_plist import check_plist
 from .check_maintainer import check_maintainer
 from .check_categories import check_categories
@@ -27,55 +28,77 @@
 from .show_categories import show_categories
 from .show_maintainers import show_maintainers
 from .show_notifications import show_notifications, output_notifications
 from .show_summary import show_summary
 
 
 # Version string used by the what(1) and ident(1) commands:
-ID = "@(#) $Id: portstreelint - FreeBSD ports tree lint v1.2.1 (March 23, 2024) by Hubert Tournier $"
+ID = "@(#) $Id: portstreelint - FreeBSD ports tree lint v1.3.0 (April 1st, 2024) by Hubert Tournier $"
 
 # Default parameters. Can be overcome by command line options:
 parameters = {
+    "Load config": True,
+    "INI filename": "",
     "Ports dir": "/usr/ports",
+    "CSV filename": "",
     "Show categories": False,
     "Show maintainers": False,
+
     "Checks": {
+        "port-path": True,
+		"installation-prefix": True,
+		"comment": True,
+		"description-file": True,
+		"plist": True,
+		"maintainer": True,
+		"categories": True,
+		"www-site": True,
         "Hostnames": False,
         "URL": False,
+		"Marks": True,
+		"Unchanging ports": True,
+		"Vulnerabilities": True,
     },
     "Limits": {
         "PLIST abuse": 7, # entries
         "BROKEN since": 6 * 30, # days
         "FORBIDDEN since": 3 * 30, # days
         "DEPRECATED since": 6 * 30, # days
         "Unchanged since": 3 * 365, # days
     },
-    "Output filename": "",
-    "Categories": [],
-    "Maintainers": [],
-    "Ports": [],
+    "Selections": {
+        "Categories": [],
+        "Maintainers": [],
+        "Ports": [],
+    },
+    "Exclusions": {
+        "Vulnerabilities": [],
+    },
 }
 
 
 ####################################################################################################
 def _display_help():
     """ Display usage and help """
     #pylint: disable=C0301
-    print("usage: portstreelint [--tree|-t DIR] [--show-cat|-C] [--show-mnt|-M]", file=sys.stderr)
+    print("usage: portstreelint [--nocfg|-n] [--gencfg|-g FILE]", file=sys.stderr)
+    print("        [--tree|-t DIR] [--show-cat|-C] [--show-mnt|-M]", file=sys.stderr)
     print("        [--cat|-c LIST] [--mnt|-m LIST] [--port|-p LIST] [--plist NUM]", file=sys.stderr)
     print("        [--broken NUM] [--deprecated NUM] [--forbidden NUM] [--unchanged NUM]", file=sys.stderr)
     print("        [--check-host|-h] [--check-url|-u] [--output|-o FILE]", file=sys.stderr)
     print("        [--debug] [--help|-?] [--info] [--version] [--]", file=sys.stderr)
     print("  ------------------  -------------------------------------------------------", file=sys.stderr)
-    print("  --tree|-t DIR       Ports directory (default=/usr/ports)", file=sys.stderr)
+    print("  --nocfg|-n          Don't use the configuration file", file=sys.stderr)
+    print("  --gencfg|-g FILE    Generate a default configuration file in FILE", file=sys.stderr)
     print("  --show-cat|-C       Show categories with ports count", file=sys.stderr)
     print("  --show-mnt|-M       Show maintainers with ports count", file=sys.stderr)
     print("  --cat|-c LIST       Select only the comma-separated categories in LIST", file=sys.stderr)
     print("  --mnt|-m LIST       Select only the comma-separated maintainers in LIST", file=sys.stderr)
     print("  --port|-p LIST      Select only the comma-separated ports in LIST", file=sys.stderr)
+    print("  --tree|-t DIR       Set ports directory (default=/usr/ports)", file=sys.stderr)
     print("  --plist NUM         Set PLIST_FILES abuse to NUM files", file=sys.stderr)
     print("  --broken NUM        Set BROKEN since to NUM days", file=sys.stderr)
     print("  --deprecated NUM    Set DEPRECATED since to NUM days", file=sys.stderr)
     print("  --forbidden NUM     Set FORBIDDEN since to NUM days", file=sys.stderr)
     print("  --unchanged NUM     Set Unchanged since to NUM days", file=sys.stderr)
     print("  --check-host|-h     Enable checking hostname resolution (long!)", file=sys.stderr)
     print("  --check-url|-u      Enable checking URL (very long!)", file=sys.stderr)
@@ -114,26 +137,28 @@
     """ Process command line options """
     #pylint: disable=C0103, W0602
     global parameters
     #pylint: enable=C0103, W0602
 
     # option letters followed by : expect an argument
     # same for option strings followed by =
-    character_options = "CMc:hm:o:p:t:u?"
+    character_options = "CMc:g:hm:no:p:t:u?"
     string_options = [
         "broken=",
         "cat=",
         "check-host",
         "check-url",
         "debug",
         "deprecated=",
         "forbidden=",
+        "gencfg=",
         "help",
         "info",
         "mnt=",
+        "nocfg",
         "output=",
         "port=",
         "plist=",
         "show-cat",
         "show-mnt",
         "tree=",
         "unchanged=",
@@ -171,15 +196,15 @@
                 logging.critical("Syntax error: expecting a number of days after the broken option")
                 sys.exit(1)
             if parameters["Checks"]["BROKEN since"] < 30:
                 logging.critical("The number of days after the broken option must be >= 30")
                 sys.exit(1)
 
         elif option in ("--cat", "-c"):
-            parameters["Categories"] = argument.lower().split(",")
+            parameters["Selections"]["Categories"] = argument.lower().split(",")
 
         elif option in ("--check-host", "-h"):
             parameters["Checks"]["Hostnames"] = True
 
         elif option in ("--check-url", "-u"):
             parameters["Checks"]["Hostnames"] = True
             parameters["Checks"]["URL"] = True
@@ -200,34 +225,43 @@
             except ValueError:
                 logging.critical("Syntax error: expecting a number of days after the forbidden option")
                 sys.exit(1)
             if parameters["Checks"]["FORBIDDEN since"] < 30:
                 logging.critical("The number of days after the forbidden option must be >= 30")
                 sys.exit(1)
 
+        elif option in ("--gencfg", "-g"):
+            if not os.path.exists(argument):
+                parameters["INI filename"] = argument
+            else:
+                logging.critical("--gencfg|-g argument cannot be an existing filesystem item")
+                sys.exit(1)
+
         elif option in ("--mnt", "-m"):
             maintainers = argument.lower().split(",")
-            parameters["Maintainers"] = [m if '@' in m else f"{m}@freebsd.org" for m in maintainers]
+            parameters["Selections"]["Maintainers"] = [m if '@' in m else f"{m}@freebsd.org" for m in maintainers]
 
+        elif option in ("--nocfg", "-n"):
+            parameters["Load config"] = False
 
         elif option in ("--output", "-o"):
-            parameters["Output filename"] = argument
+            parameters["CSV filename"] = argument
 
         elif option == "--plist":
             try:
                 parameters["Checks"]["PLIST abuse"] = int(argument)
             except ValueError:
                 logging.critical("Syntax error: expecting a number of files after the plist option")
                 sys.exit(1)
             if parameters["Checks"]["PLIST abuse"] < 3:
                 logging.critical("The number of files after the plist option must be >= 3")
                 sys.exit(1)
 
         elif option in ("--port", "-p"):
-            parameters["Ports"] = argument.split(",")
+            parameters["Selections"]["Ports"] = argument.split(",")
 
         elif option in ("--show-cat", "-C"):
             parameters["Show categories"] = True
             parameters["Show maintainers"] = False
 
         elif option in ("--show-mnt", "-M"):
             parameters["Show maintainers"] = True
@@ -260,18 +294,25 @@
 
     return remaining_arguments
 
 
 ####################################################################################################
 def main():
     """ The program's main entry point """
+    #pylint: disable=C0103, W0602
+    global parameters
+    #pylint: enable=C0103, W0602
+
     program_name = os.path.basename(sys.argv[0])
 
     libpnu.initialize_debugging(program_name)
     libpnu.handle_interrupt_signals(libpnu.interrupt_handler_function)
+
+    if parameters["Load config"]:
+        parameters = load_config(parameters)
     _process_environment_variables()
     _ = _process_command_line()
 
     # Load the FreeBSD ports INDEX file
     # and verify structural integrity (ie: 13 pipe-separated fields)
     # and unicity of distribution-names
     try:
@@ -279,67 +320,86 @@
     except SystemError:
         logging.critical("This program will only run on a FreeBSD operating system")
         sys.exit(1)
     except FileNotFoundError:
         logging.critical("The ports tree is missing. Please install and update it as root ('portsnap fetch extract')")
         sys.exit(1)
 
-    if parameters["Show categories"]:
+    if parameters["INI filename"]:
+        # Only generate a configuration file
+        generate_config(parameters)
+    elif parameters["Show categories"]:
         # Only show port categories with count of associated ports
         show_categories(ports)
     elif parameters["Show maintainers"]:
         # Only show port maintainers with count of associated ports
         show_maintainers(ports)
     else:
-        ports = filter_ports(ports, parameters["Categories"], parameters["Maintainers"], parameters["Ports"])
+        ports = filter_ports(
+            ports,
+            parameters["Selections"]["Categories"],
+            parameters["Selections"]["Maintainers"],
+            parameters["Selections"]["Ports"]
+        )
 
         # Check the existence of port Makefile and load its variables
         ports = update_with_makefiles(ports, parameters["Ports dir"])
 
         # Check the existence of port-path
-        check_port_path(ports, parameters["Ports dir"])
+        if parameters["Checks"]["port-path"]:
+            check_port_path(ports, parameters["Ports dir"])
 
         # Check unusual installation-prefix
-        check_installation_prefix(ports)
+        if parameters["Checks"]["installation-prefix"]:
+            check_installation_prefix(ports)
 
         # Cross-check comment identity between Index and Makefile
-        check_comment(ports)
+        if parameters["Checks"]["comment"]:
+            check_comment(ports)
 
         # Check the existence of description-file
-        check_description_file(ports, parameters["Ports dir"])
+        if parameters["Checks"]["description-file"]:
+            check_description_file(ports, parameters["Ports dir"])
 
         # Check the package list
-        check_plist(ports, parameters["Limits"]["PLIST abuse"], parameters["Ports dir"])
+        if parameters["Checks"]["plist"]:
+            check_plist(ports, parameters["Limits"]["PLIST abuse"], parameters["Ports dir"])
 
         # Cross-check maintainer identity between Index and Makefile
-        check_maintainer(ports)
+        if parameters["Checks"]["maintainer"]:
+            check_maintainer(ports)
 
         # Cross-check categories identity between Index and Makefile
         # and belonging to the official list of categories
-        check_categories(ports)
+        if parameters["Checks"]["categories"]:
+            check_categories(ports)
 
         # Check that www-site is not empty, that the hostnames exist,
         # that the URL is accessible, and identity between Index and Makefile
-        check_www_site(ports, parameters["Checks"]["Hostnames"], parameters["Checks"]["URL"])
+        if parameters["Checks"]["www-site"]:
+            check_www_site(ports, parameters["Checks"]["Hostnames"], parameters["Checks"]["URL"])
 
         # Check the existence of marks variables (ie. BROKEN, etc.) in Makefiles
-        check_marks(ports, parameters["Limits"])
+        if parameters["Checks"]["Marks"]:
+            check_marks(ports, parameters["Limits"])
 
         # Check static ports
-        check_unchanging_ports(ports, parameters["Limits"]["Unchanged since"])
+        if parameters["Checks"]["Unchanging ports"]:
+            check_unchanging_ports(ports, parameters["Limits"]["Unchanged since"])
 
         # Check vulnerabilities
-        check_vulnerabilities(ports)
+        if parameters["Checks"]["Vulnerabilities"]:
+            check_vulnerabilities(ports, parameters["Exclusions"]["Vulnerabilities"])
 
         # Print results per maintainer
         show_notifications()
 
         # Output per maintainer results in a CSV file
-        if parameters["Output filename"]:
-            output_notifications(parameters["Output filename"])
+        if parameters["CSV filename"]:
+            output_notifications(parameters["CSV filename"])
 
         # Print summary of findings
         show_summary(parameters["Limits"])
 
     sys.exit(0)
```

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/show_categories.py` & `pnu-portstreelint-1.3.0/src/portstreelint/show_categories.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/show_maintainers.py` & `pnu-portstreelint-1.3.0/src/portstreelint/show_maintainers.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/show_notifications.py` & `pnu-portstreelint-1.3.0/src/portstreelint/show_notifications.py`

 * *Files identical despite different names*

### Comparing `pnu-portstreelint-1.2.1/src/portstreelint/show_summary.py` & `pnu-portstreelint-1.3.0/src/portstreelint/show_summary.py`

 * *Files identical despite different names*

