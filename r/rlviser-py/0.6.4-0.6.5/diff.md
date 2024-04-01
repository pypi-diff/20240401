# Comparing `tmp/rlviser_py-0.6.4.tar.gz` & `tmp/rlviser_py-0.6.5.tar.gz`

## Comparing `rlviser_py-0.6.4.tar` & `rlviser_py-0.6.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.4/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/LICENSE
--rw-r--r--   0     1001      127     1557 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/README.md
--rw-r--r--   0     1001      127     2877 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/gym_renderer.py
--rw-r--r--   0     1001      127     2379 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/pygymtest.py
--rw-r--r--   0     1001      127      699 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/rlviser_py.pyi
--rw-r--r--   0     1001      127    16879 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/src/bytes.rs
--rw-r--r--   0     1001      127     3034 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/src/lib.rs
--rw-r--r--   0     1001      127     2308 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/src/socket.rs
--rw-r--r--   0     1001      127     7861 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/Cargo.lock
--rw-r--r--   0     1001      127      387 2024-03-30 21:29:04.000000 rlviser_py-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.5/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/LICENSE
+-rw-r--r--   0     1001      127     1557 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/README.md
+-rw-r--r--   0     1001      127     2877 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/gym_renderer.py
+-rw-r--r--   0     1001      127     2379 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/pygymtest.py
+-rw-r--r--   0     1001      127     1030 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/rlviser_py.pyi
+-rw-r--r--   0     1001      127    16891 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/src/bytes.rs
+-rw-r--r--   0     1001      127     3034 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/src/lib.rs
+-rw-r--r--   0     1001      127     2356 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/src/socket.rs
+-rw-r--r--   0     1001      127     7861 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/Cargo.lock
+-rw-r--r--   0     1001      127      387 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.5/PKG-INFO
```

### Comparing `rlviser_py-0.6.4/Cargo.toml` & `rlviser_py-0.6.5/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlviser-py"
-version = "0.6.4"
+version = "0.6.5"
 edition = "2021"
 description = "Python implementation that manages a UDP connection to RLViser"
 license = "MIT"
 repository = "https://github.com/VirxEC/rlviser-py"
 readme = "README.md"
 keywords = ["rlviser", "rocket-league", "udp", "python", "rlbot"]
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore"]
```

### Comparing `rlviser_py-0.6.4/LICENSE` & `rlviser_py-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.4/README.md` & `rlviser_py-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.4/gym_renderer.py` & `rlviser_py-0.6.5/gym_renderer.py`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.4/pygymtest.py` & `rlviser_py-0.6.5/pygymtest.py`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.4/src/bytes.rs` & `rlviser_py-0.6.5/src/bytes.rs`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             heatseeker_time_since_hit: 0.,
         }
     }
 }
 
 impl BallState {
     #[inline]
-    pub fn to_array(self) -> TBall {
+    pub const fn to_array(self) -> TBall {
         (
             self.pos.to_array(),
             self.rot_mat.to_array(),
             self.vel.to_array(),
             self.ang_vel.to_array(),
         )
     }
@@ -228,15 +228,15 @@
     pub config: CarConfig,
 }
 
 pub type TCar = (u32, TVec3, TRotMat, TVec3, TVec3, f32, bool, bool, bool, f32);
 
 impl CarInfo {
     #[inline]
-    pub fn to_array(self) -> TCar {
+    pub const fn to_array(self) -> TCar {
         (
             self.id,
             self.state.pos.to_array(),
             self.state.rot_mat.to_array(),
             self.state.vel.to_array(),
             self.state.ang_vel.to_array(),
             self.state.boost,
```

### Comparing `rlviser_py-0.6.4/src/lib.rs` & `rlviser_py-0.6.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.4/src/socket.rs` & `rlviser_py-0.6.5/src/socket.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 use std::{
     io,
     net::{SocketAddr, UdpSocket},
     process::Command,
     sync::OnceLock,
 };
 
+const ROCKETSIM_PORT: u16 = 34254;
+
 #[repr(u8)]
 enum UdpPacketTypes {
     Quit,
     GameState,
 }
 
 const RLVISER_PATH: &str = if cfg!(windows) { "./rlviser.exe" } else { "./rlviser" };
@@ -19,15 +21,15 @@
 pub fn init() -> io::Result<(UdpSocket, SocketAddr)> {
     // launch RLViser
     if let Err(e) = Command::new(RLVISER_PATH).spawn() {
         println!("Failed to launch RLViser ({RLVISER_PATH}): {e}");
     }
 
     // Connect to RLViser
-    let socket = UdpSocket::bind("0.0.0.0:34254")?;
+    let socket = UdpSocket::bind(("0.0.0.0", ROCKETSIM_PORT))?;
 
     println!("Waiting for connection to socket...");
     let mut buf = [0; 1];
     let (_, src) = socket.recv_from(&mut buf)?;
 
     if buf[0] == 1 {
         println!("Connection established to {src}");
```

### Comparing `rlviser_py-0.6.4/Cargo.lock` & `rlviser_py-0.6.5/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -99,17 +99,17 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a02a88a17e74cadbc8ce77855e1d6c8ad0ab82901a4a9b5046bd01c1c0bd95cd"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -117,49 +117,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5eb0b6ecba38961f6f4bd6cd5906dfab3cd426ff37b2eed5771006aa31656f1"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba8a6e48a29b5d22e4fdaf132d8ba8d3203ee9f06362d48f244346902a594ec3"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e80493c5965f94a747d0782a607b2328a4eea5391327b152b00e2f3b001cede"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcd7d86f42004025200e12a6a8119bd878329e6fddef8178eaafa4e4b5906c5b"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -180,15 +180,15 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.6.4"
+version = "0.6.5"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
```

### Comparing `rlviser_py-0.6.4/PKG-INFO` & `rlviser_py-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlviser-py
-Version: 0.6.4
+Version: 0.6.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python implementation that manages a UDP connection to RLViser
 Keywords: rlviser,rocket-league,udp,python,rlbot
 License: MIT
```

