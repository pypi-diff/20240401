# Comparing `tmp/ccsds-0.1.0a6.tar.gz` & `tmp/ccsds-0.1.0b3.tar.gz`

## Comparing `ccsds-0.1.0a6.tar` & `ccsds-0.1.0b3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 ccsds-0.1.0a6/Cargo.toml
--rw-rw----   0     1000     1000       79 2024-01-28 20:54:27.000000 ccsds-0.1.0a6/.gitattributes
--rw-rw-r--   0     1000     1000     2825 2024-01-27 02:47:54.000000 ccsds-0.1.0a6/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      686 2024-01-27 02:47:54.000000 ccsds-0.1.0a6/.gitignore
--rw-rw-r--   0     1000     1000    35149 2024-01-27 23:15:56.000000 ccsds-0.1.0a6/LICENSE.txt
--rw-rw-r--   0     1000     1000      345 2024-01-29 19:03:44.000000 ccsds-0.1.0a6/README.md
--rw-r--r--   0     1000     1000     3336 2024-01-29 19:02:34.000000 ccsds-0.1.0a6/ccsds.pyi
--rw-rw-r--   0     1000     1000     9898 2024-01-29 19:20:04.000000 ccsds-0.1.0a6/src/lib.rs
--rw-rw-r--   0     1000     1000    66560 2024-01-28 20:53:44.000000 ccsds-0.1.0a6/tests/fixtures/snpp_synchronized_cadus.dat
--rw-r--r--   0     1000     1000     1696 2024-01-29 15:20:40.000000 ccsds-0.1.0a6/tests/fixtures/snpp_synchronized_cadus.txt
--rw-rw-r--   0     1000     1000      522 2024-01-29 19:03:20.000000 ccsds-0.1.0a6/tests/test.py
--rw-rw-r--   0     1000     1000    19157 2024-01-29 19:35:45.000000 ccsds-0.1.0a6/Cargo.lock
--rw-rw-r--   0     1000     1000      438 2024-01-29 19:12:16.000000 ccsds-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 ccsds-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 ccsds-0.1.0b3/Cargo.toml
+-rw-rw----   0     1000     1000       79 2024-01-28 20:54:27.000000 ccsds-0.1.0b3/.gitattributes
+-rw-rw-r--   0     1000     1000     2825 2024-01-27 02:47:54.000000 ccsds-0.1.0b3/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      705 2024-04-01 20:19:08.000000 ccsds-0.1.0b3/.gitignore
+-rw-rw-r--   0     1000     1000    35149 2024-01-27 23:15:56.000000 ccsds-0.1.0b3/LICENSE.txt
+-rw-rw-r--   0     1000     1000      671 2024-04-01 20:18:47.000000 ccsds-0.1.0b3/README.md
+-rw-rw-r--   0     1000     1000     1340 2024-04-01 15:04:02.000000 ccsds-0.1.0b3/ccsds.pyi
+-rw-rw-r--   0     1000     1000    19393 2024-04-01 19:42:56.000000 ccsds-0.1.0b3/src/lib.rs
+-rw-rw-r--   0     1000     1000    66560 2024-01-28 20:53:44.000000 ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.dat
+-rw-r--r--   0     1000     1000     1696 2024-01-29 15:20:40.000000 ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.txt
+-rw-rw-r--   0     1000     1000      522 2024-01-29 19:03:20.000000 ccsds-0.1.0b3/tests/test.py
+-rw-rw-r--   0     1000     1000    23562 2024-04-01 20:22:27.000000 ccsds-0.1.0b3/Cargo.lock
+-rw-rw-r--   0     1000     1000      438 2024-01-29 19:12:16.000000 ccsds-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1361 1970-01-01 00:00:00.000000 ccsds-0.1.0b3/PKG-INFO
```

### Comparing `ccsds-0.1.0a6/.github/workflows/CI.yml` & `ccsds-0.1.0b3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0a6/.gitignore` & `ccsds-0.1.0b3/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+spacecraftsdb.json
 /target
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
```

### Comparing `ccsds-0.1.0a6/LICENSE.txt` & `ccsds-0.1.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0a6/tests/fixtures/snpp_synchronized_cadus.dat` & `ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.dat`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0a6/tests/fixtures/snpp_synchronized_cadus.txt` & `ccsds-0.1.0b3/tests/fixtures/snpp_synchronized_cadus.txt`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0a6/tests/test.py` & `ccsds-0.1.0b3/tests/test.py`

 * *Files identical despite different names*

### Comparing `ccsds-0.1.0a6/Cargo.lock` & `ccsds-0.1.0b3/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -14,26 +14,38 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "anyhow"
+version = "1.0.81"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "bumpalo"
 version = "3.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
 
 [[package]]
 name = "cc"
@@ -42,34 +54,38 @@
 checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "ccsds"
-version = "0.1.0-alpha.5"
+version = "0.1.0-beta.3"
+dependencies = [
+ "ccsds 0.1.0-beta.3 (registry+https://github.com/rust-lang/crates.io-index)",
+ "pyo3",
+ "spacecrafts",
+]
+
+[[package]]
+name = "ccsds"
+version = "0.1.0-beta.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e6c65b278e658512f1cf9fbeecca9ec62e58f3891768580d333deaaa0c16327"
+checksum = "e0c2f521790a26fed2945439b2cc67cb4f950f4b0f3293c0e1bdfce36d4a9a17"
 dependencies = [
  "chrono",
+ "crossbeam",
  "ndarray",
  "rayon",
  "rs2",
  "serde",
  "serde_json",
+ "spacecrafts",
  "thiserror",
  "threadpool",
-]
-
-[[package]]
-name = "ccsds"
-version = "0.1.0-alpha.6"
-dependencies = [
- "ccsds 0.1.0-alpha.5",
- "pyo3",
+ "tracing",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -92,14 +108,36 @@
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
+name = "crossbeam"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1137cd7e7fc0fb5d3c5a8678be38ec56e819125d8d7907411fe24ccb943faca8"
+dependencies = [
+ "crossbeam-channel",
+ "crossbeam-deque",
+ "crossbeam-epoch",
+ "crossbeam-queue",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-channel"
+version = "0.5.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
  "crossbeam-epoch",
  "crossbeam-utils",
@@ -111,26 +149,67 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "crossbeam-queue"
+version = "0.3.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "df0346b5d5e76ac2fe4e327c5fd1118d6be7c51dfb18f9b7922923f287471e35"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
+name = "dirs"
+version = "5.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
+dependencies = [
+ "dirs-sys",
+]
+
+[[package]]
+name = "dirs-sys"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
+dependencies = [
+ "libc",
+ "option-ext",
+ "redox_users",
+ "windows-sys",
+]
+
+[[package]]
 name = "either"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
+name = "getrandom"
+version = "0.2.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
 name = "hermit-abi"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d3d0e0f38255e7fa3cf31335b3a56f05febd18025f4db5ef7a0cfb4f8da651f"
 
 [[package]]
 name = "iana-time-zone"
@@ -179,14 +258,24 @@
 [[package]]
 name = "libc"
 version = "0.2.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
 
 [[package]]
+name = "libredox"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
+dependencies = [
+ "bitflags 2.5.0",
+ "libc",
+]
+
+[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -271,14 +360,20 @@
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -294,14 +389,20 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "pin-project-lite"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
@@ -403,15 +504,26 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "redox_users"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
+dependencies = [
+ "getrandom",
+ "libredox",
+ "thiserror",
 ]
 
 [[package]]
 name = "rs2"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44b2e9b1a862d7e012298e5f24642050cc205e973bce20a656befe95d8c4a0d3"
@@ -462,14 +574,26 @@
 [[package]]
 name = "smallvec"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
+name = "spacecrafts"
+version = "0.1.0-beta.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e58f5eaffcab38b70cdd65f05b3bf0e781d3947ba0fae71fd1e934fd00366a8a"
+dependencies = [
+ "anyhow",
+ "dirs",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -519,26 +643,64 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
 dependencies = [
  "num_cpus",
 ]
 
 [[package]]
+name = "tracing"
+version = "0.1.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
+dependencies = [
+ "log",
+ "pin-project-lite",
+ "tracing-attributes",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-attributes"
+version = "0.1.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.48",
+]
+
+[[package]]
+name = "tracing-core"
+version = "0.1.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
+dependencies = [
+ "once_cell",
+]
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+
+[[package]]
 name = "wasm-bindgen"
 version = "0.2.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1223296a201415c7fad14792dbefaace9bd52b62d33453ade1c5b5f07555406"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
@@ -594,14 +756,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
  "windows-targets 0.52.0",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.5",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.5",
  "windows_aarch64_msvc 0.48.5",
```

### Comparing `ccsds-0.1.0a6/PKG-INFO` & `ccsds-0.1.0b3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ccsds
-Version: 0.1.0a6
+Version: 0.1.0b3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: pytest ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE.txt
@@ -20,8 +20,13 @@
 
 [![Actions Status](https://img.shields.io/github/actions/workflow/status/bmflynn/ccsdspy/CI.yml?branch=main&logo=github&style=flat-square)](https://github.com/bmflynn/ccsdspy/actions)
 
 `ccsdspy` provides Python bindnigs for the [ccsds](https://github.com/bmflynn/ccsds-rs)
 Rust bindings using [pyo3](https://pyo3.rs).
 
 
+## Related
+
+* [spacecraftsdb](https://github.com/bmflynn/spacecraftsdb): JSON Spacecraft metadata database
+* [spacecrafts-rs](https://github.com/bmflynn/spacecrafts-rs): Rust crate interfacing with `spacecraftsdb`
+* [ccsds-rs](https://github.com/bmflynn/ccsds-rs): Rust crate for CCSDS spacecraft frame & spacepacket decoding
```

