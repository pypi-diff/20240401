# Comparing `tmp/qteasy-1.1.4.tar.gz` & `tmp/qteasy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-yj4u_w9j/qteasy-1.1.4.tar", last modified: Sat Mar 30 12:36:10 2024, max compression
+gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-q06mcg69/qteasy-1.1.5.tar", last modified: Mon Apr  1 14:11:17 2024, max compression
```

## Comparing `qteasy-1.1.4.tar` & `qteasy-1.1.5.tar`

### file list

```diff
@@ -1,60 +1,36 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.4/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    25619 2024-03-30 12:36:10.000000 qteasy-1.1.4/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24517 2024-03-27 07:12:17.000000 qteasy-1.1.4/README.md
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8509 2024-03-29 09:39:28.000000 qteasy-1.1.4/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    52573 2024-03-30 05:38:17.000000 qteasy-1.1.4/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2023-11-11 15:36:59.000000 qteasy-1.1.4/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-03-08 14:36:48.000000 qteasy-1.1.4/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   109841 2024-03-30 12:16:07.000000 qteasy-1.1.4/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   380638 2024-03-30 12:16:07.000000 qteasy-1.1.4/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    33669 2024-03-25 14:02:24.000000 qteasy-1.1.4/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    37690 2024-03-16 06:43:01.000000 qteasy-1.1.4/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   101000 2024-03-27 15:37:54.000000 qteasy-1.1.4/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-03-30 06:26:16.000000 qteasy-1.1.4/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-03-30 12:16:07.000000 qteasy-1.1.4/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    33875 2023-09-19 14:43:44.000000 qteasy-1.1.4/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-03-16 06:43:01.000000 qteasy-1.1.4/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-03-27 15:09:44.000000 qteasy-1.1.4/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    47486 2024-03-26 12:08:25.000000 qteasy-1.1.4/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)   180400 2024-03-18 12:27:53.000000 qteasy-1.1.4/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    67732 2024-03-29 02:43:40.000000 qteasy-1.1.4/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/tsfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    74255 2024-03-30 12:30:55.000000 qteasy-1.1.4/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79726 2024-03-25 14:11:45.000000 qteasy-1.1.4/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    25619 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1177 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.4/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      160 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1290 2024-03-30 12:36:10.000000 qteasy-1.1.4/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2023-01-23 13:51:42.000000 qteasy-1.1.4/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.4/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8091 2023-02-23 16:04:07.000000 qteasy-1.1.4/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.4/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17494 2024-03-30 11:09:35.000000 qteasy-1.1.4/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17540 2024-03-16 06:43:01.000000 qteasy-1.1.4/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   105972 2024-03-08 14:36:48.000000 qteasy-1.1.4/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.4/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73675 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.4/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.4/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   326237 2024-03-16 06:43:01.000000 qteasy-1.1.4/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169128 2024-03-02 15:43:47.000000 qteasy-1.1.4/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    46025 2024-03-30 10:08:54.000000 qteasy-1.1.4/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.4/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43381 2024-03-26 01:54:48.000000 qteasy-1.1.4/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    42435 2024-03-30 12:16:07.000000 qteasy-1.1.4/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   159385 2024-03-07 05:52:10.000000 qteasy-1.1.4/tests/test_trading.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.4/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43297 2023-12-06 18:45:12.000000 qteasy-1.1.4/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-01 14:11:17.000000 qteasy-1.1.5/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.5/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27472 2024-04-01 14:11:17.000000 qteasy-1.1.5/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24521 2024-03-31 16:24:53.000000 qteasy-1.1.5/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2013 2024-04-01 14:11:07.000000 qteasy-1.1.5/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-01 14:11:17.000000 qteasy-1.1.5/qteasy/
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-01 14:11:17.000000 qteasy-1.1.5/qteasy/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27472 2024-04-01 14:11:17.000000 qteasy-1.1.5/qteasy/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)      735 2024-04-01 14:11:17.000000 qteasy-1.1.5/qteasy/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-01 14:11:17.000000 qteasy-1.1.5/qteasy/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)      160 2024-04-01 14:11:17.000000 qteasy-1.1.5/qteasy/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)       38 2024-04-01 14:11:17.000000 qteasy-1.1.5/qteasy/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)       38 2024-04-01 14:11:17.000000 qteasy-1.1.5/setup.cfg
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-01 14:11:17.000000 qteasy-1.1.5/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.5/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8091 2023-02-23 16:04:07.000000 qteasy-1.1.5/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.5/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17494 2024-03-31 16:24:53.000000 qteasy-1.1.5/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17540 2024-03-16 06:43:01.000000 qteasy-1.1.5/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   105972 2024-03-31 16:24:53.000000 qteasy-1.1.5/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.5/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73675 2023-01-29 16:18:32.000000 qteasy-1.1.5/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.5/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.5/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.5/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   326237 2024-03-16 06:43:01.000000 qteasy-1.1.5/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169128 2024-03-02 15:43:47.000000 qteasy-1.1.5/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44354 2024-03-30 13:43:29.000000 qteasy-1.1.5/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.5/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.5/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43381 2024-03-26 01:54:48.000000 qteasy-1.1.5/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    42435 2024-03-30 12:16:07.000000 qteasy-1.1.5/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   159385 2024-03-07 05:52:10.000000 qteasy-1.1.5/tests/test_trading.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.5/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43297 2023-12-06 18:45:12.000000 qteasy-1.1.5/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.5/tests/test_visual.py
```

### Comparing `qteasy-1.1.4/LICENSE` & `qteasy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/PKG-INFO` & `qteasy-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: qteasy
-Version: 1.1.4
-Summary: A fast quantitative investment tool kit
-Home-page: https://github.com/shepherdpp/qteasy
-Author: Jackie PENG
-Author-email: jackie.pengzhao@gmail.com
-Maintainer: Jackie PENG
-License: BSD License
-Keywords: quantitative investment,quant
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Documentation :: Sphinx
-Classifier: Topic :: Office/Business :: Financial
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: <3.9,>=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: database
-Provides-Extra: hdf
-Provides-Extra: feather
-License-File: LICENSE
-
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
 [![Build Status](https://app.travis-ci.com/shepherdpp/qteasy.svg?branch=master)](https://app.travis-ci.com/shepherdpp/qteasy)
 [![Documentation Status](https://readthedocs.org/projects/qteasy/badge/?version=latest)](https://qteasy.readthedocs.io/zh/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/shepherdpp/qteasy)
@@ -80,17 +50,17 @@
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
-4. **灵活多变** 使用qteasy提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
+4. **灵活多变** 使用`qteasy`提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
 
-## qteasy能做什么？
+## `qteasy`能做什么？
 
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
```

### Comparing `qteasy-1.1.4/README.md` & `qteasy-1.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,50 @@
+Metadata-Version: 2.1
+Name: qteasy
+Version: 1.1.5
+Summary: A fast quantitative investment tool kit
+Author-email: jackie PENG <jackie.pengzhao@gmail.com>
+Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
+License: Copyright <2019> <JACKIE PENG>
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: Homepage, https://github.com/shepherdpp/qteasy
+Project-URL: Documentation, https://https://qteasy.readthedocs.io/zh/latest/
+Project-URL: Issues, https://github.com/shepherdpp/qteasy/issues
+Keywords: quantitative investment,quantitative trading,stock,finance,investment
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Office/Business :: Financial
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: database
+Provides-Extra: hdf
+Provides-Extra: feather
+License-File: LICENSE
+
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
 
 ![PyPI](https://img.shields.io/pypi/v/qteasy)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/qteasy)
 [![Build Status](https://app.travis-ci.com/shepherdpp/qteasy.svg?branch=master)](https://app.travis-ci.com/shepherdpp/qteasy)
 [![Documentation Status](https://readthedocs.org/projects/qteasy/badge/?version=latest)](https://qteasy.readthedocs.io/zh/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/shepherdpp/qteasy)
@@ -50,17 +93,17 @@
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
-4. **灵活多变** 使用qteasy提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
+4. **灵活多变** 使用`qteasy`提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
 
-## qteasy能做什么？
+## `qteasy`能做什么？
 
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
```

### Comparing `qteasy-1.1.4/qteasy.egg-info/PKG-INFO` & `qteasy-1.1.5/qteasy/qteasy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.4
+Version: 1.1.5
 Summary: A fast quantitative investment tool kit
-Home-page: https://github.com/shepherdpp/qteasy
-Author: Jackie PENG
-Author-email: jackie.pengzhao@gmail.com
-Maintainer: Jackie PENG
-License: BSD License
-Keywords: quantitative investment,quant
+Author-email: jackie PENG <jackie.pengzhao@gmail.com>
+Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
+License: Copyright <2019> <JACKIE PENG>
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: Homepage, https://github.com/shepherdpp/qteasy
+Project-URL: Documentation, https://https://qteasy.readthedocs.io/zh/latest/
+Project-URL: Issues, https://github.com/shepherdpp/qteasy/issues
+Keywords: quantitative investment,quantitative trading,stock,finance,investment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: <3.9,>=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: database
 Provides-Extra: hdf
 Provides-Extra: feather
 License-File: LICENSE
 
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
@@ -80,17 +93,17 @@
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
-4. **灵活多变** 使用qteasy提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
+4. **灵活多变** 使用`qteasy`提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
 
-## qteasy能做什么？
+## `qteasy`能做什么？
 
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
```

### Comparing `qteasy-1.1.4/tests/test_broker.py` & `qteasy-1.1.5/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_cashplan.py` & `qteasy-1.1.5/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_config.py` & `qteasy-1.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_core_sub_funcs.py` & `qteasy-1.1.5/tests/test_core_sub_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_cost.py` & `qteasy-1.1.5/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_datasource.py` & `qteasy-1.1.5/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_eastmoney.py` & `qteasy-1.1.5/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_evaluations.py` & `qteasy-1.1.5/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_fast_experiments.py` & `qteasy-1.1.5/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_historypanel.py` & `qteasy-1.1.5/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_loop.py` & `qteasy-1.1.5/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_operator_and_strategy.py` & `qteasy-1.1.5/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_qt.py` & `qteasy-1.1.5/tests/test_qt.py`

 * *Files 11% similar despite different names*

```diff
@@ -249,800 +249,800 @@
         else:  # 其余情况不产生任何信号
             return 0
 
 
 class TestQT(unittest.TestCase):
     """对qteasy系统进行总体测试"""
 
-    # def setUp(self):
-    #     # 准备测试所需数据，确保本地数据源有足够的数据
-    #
-    #     self.op = qt.Operator(strategies=['dma', 'macd'])
-    #     print('  START TO TEST QT GENERAL OPERATIONS\n'
-    #           '=======================================')
-    #     print(' test environment information')
-    #     print(f'  python version: {sys.version}')
-    #     print(f'  qteasy version: {qt.__version__}')
-    #     print(f'  qteasy root path: {qt.QT_ROOT_PATH}')
-    #     print(f'  numpy version: {np.__version__}')
-    #     print(f'  numba version: {nb.__version__}')
-    #     print(f'  pandas version: {pd.__version__}')
-    #     self.op.set_parameter('dma', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
-    #     self.op.set_parameter('macd', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
-    #     self.op.signal_type = 'pt'
-    #
-    #     qt.configure(benchmark_asset='000300.SH',
-    #                  mode=1,
-    #                  benchmark_asset_type='IDX',
-    #                  asset_pool='000300.SH',
-    #                  asset_type='IDX',
-    #                  opti_output_count=50,
-    #                  invest_start='20070110',
-    #                  trade_batch_size=0.,
-    #                  sell_batch_size=0.,
-    #                  parallel=True,
-    #                  hist_dnld_retry_cnt=3,  # 减少数据下载重试次数，加快测试速度
-    #                  hist_dnld_retry_wait=0.5,  # 减少数据下载重试等待时间，加快测试速度
-    #                  hist_dnld_backoff=1.2,  # 减少数据下载重试等待时间，加快测试速度
-    #                  )
-    #
-    #     timing_pars1 = (165, 191, 23)
-    #     timing_pars2 = {'000100': (77, 118, 144),
-    #                     '000200': (75, 128, 138),
-    #                     '000300': (73, 120, 143)}
-    #     timing_pars3 = (115, 197, 54)
-    #     self.op.set_blender('pos_2_0(s0, s1)')
-    #     self.op.set_parameter(stg_id='dma', pars=timing_pars1)
-    #     self.op.set_parameter(stg_id='macd', pars=timing_pars3)
-    #
-    # def test_configure(self):
-    #     """测试参数设置
-    #         通过configure设置参数
-    #         通过QR_CONFIG直接设置参数
-    #         设置不存在的参数时报错
-    #         设置不合法参数时报错
-    #         参数设置后可以重用
-    #
-    #     """
-    #     config = qt.QT_CONFIG
-    #     self.assertEqual(config.mode, 1)
-    #     qt.configure(mode=2)
-    #     self.assertEqual(config.mode, 2)
-    #     self.assertEqual(qt.QT_CONFIG.mode, 2)
-    #     self.assertEqual(config.benchmark_asset, '000300.SH')
-    #     self.assertEqual(config.benchmark_asset_type, 'IDX')
-    #     self.assertEqual(config.asset_pool, '000300.SH')
-    #     self.assertEqual(config.invest_start, '20070110')
-    #     # test temp config_key in run() that works only in run()
-    #     qt.run(self.op,
-    #            mode=1,
-    #            asset_pool='000001.SZ',
-    #            asset_type='E',
-    #            invest_start='20100101',
-    #            visual=False)
-    #     self.assertEqual(config.mode, 2)
-    #     self.assertEqual(qt.QT_CONFIG.mode, 2)
-    #     self.assertEqual(config.benchmark_asset, '000300.SH')
-    #     self.assertEqual(config.benchmark_asset_type, 'IDX')
-    #     self.assertEqual(config.asset_pool, '000300.SH')
-    #     self.assertEqual(config.invest_start, '20070110')
-    #
-    #     config_copy = config.copy()
-    #     qt.configure(config_copy,
-    #                  mode=1,
-    #                  benchmark_asset='000002.SZ',
-    #                  benchmark_asset_type='E')
-    #     self.assertEqual(config.mode, 2)
-    #     self.assertEqual(config.benchmark_asset, '000300.SH')
-    #     self.assertEqual(config.benchmark_asset_type, 'IDX')
-    #     self.assertEqual(config.asset_pool, '000300.SH')
-    #     self.assertEqual(config.invest_start, '20070110')
-    #     self.assertEqual(config_copy.mode, 1)
-    #     self.assertEqual(config_copy.benchmark_asset, '000002.SZ')
-    #     self.assertEqual(config_copy.benchmark_asset_type, 'E')
-    #     self.assertEqual(config_copy.asset_pool, '000300.SH')
-    #     self.assertEqual(config_copy.invest_start, '20070110')
-    #
-    # def test_configuration(self):
-    #     """ 测试CONFIG的显示"""
-    #     print(f'configuration without argument\n')
-    #     qt.configuration()
-    #     print(f'configuration with level=1\n')
-    #     qt.configuration(level=1)
-    #     print(f'configuration with level2\n')
-    #     qt.configuration(level=2)
-    #     print(f'configuration with level3\n')
-    #     qt.configuration(level=3)
-    #     print(f'configuration with level4\n')
-    #     qt.configuration(level=4)
-    #     print(f'configuration with level=1, up_to=3\n')
-    #     qt.configuration(level=1, up_to=3)
-    #     print(f'configuration with info=True\n')
-    #     qt.configuration(default=True)
-    #     print(f'configuration with info=True, verbose=True\n')
-    #     qt.configuration(default=True, verbose=True)
-    #
-    # def test_run_mode_0(self):
-    #     """测试策略的实时信号生成模式"""
-    #     op = qt.Operator(strategies=['stema'], op_type='stepwise')
-    #     op.set_parameter('stema', pars=(6,))
-    #     qt.QT_CONFIG.mode = 0
-    #     # qt.run(op)
-    #     # TODO: running qteasy in mode 0 will enter interactive shell, which is not testable
-    #
-    # def test_run_mode_1(self):
-    #     """测试策略的回测模式,结果打印但不可视化"""
-    #     qt.configure(mode=1,
-    #                  trade_batch_size=1,
-    #                  visual=False,
-    #                  trade_log=True,
-    #                  invest_cash_dates='20070604', )
-    #     qt.run(self.op)
-    #
-    # def test_run_mode_1_visual(self):
-    #     """测试策略的回测模式，结果可视化但不打印"""
-    #     print(f'test plot with no buy-sell points and position indicators')
-    #     qt.configuration(up_to=1, default=True)
-    #     res = qt.run(
-    #             self.op,
-    #             mode=1,
-    #             trade_batch_size=1,
-    #             visual=True,
-    #             trade_log=False,
-    #             buy_sell_points=False,
-    #             show_positions=False,
-    #             invest_cash_dates='20070616',
-    #     )
-    #     self.assertIsInstance(res, dict)
-    #     self.assertIsNone(res['trade_log'])
-    #
-    #     print(f'test plot with both buy-sell points and position indicators')
-    #     qt.configuration(up_to=1, default=True)
-    #     res = qt.run(
-    #             self.op,
-    #             mode=1,
-    #             trade_batch_size=1,
-    #             invest_start='20070604',
-    #             invest_end='20190329',
-    #             invest_cash_amounts=[100_000],
-    #             visual=True,
-    #             trade_log=True,
-    #             buy_sell_points=True,
-    #             show_positions=True,
-    #             invest_cash_dates='20070604',
-    #     )
-    #     self.assertIsInstance(res, dict)
-    #     self.assertIsNotNone(res['trade_log'])
-    #     self.assertIsInstance(res['report'], str)
-    #     print(res['trade_log'])
-    #     print(res['report'])
-    #     print(res['trade_record'])
-    #     print(res['final_value'])
-    #     print(res['info'])
-    #     print(res['sharp'])
-    #     self.assertAlmostEqual(res['final_value'], 341175.59, 0)
-    #
-    # def test_run_mode_2_montecarlo(self):
-    #     """测试策略的优化模式，使用蒙特卡洛寻优"""
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=False)
-    #     print(f'strategy optimization in Montecarlo algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in Montecarlo with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in Montecarlo with multiple sub-idx_range testing')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_montecarlo_visual(self):
-    #     """测试策略的优化模式，使用蒙特卡洛寻优"""
-    #     print(f'strategy optimization in Montecarlo algorithm with parallel ON')
-    #     qt.configuration(up_to=1, default=True)
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20140601',
-    #            opti_cash_dates='20060407',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            test_cash_dates='20140604',
-    #            test_indicators='years,fv,return,mdd,v,ref,alpha,beta,sharp,info',
-    #            # 'years,fv,return,mdd,v,ref,alpha,beta,sharp,info'
-    #            indicator_plot_type='violin',
-    #            parallel=True,
-    #            visual=True)
-    #     qt.configuration(up_to=1, default=True)
-    #
-    # def test_run_mode_2_grid(self):
-    #     """测试策略的优化模式，使用网格寻优"""
-    #     print(f'strategy optimization in grid search algorithm with parallel OFF')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=False)
-    #     print(f'strategy optimization in grid search algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_grid_visual(self):
-    #     """测试策略的优化模式，使用网格寻优"""
-    #     print(f'strategy optimization in grid search algorithm with parallel OFF')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=True,
-    #            indicator_plot_type=0)
-    #     print(f'strategy optimization in grid search algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True,
-    #            indicator_plot_type=1)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True,
-    #            indicator_plot_type=2)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True,
-    #            indicator_plot_type=3)
-    #
-    # def test_run_mode_2_incremental(self):
-    #     """测试策略的优化模式，使用递进步长蒙特卡洛寻优"""
-    #     print(f'strategy optimization in incremental algorithm with parallel OFF')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=10,
-    #            opti_min_volume=5E7,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental with multiple sub-idx_range testing')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_incremental_visual(self):
-    #     """测试策略的优化模式，使用递进步长蒙特卡洛寻优，结果以图表输出"""
-    #     print(f'strategy optimization in incremental algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #     print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #
-    # def test_run_mode_2_predict(self):
-    #     """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果"""
-    #     print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_output_count=20,
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental with with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_predict_visual(self):
-    #     """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果，结果以图表方式输出"""
-    #     print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_output_count=20,
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #     print(f'strategy optimization in incremental with with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #
-    # def test_built_in_timing(self):
-    #     """测试内置的择时策略"""
-    #     # 使用以下参数测试所有qt.built_in中的交易策略
-    #     #   mode=1,
-    #     #   asset_pool='000300.SH, 399006.SZ',
-    #     #   start='20200101',
-    #     #   end='20211231',
-    #     #   trade_log=False,
-    #     #   visual=False,
-    #     # 其他均为默认参数
-    #     print(f'testing built-in strategies')
-    #     for strategy in qt.built_in_strategies():
-    #         print(f'testing strategy {strategy}')
-    #         op = qt.Operator(strategies=[strategy])
-    #         qt.run(
-    #                 op,
-    #                 mode=1,
-    #                 asset_pool='000300.SH, 399006.SZ',
-    #                 invest_start='20200101',
-    #                 invest_end='20211231',
-    #                 trade_log=False,
-    #                 visual=False,
-    #         )
-    #
-    # def test_multi_share_mode_1(self):
-    #     """test built-in strategy selecting finance
-    #     """
-    #     op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
-    #     all_shares = qt.filter_stocks(date='20070101')
-    #     shares_banking = qt.filter_stock_codes(date='20070101', industry='银行')
-    #     print('extracted banking share pool:')
-    #     print(all_shares.loc[all_shares.index.isin(shares_banking)])
-    #     shares_estate = list(all_shares.loc[all_shares.industry == "全国地产"].index.values)
-    #     qt.configure(asset_pool=shares_banking[0:10],
-    #                  asset_type='E',
-    #                  benchmark_asset='000300.SH',
-    #                  benchmark_asset_type='IDX',
-    #                  opti_output_count=50,
-    #                  invest_start='20070101',
-    #                  invest_end='20181231',
-    #                  invest_cash_dates=None,
-    #                  trade_batch_size=1.,
-    #                  mode=1,
-    #                  trade_log=True)
-    #     op.set_parameter('long', pars=())
-    #     op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 0.4),
-    #                      strategy_run_freq='Q',
-    #                      strategy_data_types='pe',
-    #                      sort_ascending=True,
-    #                      weighting='proportion',
-    #                      condition='greater',
-    #                      ubound=0,
-    #                      lbound=0,
-    #                      max_sel_count=0.4)
-    #     op.set_parameter('signal_none', pars=())
-    #     op.set_blender('avg(s0, s1, s2)', 'ls')
-    #     op.info()
-    #     print(f'test portfolio selecting from shares_estate: \n{shares_estate}')
-    #     qt.configuration()
-    #     qt.run(op, visual=True, trade_log=True, trade_batch_size=100)
-    #
-    # def test_many_share_mode_1(self):
-    #     """test built-in strategy selecting finance
-    #     """
-    #     print(f'test portfolio selection from large quantities of shares')
-    #     op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
-    #     qt.configure(asset_pool=qt.filter_stock_codes(date='20070101',
-    #                                                   industry=['银行', '全国地产', '互联网', '环境保护', '区域地产',
-    #                                                             '酒店餐饮', '运输设备', '综合类', '建筑工程', '玻璃',
-    #                                                             '家用电器', '文教休闲', '其他商业', '元器件', 'IT设备',
-    #                                                             '其他建材', '汽车服务', '火力发电', '医药商业', '汽车配件',
-    #                                                             '广告包装', '轻工机械', '新型电力', '多元金融', '饲料',
-    #                                                             '铜', '普钢', '航空', '特种钢',
-    #                                                             '种植业', '出版业', '焦炭加工', '啤酒', '公路', '超市连锁',
-    #                                                             '钢加工', '渔业', '农用机械', '软饮料', '化工机械', '塑料',
-    #                                                             '红黄酒', '橡胶', '家居用品', '摩托车', '电器仪表', '服饰',
-    #                                                             '仓储物流', '纺织机械', '电器连锁', '装修装饰', '半导体',
-    #                                                             '电信运营', '石油开采', '乳制品', '商品城', '公共交通',
-    #                                                             '陶瓷', '船舶'],
-    #                                                   area=['深圳', '北京', '吉林', '江苏', '辽宁', '广东',
-    #                                                         '安徽', '四川', '浙江', '湖南', '河北', '新疆',
-    #                                                         '山东', '河南', '山西', '江西', '青海', '湖北',
-    #                                                         '内蒙', '海南', '重庆', '陕西', '福建', '广西',
-    #                                                         '上海']),
-    #                  asset_type='E',
-    #                  benchmark_asset='000300.SH',
-    #                  benchmark_asset_type='IDX',
-    #                  opti_output_count=50,
-    #                  invest_start='20070101',
-    #                  invest_end='20171228',
-    #                  invest_cash_dates=None,
-    #                  trade_batch_size=1.,
-    #                  mode=1,
-    #                  trade_log=False,
-    #                  hist_dnld_parallel=0)
-    #     print(f'in total a number of {len(qt.QT_CONFIG.asset_pool)} shares are selected!')
-    #     op.set_parameter('long', pars=())
-    #     op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 30),
-    #                      strategy_run_freq='Q',
-    #                      strategy_data_types='basic_eps',
-    #                      sort_ascending=True,
-    #                      weighting='proportion',
-    #                      condition='greater',
-    #                      ubound=0,
-    #                      lbound=0,
-    #                      max_sel_count=30)
-    #     op.set_parameter('signal_none', pars=())
-    #     op.set_blender('avg(s0, s1, s2)', 'close')
-    #     qt.run(op, visual=False, trade_log=True)
-    #
-    # def test_op_stepwise(self):
-    #     """测试stepwise模式下的operator的表，使用两个测试专用交易策略"""
-    #     # confirm that operator running results are same in stepwise and batch type
-    #     op_batch = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='batch')
-    #     op_stepwise = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='step')
-    #     for op in [op_batch, op_stepwise]:
-    #         op.set_parameter(0, window_length=100, pars=(12, 26, 9))
-    #         op.set_parameter(1, window_length=100, pars=(12, 26, 9))
-    #
-    #     qt.configure(
-    #             benchmark_asset='000300.SH',
-    #             benchmark_asset_type='IDX',
-    #             asset_pool='601398.SH, 600000.SH, 000002.SZ',
-    #             asset_type='E',
-    #             opti_output_count=50,
-    #             invest_start='20190101',
-    #             invest_end='20190331',
-    #             trade_batch_size=1.,
-    #             sell_batch_size=1.,
-    #             parallel=True,
-    #             trade_log=False
-    #     )
-    #     print('backtest in batch mode:')
-    #     res_batch = op_batch.run(mode=1)
-    #     print('backtest in stepwise mode:')
-    #     res_stepwise = op_stepwise.run(mode=1)
-    #     val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     print(f'the result of batched operation is\n'
-    #           f'shape: {val_batch.shape}\n'
-    #           f'{val_batch}\n'
-    #           f'and the result of stepwise operation is\n'
-    #           f'shape: {val_stepwise.shape}\n'
-    #           f'{val_stepwise}')
-    #
-    #     self.assertTrue(np.allclose(val_batch, val_stepwise))
-    #     self.assertEqual(res_batch['final_value'],
-    #                      res_stepwise['final_value'])
-    #
-    #     print('backtest in batch mode:')
-    #     res_batch = op_batch.run(
-    #             mode=1,
-    #             invest_start='20180101',
-    #             invest_end='20191231'
-    #     )
-    #     print('backtest in stepwise mode:')
-    #     res_stepwise = op_stepwise.run(
-    #             mode=1,
-    #             invest_start='20180101',
-    #             invest_end='20191231'
-    #     )
-    #     val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #
-    #     self.assertTrue(np.allclose(val_batch, val_stepwise))
-    #     self.assertEqual(res_batch['final_value'],
-    #                      res_stepwise['final_value'])
-    #
-    #     # test operator that utilizes trade data
-    #     stg1 = TestLSStrategy()
-    #     stg2 = TestSelStrategy()
-    #     stg1.window_length = 100
-    #     stg2.window_length = 100
-    #     stg2.strategy_run_freq = '2w'
-    #     op_batch = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='batch')
-    #     op_stepwise = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='stepwise')
-    #     par_stg1 = {'000100': (20, 10),
-    #                 '000200': (20, 10),
-    #                 '000300': (20, 6)}
-    #     par_stg2 = ()
-    #     for op in [op_batch, op_stepwise]:
-    #         op.set_parameter(0, pars=par_stg1, opt_tag=1, par_range=([1, 20], [2, 100]))
-    #         op.set_parameter(1, pars=par_stg2, opt_tag=1)
-    #
-    #     qt.configure(
-    #             benchmark_asset='000300.SH',
-    #             benchmark_asset_type='IDX',
-    #             asset_pool='601398.SH, 600000.SH, 000002.SZ',
-    #             asset_type='E',
-    #             opti_output_count=50,
-    #             invest_start='20190101',
-    #             invest_end='20190331',
-    #             opti_start='20190101',
-    #             opti_end='20191231',
-    #             test_start='20200101',
-    #             test_end='20200331',
-    #             trade_batch_size=100.,
-    #             sell_batch_size=100.,
-    #             parallel=True,
-    #             trade_log=False
-    #     )
-    #     print('output result back testing with test data')
-    #
-    #     print('backtest in batch mode:')
-    #     res_batch = op_batch.run(mode=1)
-    #     print('backtest in stepwise mode:')
-    #     res_stepwise = op_stepwise.run(mode=1)
-    #     val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     print(f'the result of batched operation is\n'
-    #           f'{val_batch}\n'
-    #           f'and the result of stepwise operation is\n'
-    #           f'{val_stepwise}')
-    #
-    #     print('backtest in batch mode in optimization mode:')
-    #     op_batch.run(mode=2)
-    #     print('backtest in stepwise mode in optimization mode')
-    #     op_stepwise.run(mode=2)
-    #
-    #     print('test stepwise mode with different sample freq')
-    #
-    # def test_sell_short(self):
-    #     """ 测试sell_short模式是否能正常工作（买入卖出负份额）"""
-    #     op = qt.Operator([Cross_SMA_PS()], signal_type='PS')
-    #     op.set_parameter(0, pars=(23, 100, 0.02))
-    #     res = qt.run(op,
-    #                  mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=False,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertTrue(no_short_in_res)
-    #     res = qt.run(op,
-    #                  mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=True,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertFalse(no_short_in_res)
-    #     op = qt.Operator([Cross_SMA_PT()], signal_type='PT')
-    #     op.set_parameter(0, (23, 100, 0.02))
-    #     res = qt.run(op, mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=False,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertTrue(no_short_in_res)
-    #     res = qt.run(op, mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=True,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertFalse(no_short_in_res)
+    def setUp(self):
+        # 准备测试所需数据，确保本地数据源有足够的数据
+
+        self.op = qt.Operator(strategies=['dma', 'macd'])
+        print('  START TO TEST QT GENERAL OPERATIONS\n'
+              '=======================================')
+        print(' test environment information')
+        print(f'  python version: {sys.version}')
+        print(f'  qteasy version: {qt.__version__}')
+        print(f'  qteasy root path: {qt.QT_ROOT_PATH}')
+        print(f'  numpy version: {np.__version__}')
+        print(f'  numba version: {nb.__version__}')
+        print(f'  pandas version: {pd.__version__}')
+        self.op.set_parameter('dma', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
+        self.op.set_parameter('macd', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
+        self.op.signal_type = 'pt'
+
+        qt.configure(benchmark_asset='000300.SH',
+                     mode=1,
+                     benchmark_asset_type='IDX',
+                     asset_pool='000300.SH',
+                     asset_type='IDX',
+                     opti_output_count=50,
+                     invest_start='20070110',
+                     trade_batch_size=0.,
+                     sell_batch_size=0.,
+                     parallel=True,
+                     hist_dnld_retry_cnt=3,  # 减少数据下载重试次数，加快测试速度
+                     hist_dnld_retry_wait=0.5,  # 减少数据下载重试等待时间，加快测试速度
+                     hist_dnld_backoff=1.2,  # 减少数据下载重试等待时间，加快测试速度
+                     )
+
+        timing_pars1 = (165, 191, 23)
+        timing_pars2 = {'000100': (77, 118, 144),
+                        '000200': (75, 128, 138),
+                        '000300': (73, 120, 143)}
+        timing_pars3 = (115, 197, 54)
+        self.op.set_blender('pos_2_0(s0, s1)')
+        self.op.set_parameter(stg_id='dma', pars=timing_pars1)
+        self.op.set_parameter(stg_id='macd', pars=timing_pars3)
+
+    def test_configure(self):
+        """测试参数设置
+            通过configure设置参数
+            通过QR_CONFIG直接设置参数
+            设置不存在的参数时报错
+            设置不合法参数时报错
+            参数设置后可以重用
+
+        """
+        config = qt.QT_CONFIG
+        self.assertEqual(config.mode, 1)
+        qt.configure(mode=2)
+        self.assertEqual(config.mode, 2)
+        self.assertEqual(qt.QT_CONFIG.mode, 2)
+        self.assertEqual(config.benchmark_asset, '000300.SH')
+        self.assertEqual(config.benchmark_asset_type, 'IDX')
+        self.assertEqual(config.asset_pool, '000300.SH')
+        self.assertEqual(config.invest_start, '20070110')
+        # test temp config_key in run() that works only in run()
+        qt.run(self.op,
+               mode=1,
+               asset_pool='000001.SZ',
+               asset_type='E',
+               invest_start='20100101',
+               visual=False)
+        self.assertEqual(config.mode, 2)
+        self.assertEqual(qt.QT_CONFIG.mode, 2)
+        self.assertEqual(config.benchmark_asset, '000300.SH')
+        self.assertEqual(config.benchmark_asset_type, 'IDX')
+        self.assertEqual(config.asset_pool, '000300.SH')
+        self.assertEqual(config.invest_start, '20070110')
+
+        config_copy = config.copy()
+        qt.configure(config_copy,
+                     mode=1,
+                     benchmark_asset='000002.SZ',
+                     benchmark_asset_type='E')
+        self.assertEqual(config.mode, 2)
+        self.assertEqual(config.benchmark_asset, '000300.SH')
+        self.assertEqual(config.benchmark_asset_type, 'IDX')
+        self.assertEqual(config.asset_pool, '000300.SH')
+        self.assertEqual(config.invest_start, '20070110')
+        self.assertEqual(config_copy.mode, 1)
+        self.assertEqual(config_copy.benchmark_asset, '000002.SZ')
+        self.assertEqual(config_copy.benchmark_asset_type, 'E')
+        self.assertEqual(config_copy.asset_pool, '000300.SH')
+        self.assertEqual(config_copy.invest_start, '20070110')
+
+    def test_configuration(self):
+        """ 测试CONFIG的显示"""
+        print(f'configuration without argument\n')
+        qt.configuration()
+        print(f'configuration with level=1\n')
+        qt.configuration(level=1)
+        print(f'configuration with level2\n')
+        qt.configuration(level=2)
+        print(f'configuration with level3\n')
+        qt.configuration(level=3)
+        print(f'configuration with level4\n')
+        qt.configuration(level=4)
+        print(f'configuration with level=1, up_to=3\n')
+        qt.configuration(level=1, up_to=3)
+        print(f'configuration with info=True\n')
+        qt.configuration(default=True)
+        print(f'configuration with info=True, verbose=True\n')
+        qt.configuration(default=True, verbose=True)
+
+    def test_run_mode_0(self):
+        """测试策略的实时信号生成模式"""
+        op = qt.Operator(strategies=['stema'], op_type='stepwise')
+        op.set_parameter('stema', pars=(6,))
+        qt.QT_CONFIG.mode = 0
+        # qt.run(op)
+        # TODO: running qteasy in mode 0 will enter interactive shell, which is not testable
+
+    def test_run_mode_1(self):
+        """测试策略的回测模式,结果打印但不可视化"""
+        qt.configure(mode=1,
+                     trade_batch_size=1,
+                     visual=False,
+                     trade_log=True,
+                     invest_cash_dates='20070604', )
+        qt.run(self.op)
+
+    def test_run_mode_1_visual(self):
+        """测试策略的回测模式，结果可视化但不打印"""
+        print(f'test plot with no buy-sell points and position indicators')
+        qt.configuration(up_to=1, default=True)
+        res = qt.run(
+                self.op,
+                mode=1,
+                trade_batch_size=1,
+                visual=True,
+                trade_log=False,
+                buy_sell_points=False,
+                show_positions=False,
+                invest_cash_dates='20070616',
+        )
+        self.assertIsInstance(res, dict)
+        self.assertIsNone(res['trade_log'])
+
+        print(f'test plot with both buy-sell points and position indicators')
+        qt.configuration(up_to=1, default=True)
+        res = qt.run(
+                self.op,
+                mode=1,
+                trade_batch_size=1,
+                invest_start='20070604',
+                invest_end='20190329',
+                invest_cash_amounts=[100_000],
+                visual=True,
+                trade_log=True,
+                buy_sell_points=True,
+                show_positions=True,
+                invest_cash_dates='20070604',
+        )
+        self.assertIsInstance(res, dict)
+        self.assertIsNotNone(res['trade_log'])
+        self.assertIsInstance(res['report'], str)
+        print(res['trade_log'])
+        print(res['report'])
+        print(res['trade_record'])
+        print(res['final_value'])
+        print(res['info'])
+        print(res['sharp'])
+        self.assertAlmostEqual(res['final_value'], 341175.59, 0)
+
+    def test_run_mode_2_montecarlo(self):
+        """测试策略的优化模式，使用蒙特卡洛寻优"""
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=False)
+        print(f'strategy optimization in Montecarlo algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in Montecarlo with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='multiple',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in Montecarlo with multiple sub-idx_range testing')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_montecarlo_visual(self):
+        """测试策略的优化模式，使用蒙特卡洛寻优"""
+        print(f'strategy optimization in Montecarlo algorithm with parallel ON')
+        qt.configuration(up_to=1, default=True)
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20140601',
+               opti_cash_dates='20060407',
+               test_start='20120604',
+               test_end='20201130',
+               test_cash_dates='20140604',
+               test_indicators='years,fv,return,mdd,v,ref,alpha,beta,sharp,info',
+               # 'years,fv,return,mdd,v,ref,alpha,beta,sharp,info'
+               indicator_plot_type='violin',
+               parallel=True,
+               visual=True)
+        qt.configuration(up_to=1, default=True)
+
+    def test_run_mode_2_grid(self):
+        """测试策略的优化模式，使用网格寻优"""
+        print(f'strategy optimization in grid search algorithm with parallel OFF')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=False)
+        print(f'strategy optimization in grid search algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_grid_visual(self):
+        """测试策略的优化模式，使用网格寻优"""
+        print(f'strategy optimization in grid search algorithm with parallel OFF')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=True,
+               indicator_plot_type=0)
+        print(f'strategy optimization in grid search algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True,
+               indicator_plot_type=1)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True,
+               indicator_plot_type=2)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True,
+               indicator_plot_type=3)
+
+    def test_run_mode_2_incremental(self):
+        """测试策略的优化模式，使用递进步长蒙特卡洛寻优"""
+        print(f'strategy optimization in incremental algorithm with parallel OFF')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=10,
+               opti_min_volume=5E7,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=False)
+        print(f'strategy optimization in incremental algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='multiple',
+               test_type='single',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in incremental with multiple sub-idx_range testing')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_incremental_visual(self):
+        """测试策略的优化模式，使用递进步长蒙特卡洛寻优，结果以图表输出"""
+        print(f'strategy optimization in incremental algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+        print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='multiple',
+               test_type='single',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+
+    def test_run_mode_2_predict(self):
+        """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果"""
+        print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_output_count=20,
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in incremental with with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_predict_visual(self):
+        """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果，结果以图表方式输出"""
+        print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_output_count=20,
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+        print(f'strategy optimization in incremental with with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+
+    def test_built_in_timing(self):
+        """测试内置的择时策略"""
+        # 使用以下参数测试所有qt.built_in中的交易策略
+        #   mode=1,
+        #   asset_pool='000300.SH, 399006.SZ',
+        #   start='20200101',
+        #   end='20211231',
+        #   trade_log=False,
+        #   visual=False,
+        # 其他均为默认参数
+        print(f'testing built-in strategies')
+        for strategy in qt.built_in_strategies():
+            print(f'testing strategy {strategy}')
+            op = qt.Operator(strategies=[strategy])
+            qt.run(
+                    op,
+                    mode=1,
+                    asset_pool='000300.SH, 399006.SZ',
+                    invest_start='20200101',
+                    invest_end='20211231',
+                    trade_log=False,
+                    visual=False,
+            )
+
+    def test_multi_share_mode_1(self):
+        """test built-in strategy selecting finance
+        """
+        op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
+        all_shares = qt.filter_stocks(date='20070101')
+        shares_banking = qt.filter_stock_codes(date='20070101', industry='银行')
+        print('extracted banking share pool:')
+        print(all_shares.loc[all_shares.index.isin(shares_banking)])
+        shares_estate = list(all_shares.loc[all_shares.industry == "全国地产"].index.values)
+        qt.configure(asset_pool=shares_banking[0:10],
+                     asset_type='E',
+                     benchmark_asset='000300.SH',
+                     benchmark_asset_type='IDX',
+                     opti_output_count=50,
+                     invest_start='20070101',
+                     invest_end='20181231',
+                     invest_cash_dates=None,
+                     trade_batch_size=1.,
+                     mode=1,
+                     trade_log=True)
+        op.set_parameter('long', pars=())
+        op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 0.4),
+                         strategy_run_freq='Q',
+                         strategy_data_types='pe',
+                         sort_ascending=True,
+                         weighting='proportion',
+                         condition='greater',
+                         ubound=0,
+                         lbound=0,
+                         max_sel_count=0.4)
+        op.set_parameter('signal_none', pars=())
+        op.set_blender('avg(s0, s1, s2)', 'ls')
+        op.info()
+        print(f'test portfolio selecting from shares_estate: \n{shares_estate}')
+        qt.configuration()
+        qt.run(op, visual=True, trade_log=True, trade_batch_size=100)
+
+    def test_many_share_mode_1(self):
+        """test built-in strategy selecting finance
+        """
+        print(f'test portfolio selection from large quantities of shares')
+        op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
+        qt.configure(asset_pool=qt.filter_stock_codes(date='20070101',
+                                                      industry=['银行', '全国地产', '互联网', '环境保护', '区域地产',
+                                                                '酒店餐饮', '运输设备', '综合类', '建筑工程', '玻璃',
+                                                                '家用电器', '文教休闲', '其他商业', '元器件', 'IT设备',
+                                                                '其他建材', '汽车服务', '火力发电', '医药商业', '汽车配件',
+                                                                '广告包装', '轻工机械', '新型电力', '多元金融', '饲料',
+                                                                '铜', '普钢', '航空', '特种钢',
+                                                                '种植业', '出版业', '焦炭加工', '啤酒', '公路', '超市连锁',
+                                                                '钢加工', '渔业', '农用机械', '软饮料', '化工机械', '塑料',
+                                                                '红黄酒', '橡胶', '家居用品', '摩托车', '电器仪表', '服饰',
+                                                                '仓储物流', '纺织机械', '电器连锁', '装修装饰', '半导体',
+                                                                '电信运营', '石油开采', '乳制品', '商品城', '公共交通',
+                                                                '陶瓷', '船舶'],
+                                                      area=['深圳', '北京', '吉林', '江苏', '辽宁', '广东',
+                                                            '安徽', '四川', '浙江', '湖南', '河北', '新疆',
+                                                            '山东', '河南', '山西', '江西', '青海', '湖北',
+                                                            '内蒙', '海南', '重庆', '陕西', '福建', '广西',
+                                                            '上海']),
+                     asset_type='E',
+                     benchmark_asset='000300.SH',
+                     benchmark_asset_type='IDX',
+                     opti_output_count=50,
+                     invest_start='20070101',
+                     invest_end='20171228',
+                     invest_cash_dates=None,
+                     trade_batch_size=1.,
+                     mode=1,
+                     trade_log=False,
+                     hist_dnld_parallel=0)
+        print(f'in total a number of {len(qt.QT_CONFIG.asset_pool)} shares are selected!')
+        op.set_parameter('long', pars=())
+        op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 30),
+                         strategy_run_freq='Q',
+                         strategy_data_types='basic_eps',
+                         sort_ascending=True,
+                         weighting='proportion',
+                         condition='greater',
+                         ubound=0,
+                         lbound=0,
+                         max_sel_count=30)
+        op.set_parameter('signal_none', pars=())
+        op.set_blender('avg(s0, s1, s2)', 'close')
+        qt.run(op, visual=False, trade_log=True)
+
+    def test_op_stepwise(self):
+        """测试stepwise模式下的operator的表，使用两个测试专用交易策略"""
+        # confirm that operator running results are same in stepwise and batch type
+        op_batch = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='batch')
+        op_stepwise = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='step')
+        for op in [op_batch, op_stepwise]:
+            op.set_parameter(0, window_length=100, pars=(12, 26, 9))
+            op.set_parameter(1, window_length=100, pars=(12, 26, 9))
+
+        qt.configure(
+                benchmark_asset='000300.SH',
+                benchmark_asset_type='IDX',
+                asset_pool='601398.SH, 600000.SH, 000002.SZ',
+                asset_type='E',
+                opti_output_count=50,
+                invest_start='20190101',
+                invest_end='20190331',
+                trade_batch_size=1.,
+                sell_batch_size=1.,
+                parallel=True,
+                trade_log=False
+        )
+        print('backtest in batch mode:')
+        res_batch = op_batch.run(mode=1)
+        print('backtest in stepwise mode:')
+        res_stepwise = op_stepwise.run(mode=1)
+        val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        print(f'the result of batched operation is\n'
+              f'shape: {val_batch.shape}\n'
+              f'{val_batch}\n'
+              f'and the result of stepwise operation is\n'
+              f'shape: {val_stepwise.shape}\n'
+              f'{val_stepwise}')
+
+        self.assertTrue(np.allclose(val_batch, val_stepwise))
+        self.assertEqual(res_batch['final_value'],
+                         res_stepwise['final_value'])
+
+        print('backtest in batch mode:')
+        res_batch = op_batch.run(
+                mode=1,
+                invest_start='20180101',
+                invest_end='20191231'
+        )
+        print('backtest in stepwise mode:')
+        res_stepwise = op_stepwise.run(
+                mode=1,
+                invest_start='20180101',
+                invest_end='20191231'
+        )
+        val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+
+        self.assertTrue(np.allclose(val_batch, val_stepwise))
+        self.assertEqual(res_batch['final_value'],
+                         res_stepwise['final_value'])
+
+        # test operator that utilizes trade data
+        stg1 = TestLSStrategy()
+        stg2 = TestSelStrategy()
+        stg1.window_length = 100
+        stg2.window_length = 100
+        stg2.strategy_run_freq = '2w'
+        op_batch = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='batch')
+        op_stepwise = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='stepwise')
+        par_stg1 = {'000100': (20, 10),
+                    '000200': (20, 10),
+                    '000300': (20, 6)}
+        par_stg2 = ()
+        for op in [op_batch, op_stepwise]:
+            op.set_parameter(0, pars=par_stg1, opt_tag=1, par_range=([1, 20], [2, 100]))
+            op.set_parameter(1, pars=par_stg2, opt_tag=1)
+
+        qt.configure(
+                benchmark_asset='000300.SH',
+                benchmark_asset_type='IDX',
+                asset_pool='601398.SH, 600000.SH, 000002.SZ',
+                asset_type='E',
+                opti_output_count=50,
+                invest_start='20190101',
+                invest_end='20190331',
+                opti_start='20190101',
+                opti_end='20191231',
+                test_start='20200101',
+                test_end='20200331',
+                trade_batch_size=100.,
+                sell_batch_size=100.,
+                parallel=True,
+                trade_log=False
+        )
+        print('output result back testing with test data')
+
+        print('backtest in batch mode:')
+        res_batch = op_batch.run(mode=1)
+        print('backtest in stepwise mode:')
+        res_stepwise = op_stepwise.run(mode=1)
+        val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        print(f'the result of batched operation is\n'
+              f'{val_batch}\n'
+              f'and the result of stepwise operation is\n'
+              f'{val_stepwise}')
+
+        print('backtest in batch mode in optimization mode:')
+        op_batch.run(mode=2)
+        print('backtest in stepwise mode in optimization mode')
+        op_stepwise.run(mode=2)
+
+        print('test stepwise mode with different sample freq')
+
+    def test_sell_short(self):
+        """ 测试sell_short模式是否能正常工作（买入卖出负份额）"""
+        op = qt.Operator([Cross_SMA_PS()], signal_type='PS')
+        op.set_parameter(0, pars=(23, 100, 0.02))
+        res = qt.run(op,
+                     mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=False,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertTrue(no_short_in_res)
+        res = qt.run(op,
+                     mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=True,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertFalse(no_short_in_res)
+        op = qt.Operator([Cross_SMA_PT()], signal_type='PT')
+        op.set_parameter(0, (23, 100, 0.02))
+        res = qt.run(op, mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=False,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertTrue(no_short_in_res)
+        res = qt.run(op, mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=True,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertFalse(no_short_in_res)
 
 
 if __name__ == '__main__':
     # get all stock prices from year 2020 to year 2022
     qt.refill_data_source(qt.QT_DATA_SOURCE, tables='stock_daily', start_date='20200101', end_date='20221231')
 
     # get index prices of 000300 and 399006 data from 2005 to year 2022
```

### Comparing `qteasy-1.1.4/tests/test_space.py` & `qteasy-1.1.5/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_ta_funcs.py` & `qteasy-1.1.5/tests/test_ta_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_trader.py` & `qteasy-1.1.5/tests/test_trader.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_trader_shell.py` & `qteasy-1.1.5/tests/test_trader_shell.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_trading.py` & `qteasy-1.1.5/tests/test_trading.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_tushare.py` & `qteasy-1.1.5/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_utilityfuncs.py` & `qteasy-1.1.5/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_visual.py` & `qteasy-1.1.5/tests/test_visual.py`

 * *Files identical despite different names*

