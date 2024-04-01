# Comparing `tmp/owasp-depscan-5.2.8.tar.gz` & `tmp/owasp-depscan-5.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owasp-depscan-5.2.8.tar", last modified: Tue Feb 13 22:57:32 2024, max compression
+gzip compressed data, was "owasp-depscan-5.2.9.tar", last modified: Wed Feb 14 19:00:26 2024, max compression
```

## Comparing `owasp-depscan-5.2.8.tar` & `owasp-depscan-5.2.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.683500 owasp-depscan-5.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-02-13 22:57:32.683500 owasp-depscan-5.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.667500 owasp-depscan-5.2.8/depscan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38835 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.671500 owasp-depscan-5.2.8/depscan/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58149 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/license.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/orasclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/depscan/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.683500 owasp-depscan-5.2.8/owasp_depscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-02-13 22:57:32.000000 owasp-depscan-5.2.8/owasp_depscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-13 22:57:32.000000 owasp-depscan-5.2.8/owasp_depscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 22:57:32.000000 owasp-depscan-5.2.8/owasp_depscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-13 22:57:32.000000 owasp-depscan-5.2.8/owasp_depscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-13 22:57:32.000000 owasp-depscan-5.2.8/owasp_depscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-13 22:57:32.000000 owasp-depscan-5.2.8/owasp_depscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-13 22:57:11.000000 owasp-depscan-5.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 22:57:32.683500 owasp-depscan-5.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.671500 owasp-depscan-5.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.675500 owasp-depscan-5.2.8/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.667500 owasp-depscan-5.2.8/vendor/choosealicense.com/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.675500 owasp-depscan-5.2.8/vendor/choosealicense.com/_data/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_data/fields.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_data/meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_data/rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.683500 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/0bsd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/afl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/agpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/artistic-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cc0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cecill-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ecl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/epl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/epl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/eupl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/eupl-1.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/gpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/gpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/isc.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mit-0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ms-pl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ms-rl.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ncsa.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/odbl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ofl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/osl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/upl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/vim.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/wtfpl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/zlib.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.667500 owasp-depscan-5.2.8/vendor/spdx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 22:57:32.683500 owasp-depscan-5.2.8/vendor/spdx/json/
--rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-02-13 22:57:12.000000 owasp-depscan-5.2.8/vendor/spdx/json/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.170227 owasp-depscan-5.2.9/depscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38835 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.174227 owasp-depscan-5.2.9/depscan/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58149 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14515 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/orasclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/depscan/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/owasp_depscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-14 19:00:26.000000 owasp-depscan-5.2.9/owasp_depscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.174227 owasp-depscan-5.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.178227 owasp-depscan-5.2.9/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.170227 owasp-depscan-5.2.9/vendor/choosealicense.com/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.178227 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_data/rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/0bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/afl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/agpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/artistic-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cecill-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ecl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/isc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit-0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-rl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ncsa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/odbl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ofl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/osl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/upl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/vim.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/wtfpl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/zlib.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.170227 owasp-depscan-5.2.9/vendor/spdx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:00:26.186227 owasp-depscan-5.2.9/vendor/spdx/json/
+-rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-02-14 19:00:09.000000 owasp-depscan-5.2.9/vendor/spdx/json/licenses.json
```

### Comparing `owasp-depscan-5.2.8/LICENSE` & `owasp-depscan-5.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/PKG-INFO` & `owasp-depscan-5.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.2.8
+Version: 5.2.9
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `owasp-depscan-5.2.8/README.md` & `owasp-depscan-5.2.9/README.md`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/cli.py` & `owasp-depscan-5.2.9/depscan/cli.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/analysis.py` & `owasp-depscan-5.2.9/depscan/lib/analysis.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/audit.py` & `owasp-depscan-5.2.9/depscan/lib/audit.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/bom.py` & `owasp-depscan-5.2.9/depscan/lib/bom.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/config.py` & `owasp-depscan-5.2.9/depscan/lib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,7 +545,19 @@
     "libssh",
     "subversion",
     "vim",
     "vim-minimal",
 )
 
 OS_PKG_IGNORABLE = ("linux", "systemd", "ncurses", "kernel")
+
+RUBY_PLATFORM_MARKERS = [
+  "-x86_64",
+  "-x86",
+  "-x64",
+  "-aarch",
+  "-arm",
+  "-ruby",
+  "-universal",
+  "-java",
+  "-truffle"
+]
```

### Comparing `owasp-depscan-5.2.8/depscan/lib/csaf.py` & `owasp-depscan-5.2.9/depscan/lib/csaf.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/explainer.py` & `owasp-depscan-5.2.9/depscan/lib/explainer.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/github.py` & `owasp-depscan-5.2.9/depscan/lib/github.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/license.py` & `owasp-depscan-5.2.9/depscan/lib/license.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/logger.py` & `owasp-depscan-5.2.9/depscan/lib/logger.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/normalize.py` & `owasp-depscan-5.2.9/depscan/lib/normalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,27 @@
                             {
                                 "vendor": "npm",
                                 "name": pkg_dict.get("name"),
                                 "version": pkg_dict.get("version"),
                             }
                         )
                     return pkg_list
+                # For Rubygems, version string could include the plaform.
+                # So we create an alias without the platform to improve the results
+                if pkg_type in ("gem",):
+                    for plaform_marker in config.RUBY_PLATFORM_MARKERS:
+                        if pkg_dict.get("version") and plaform_marker in pkg_dict["version"]:
+                            pkg_list.append(
+                                {
+                                    "vendor": vendor,
+                                    "name": pkg_dict.get("name"),
+                                    "version": pkg_dict["version"].split(plaform_marker)[0],
+                                }
+                            )
+                            break
                 if qualifiers and qualifiers.get("distro_name"):
                     os_distro_name = qualifiers.get("distro_name")
                     name_aliases.add(f"""{os_distro_name}/{name}""")
                 if qualifiers and qualifiers.get("distro"):
                     os_distro = qualifiers.get("distro")
                     name_aliases.add(f"""{os_distro}/{name}""")
                     # almalinux-9.2 becomes almalinux-9
```

### Comparing `owasp-depscan-5.2.8/depscan/lib/orasclient.py` & `owasp-depscan-5.2.9/depscan/lib/orasclient.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/pkg_query.py` & `owasp-depscan-5.2.9/depscan/lib/pkg_query.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/depscan/lib/utils.py` & `owasp-depscan-5.2.9/depscan/lib/utils.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/owasp_depscan.egg-info/PKG-INFO` & `owasp-depscan-5.2.9/owasp_depscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.2.8
+Version: 5.2.9
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `owasp-depscan-5.2.8/owasp_depscan.egg-info/SOURCES.txt` & `owasp-depscan-5.2.9/owasp_depscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/pyproject.toml` & `owasp-depscan-5.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "owasp-depscan"
-version = "5.2.8"
+version = "5.2.9"
 description = "Fully open-source security audit for project dependencies based on known vulnerabilities and advisories."
 authors = [
     {name = "Team AppThreat", email = "cloud@appthreat.com"},
 ]
 dependencies = [
     "appthreat-vulnerability-db==5.6.2",
     "defusedxml",
```

### Comparing `owasp-depscan-5.2.8/test/test_analysis.py` & `owasp-depscan-5.2.9/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/test/test_bom.py` & `owasp-depscan-5.2.9/test/test_bom.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/test/test_csaf.py` & `owasp-depscan-5.2.9/test/test_csaf.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/test/test_github.py` & `owasp-depscan-5.2.9/test/test_github.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/test/test_license.py` & `owasp-depscan-5.2.9/test/test_license.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/test/test_norm.py` & `owasp-depscan-5.2.9/test/test_norm.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/test/test_pkg_query.py` & `owasp-depscan-5.2.9/test/test_pkg_query.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/test/test_utils.py` & `owasp-depscan-5.2.9/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_data/fields.yml` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_data/fields.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_data/meta.yml` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_data/meta.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_data/rules.yml` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_data/rules.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/0bsd.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/0bsd.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/afl-3.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/agpl-3.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/apache-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/artistic-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-2-clause.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-3-clause.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsd-4-clause.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/bsl-1.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cc-by-4.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cc0-1.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cecill-2.1.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ecl-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/epl-1.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/epl-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/eupl-1.1.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/eupl-1.2.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/gfdl-1.3.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/gpl-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/gpl-3.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/isc.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/isc.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/lgpl-2.1.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/lgpl-3.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/lppl-1.3c.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/lppl-1.3c.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mit-0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit-0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mit.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mit.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mpl-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ms-pl.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-pl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ms-rl.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ms-rl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ncsa.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ncsa.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/odbl-1.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/odbl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/ofl-1.1.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/ofl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/osl-3.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/postgresql.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/postgresql.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/unlicense.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/unlicense.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/upl-1.0.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/upl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/vim.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/vim.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/wtfpl.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/choosealicense.com/_licenses/zlib.txt` & `owasp-depscan-5.2.9/vendor/choosealicense.com/_licenses/zlib.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.2.8/vendor/spdx/json/licenses.json` & `owasp-depscan-5.2.9/vendor/spdx/json/licenses.json`

 * *Files identical despite different names*

