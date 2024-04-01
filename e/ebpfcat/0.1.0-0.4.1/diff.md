# Comparing `tmp/ebpfcat-0.1.0.tar.gz` & `tmp/ebpfcat-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/ebpfcat/dist/tmpga44uj35/ebpfcat-0.1.0.tar", last modified: Fri Mar  5 20:11:29 2021, max compression
+gzip compressed data, was "ebpfcat-0.4.1.tar", last modified: Mon Apr  1 12:59:16 2024, max compression
```

## Comparing `ebpfcat-0.1.0.tar` & `ebpfcat-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/
--rw-r--r--   0 pi        (1000) pi        (1000)      257 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      408 2021-03-05 08:11:41.000000 ebpfcat-0.1.0/README.rst
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/ebpfcat/
--rw-r--r--   0 pi        (1000) pi        (1000)      835 2021-03-05 19:29:30.000000 ebpfcat-0.1.0/ebpfcat/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5314 2021-03-05 08:00:13.000000 ebpfcat-0.1.0/ebpfcat/arraymap.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4972 2021-03-05 19:29:30.000000 ebpfcat-0.1.0/ebpfcat/bpf.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6218 2021-03-04 23:53:04.000000 ebpfcat-0.1.0/ebpfcat/devices.py
--rw-r--r--   0 pi        (1000) pi        (1000)    35896 2021-03-04 23:53:04.000000 ebpfcat-0.1.0/ebpfcat/ebpf.py
--rw-r--r--   0 pi        (1000) pi        (1000)    30442 2021-03-05 19:29:30.000000 ebpfcat-0.1.0/ebpfcat/ebpf_test.py
--rw-r--r--   0 pi        (1000) pi        (1000)    14336 2021-03-05 19:29:30.000000 ebpfcat-0.1.0/ebpfcat/ebpfcat.py
--rw-r--r--   0 pi        (1000) pi        (1000)    28429 2021-03-05 19:29:30.000000 ebpfcat-0.1.0/ebpfcat/ethercat.py
--rw-r--r--   0 pi        (1000) pi        (1000)    12908 2021-03-05 19:29:30.000000 ebpfcat-0.1.0/ebpfcat/ethercat_test.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4065 2021-03-04 23:53:04.000000 ebpfcat-0.1.0/ebpfcat/hashmap.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3418 2021-03-04 23:53:04.000000 ebpfcat-0.1.0/ebpfcat/serial.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3553 2021-03-04 23:53:04.000000 ebpfcat-0.1.0/ebpfcat/terminals.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5040 2021-03-04 23:53:04.000000 ebpfcat-0.1.0/ebpfcat/xdp.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/ebpfcat.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      257 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/ebpfcat.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      410 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/ebpfcat.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/ebpfcat.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/ebpfcat.egg-info/top_level.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/examples/
--rw-r--r--   0 pi        (1000) pi        (1000)      544 2021-03-05 19:59:31.000000 ebpfcat-0.1.0/examples/count.py
--rw-r--r--   0 pi        (1000) pi        (1000)      249 2021-03-05 20:11:29.000000 ebpfcat-0.1.0/setup.cfg
+drwxr-xr-x   0 papa      (1001) papa      (1002)        0 2024-04-01 12:59:16.064608 ebpfcat-0.4.1/
+-rw-r--r--   0 papa      (1001) papa      (1002)    18092 2023-12-25 10:28:18.000000 ebpfcat-0.4.1/LICENSE
+-rw-r--r--   0 papa      (1001) papa      (1002)      223 2024-04-01 12:59:16.064608 ebpfcat-0.4.1/PKG-INFO
+-rw-r--r--   0 papa      (1001) papa      (1002)      408 2023-12-25 10:28:18.000000 ebpfcat-0.4.1/README.rst
+drwxr-xr-x   0 papa      (1001) papa      (1002)        0 2024-04-01 12:59:16.063608 ebpfcat-0.4.1/ebpfcat/
+-rw-r--r--   0 papa      (1001) papa      (1002)      835 2023-12-25 10:28:18.000000 ebpfcat-0.4.1/ebpfcat/__init__.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     4209 2023-12-30 18:44:20.000000 ebpfcat-0.4.1/ebpfcat/arraymap.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     5438 2023-12-30 18:44:20.000000 ebpfcat-0.4.1/ebpfcat/bpf.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     6376 2023-12-30 18:44:20.000000 ebpfcat-0.4.1/ebpfcat/devices.py
+-rw-r--r--   0 papa      (1001) papa      (1002)    45137 2024-03-19 11:26:55.000000 ebpfcat-0.4.1/ebpfcat/ebpf.py
+-rw-r--r--   0 papa      (1001) papa      (1002)    49180 2024-03-19 11:17:39.000000 ebpfcat-0.4.1/ebpfcat/ebpf_test.py
+-rw-r--r--   0 papa      (1001) papa      (1002)    22032 2024-03-18 07:40:24.000000 ebpfcat-0.4.1/ebpfcat/ebpfcat.py
+-rw-r--r--   0 papa      (1001) papa      (1002)    36241 2024-03-18 07:40:24.000000 ebpfcat-0.4.1/ebpfcat/ethercat.py
+-rw-r--r--   0 papa      (1001) papa      (1002)    17840 2024-02-23 11:36:08.000000 ebpfcat-0.4.1/ebpfcat/ethercat_test.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     3978 2023-12-30 18:44:20.000000 ebpfcat-0.4.1/ebpfcat/hashmap.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     6068 2024-02-23 11:36:08.000000 ebpfcat-0.4.1/ebpfcat/scripts.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     3418 2023-12-25 10:28:18.000000 ebpfcat-0.4.1/ebpfcat/serial.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     6620 2024-03-18 07:40:24.000000 ebpfcat-0.4.1/ebpfcat/terminals.py
+-rw-r--r--   0 papa      (1001) papa      (1002)    96161 2023-12-25 10:28:18.000000 ebpfcat-0.4.1/ebpfcat/testdata.py
+-rw-r--r--   0 papa      (1001) papa      (1002)      893 2023-12-25 10:28:18.000000 ebpfcat-0.4.1/ebpfcat/util.py
+-rw-r--r--   0 papa      (1001) papa      (1002)     8768 2023-12-30 18:44:20.000000 ebpfcat-0.4.1/ebpfcat/xdp.py
+drwxr-xr-x   0 papa      (1001) papa      (1002)        0 2024-04-01 12:59:16.064608 ebpfcat-0.4.1/ebpfcat.egg-info/
+-rw-r--r--   0 papa      (1001) papa      (1002)      223 2024-04-01 12:59:16.000000 ebpfcat-0.4.1/ebpfcat.egg-info/PKG-INFO
+-rw-r--r--   0 papa      (1001) papa      (1002)      504 2024-04-01 12:59:16.000000 ebpfcat-0.4.1/ebpfcat.egg-info/SOURCES.txt
+-rw-r--r--   0 papa      (1001) papa      (1002)        1 2024-04-01 12:59:16.000000 ebpfcat-0.4.1/ebpfcat.egg-info/dependency_links.txt
+-rw-r--r--   0 papa      (1001) papa      (1002)      166 2024-04-01 12:59:16.000000 ebpfcat-0.4.1/ebpfcat.egg-info/entry_points.txt
+-rw-r--r--   0 papa      (1001) papa      (1002)        8 2024-04-01 12:59:16.000000 ebpfcat-0.4.1/ebpfcat.egg-info/top_level.txt
+-rw-r--r--   0 papa      (1001) papa      (1002)      395 2024-04-01 12:59:00.000000 ebpfcat-0.4.1/pyproject.toml
+-rw-r--r--   0 papa      (1001) papa      (1002)      249 2024-04-01 12:59:16.064608 ebpfcat-0.4.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ebpfcat-0.1.0/ebpfcat/__init__.py` & `ebpfcat-0.4.1/ebpfcat/__init__.py`

 * *Files identical despite different names*

### Comparing `ebpfcat-0.1.0/ebpfcat/arraymap.py` & `ebpfcat-0.4.1/ebpfcat/arraymap.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,138 +11,112 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
+"""The ``arraymap`` module defines array maps, usually used for global
+variables in EBPF programs"""
+
+__all__ = ["ArrayMap"]
+
 from itertools import chain
+from mmap import mmap
 from struct import pack_into, unpack_from, calcsize
 
-from .ebpf import FuncId, Map, MemoryDesc
-from .bpf import create_map, lookup_elem, MapType, update_elem
+from .ebpf import Expression, FuncId, Map, MemoryDesc, Opcode, SubProgram
+from .bpf import create_map, lookup_elem, MapType, MapFlags, update_elem
 
 
 class ArrayGlobalVarDesc(MemoryDesc):
     base_register = 0
 
-    def __init__(self, map, fmt, write=False):
+    def __init__(self, map, fmt):
         self.map = map
         self.fmt = fmt
-        self.write = write
+        self.fixed = fmt == "x"
 
     def fmt_addr(self, ebpf):
         return self.fmt, ebpf.__dict__[self.name]
 
     def __set_name__(self, owner, name):
         self.name = name
 
     def __get__(self, instance, owner):
         if instance is None:
             return self
         if instance.ebpf.loaded:
             fmt, addr = self.fmt_addr(instance)
             data = instance.ebpf.__dict__[self.map.name].data
-            ret = unpack_from(fmt, data, addr)
+            if fmt == "x":
+                return unpack_from("q", data, addr)[0] / Expression.FIXED_BASE
+            else:
+                ret = unpack_from(fmt, data, addr)
             if len(ret) == 1:
                 return ret[0]
             else:
                 return ret
         else:
             return super().__get__(instance, owner)
 
     def __set__(self, instance, value):
         if instance.ebpf.loaded:
             fmt, addr = self.fmt_addr(instance)
+            if fmt == "x":
+                fmt = "q"
+                value = int(value * Expression.FIXED_BASE)
             if not isinstance(value, tuple):
                 value = value,
             pack_into(fmt, instance.ebpf.__dict__[self.map.name].data,
                       addr, *value)
         else:
             super().__set__(instance, value)
 
 
 class ArrayMapAccess:
     """This is the array map proper"""
-    def __init__(self, fd, write_size, size):
+    def __init__(self, fd, size):
+        self.data = mmap(fd, size)
         self.fd = fd
-        self.write_size = write_size
         self.size = size
-        self.data = bytearray(size)
-
-    def read(self):
-        """read all variables in the map from EBPF to user space"""
-        self.data = lookup_elem(self.fd, b"\0\0\0\0", self.size)
-
-    def write(self):
-        """write all variables in the map from user space to EBPF
-
-        *all* variables are written, even those not marked ``write=True``
-        """
-        update_elem(self.fd, b"\0\0\0\0", self.data, 0)
-
-    def readwrite(self):
-        """read variables from EBPF and write them out immediately
-
-        This reads all variables, swaps in the user-modified values for
-        the ``write=True`` variables, and writes the out again
-        immediately.
-
-        This means that even the read-only variables will be overwritten
-        with the values we have just read. If the EBPF program changed
-        the value in the meantime, that may be a problem.
-
-        Note that after this method returns, all *write* variables
-        will have the value from the EBPF program in user space, and
-        vice-versa.
-        """
-        write = self.data[:self.write_size]
-        data = lookup_elem(self.fd, b"\0\0\0\0", self.size)
-        self.data[:] = data
-        data[:self.write_size] = write
-        update_elem(self.fd, b"\0\0\0\0", data, 0)
 
 
 class ArrayMap(Map):
     """A descriptor for an array map"""
-    def globalVar(self, fmt="I", write=False):
-        return ArrayGlobalVarDesc(self, fmt, write)
+
+    def globalVar(self, fmt="I"):
+        return ArrayGlobalVarDesc(self, fmt)
 
     def collect(self, ebpf):
         collection = []
 
         for prog in chain([ebpf], ebpf.subprograms):
             for k, v in prog.__class__.__dict__.items():
                 if isinstance(v, ArrayGlobalVarDesc):
-                    collection.append((v.write, calcsize(v.fmt), prog, k))
-        collection.sort(key=lambda t: t[:2], reverse=True)
+                    collection.append((8 if v.fmt == "x" else calcsize(v.fmt),
+                                       prog, k))
+        collection.sort(key=lambda t: t[0], reverse=True)
         position = 0
-        last_write = write = True
-        for write, size, prog, name in collection:
-            if last_write != write:
-                position = (position + 7) & -8
-                write_size = position
+        for size, prog, name in collection:
             prog.__dict__[name] = position
             position += size
-            last_write = write
-        if write:  # there are read variables
-            return position, position
-        else:
-            return write_size, position
+        return position
 
     def __set_name__(self, owner, name):
         self.name = name
 
-    def init(self, ebpf):
+    def init(self, ebpf, fd):
         setattr(ebpf, self.name, 0)
-        write_size, size = self.collect(ebpf)
+        size = self.collect(ebpf)
         if not size:  # nobody is actually using the map
             return
-        fd = create_map(MapType.ARRAY, 4, size, 1)
-        setattr(ebpf, self.name, ArrayMapAccess(fd, write_size, size))
+        if fd is None:
+            fd = create_map(MapType.ARRAY, 4, size, 1, MapFlags.MMAPABLE)
+        setattr(ebpf, self.name, ArrayMapAccess(fd, size))
         with ebpf.save_registers(list(range(6))), ebpf.get_stack(4) as stack:
             ebpf.mI[ebpf.r10 + stack] = 0
             ebpf.r1 = ebpf.get_fd(fd)
             ebpf.r2 = ebpf.r10 + stack
             ebpf.call(FuncId.map_lookup_elem)
             with ebpf.r0 == 0:
                 ebpf.exit()
```

### Comparing `ebpfcat-0.1.0/ebpfcat/bpf.py` & `ebpfcat-0.4.1/ebpfcat/bpf.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 """\
 A module that wraps the `bpf` system call in Python, using `ctypes`.
 """
 from ctypes import CDLL, c_int, get_errno, cast, c_void_p, create_string_buffer, c_char_p, addressof, c_char
-from enum import Enum
+from enum import Enum, Flag
 from struct import pack, unpack
 from platform import machine
 
 from os import strerror
 
 try:
     SYS_BPF = {
         "armv7l": 386,
         "x86_64": 321,
+        "aarch64": 280,
         }[machine()]
 except KeyError:
     print("Unknown platform:", machine())
 
 
 class BPFError(OSError):
     pass
@@ -56,14 +57,18 @@
     DEVMAP = 14
     SOCKMAP = 15
     CPUMAP = 16
     XSKMAP = 17
     SOCKHASH = 18
 
 
+class MapFlags(Flag):
+    MMAPABLE = 1 << 10
+
+
 class ProgType(Enum):
     UNSPEC = 0
     SOCKET_FILTER = 1
     KPROBE = 2
     SCHED_CLS = 3
     SCHED_ACT = 4
     TRACEPOINT = 5
@@ -92,17 +97,20 @@
     attr = pack(fmt, *args)
     attr = create_string_buffer(attr, len(attr))
     ret = libc.syscall(SYS_BPF, c_int(cmd), attr, len(attr))
     if ret == -1:
         raise OSError(get_errno(), strerror(get_errno()))
     return ret, unpack(fmt, attr.raw)
 
-def create_map(map_type, key_size, value_size, max_entries):
+def create_map(map_type, key_size, value_size, max_entries,
+               attributes=MapFlags(0)):
     assert isinstance(map_type, MapType)
-    return bpf(0, "IIII", map_type.value, key_size, value_size, max_entries)[0]
+    assert isinstance(attributes, MapFlags)
+    return bpf(0, "IIIII", map_type.value, key_size, value_size, max_entries,
+               attributes.value)[0]
 
 def lookup_elem(fd, key, size):
     value = bytearray(size)
     addr = addressof(c_char.from_buffer(value))
     ret, _ = bpf(1, "IQQQ", fd, addrof(key), addr, 0)
     if ret == 0:
         return value
@@ -112,14 +120,17 @@
 def update_elem(fd, key, value, flags):
     if isinstance(value, bytearray):
         addr = addressof(c_char.from_buffer(value))
     else:
         addr = addrof(value)
     return bpf(2, "IQQQ", fd, addrof(key), addr, flags)[0]
 
+def delete_elem(fd, key):
+    return bpf(3, "IQ", fd, addrof(key))[0]
+
 def prog_load(prog_type, insns, license,
               log_level=0, log_size=4096, kern_version=0, flags=0,
               name="", ifindex=0, attach_type=0):
     if log_level == 0:
         log_buf = 0
         log_size = 0
     else:
@@ -136,14 +147,23 @@
             raise BPFError(e.errno, the_logbuf.value.decode("utf8"))
         raise
     if log_level != 0:
         return fd, the_logbuf.value.decode("utf8")
     else:
         return fd
 
+def obj_pin(pathname, fd):
+    pn = pathname.encode("utf8")
+    bpf(6, "QI", addrof(pn), fd)
+
+def obj_get(pathname):
+    pn = pathname.encode("utf8")
+    fd, _ = bpf(7, "Q", addrof(pn))
+    return fd
+
 def prog_test_run(fd, data_in, data_out, ctx_in, ctx_out,
                   repeat=1):
     if isinstance(data_in, int):
         data_in = create_string_buffer(data_in)
     else:
         data_in = create_string_buffer(data_in, len(data_in))
     if isinstance(ctx_in, int):
```

### Comparing `ebpfcat-0.1.0/ebpfcat/devices.py` & `ebpfcat-0.4.1/ebpfcat/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,28 @@
     It will read from there and return the result in its
     parameter `value`.
     """
     value = DeviceVar(write=False)
     data = TerminalVar()
 
     def __init__(self, data):
+        super().__init__()
         self.data = data
 
     def program(self):
-        self.value = self.data
+        # it does not make much sense to copy data faster than
+        # we can process
+        return
 
     def update(self):
         self.value = self.data
 
+    def fast_update(self):
+        self.value = self.data
+
 
 class AnalogOutput(Device):
     """Generic analog output device
 
     This device can be linked to an analog output of a terminal.
     It will write the `value` to that terminal.
     """
```

### Comparing `ebpfcat-0.1.0/ebpfcat/ebpf.py` & `ebpfcat-0.4.1/ebpfcat/ebpf.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,21 +11,27 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
+"""The ``ebpf`` module contains the core ebpf code generation"""
+
+__all__ = ["EBPF", "LocalVar", "prandom", "ktime"]
+
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from contextlib import contextmanager, ExitStack
+from operator import index
 from struct import pack, unpack, calcsize
 from enum import Enum
 
 from . import bpf
+from .util import sub
 
 Instruction = namedtuple("Instruction",
                          ["opcode", "dst", "src", "off", "imm"])
 
 
 class FuncId(Enum):
     unspec = 0
@@ -224,14 +230,16 @@
     B = 0x10
     DW = 0x18
 
     LD = 0x61
     ST = 0x62
     STX = 0x63
     XADD = 0xc3
+    LE = 0xd4
+    BE = 0xdc
 
     def __mul__(self, value):
         if value:
             return OpcodeFlags({self})
         else:
             return OpcodeFlags(set())
 
@@ -262,35 +270,53 @@
         return self.value == value.value
 
 
 class AssembleError(Exception):
     pass
 
 
-def comparison(uposop, unegop, sposop=None, snegop=None):
-    if sposop is None:
-        sposop = uposop
-        snegop = unegop
+def comparison(uposop, unegop, sposop, snegop):
     def ret(self, value):
-        return SimpleComparison(self.ebpf, self, value,
-                                (uposop, unegop, sposop, snegop))
+        value = ensure_expression(self.ebpf, value)
+        myself = self
+        if self.fixed != value.fixed:
+            if self.fixed:
+                value *= self.FIXED_BASE
+            else:
+                myself *= self.FIXED_BASE
+
+        if self.signed or value.signed:
+            return SimpleComparison(self.ebpf, myself, value, (sposop, snegop))
+        else:
+            return SimpleComparison(self.ebpf, myself, value, (uposop, unegop))
     return ret
 
 
+class Elser:
+    def __init__(self, comp):
+        self.comp = comp
+
+    def __enter__(self):
+        return self.comp.Else()
+
+    def __exit__(self, exc_type, exc, tb):
+        self.comp.__exit__(exc_type, exc, tb)
+
+
 class Comparison(ABC):
     """Base class for all logical operations"""
 
     def __init__(self, ebpf):
         self.ebpf = ebpf
         self.else_origin = None
 
     def __enter__(self):
         if self.else_origin is None:
             self.compare(True)
-        return self
+        return Elser(self)
 
     def __exit__(self, exc_type, exc, tb):
         if self.else_origin is None:
             self.target()
             return
         assert self.ebpf.opcodes[self.else_origin] is None
         self.ebpf.opcodes[self.else_origin] = Instruction(
@@ -331,48 +357,47 @@
     def __or__(self, value):
         return AndOrComparison(self.ebpf, self, value, False)
 
     def __invert__(self):
         return InvertComparison(self.ebpf, self)
 
     def __bool__(self):
-        raise RuntimeError("Use with statement for comparisons")
+        raise AssembleError("Use with statement for comparisons")
 
 
 class SimpleComparison(Comparison):
     """A simple numerical comparison, results in a jump instruction"""
 
     def __init__(self, ebpf, left, right, opcode):
         super().__init__(ebpf)
         self.left = left
         self.right = right
         self.opcode = opcode
 
     def compare(self, negative):
-        with self.left.calculate(None, None, None) as (self.dst, _, lsigned):
+        with self.left.calculate(None, None) as (self.dst, _):
             with ExitStack() as exitStack:
-                if isinstance(self.right, int):
-                    rsigned = (self.right < 0)
-                else:
-                    self.src, _, rsigned = exitStack.enter_context(
-                            self.right.calculate(None, None, None))
+                if not self.right.small_constant:
+                    self.src, _ = exitStack.enter_context(
+                        self.right.calculate(None, None))
                 self.origin = len(self.ebpf.opcodes)
                 self.ebpf.opcodes.append(None)
-                self.opcode = self.opcode[negative + 2 * (lsigned or rsigned)]
+                self.opcode = self.opcode[negative]
         self.owners = self.ebpf.owners.copy()
 
     def target(self, retarget=False):
         assert retarget or self.ebpf.opcodes[self.origin] is None
         if self.opcode == Opcode.JMP:
             inst = Instruction(Opcode.JMP, 0, 0,
                                len(self.ebpf.opcodes) - self.origin - 1, 0)
-        elif isinstance(self.right, int):
+        elif self.right.small_constant:
             inst = Instruction(
                 self.opcode, self.dst, 0,
-                len(self.ebpf.opcodes) - self.origin - 1, self.right)
+                len(self.ebpf.opcodes) - self.origin - 1,
+                int(self.right.value))
         else:
             inst = Instruction(
                 self.opcode + Opcode.REG, self.dst, self.src,
                 len(self.ebpf.opcodes) - self.origin - 1, 0)
         self.ebpf.opcodes[self.origin] = inst
         if not retarget:
             self.ebpf.owners, self.owners = \
@@ -381,15 +406,14 @@
 
 class AndOrComparison(Comparison):
     def __init__(self, ebpf, left, right, is_and):
         super().__init__(ebpf)
         self.left = left
         self.right = right
         self.is_and = is_and
-        self.targetted = False
 
     def compare(self, negative):
         self.negative = negative
         self.left.compare(self.is_and)
         self.right.compare(negative)
         self.origin = len(self.ebpf.opcodes)
         if self.is_and != negative:
@@ -400,246 +424,339 @@
         if self.is_and == self.negative:
             self.left.target(retarget)
         self.right.target(retarget)
 
 
 class InvertComparison(Comparison):
     def __init__(self, ebpf, value):
-        self.ebpf = ebpf
+        super().__init__(ebpf)
         self.value = value
 
     def compare(self, negative):
         self.value.compare(not negative)
+        self.owners = self.value.owners
 
+    def target(self, retarget=False):
+        self.value.target(retarget)
 
-def binary(opcode):
-    def ret(self, value):
-        return Binary(self.ebpf, self, value, opcode)
-    return ret
 
-def rbinary(opcode):
-    def ret(self, value):
-        return ReverseBinary(self.ebpf, value, self, opcode)
-    return ret
+def ensure_expression(ebpf, value):
+    if isinstance(value, Expression):
+        return value
+    else:
+        return Constant(ebpf, value)
 
 
 class Expression:
     """the base class for all numerical expressions"""
-    __radd__ = __add__ = binary(Opcode.ADD)
-    __sub__ = binary(Opcode.SUB)
-    __rsub__ = rbinary(Opcode.SUB)
-    __rmul__ = __mul__ = binary(Opcode.MUL)
-    __truediv__ = binary(Opcode.DIV)
-    __rtruediv__ = rbinary(Opcode.DIV)
-    __ror__ = __or__ = binary(Opcode.OR)
-    __lshift__ = binary(Opcode.LSH)
-    __rlshift__ = rbinary(Opcode.LSH)
-    __rshift__ = binary(Opcode.RSH)
-    __rrshift__ = rbinary(Opcode.RSH)
-    __mod__ = binary(Opcode.MOD)
-    __rmod__ = rbinary(Opcode.MOD)
-    __rxor__ = __xor__ = binary(Opcode.XOR)
 
-    __eq__ = comparison(Opcode.JEQ, Opcode.JNE)
+    FIXED_BASE = 100000
+    small_constant = False
+
+    def _binary(self, value, opcode):
+        value = ensure_expression(self.ebpf, value)
+        return Binary(self.ebpf, self, value, opcode,
+                      self.signed or value.signed, False)
+
+    __ror__ = __or__ = lambda self, value: self._binary(value, Opcode.OR)
+    __lshift__ = lambda self, value: self._binary(value, Opcode.LSH)
+    __rlshift__ = lambda self, value: Constant(self.ebpf, value) << self
+    __rxor__ = __xor__ = lambda self, value: self._binary(value, Opcode.XOR)
+
     __gt__ = comparison(Opcode.JGT, Opcode.JLE, Opcode.JSGT, Opcode.JSLE)
     __ge__ = comparison(Opcode.JGE, Opcode.JLT, Opcode.JSGE, Opcode.JSLT)
     __lt__ = comparison(Opcode.JLT, Opcode.JGE, Opcode.JSLT, Opcode.JSGE)
     __le__ = comparison(Opcode.JLE, Opcode.JGT, Opcode.JSLE, Opcode.JSGT)
-    __ne__ = comparison(Opcode.JNE, Opcode.JEQ)
+    __ne__ = comparison(Opcode.JNE, Opcode.JEQ, Opcode.JNE, Opcode.JEQ)
+
+    def _sum(self, value, opcode):
+        value = ensure_expression(self.ebpf, value)
+        myself = self
+        if self.fixed != value.fixed:
+            if self.fixed:
+                value *= self.FIXED_BASE
+            else:
+                myself *= self.FIXED_BASE
+
+        return Binary(self.ebpf, myself, value, opcode,
+                      self.signed or value.signed, self.fixed or value.fixed)
+
+    __radd__ = __add__ = lambda self, value: self._sum(value, Opcode.ADD)
+    __sub__ = lambda self, value: self._sum(value, Opcode.SUB)
+    __rsub__ = lambda self, value: Constant(self.ebpf, value) - self
+    __mod__ = lambda self, value: self._sum(value, Opcode.MOD)
+    __rmod__ = lambda self, value: Constant(self.ebpf, value) % self
+
+    def __mul__(self, value):
+        value = ensure_expression(self.ebpf, value)
+        ret = Binary(self.ebpf, self, value, Opcode.MUL,
+                     self.signed or value.signed, self.fixed or value.fixed)
+        if self.fixed and value.fixed:
+            ret /= self.FIXED_BASE
+        return ret
+    __rmul__ = __mul__
+
+    def __truediv__(self, value):
+        value = ensure_expression(self.ebpf, value)
+        myself = self
+        if not self.fixed and value.fixed:
+            myself *= self.FIXED_BASE ** 2
+        elif self.fixed == value.fixed:
+            myself *= self.FIXED_BASE
+
+        return Binary(self.ebpf, myself, value, Opcode.DIV,
+                      self.signed or value.signed, True)
+
+    def _reverse(self, op, value):
+        return op(Constant(self.ebpf, value), self)
+
+    __rtruediv__ = lambda self, value: Constant(self.ebpf, value) / self
+
+    def __floordiv__(self, value):
+        value = ensure_expression(self.ebpf, value)
+        myself = self
+        if not self.fixed and value.fixed:
+            myself *= self.FIXED_BASE
+        elif self.fixed and not value.fixed:
+            value *= self.FIXED_BASE
+
+        return Binary(self.ebpf, myself, value, Opcode.DIV,
+                      self.signed or value.signed, False)
+
+    def __rfloordiv__(self, value):
+        if self.fixed:
+            value = Constant(self.ebpf, value)
+            if not value.fixed:
+                value *= self.FIXED_BASE
+        else:
+            value = Constant(self.ebpf, int(value))
+
+        return Binary(self.ebpf, value, self, Opcode.DIV,
+                      self.signed or value.signed, False)
+
+    def __rshift__(self, value):
+        opcode = Opcode.ARSH if self.signed else Opcode.RSH
+        return Binary(self.ebpf, self, ensure_expression(self.ebpf, value),
+                      opcode, self.signed, False)
+
+    __rrshift__ = lambda self, value: Constant(self.ebpf, value) >> self
 
     def __and__(self, value):
-        return AndExpression(self.ebpf, self, value)
+        return AndExpression(self.ebpf, self,
+                             ensure_expression(self.ebpf, value))
+
+    def __eq__(self, value):
+        return ~(self != value)
 
     __rand__ = __and__
 
     def __neg__(self):
-        return Negate(self.ebpf, self)
+        return Negate(self)
+
+    def __abs__(self):
+        return Absolute(self)
+
+    def switch_endian(self, fmt):
+        if isinstance(fmt, str) and len(fmt) > 1:
+            return SwitchEndian(self, fmt)
+        return self
 
     def __bool__(self):
-        raise RuntimeError("Expression only has a value at execution time")
+        raise AssembleError("Expression only has a value at execution time")
 
     def __enter__(self):
         ret = self != 0
         self.as_comparison = ret
         return ret.__enter__()
 
     def __exit__(self, exc_type, exc, tb):
         return self.as_comparison.__exit__(exc_type, exc, tb)
 
     @contextmanager
-    def calculate(self, dst, long, signed, force=False):
+    def calculate(self, dst, long, force=False):
         """issue the code that calculates the value of this expression
 
         this method returns three values:
 
         - the number of the register with the result
         - a boolean indicating whether this is a 64 bit value
-        - and a booleand indicating whether the result is to be
-          considered signed.
 
         this method is a contextmanager to be used in a `with`
         statement. At the end of the `with` block the result is
         freed again, i.e. the register will not be reserved for the
         result anymore.
 
         the default implementation calls `get_address` for values
         which actually are in memory and moves that into a register.
 
         :param dst: the number of the register to put the result in,
            or `None` if that does not matter.
         :param long: True if the result is supposed to be 64 bit. None
            if it does not matter.
-        :param signed: True if the result should be considered signed.
-           None if it does not matter.
         :param force: if true, `dst` must be respected, otherwise this
            is optional.
         """
         with self.ebpf.get_free_register(dst) as dst:
-            with self.get_address(dst, long, signed) as (src, fmt):
-                self.ebpf.append(Opcode.LD + Memory.fmt_to_opcode[fmt],
+            with self.get_address(dst, long) as (src, fmt):
+                self.ebpf.append(Opcode.LD + fmt_to_opcode(fmt),
                                  dst, src, 0, 0)
-                yield dst, long, self.signed
+                yield dst, long
 
     @contextmanager
-    def get_address(self, dst, long, signed, force=False):
+    def get_address(self, dst, long, force=False):
         """get the address of the value of this expression
 
         this method returns the address of the result of this expression,
         and its format letter. The default implementation uses
         `calculate` to evaluate the expression and pushes the result onto
         the stack.
         """
         with self.ebpf.get_stack(4 + 4 * long) as stack:
-            with self.calculate(dst, long, signed) as (src, _, _):
+            with self.calculate(dst, long) as (src, _):
                 self.ebpf.append(Opcode.STX + Opcode.DW * long,
                                  10, src, stack, 0)
                 self.ebpf.append(Opcode.MOV + Opcode.LONG + Opcode.REG,
                                  dst, 10, 0, 0)
                 self.ebpf.append(Opcode.ADD + Opcode.LONG, dst, 0, 0, stack)
             yield dst, "Q" if long else "I"
 
     def contains(self, no):
         """return whether this expression contains the register `no`"""
         return False
 
 
 class Binary(Expression):
     """represent all binary expressions"""
-    def __init__(self, ebpf, left, right, operator):
+    def __init__(self, ebpf, left, right, operator, signed, fixed):
         self.ebpf = ebpf
         self.left = left
         self.right = right
         self.operator = operator
+        self.signed = signed
+        self.fixed = fixed
 
     @contextmanager
-    def calculate(self, dst, long, signed, force=False):
+    def calculate(self, dst, long, force=False):
         orig_dst = dst
-        if not isinstance(self.right, int) and self.right.contains(dst):
+        if isinstance(self.right, Expression) and self.right.contains(dst):
             dst = None
         with self.ebpf.get_free_register(dst) as dst:
-            with self.left.calculate(dst, long, signed, True) \
-                    as (dst, l_long, l_signed):
+            with self.left.calculate(dst, long, True) as (dst, l_long):
                 if long is None:
                     long = l_long
-                signed = signed or l_signed
-            if self.operator is Opcode.RSH and signed:  # >>=
-                operator = Opcode.ARSH
+            if self.right.small_constant:
+                self.ebpf.append(self.operator + Opcode.LONG * long,
+                                 dst, 0, 0, int(self.right.value))
             else:
-                operator = self.operator
-            if isinstance(self.right, int):
-                r_signed = self.right < 0
-                self.ebpf.append(operator + Opcode.LONG * long,
-                                 dst, 0, 0, self.right)
-            else:
-                with self.right.calculate(None, long, None) as \
-                        (src, r_long, r_signed):
+                with self.right.calculate(None, long) as (src, r_long):
                     self.ebpf.append(
-                        operator + Opcode.REG
+                        self.operator + Opcode.REG
                         + Opcode.LONG * ((r_long or l_long)
                                          if long is None else long),
                         dst, src, 0, 0)
             if orig_dst is None or orig_dst == dst:
-                yield dst, long, signed or r_signed
+                yield dst, long
                 return
         self.ebpf.append(Opcode.MOV + Opcode.REG + Opcode.LONG * long, orig_dst, dst, 0, 0)
-        yield orig_dst, long, signed or r_signed
+        yield orig_dst, long
 
     def contains(self, no):
-        return self.left.contains(no) or (not isinstance(self.right, int)
+        return self.left.contains(no) or (isinstance(self.right, Expression)
                                           and self.right.contains(no))
 
 
-class ReverseBinary(Expression):
-    def __init__(self, ebpf, left, right, operator):
-        self.ebpf = ebpf
-        self.left = left
-        self.right = right
-        self.operator = operator
+class Unary(Expression):
+    def __init__(self, arg):
+        self.arg = arg
+        self.ebpf = arg.ebpf
+        self.signed = arg.signed
+        self.fixed = arg.fixed
 
     @contextmanager
-    def calculate(self, dst, long, signed, force=False):
-        with self.ebpf.get_free_register(dst) as dst:
-            self.ebpf._load_value(dst, self.left)
-            if self.operator is Opcode.RSH and self.left < 0:  # >>=
-                operator = Opcode.ARSH
-            else:
-                operator = self.operator
-
-            with self.right.calculate(None, long, None) as (src, long, _):
-                self.ebpf.append(operator + Opcode.LONG * long + Opcode.REG,
-                                 dst, src, 0, 0)
-            yield dst, long, signed
+    def calculate(self, dst, long, force=False):
+        with self.arg.calculate(dst, long, force) as (dst, long):
+            self.calculate_unary(dst, long)
+            yield dst, long
 
     def contains(self, no):
-        return self.right.contains(no)
+        return self.arg.contains(no)
 
 
-class Negate(Expression):
-    def __init__(self, ebpf, arg):
-        self.ebpf = ebpf
-        self.arg = arg
+class Negate(Unary):
+    def __init__(self, arg):
+        super().__init__(arg)
+        self.signed = True
 
-    @contextmanager
-    def calculate(self, dst, long, signed, force=False):
-        with self.arg.calculate(dst, long, signed, force) as \
-                (dst, long, signed):
-            self.ebpf.append(Opcode.NEG + Opcode.LONG * long, dst, 0, 0, 0)
-            yield dst, long, signed
+    def calculate_unary(self, dst, long):
+        self.ebpf.append(Opcode.NEG + Opcode.LONG * long, dst, 0, 0, 0)
 
-    def contains(self, no):
-        return self.arg.contains(no)
+
+class Absolute(Unary):
+    def __init__(self, arg):
+        super().__init__(arg)
+        self.signed = False
+
+    def calculate_unary(self, dst, long):
+        with self.ebpf.sr[dst] < 0:
+            self.ebpf.sr[dst] = -self.ebpf.sr[dst]
+
+
+class SwitchEndian(Unary):
+    def __init__(self, arg, fmt):
+        super().__init__(arg)
+        self.fmt = fmt
+
+    def calculate_unary(self, dst, long):
+        endian, size = self.fmt
+        if endian == "<":
+            opcode = Opcode.LE
+        elif endian in ">!":
+            opcode = Opcode.BE
+        self.ebpf.append(opcode, dst, 0, 0, calcsize(size) * 8)
 
 
 class Sum(Binary):
     """represent the sum of one register and a constant value
 
     this is used to optimize memory addressing code.
     """
     def __init__(self, ebpf, left, right):
-        super().__init__(ebpf, left, right, Opcode.ADD)
+        super().__init__(ebpf, left, right, Opcode.ADD, right.value < 0, False)
 
     def __add__(self, value):
-        if isinstance(value, int):
-            return Sum(self.ebpf, self.left, self.right + value)
-        else:
+        try:
+            self.right.value += index(value)
+        except TypeError:
             return super().__add__(value)
 
     __radd__ = __add__
 
     def __sub__(self, value):
-        if isinstance(value, int):
-            return Sum(self.ebpf, self.left, self.right - value)
-        else:
-            return super().__sub__(value)
+        try:
+            self.right.value -= index(value)
+        except TypeError:
+            return super().__add__(value)
+
+
+class AndExpression(Binary):
+    # there is a special comparison with & instruction
+    def __init__(self, ebpf, left, right):
+        super().__init__(ebpf, left, right, Opcode.AND, False, False)
 
+    def __ne__(self, value):
+        if isinstance(value, int) and value == 0:
+            return AndComparison(self.ebpf, self.left, self.right)
+        return super().__ne__(value)
 
-class AndExpression(SimpleComparison, Binary):
-    """The & operator may also be used as a comparison"""
+
+class AndComparison(SimpleComparison):
+    # there is a special comparison with & instruction
+    # it is the only one which has not inversion
     def __init__(self, ebpf, left, right):
-        Binary.__init__(self, ebpf, left, right, Opcode.AND)
+        Binary.__init__(self, ebpf, left, right, Opcode.AND, False, False)
         SimpleComparison.__init__(self, ebpf, left, right, Opcode.JSET)
         self.opcode = (Opcode.JSET, None, Opcode.JSET, None)
         self.invert = None
 
     def compare(self, negative):
         super().compare(False)
         if negative:
@@ -669,241 +786,365 @@
         else:
             self.ebpf.opcodes[self.origin] = \
                 Instruction(op, dst, src, off+1, imm)
         self.else_origin = len(self.ebpf.opcodes)
         self.ebpf.opcodes.append(None)
         return self
 
+class Constant(Expression):
+    def __init__(self, ebpf, value):
+        try:
+            self.value = index(value)
+            self.fixed = False
+        except TypeError:
+            self.value = float(value) * Expression.FIXED_BASE
+            self.fixed = True
+        self.ebpf = ebpf
+        self.signed = value < 0
+
+    @property
+    def small_constant(self):
+        return -0x80000000 <= self.value < 0x80000000
+
+    def __imul__(self, value):
+        self.value *= value
+        return self
+
+    @contextmanager
+    def calculate(self, dst, long, force=False):
+        value = int(self.value)
+        with self.ebpf.get_free_register(dst) as dst:
+            if self.small_constant:
+                self.ebpf.append(Opcode.MOV + Opcode.LONG, dst, 0, 0, value)
+            else:
+                self.ebpf.append(Opcode.DW, dst, 0, 0, value & 0xffffffff)
+                self.ebpf.append(Opcode.W, 0, 0, 0, value >> 32)
+            yield dst, not (-0x80000000 <= value < 0x100000000)
+
+    def switch_endian(self, fmt):
+        if not isinstance(fmt, str) or len(fmt) == 1:
+            return self
+        return Constant(self.ebpf, *unpack(fmt, pack(fmt[-1], self.value)))
+
+
 class Register(Expression):
     """represent one EBPF register"""
     offset = 0
 
-    def __init__(self, no, ebpf, long, signed):
+    def __init__(self, no, ebpf, long, signed, fixed=False):
         self.no = no
         self.ebpf = ebpf
         self.long = long
         self.signed = signed
+        self.fixed = fixed
 
     def __add__(self, value):
-        if isinstance(value, int) and self.long:
-            return Sum(self.ebpf, self, value)
-        else:
-            return super().__add__(value)
+        if self.long and not self.fixed:
+            try:
+                return Sum(self.ebpf, self, Constant(self.ebpf, index(value)))
+            except TypeError:
+                pass
+        return super().__add__(value)
 
     __radd__ = __add__
 
     def __sub__(self, value):
-        if isinstance(value, int) and self.long:
-            return Sum(self.ebpf, self, -value)
-        else:
-            return super().__sub__(value)
+        if self.long and not self.fixed:
+            try:
+                return Sum(self.ebpf, self, Constant(self.ebpf, -index(value)))
+            except TypeError:
+                pass
+        return super().__sub__(value)
 
     @contextmanager
-    def calculate(self, dst, long, signed, force=False):
+    def calculate(self, dst, long, force=False):
         if self.no not in self.ebpf.owners:
             raise AssembleError("register has no value")
         if dst != self.no and force:
             self.ebpf.append(Opcode.MOV + Opcode.REG + Opcode.LONG * self.long,
                              dst, self.no, 0, 0)
-            yield dst, self.long, self.signed
+            yield dst, self.long
         else:
-            yield self.no, self.long, self.signed
+            yield self.no, self.long
 
     def contains(self, no):
         return self.no == no
 
 
 class IAdd:
     """represent an in-place addition"""
-    def __init__(self, value):
-        self.value = value
+    def __init__(self, ebpf, value):
+        if isinstance(value, Expression):
+            self.value = value
+        else:
+            self.value = Constant(ebpf, value)
 
 
+def fmt_to_opcode(fmt):
+    fmt_to_opcode = {'I': Opcode.W, 'H': Opcode.H, 'B': Opcode.B, 'Q': Opcode.DW,
+                     'i': Opcode.W, 'h': Opcode.H, 'b': Opcode.B, 'q': Opcode.DW,
+                     'A': Opcode.W, 'x': Opcode.DW}
+    if isinstance(fmt, str):
+        return fmt_to_opcode[fmt[-1]]
+    else:
+        return Opcode.B
+
 class Memory(Expression):
     bits_to_opcode = {32: Opcode.W, 16: Opcode.H, 8: Opcode.B, 64: Opcode.DW}
-    fmt_to_opcode = {'I': Opcode.W, 'H': Opcode.H, 'B': Opcode.B, 'Q': Opcode.DW,
-                     'i': Opcode.W, 'h': Opcode.H, 'b': Opcode.B, 'q': Opcode.DW}
 
-    def __init__(self, ebpf, fmt, address, signed=False, long=False):
+    def __init__(self, ebpf, fmt, address):
         self.ebpf = ebpf
         self.fmt = fmt
         self.address = address
-        self.signed = signed
-        self.long = long
 
     def __iadd__(self, value):
-        if self.fmt in "qQiI":
-            return IAdd(value)
+        if self.fmt in "qQiIx":
+            return IAdd(self.ebpf, value)
         else:
             return NotImplemented
 
     def __isub__(self, value):
-        if self.fmt in "qQiI":
-            return IAdd(-value)
+        if self.fmt in "qQiIx":
+            return IAdd(self.ebpf, -value)
         else:
             return NotImplemented
 
     @contextmanager
-    def calculate(self, dst, long, signed, force=False):
-        if isinstance(self.address, Sum):
-            with self.ebpf.get_free_register(dst) as dst:
-                self.ebpf.append(Opcode.LD + self.fmt_to_opcode[self.fmt], dst,
-                                 self.address.left.no, self.address.right, 0)
-                yield dst, self.long, self.signed
-        else:
-            with super().calculate(dst, long, signed, force) as (dst, _, _):
-                yield dst, self.long, self.signed
+    def calculate(self, dst, long, force=False):
+        if self.has_endian():
+            with self.without_endian().switch_endian(self.fmt) \
+                 .calculate(dst, long, force) as (dst, long):
+                yield dst, long
+                return
+        with ExitStack() as exitStack:
+            if isinstance(self.address, Sum):
+                dst = exitStack.enter_context(self.ebpf.get_free_register(dst))
+                opcode = fmt_to_opcode(self.fmt)
+                self.ebpf.append(Opcode.LD + opcode, dst, self.address.left.no,
+                                 self.address.right.value, 0)
+            else:
+                dst, _ = exitStack.enter_context(
+                    super().calculate(dst, long, force))
+            if isinstance(self.fmt, tuple):
+                self.ebpf.r[dst] &= ((1 << self.fmt[1]) - 1) << self.fmt[0]
+                if self.fmt[0] > 0:
+                    self.ebpf.r[dst] >>= self.fmt[0]
+                yield dst, "B"
+            else:
+                yield dst, self.fmt[-1] in "QqAx"
 
     @contextmanager
-    def get_address(self, dst, long, signed, force=False):
-        with self.address.calculate(dst, True, None) as (src, _, _):
+    def get_address(self, dst, long, force=False):
+        with self.address.calculate(dst, True) as (src, _):
             yield src, self.fmt
 
     def contains(self, no):
         return self.address.contains(no)
 
+    @property
+    def signed(self):
+        return isinstance(self.fmt, str) and self.fmt.islower()
+
+    @property
+    def fixed(self):
+        return isinstance(self.fmt, str) and self.fmt == "x"
+
+    def has_endian(self):
+        return isinstance(self.fmt, str) and len(self.fmt) > 1
+
+    def without_endian(self):
+        if self.has_endian():
+            return Memory(self.ebpf, self.fmt[-1], self.address)
+        return self
+
+    def __invert__(self):
+        if not isinstance(self.fmt, tuple) or self.fmt[1] != 1:
+            return NotImplemented
+        return self == 0
+
+    def __ne__(self, value):
+        if isinstance(self.fmt, tuple) and isinstance(value, int) \
+                and value == 0:
+            mask = ((1 << self.fmt[1]) - 1) << self.fmt[0]
+            return Memory(self.ebpf, "B", self.address) & mask != 0
+        return super().__ne__(value)
+
+    def _set(self, value):
+        opcode = Opcode.STX
+        with ExitStack() as exitStack:
+            if isinstance(self.fmt, tuple):
+                pos, bits = self.fmt
+                self.fmt = "B"
+                if bits == 1:
+                    try:
+                        if value:
+                            value = self | (1 << pos)
+                        else:
+                            value = self & ~(1 << pos)
+                    except AssembleError:
+                        exitStack.enter_context(self.ebpf.wtmp)
+                        with value as Else:
+                            self.ebpf.wtmp = self | (1 << pos)
+                        with Else:
+                            self.ebpf.wtmp = self & ~(1 << pos)
+                        value = self.ebpf.wtmp
+                else:
+                    mask = ((1 << bits) - 1) << pos
+                    value = (mask & (value << pos) | ~mask & self)
+            elif isinstance(value, IAdd):
+                value = value.value
+                opcode = Opcode.XADD
+            elif not isinstance(value, Expression):
+                value = Constant(self.ebpf, value)
+            if self.fmt == "x" and not value.fixed:
+                value *= Expression.FIXED_BASE
+            elif self.fmt != "x" and value.fixed:
+                value /= Expression.FIXED_BASE
+            if isinstance(self.address, Sum):
+                dst = self.address.left.no
+                offset = self.address.right.value
+            else:
+                dst, _ = exitStack.enter_context(
+                    self.address.calculate(None, True))
+                offset = 0
+            value = value.switch_endian(self.fmt)
+            if value.small_constant and opcode == Opcode.STX:
+                self.ebpf.append(Opcode.ST + fmt_to_opcode(self.fmt), dst, 0,
+                                 offset, int(value.value))
+                return
+            src, _ = exitStack.enter_context(
+                value.calculate(None, isinstance(self.fmt, str)
+                                      and self.fmt[-1] in 'qQx'))
+            self.ebpf.append(opcode + fmt_to_opcode(self.fmt),
+                             dst, src, offset, 0)
+
+
 
 class MemoryDesc:
     """A base class used by descriptors for memory
 
     All memory access is relative to a base register. This is
     defined by the member variable `base_register` in deriving
     classes.
     """
+
+    fixed = False  # only selected memory can have fixe value vars
+
     def __get__(self, instance, owner):
         if instance is None:
             return self
         fmt, addr = self.fmt_addr(instance)
         return Memory(instance.ebpf, fmt,
-                      instance.ebpf.r[self.base_register] + addr,
-                      fmt.islower())
+                      instance.ebpf.r[self.base_register] + addr)
 
     def __set__(self, instance, value):
-        ebpf = instance.ebpf
         fmt, addr = self.fmt_addr(instance)
-        bits = Memory.fmt_to_opcode[fmt]
-        if isinstance(value, int):
-            ebpf.append(Opcode.ST + bits, self.base_register, 0,
-                        addr, value)
-            return
-        elif isinstance(value, IAdd):
-            value = value.value
-            if isinstance(value, int):
-                with ebpf.get_free_register(None) as src:
-                    ebpf.r[src] = value
-                    ebpf.append(Opcode.XADD + bits, self.base_register,
-                                src, addr, 0)
-                return
-            opcode = Opcode.XADD
-        else:
-            opcode = Opcode.STX
-        with value.calculate(None, fmt in 'qQ', fmt.islower()) as (src, _, _):
-            ebpf.append(opcode + bits, self.base_register, src, addr, 0)
-
+        memory = Memory(instance.ebpf, fmt,
+                        instance.ebpf.r[self.base_register] + addr)
+        memory._set(value)
 
 class LocalVar(MemoryDesc):
     """variables on the stack"""
     base_register = 10
 
     def __init__(self, fmt='I'):
         self.fmt = fmt
+        self.fixed = fmt == "x"
 
     def __set_name__(self, owner, name):
-        size = calcsize(self.fmt)
+        if self.fmt == "x":
+            size = 8
+        elif isinstance(self.fmt, str):
+            size = calcsize(self.fmt)
+        else:  # this is to support bit addressing, mostly for testing
+            size = 1
         owner.stack -= size
         owner.stack &= -size
         self.relative_addr = owner.stack
         self.name = name
 
     def fmt_addr(self, instance):
         if isinstance(instance, SubProgram):
             return self.fmt, (instance.ebpf.stack & -8) + self.relative_addr
         else:
             return self.fmt, self.relative_addr
 
 
 class MemoryMap:
-    def __init__(self, ebpf, fmt, signed=False, long=False):
+    def __init__(self, ebpf, fmt):
         self.ebpf = ebpf
         self.fmt = fmt
-        self.long = long
-        self.signed = signed
 
     def __setitem__(self, addr, value):
-        with ExitStack() as exitStack:
-            if isinstance(addr, Sum):
-                dst = addr.left.no
-                offset = addr.right
-            else:
-                dst, _, _ = exitStack.enter_context(
-                        addr.calculate(None, True, None))
-                offset = 0
-            if isinstance(value, int):
-                self.ebpf.append(Opcode.ST + Memory.fmt_to_opcode[self.fmt],
-                                 dst, 0, offset, value)
-                return
-            elif isinstance(value, IAdd):
-                value = value.value
-                if isinstance(value, int):
-                    with self.ebpf.get_free_register(None) as src:
-                        self.ebpf.r[src] = value
-                        self.ebpf.append(
-                            Opcode.XADD + Memory.fmt_to_opcode[self.fmt],
-                            dst, src, offset, 0)
-                    return
-                opcode = Opcode.XADD
-            else:
-                opcode = Opcode.STX
-            with value.calculate(None, None, None) as (src, _, _):
-                self.ebpf.append(opcode + Memory.fmt_to_opcode[self.fmt],
-                                 dst, src, offset, 0)
+        memory = Memory(self.ebpf, self.fmt, addr)
+        memory._set(value)
 
     def __getitem__(self, addr):
         if isinstance(addr, Register):
             addr = addr + 0
-        return Memory(self.ebpf, self.fmt, addr, self.signed, self.long)
+        return Memory(self.ebpf, self.fmt, addr)
 
 
 class Map(ABC):
     """The base class for all maps"""
+    def __set_name__(self, owner, name):
+        self.filename = name
+
     @abstractmethod
     def init(self, ebpf):
         """create the map and initialize its values"""
 
     def load(self, ebpf):
         """called after the program has been loaded"""
 
 
 class PseudoFd(Expression):
     """represent a file descriptor to a map"""
     def __init__(self, ebpf, fd):
         self.ebpf = ebpf
         self.fd = fd
+        self.fixed = False
 
     @contextmanager
-    def calculate(self, dst, long, signed, force=False):
+    def calculate(self, dst, long, force=False):
         with self.ebpf.get_free_register(dst) as dst:
             self.ebpf.append(Opcode.DW, dst, 1, 0, self.fd)
             self.ebpf.append(Opcode.W, 0, 0, 0, 0)
-            yield dst, long, signed
+            yield dst, long
 
 
 class ktime(Expression):
     """a function that returns the current ktime in ns"""
     def __init__(self, ebpf):
         self.ebpf = ebpf
+        self.fixed = False
 
     @contextmanager
-    def calculate(self, dst, long, signed, force=False):
+    def calculate(self, dst, long, force=False):
         with self.ebpf.get_free_register(dst) as dst:
             with self.ebpf.save_registers([i for i in range(6) if i != dst]):
                 self.ebpf.call(FuncId.ktime_get_ns)
                 if dst != 0:
                     self.ebpf.r[dst] = self.ebpf.r0
-            yield dst, True, False
+            yield dst, True
+
+
+class prandom(Expression):
+    """a function that returns the current ktime in ns"""
+    def __init__(self, ebpf):
+        self.ebpf = ebpf
+
+    @contextmanager
+    def calculate(self, dst, long, force=False):
+        with self.ebpf.get_free_register(dst) as dst:
+            with self.ebpf.save_registers([i for i in range(6) if i != dst]):
+                self.ebpf.call(FuncId.get_prandom_u32)
+                if dst != 0:
+                    self.ebpf.r[dst] = self.ebpf.r0
+            yield dst, True
 
 
 class RegisterDesc:
     def __init__(self, no, array):
         self.no = no
         self.array = array
 
@@ -914,37 +1155,38 @@
             return getattr(instance, self.array)[self.no]
 
     def __set__(self, instance, value):
         getattr(instance, self.array)[self.no] = value
 
 
 class RegisterArray:
-    def __init__(self, ebpf, long, signed):
+    def __init__(self, ebpf, long, signed, fixed=False):
         self.ebpf = ebpf
         self.long = long
         self.signed = signed
+        self.fixed = fixed
 
     def __setitem__(self, no, value):
         self.ebpf.owners.add(no)
-        if isinstance(value, int):
-            self.ebpf._load_value(no, value)
-        elif isinstance(value, Expression):
-            with value.calculate(no, self.long, self.signed, True):
-                pass
-        else:
-            raise AssembleError("cannot compile")
+        value = ensure_expression(self.ebpf, value)
+        if self.fixed and not value.fixed:
+            value *= Expression.FIXED_BASE
+        elif not self.fixed and value.fixed:
+            value /= Expression.FIXED_BASE
+        with value.calculate(no, self.long, True):
+            pass
 
     def __getitem__(self, no):
-        return Register(no, self.ebpf, self.long, self.signed)
+        return Register(no, self.ebpf, self.long, self.signed, self.fixed)
 
 
 
 class Temporary(Register):
-    def __init__(self, ebpf, long, signed):
-        super().__init__(None, ebpf, long, signed)
+    def __init__(self, ebpf, long, signed, fixed):
+        super().__init__(None, ebpf, long, signed, fixed)
         self.nos = []
         self.gfrs = []
 
     def __enter__(self):
         gfr = self.ebpf.get_free_register(None)
         self.nos.append(self.no)
         self.no = gfr.__enter__()
@@ -963,76 +1205,116 @@
     def __get__(self, instance, owner=None):
         if instance is None:
             return self
         arr = getattr(instance, self.array)
         ret = instance.__dict__.get(self.name, None)
         if ret is None:
             ret = instance.__dict__[self.name] = \
-                    Temporary(instance, arr.long, arr.signed)
+                    Temporary(instance, arr.long, arr.signed, arr.fixed)
         return ret
 
     def __set__(self, instance, value):
         no = getattr(instance, self.name).no
         getattr(instance, self.array)[no] = value
 
 
 class EBPF:
     """The base class for all EBPF programs
 
-    This class may even be instantiated directly, in which case you
-    can just issue the program before the it is loaded.
+    Usually this class is sub-classed, and the actual program is defined
+    in the overwritten `program` method. Then the program may be loaded into
+    the kernel. Alternatively, this class may even be instantiated directly,
+    in which case you can just issue the program before it is loaded.
+
+    After a program is loaded, its maps may be written to a bpf file system
+    using :meth:`pin_maps`. Those maps may be used at a later time, especially
+    also in a different task, if the parameter `load_maps` is given, in which
+    case we assume the program has already been loaded.
+
+    :param load_maps: a prefix to load pinned maps from. Must be existing in a
+        bpf file system, and usually ends in a "/".
     """
     stack = 0
     name = None
     license = None
 
     def __init__(self, prog_type=0, license=None, kern_version=0,
-                 name=None, subprograms=()):
+                 name=None, load_maps=None, subprograms=()):
         self.opcodes = []
         self.prog_type = prog_type
         if license is not None:
             self.license = license
         self.kern_version = kern_version
         if name is None:
             if self.name is None:
                 self.name = self.__class__.__name__[:16]
         else:
             self.name = name
-        self.loaded = False
+        self.loaded = load_maps is not None
 
         self.mB = MemoryMap(self, "B")
         self.mH = MemoryMap(self, "H")
         self.mI = MemoryMap(self, "I")
-        self.mA = MemoryMap(self, "I", False, True)
-        self.mQ = MemoryMap(self, "Q", False, True)
+        self.mA = MemoryMap(self, "A")  # actually I, but treat as Q
+        self.mQ = MemoryMap(self, "Q")
+        self.mb = MemoryMap(self, "b")
+        self.mh = MemoryMap(self, "h")
+        self.mi = MemoryMap(self, "i")
+        self.mq = MemoryMap(self, "q")
+        self.mx = MemoryMap(self, "x")
 
         self.r = RegisterArray(self, True, False)
         self.sr = RegisterArray(self, True, True)
         self.w = RegisterArray(self, False, False)
         self.sw = RegisterArray(self, False, True)
+        self.x = RegisterArray(self, True, True, True)
 
         self.owners = {1, 10}
 
         self.subprograms = subprograms
         for p in subprograms:
             p.ebpf = self
 
-        for v in self.__class__.__dict__.values():
+        for k, v in self.__class__.__dict__.items():
+            if isinstance(v, Map):
+                if load_maps is None:
+                    v.init(self, None)
+                else:
+                    v.init(self, bpf.obj_get(load_maps + k))
+
+    def pin_maps(self, path):
+        """pin the maps of this program to files with prefix `path`
+
+        This path must be in a bpf file system, and all parent
+        directories must already exist, while the individual files
+        must not exist.
+        """
+        for k, v in self.__class__.__dict__.items():
             if isinstance(v, Map):
-                v.init(self)
+                bpf.obj_pin(path + k, getattr(self, v.name).fd)
 
     def program(self):
         """overwrite this method with your program while subclassing"""
 
     def append(self, opcode, dst, src, off, imm):
         self.opcodes.append(Instruction(opcode, dst, src, off, imm))
 
+    def append_endian(self, fmt, dst):
+        if not isinstance(fmt, str) or len(fmt) != 2:
+            return
+        endian, size = fmt
+        if endian == "<":
+            opcode = Opcode.LE
+        elif endian in ">!":
+            opcode = Opcode.BE
+        self.append(opcode, dst, 0, 0, calcsize(fmt) * 8)
+
     def assemble(self):
         """return the assembled program"""
-        self.program()
+        sub(EBPF, self).program()
         return b"".join(
             pack("<BBHI", i.opcode.value, i.dst | i.src << 4,
                  i.off % 0x10000, i.imm % 0x100000000)
             for i in self.opcodes)
 
     def load(self, log_level=0, log_size=10 * 4096):
         """load the program into the kernel"""
@@ -1045,14 +1327,16 @@
             if isinstance(v, Map):
                 v.load(self)
 
         return ret
 
     def jumpIf(self, comp):
         """jump if `comp` is true to a later defined `target`"""
+        if isinstance(comp, Expression):
+            comp = comp != 0
         comp.compare(False)
         return comp
 
     def jump(self):
         """unconditionally jump to a later defined `target`"""
         comp = SimpleComparison(self, None, 0, Opcode.JMP)
         comp.origin = len(self.opcodes)
@@ -1088,21 +1372,14 @@
             if i not in self.owners:
                 self.owners.add(i)
                 yield i
                 self.owners.discard(i)
                 return
         raise AssembleError("not enough registers")
 
-    def _load_value(self, no, value):
-        if -0x80000000 <= value < 0x80000000:
-            self.append(Opcode.MOV + Opcode.LONG, no, 0, 0, value)
-        else:
-            self.append(Opcode.DW, no, 0, 0, value & 0xffffffff)
-            self.append(Opcode.W, 0, 0, 0, value >> 32)
-
     @contextmanager
     def save_registers(self, registers):
         oldowners = self.owners.copy()
         self.owners |= set(registers)
         save = []
         with ExitStack() as exitStack:
             for i in registers:
@@ -1127,24 +1404,28 @@
     def ebpf(self):
         return self
 
     tmp = TemporaryDesc(None, "r")
     stmp = TemporaryDesc(None, "sr")
     wtmp = TemporaryDesc(None, "w")
     swtmp = TemporaryDesc(None, "sw")
+    xtmp = TemporaryDesc(None, "x")
 
 
 for i in range(11):
     setattr(EBPF, f"r{i}", RegisterDesc(i, "r"))
 
 for i in range(10):
     setattr(EBPF, f"sr{i}", RegisterDesc(i, "sr"))
 
 for i in range(10):
     setattr(EBPF, f"w{i}", RegisterDesc(i, "w"))
 
 for i in range(10):
     setattr(EBPF, f"sw{i}", RegisterDesc(i, "sw"))
 
+for i in range(10):
+    setattr(EBPF, f"x{i}", RegisterDesc(i, "x"))
+
 
 class SubProgram:
     stack = 0
```

### Comparing `ebpfcat-0.1.0/ebpfcat/ethercat.py` & `ebpfcat-0.4.1/ebpfcat/ethercat.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,19 +22,28 @@
 
 """\
 Low-level access to EtherCAT
 ============================
 
 this modules contains the code to actually talk to EtherCAT terminals.
 """
-from asyncio import ensure_future, Event, Future, gather, get_event_loop, Protocol, Queue, Lock
-from enum import Enum
+from asyncio import (
+    CancelledError, ensure_future, Event, Future, gather, get_event_loop,
+    Protocol, Queue, Lock)
+from contextlib import asynccontextmanager
+from enum import Enum, IntEnum
+from itertools import count
+import logging
 from random import randint
 from socket import socket, AF_PACKET, SOCK_DGRAM
-from struct import pack, unpack, calcsize
+from struct import pack, unpack, unpack_from, calcsize
+
+class EtherCatError(Exception):
+    pass
+
 
 class ECCmd(Enum):
    NOP = 0  # No Operation
    APRD = 1  # Auto Increment Read
    APWR = 2  # Auto Increment Write
    APRW = 3  # Auto Increment Read Write
    FPRD = 4  # Configured Address Read
@@ -116,24 +125,51 @@
    DOWN_EXP = 0x23
    DOWN_INIT_CA = 0x31
    UP_REQ = 0x40
    UP_REQ_CA = 0x50
    SEG_UP_REQ = 0x60
    ABORT = 0x80
 
+class EEPROM(IntEnum):
+    VENDOR_ID = 8
+    PRODUCT_CODE = 10
+    REVISION = 12
+    SERIAL_NO = 14
+
+class MachineState(Enum):
+    """The states of the EtherCAT state machine
+
+    The states are in the order in which they should
+    be taken, BOOTSTRAP is at the end as this is a
+    state we usually do not go to.
+    """
+    INIT = 1
+    PRE_OPERATIONAL = 2
+    SAFE_OPERATIONAL = 4
+    OPERATIONAL = 8
+    BOOTSTRAP = 3
+
+class SyncManager(Enum):
+    OUT = 2
+    IN = 3
 
 class ObjectDescription:
     def __init__(self, terminal):
         self.terminal = terminal
 
     def __getitem__(self, idx):
         return self.entries[idx]
 
+    def __repr__(self):
+        return " ".join(f"[{k:X}: {v}]" for k, v in self.entries.items())
+
 
 class ObjectEntry:
+    name = None
+
     def __init__(self, desc):
         self.desc = desc
 
     async def read(self):
         ret = await self.desc.terminal.sdo_read(self.desc.index, self.valueInfo)
         if self.dataType in (ECDataType.VISIBLE_STRING,
                              ECDataType.UNICODE_STRING):
@@ -151,14 +187,21 @@
             d = data
         else:
             d = pack("<" + self.dataType.fmt, data)
 
         return await self.desc.terminal.sdo_write(d, self.desc.index,
                                                   self.valueInfo)
 
+    def __repr__(self):
+        if self.name is None:
+            return "[unread ObjectEntry]"
+
+        return f'"{self.name}" {self.dataType}:{self.bitLength} ' \
+               f'{self.objectAccess:X}'
+
 
 def datasize(args, data):
     out = calcsize("<" + "".join(arg for arg in args if isinstance(arg, str)))
     if isinstance(data, int):
         out += data
     elif data is not None:
         out += len(data)
@@ -168,68 +211,78 @@
 class Packet:
     """An EtherCAT packet representation
 
     A packet contains one or more datagrams which are sent as EtherNet
     packets. We implicitly add a datagram in the front which later serves
     as an identifier for the packet.
     """
-    MAXSIZE = 1000  # maximum size we use for an EtherCAT packet
+    MAXSIZE = 1500  # maximum size we use for an EtherCAT packet
     ETHERNET_HEADER = 14
+    PACKET_HEADER = 16
     DATAGRAM_HEADER = 10
     DATAGRAM_TAIL = 2
 
     def __init__(self):
         self.data = []
-        self.size = 14
+        self.size = self.PACKET_HEADER
 
     def append(self, cmd, data, idx, *address):
         """Append a datagram to the packet
 
         :param cmd: EtherCAT command
         :type cmd: ECCmd
         :param data: the data in the datagram
         :param idx: the datagram index, unchanged by terminals
 
         Depending on the command, one or two more parameters represent the
         address, either terminal and offset for position or node addressing,
         or one value for logical addressing."""
+        newsize = self.size + len(data) + self.DATAGRAM_HEADER \
+                  + self.DATAGRAM_TAIL
+        if newsize > self.MAXSIZE:
+            raise OverflowError("ethercat packet size too big")
+        elif len(self.data) > 14:
+            raise OverflowError("Too many datagrams per packet")
+
         self.data.append((cmd, data, idx) + address)
-        self.size += len(data) + self.DATAGRAM_HEADER + self.DATAGRAM_TAIL
+        self.size = newsize
 
     def assemble(self, index):
         """Assemble the datagrams into a packet
 
         :param index: an identifier for the packet
 
         An implicit empty datagram is added at the beginning of the packet
         that may be used as an identifier for the packet.
         """
-        ret = [pack("<HBBiHHH", self.size | 0x1000, 0, 0, index, 1 << 15, 0, 0)]
+        ret = [pack("<HBBiHHHH", (self.size-2) | 0x1000, 0, 0, index, 0x8002, 0, 0, 0)]
         for i, (cmd, data, *dgram) in enumerate(self.data, start=1):
             ret.append(pack("<BBhHHH" if len(dgram) == 3 else "<BBiHH",
                             cmd.value, *dgram,
                             len(data) | ((i < len(self.data)) << 15), 0))
             ret.append(data)
             ret.append(b"\0\0")
+        if self.size < 46:
+            ret.append(b"3" * (46 - self.size))
         return b''.join(ret)
 
     def __str__(self):
         ret = "\n".join(f"{cmd} {data} {idx} {addr}"
                         for cmd, data, idx, *addr in self.data)
         return "Packet([" + ret + "]"
 
     def disassemble(self, data):
         pos = 14 + self.DATAGRAM_HEADER
         ret = []
         for cmd, bits, *dgram in self.data:
-            ret.append((data[pos-self.DATAGRAM_HEADER],
-                        data[pos:pos+len(bits)],
+            ret.append(unpack("<Bxh6x", data[pos-self.DATAGRAM_HEADER:pos])
+                       + (data[pos:pos+len(bits)],
                         unpack("<H", data[pos+len(bits):pos+len(bits)+2])[0]))
             pos += self.DATAGRAM_HEADER + self.DATAGRAM_TAIL
-        return ''.join(f"{i}: {c} {f} {d}\n" for i, (c, d, f) in enumerate(ret))
+        return ''.join(f"{i}: {c} {a} {f} {d}\n" for i, (c, a, d, f) in enumerate(ret))
 
     def full(self):
         """Is the data limit reached?"""
         return self.size > self.MAXSIZE or len(self.data) > 14
 
 
 class EtherCat(Protocol):
@@ -241,41 +294,70 @@
     This class supports both to send individual datagrams and wait for their
     response, but also to send and receive entire packets. """
     def __init__(self, network):
         """
         :param network: the name of the network adapter, like "eth0"
         """
         self.addr = (network, 0x88A4, 0, 0, b"\xff\xff\xff\xff\xff\xff")
-        self.send_queue = Queue()
         self.wait_futures = {}
 
     async def connect(self):
         """connect to the EtherCAT loop"""
+        self.send_queue = Queue()
         await get_event_loop().create_datagram_endpoint(
             lambda: self, family=AF_PACKET, proto=0xA488)
 
     async def sendloop(self):
         """the eternal datagram sending loop
 
         This method runs while we are connected, takes the datagrams
         to be sent from a queue, packs them in a packet and ships them
         out. """
-        packet = Packet()
-        dgrams = []
-        while True:
-            *dgram, future = await self.send_queue.get()
-            lastsize = packet.size
-            packet.append(*dgram)
-            dgrams.append((lastsize + 10, packet.size - 2, future))
-            if packet.full() or self.send_queue.empty():
-                data = await self.roundtrip_packet(packet)
-                for start, stop, future in dgrams:
-                    future.set_result(data[start:stop])
+        try:
+            dgrams = []
+            packet = Packet()
+            sent = True
+            while True:
+                if sent:
+                   *dgram, future = await self.send_queue.get()
+                try:
+                   lastsize = packet.size
+                   packet.append(*dgram)
+                   dgrams.append((lastsize + 10, packet.size - 2, future))
+                   sent = True
+                   if not self.send_queue.empty():
+                       continue
+                except OverflowError:
+                    sent = False
+                ensure_future(self.process_packet(dgrams, packet))
                 dgrams = []
                 packet = Packet()
+        except CancelledError:
+            raise
+        except Exception:
+            logging.exception("sendloop failed")
+            raise
+
+    async def process_packet(self, dgrams, packet):
+        try:
+            data = await self.roundtrip_packet(packet)
+            for start, stop, future in dgrams:
+                wkc, = unpack("<H", data[stop:stop+2])
+                if wkc == 0:
+                    future.set_exception(
+                        EtherCatError("datagram was not processed"))
+                elif not future.done():
+                    future.set_result(data[start:stop])
+                else:
+                    logging.info("future already done, dropped datagram")
+        except CancelledError:
+            raise
+        except Exception:
+            logging.exception("process_packet failed")
+            raise
 
     async def roundtrip_packet(self, packet):
         """Send a packet and return the response
 
         Send the `packet` to the loop and wait that it comes back,
         and return that to the caller. """
         index = randint(2000, 1000000000)
@@ -312,45 +394,78 @@
         interpreted as a format for a `struct.pack`, everything else is the data
         for those format. Upon returning, the received data will be unpacked
         accoding to the format strings. """
         future = Future()
         fmt = "<" + "".join(arg for arg in args[:-1] if isinstance(arg, str))
         out = pack(fmt, *[arg for arg in args if not isinstance(arg, str)])
         if args and isinstance(args[-1], str):
-            out += b"\0" * calcsize(args[-1])
+            out += b"\0" * calcsize("<" + args[-1])
             fmt += args[-1]
         if isinstance(data, int):
             out += b"\0" * data
         elif data is not None:
             out += data
+        assert isinstance(pos, int) and isinstance(offset, int), \
+            f"pos: {pos} offset: {offset}"
         self.send_queue.put_nowait((cmd, out, idx, pos, offset, future))
         ret = await future
         if data is None:
             return unpack(fmt, ret)
         elif args:
             if not isinstance(data, int):
                 data = len(data)
             return unpack(fmt, ret[:-data]) + (ret[-data:],)
         else:
             return ret
 
+    async def count(self):
+        """Count the number of terminals on the bus"""
+        p = Packet()
+        p.append(ECCmd.APRD, b"\0\0", 0, 0, 0x10)
+        ret = await self.roundtrip_packet(p)
+        no, = unpack_from("<h", ret, 18)  # number of terminals
+        return no
+
+    async def find_free_address(self):
+        """Find an absolute address currently not in use"""
+        while True:
+            i = randint(1000, 30000)
+            try:
+                await self.roundtrip(ECCmd.FPRD, i, 0x10, "H", 0)
+            except EtherCatError:
+                return i  # this address is not in use
+
+    async def eeprom_read(self, position, start):
+        """read 4 bytes from the eeprom of terminal `position` at `start`"""
+        while (await self.roundtrip(ECCmd.APRD, position,
+                                    0x502, "H"))[0] & 0x8000:
+            pass
+        await self.roundtrip(ECCmd.APWR, position, 0x502, "HI", 0x100, start)
+        busy = 0x8000
+        while busy & 0x8000:
+            busy, data = await self.roundtrip(ECCmd.APRD, position,
+                                              0x502, "H4xI")
+        return data
+
     def connection_made(self, transport):
         """start the send loop once the connection is made"""
         transport.get_extra_info("socket").bind(self.addr)
         self.transport = transport
         ensure_future(self.sendloop())
 
     def datagram_received(self, data, addr):
         """distribute received packets to the recipients"""
         index, = unpack("<I", data[4:8])
         self.wait_futures[index].set_result(data)
 
 
 class Terminal:
-    """Represent one terminal ("slave") in the loop"""
+    """Represent one terminal (*SubDevice* or *slave*) in the loop"""
+    def __init__(self, ethercat):
+        self.ec = ethercat
 
     async def initialize(self, relative, absolute):
         """Initialize the terminal
 
         this sets up the connection to the terminal we represent.
 
         :param relative: the position of the terminal in the loop,
@@ -361,161 +476,239 @@
         therein. It still leaves the terminal in the init state. """
         await self.ec.roundtrip(ECCmd.APWR, relative, 0x10, "H", absolute)
         self.position = absolute
 
         await self.set_state(0x11)
         await self.set_state(1)
 
+        fmmu_no, = await self.read(4, "B")
+        self.fmmu_used = [None] * fmmu_no
+        # switch off all fmmus
+        for i in range(fmmu_no):
+            await self.write(0x60c + 0x10 * i, "B", 0)
+
+        self.mbx_cnt = 1
+        self.mbx_lock = Lock()
+
+        await self.apply_eeprom()
+
+    async def apply_eeprom(self):
         async def read_eeprom(no, fmt):
-            return unpack(fmt, await self.eeprom_read_one(no))
+            return unpack(fmt, await self._eeprom_read_one(no))
 
-        self.vendorId, self.productCode = await read_eeprom(8, "<II")
-        self.revisionNo, self.serialNo = await read_eeprom(0xc, "<II")
+        self.vendorId, self.productCode = \
+                await read_eeprom(EEPROM.VENDOR_ID, "<II")
+        self.revisionNo, self.serialNo = \
+                await read_eeprom(EEPROM.REVISION, "<II")
         # this reads the mailbox configuration from the EEPROM header.
         # weirdly this does not match with the later EEPROM SM configuration
         # self.mbx_in_off, self.mbx_in_sz, self.mbx_out_off, self.mbx_out_sz = \
         #     await read_eeprom(0x18, "<HHHH")
 
-        self.mbx_cnt = 1
-        self.mbx_lock = Lock()
-
         self.eeprom = await self.read_eeprom()
+        if 41 not in self.eeprom:
+            # no sync managers defined in eeprom
+            return
         await self.write(0x800, data=0x80)  # empty out sync manager
         await self.write(0x800, data=self.eeprom[41])
         self.mbx_out_off = self.mbx_out_sz = None
         self.mbx_in_off = self.mbx_in_sz = None
         self.pdo_out_off = self.pdo_out_sz = None
         self.pdo_in_off = self.pdo_in_sz = None
+        self.pdo_in_addr = 0x818
+        self.pdo_out_addr = 0x810
         for i in range(0, len(self.eeprom[41]), 8):
             offset, size, mode = unpack("<HHB", self.eeprom[41][i:i+5])
             mode &= 0xf
             if mode == 0:
                 self.pdo_in_off = offset
                 self.pdo_in_sz = size
+                self.pdo_in_addr = 0x800 + i
             elif mode == 2:
                 self.mbx_in_off = offset
                 self.mbx_in_sz = size
             elif mode == 4:
                 self.pdo_out_off = offset
                 self.pdo_out_sz = size
+                self.pdo_out_addr = 0x800 + i
             elif mode == 6:
                 self.mbx_out_off = offset
                 self.mbx_out_sz = size
-        s = await self.read(0x800, data=0x80)
-        print(absolute, " ".join(f"{c:02x} {'|' if i % 8 == 7 else ''}" for i, c in enumerate(s)))
+            else:
+                logging.error("wrong mode parsing sync managers in EEPROM")
 
-    def parse_pdos(self):
-        def parse_pdo(s):
+    async def write_pdo_sm(self):
+        await self.write(self.pdo_out_addr + 6, "B", 0)
+        await self.write(self.pdo_out_addr + 2, "H", self.pdo_out_sz)
+        await self.write(self.pdo_out_addr + 6, "B", self.pdo_out_sz > 0)
+        await self.write(self.pdo_in_addr + 6, "B", 0)
+        await self.write(self.pdo_in_addr + 2, "H", self.pdo_in_sz)
+        await self.write(self.pdo_in_addr + 6, "B", self.pdo_in_sz > 0)
+
+    async def parse_pdos(self):
+        async def parse_eeprom(s):
             i = 0
+            bitpos = 0
             while i < len(s):
-                idx, e, sm, u1, u2, u3 = unpack("<HBBBBH", s[i:i+8])
-                print(f"idx {idx:x} sm {sm} {u1:x} {u2:x} {u3:x}")
+                # third parameter seems to indicate the sync manager, sometimes
+                idx, e, sm, u1, u2, u3 = unpack_from("<HBbBBH", s, i)
                 i += 8
                 for er in range(e):
-                    bitsize, = unpack("<5xB2x", s[i:i+8])
-                    print("  bs", bitsize, s[i:i+8])
+                    idx, subidx, k1, k2, bits, = unpack_from("<HBBBB2x", s, i)
+                    yield idx, subidx, bits
                     i += 8
 
-        if 50 in self.eeprom:
-            parse_pdo(self.eeprom[50])
-        if 51 in self.eeprom:
-            parse_pdo(self.eeprom[51])
+        async def parse_sdo(index):
+            assignment = await self.sdo_read(index)
+            bitpos = 0
+            for i in range(0, len(assignment), 2):
+                pdo, = unpack_from("<H", assignment, i)
+                if pdo == 0:
+                    continue
+                count, = unpack("B", await self.sdo_read(pdo, 0))
+                for j in range(1, count + 1):
+                    bits, subidx, idx = unpack("<BBH", await self.sdo_read(pdo, j))
+                    yield idx, subidx, bits
+
+        async def parse(func, sm):
+            bitpos = 0
+            async for idx, subidx, bits in func:
+                if idx == 0:
+                    pass
+                elif bits < 8:
+                    self.pdos[idx, subidx] = (sm, bitpos // 8, bitpos % 8)
+                elif (bits % 8) or (bitpos % 8):
+                    raise RuntimeError("PDOs must be byte-aligned")
+                else:
+                    self.pdos[idx, subidx] = \
+                        (sm, bitpos // 8,
+                         {8: "B", 16: "H", 32: "I", 64: "Q"}[bits])
+                bitpos += bits
+            return bitpos
+
+        self.pdos = {}
+        if self.has_mailbox():
+            return (await parse(parse_sdo(0x1c12), SyncManager.OUT),
+                    await parse(parse_sdo(0x1c13), SyncManager.IN))
+        else:
+            return (
+                await parse(parse_eeprom(self.eeprom[51]), SyncManager.OUT)
+                if 51 in self.eeprom else 0,
+                await parse(parse_eeprom(self.eeprom[50]), SyncManager.IN)
+                if 50 in self.eeprom else 0)
 
     async def set_state(self, state):
         """try to set the state, and return the new state"""
         await self.ec.roundtrip(ECCmd.FPWR, self.position, 0x0120, "H", state)
         ret, = await self.ec.roundtrip(ECCmd.FPRD, self.position, 0x0130, "H")
         return ret
 
     async def get_state(self):
-        """get the current state"""
-        ret, = await self.ec.roundtrip(ECCmd.FPRD, self.position, 0x0130, "H")
-        return ret
+        """get the current state, error flag and status word"""
+        state, status = await self.ec.roundtrip(ECCmd.FPRD, self.position,
+                                                0x0130, "H2xH")
+        return MachineState(state & 0xf), bool(state & 0x10), status
 
-    async def to_operational(self):
+    async def to_operational(self, target=MachineState.OPERATIONAL):
         """try to bring the terminal to operational state
 
         this tries to push the terminal through its state machine to the
-        operational state. Note that even if it reaches there, the terminal
+        target state. Note that even if it reaches there, the terminal
         will quickly return to pre-operational if no packets are sent to keep
-        it operational. """
-        order = [1, 2, 4, 8]
-        ret, error = await self.ec.roundtrip(
-                ECCmd.FPRD, self.position, 0x0130, "H2xH")
-        if ret & 0x10:
+        it operational.
+
+        return the state, error flag and status before the operation."""
+        order = list(MachineState)
+        state, error, status = ret = await self.get_state()
+        if error:
             await self.ec.roundtrip(ECCmd.FPWR, self.position,
                                     0x0120, "H", 0x11)
-            ret, error = await self.ec.roundtrip(ECCmd.FPRD, self.position,
-                                                 0x0130, "H2xH")
-        pos = order.index(ret)
-        s = 0x11
-        for state in order[pos+1:]:
+            state = MachineState.INIT
+        for current in order[order.index(state) + 1:]:
+            if state.value >= target.value:
+                return ret
             await self.ec.roundtrip(ECCmd.FPWR, self.position,
-                                    0x0120, "H", state)
-            while s != state:
-                s, error = await self.ec.roundtrip(ECCmd.FPRD, self.position,
-                                                   0x0130, "H2xH")
-                if error != 0:
-                    raise RuntimeError(f"AL register {error}")
-
-    async def get_error(self):
-        """read the error register"""
-        return (await self.ec.roundtrip(ECCmd.FPRD, self.position,
-                                        0x0134, "H"))[0]
+                                    0x0120, "H", current.value)
+            while current is not state:
+                state, error, status = await self.get_state()
+                if error:
+                    raise EtherCatError(f"AL register error {status}")
 
     async def read(self, start, *args, **kwargs):
         """read data from the terminal at offset `start`
 
         see `EtherCat.roundtrip` for details on more parameters. """
         return (await self.ec.roundtrip(ECCmd.FPRD, self.position,
                                         start, *args, **kwargs))
 
     async def write(self, start, *args, **kwargs):
-        """write data from the terminal at offset `start`
+        """write data to the terminal at offset `start`
 
         see `EtherCat.roundtrip` for details on more parameters"""
         return (await self.ec.roundtrip(ECCmd.FPWR, self.position,
                                         start, *args, **kwargs))
 
-    async def eeprom_read_one(self, start):
+    async def _eeprom_read_one(self, start):
         """read 8 bytes from the eeprom at `start`"""
         while (await self.read(0x502, "H"))[0] & 0x8000:
             pass
         await self.write(0x502, "HI", 0x100, start)
         busy = 0x8000
         while busy & 0x8000:
             busy, data = await self.read(0x502, "H4x8s")
-        return data
+        if busy & 0x40:  # otherwise we actually only read 4 bytes
+            return data
+        await self.write(0x502, "HI", 0x100, start + 2)
+        busy = 0x8000
+        while busy & 0x8000:
+            busy, data2 = await self.read(0x502, "H4x4s")
+        return data[:4] + data2
+
+    async def eeprom_write_one(self, start, data):
+        """write 2 bytes to the eeprom at `start`"""
+        while (await self.read(0x502, "H"))[0] & 0x8000:
+            pass
+        busy = 0x1000
+        while busy & 0xff00:
+            await self.write(0x502, "HIH", 0x201, start, data)
+            busy = 0x8000
+            while busy & 0x8000:
+                busy, = await self.read(0x502, "H")
+            await self.write(0x502, "H", 0)
 
     async def read_eeprom(self):
         """read the entire eeprom"""
         async def get_data(size):
             nonlocal data, pos
 
             while len(data) < size:
-                data += await self.eeprom_read_one(pos)
+                data += await self._eeprom_read_one(pos)
                 pos += 4
             ret, data = data[:size], data[size:]
             return ret
 
         pos = 0x40
         data = b""
         eeprom = {}
 
         while True:
             hd, ws = unpack("<HH", await get_data(4))
             if hd == 0xffff:
                 return eeprom
             eeprom[hd] = await get_data(ws * 2)
 
+    def has_mailbox(self):
+        return self.mbx_out_off is not None and self.mbx_in_off is not None
+
     async def mbx_send(self, type, *args, data=None, address=0, priority=0, channel=0):
         """send data to the mailbox"""
         status, = await self.read(0x805, "B")  # always using mailbox 0, OK?
         if status & 8:
-            raise RuntimeError("mailbox full, read first")
+            raise EtherCatError("mailbox full, read first")
+        assert self.mbx_out_off is not None, "not send mailbox defined"
         await self.write(self.mbx_out_off, "HHBB",
                                 datasize(args, data),
                                 address, channel | priority << 6,
                                 type.value | self.mbx_cnt << 4,
                                 *args, data=data)
         await self.write(self.mbx_out_off + self.mbx_out_sz - 1,
                                 data=1)
@@ -523,114 +716,138 @@
 
     async def mbx_recv(self):
         """receive data from the mailbox"""
         status = 0
         while status & 8 == 0:
             # always using mailbox 1, OK?
             status, = await self.read(0x80D, "B")
+        assert self.mbx_in_off is not None, "not receive mailbox defined"
         dlen, address, prio, type, data = await self.read(
                 self.mbx_in_off, "HHBB", data=self.mbx_in_sz - 6)
         return MBXType(type & 0xf), data[:dlen]
 
     async def coe_request(self, coecmd, odcmd, *args, **kwargs):
         async with self.mbx_lock:
             await self.mbx_send(MBXType.COE, "HBxH", coecmd.value << 12,
                                 odcmd.value, 0, *args, **kwargs)
             fragments = True
             ret = []
             offset = 8  # skip header in first packet
 
             while fragments:
-                type, data = await self.mbx_recv()
-                if type is not MBXType.COE:
-                    raise RuntimeError(f"expected CoE package, got {type}")
+                type = None
+                while type is not MBXType.COE:
+                    type, data = await self.mbx_recv()
+                    if type is not MBXType.COE:
+                        logging.warning(f"expected CoE package, got {type}")
                 coecmd, rodcmd, fragments = unpack("<HBxH", data[:6])
                 if rodcmd & 0x7f != odcmd.value + 1:
-                    raise RuntimeError(f"expected {odcmd.value}, got {odcmd}")
+                    raise EtherCatError(f"expected {odcmd.value}, got {rodcmd}")
                 ret.append(data[offset:])
                 offset = 6
             return b"".join(ret)
 
     async def sdo_read(self, index, subindex=None):
+        """read a single SDO entry
+
+        given an adress for a CoE entry like 6020:12, you may read
+        the value like ``await master.sdo_read(0x6020, 0x12)``.
+        """
         async with self.mbx_lock:
             await self.mbx_send(
                     MBXType.COE, "HBHB4x", CoECmd.SDOREQ.value << 12,
                     ODCmd.UP_REQ_CA.value if subindex is None
                     else ODCmd.UP_REQ.value,
                     index, 1 if subindex is None else subindex)
-            type, data = await self.mbx_recv()
-            if type is not MBXType.COE:
-                raise RuntimeError(f"expected CoE, got {type}")
+            type = None
+            while type is not MBXType.COE:
+                type, data = await self.mbx_recv()
+                if type is not MBXType.COE:
+                    logging.warning(f"expected CoE package, got {type}")
             coecmd, sdocmd, idx, subidx, size = unpack("<HBHBI", data[:10])
             if coecmd >> 12 != CoECmd.SDORES.value:
-                raise RuntimeError(f"expected CoE SDORES (3), got {coecmd>>12:x}")
+                if subindex is None and coecmd >> 12 == CoECmd.SDOREQ.value:
+                    return b""  # if there is no data, the terminal fails
+                raise EtherCatError(
+                    f"expected CoE SDORES (3), got {coecmd>>12:x} "
+                    f"for {index:X}:{9 if subindex is None else subindex:02X}")
             if idx != index:
-                raise RuntimeError(f"requested index {index}, got {idx}")
+                raise EtherCatError(f"requested index {index}, got {idx}")
             if sdocmd & 2:
                 return data[6 : 10 - ((sdocmd>>2) & 3)]
             ret = [data[10:]]
             retsize = len(ret[0])
 
             toggle = 0
             while retsize < size:
                 await self.mbx_send(
                         MBXType.COE, "HBHB4x", CoECmd.SDOREQ.value << 12,
                         ODCmd.SEG_UP_REQ.value + toggle, index,
                         1 if subindex is None else subindex)
                 type, data = await self.mbx_recv()
                 if type is not MBXType.COE:
-                    raise RuntimeError(f"expected CoE, got {type}")
+                    raise EtherCatError(f"expected CoE, got {type}")
                 coecmd, sdocmd = unpack("<HB", data[:3])
                 if coecmd >> 12 != CoECmd.SDORES.value:
-                    raise RuntimeError(f"expected CoE cmd SDORES, got {coecmd}")
+                    raise EtherCatError(
+                        f"expected CoE cmd SDORES, got {coecmd}")
                 if sdocmd & 0xe0 != 0:
-                    raise RuntimeError(f"requested index {index}, got {idx}")
+                    raise EtherCatError(f"requested index {index}, got {idx}")
                 if sdocmd & 1 and len(data) == 7:
                     data = data[:3 + (sdocmd >> 1) & 7]
                 ret += data[3:]
                 retsize += len(data) - 3
                 if sdocmd & 1:
                     break
                 toggle ^= 0x10
             if retsize != size:
-                raise RuntimeError(f"expected {size} bytes, got {retsize}")
+                raise EtherCatError(f"expected {size} bytes, got {retsize}")
             return b"".join(ret)
 
     async def sdo_write(self, data, index, subindex=None):
+        """write a single SDO entry
+
+        given a CoE address like 1200:2, one may write the value as
+        in ``await master.sdo_write(b'abc', 0x1200, 0x2)``. Note that the
+        data needs to already be a binary string matching the binary type of
+        the parameter.
+        """
         if len(data) <= 4 and subindex is not None:
             async with self.mbx_lock:
                 await self.mbx_send(
                         MBXType.COE, "HBHB4s", CoECmd.SDOREQ.value << 12,
                         ODCmd.DOWN_EXP.value | (((4 - len(data)) << 2) & 0xc),
                         index, subindex, data)
                 type, data = await self.mbx_recv()
             if type is not MBXType.COE:
-                raise RuntimeError(f"expected CoE, got {type}, {data} {odata} {index:x} {subindex}")
+                raise EtherCatError(f"expected CoE, got {type}, {data} "
+                                    f"{odata} {index:x}:{subindex:x}")
             coecmd, sdocmd, idx, subidx = unpack("<HBHB", data[:6])
             if idx != index or subindex != subidx:
-                raise RuntimeError(f"requested index {index}, got {idx}")
+                raise EtherCatError(f"requested index {index:x}:{subindex:x}, "
+                                    f"got {idx:x}:{subidx:x}")
             if coecmd >> 12 != CoECmd.SDORES.value:
-                raise RuntimeError(f"expected CoE SDORES, got {coecmd>>12:x}")
+                raise EtherCatError(f"expected CoE SDORES, got {coecmd>>12:x}")
         else:
             async with self.mbx_lock:
                 stop = min(len(data), self.mbx_out_sz - 16)
                 await self.mbx_send(
                         MBXType.COE, "HBHB4x", CoECmd.SDOREQ.value << 12,
                         ODCmd.DOWN_INIT_CA.value if subindex is None
                         else ODCmd.DOWN_INIT.value,
                         index, 1 if subindex is None else subindex,
                         data=data[:stop])
                 type, data = await self.mbx_recv()
                 if type is not MBXType.COE:
-                    raise RuntimeError(f"expected CoE, got {type}")
+                    raise EtherCatError(f"expected CoE, got {type}")
                 coecmd, sdocmd, idx, subidx = unpack("<HBHB", data[:6])
                 if coecmd >> 12 != CoECmd.SDORES.value:
-                    raise RuntimeError(f"expected CoE SDORES, got {coecmd>>12:x}")
+                    raise EtherCatError(f"expected CoE SDORES, got {coecmd>>12:x}")
                 if idx != index or subindex != subidx:
-                    raise RuntimeError(f"requested index {index}, got {idx}")
+                    raise EtherCatError(f"requested index {index}, got {idx}")
                 toggle = 0
                 while stop < len(data):
                     start = stop
                     stop = min(len(data), start + self.mbx_out_sz - 9)
                     if stop == len(data):
                         if stop - start < 7:
                             cmd = 1 + (7-stop+start << 1)
@@ -640,20 +857,20 @@
                             d = data[start:stop]
                         await self.mbx_send(
                                 MBXType.COE, "HBHB4x", CoECmd.SDOREQ.value << 12,
                                 cmd + toggle, index,
                                 1 if subindex is None else subindex, data=d)
                         type, data = await self.mbx_recv()
                         if type is not MBXType.COE:
-                            raise RuntimeError(f"expected CoE, got {type}")
+                            raise EtherCatError(f"expected CoE, got {type}")
                         coecmd, sdocmd, idx, subidx = unpack("<HBHB", data[:6])
                         if coecmd >> 12 != CoECmd.SDORES.value:
-                            raise RuntimeError(f"expected CoE SDORES")
+                            raise EtherCatError(f"expected CoE SDORES")
                         if idx != index or subindex != subidx:
-                            raise RuntimeError(f"requested index {index}")
+                            raise EtherCatError(f"requested index {index}")
                     toggle ^= 0x10
 
     async def read_ODlist(self):
         idxes = await self.coe_request(CoECmd.SDOINFO, ODCmd.LIST_REQ, "H", 1)
         idxes = unpack("<" + "H" * int(len(idxes) // 2), idxes)
 
         ret = {}
@@ -669,74 +886,55 @@
             od.maxSub = ms
             od.name = data[4:].decode("utf8")
             ret[od.index] = od
 
         for od in ret.values():
             od.entries = {}
             for i in range(1 if od.maxSub > 0 else 0, od.maxSub + 1):
-                data = await self.coe_request(CoECmd.SDOINFO, ODCmd.OE_REQ,
-                                              "HBB", od.index, i, 7)
+                try:
+                    data = await self.coe_request(CoECmd.SDOINFO, ODCmd.OE_REQ,
+                                                  "HBB", od.index, i, 7)
+                except EtherCatError as e:
+                    logging.info(f"problems reading SDO {od.index:x}:{i:x}:")
+                    continue
                 oe = ObjectEntry(od)
                 oe.valueInfo, dataType, oe.bitLength, oe.objectAccess = \
-                        unpack("<HHHH", data[:8])
+                        unpack("<BxHHH", data[:8])
                 if dataType == 0:
                     continue
                 assert i == oe.valueInfo
                 if dataType < 2048:
                     oe.dataType = ECDataType(dataType)
                 else:
                     oe.dataType = dataType
                 oe.name = data[8:].decode("utf8")
                 od.entries[i] = oe
         return ret
 
+    @asynccontextmanager
+    async def map_fmmu(self, logical, write):
+        """map the pdo to `logical` address.
+
+        :param write: a boolean indicating whether this is to be used
+            for writing (instead of reading).
+        """
+        if write:
+            offset = self.pdo_out_off
+            size = self.pdo_out_sz
+            start = 1
+        else:
+            offset = self.pdo_in_off
+            size = self.pdo_in_sz
+            start = len(self.fmmu_used)
+        assert size is not None
+        assert offset is not None
 
-async def main():
-    from .bpf import lookup_elem
+        index = start - self.fmmu_used[start::-1].index(None) - 1
 
-    ec = EtherCat("eth0")
-    await ec.connect()
-    #map_fd = await install_ebpf2()
-    tin = Terminal()
-    tin.ec = ec
-    tout = Terminal()
-    tout.ec = ec
-    tdigi = Terminal()
-    tdigi.ec = ec
-    await gather(
-        tin.initialize(-4, 19),
-        tout.initialize(-2, 55),
-        tdigi.initialize(0, 22),
-        )
-    print("tin")
-    #await tin.to_operational()
-    await tin.set_state(2)
-    print("tout")
-    await tout.to_operational()
-    print("reading odlist")
-    odlist2, odlist = await gather(tin.read_ODlist(), tout.read_ODlist())
-    #oe = odlist[0x7001][1]
-    #await oe.write(1)
-    for o in odlist.values():
-        print(hex(o.index), o.name, o.maxSub)
-        for i, p in o.entries.items():
-            print("   ", i, p.name, "|", p.dataType, p.bitLength, p.objectAccess)
-            #sdo = await tin.sdo_read(o.index, i)
-            try:
-               sdo = await p.read()
-               if isinstance(sdo, int):
-                   t = hex(sdo)
-               else:
-                   t = ""
-               print("   ", sdo, t)
-            except RuntimeError as e:
-               print("   E", e)
-    print("set sdo")
-    oe = odlist[0x8010][7]
-    print("=", await oe.read())
-    await oe.write(1)
-    print("=", await oe.read())
-    print(tdigi.eeprom[10])
-
-if __name__ == "__main__":
-    loop = get_event_loop()
-    loop.run_until_complete(main())
+        self.fmmu_used[index] = logical
+        try:
+            await self.write(0x600 + 0x10 * index, "IHBBHBBB3x", logical, size,
+                             0, 7, offset, 0, 2 if write else 1, 1)
+            yield index
+            await self.write(0x60c + 0x10 * index, "B", 0)
+        finally:
+            self.fmmu_used[index] = None
```

### Comparing `ebpfcat-0.1.0/ebpfcat/hashmap.py` & `ebpfcat-0.4.1/ebpfcat/hashmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,29 +14,28 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 from contextlib import contextmanager
 from struct import pack, unpack, unpack
 
-from .ebpf import AssembleError, Expression, Opcode, Map, FuncId, Memory
+from .ebpf import AssembleError, Expression, Opcode, Map, FuncId
 from .bpf import create_map, lookup_elem, MapType, update_elem
 
 
 class HashGlobalVar(Expression):
     def __init__(self, ebpf, count, fmt):
         self.ebpf = ebpf
         self.count = count
         self.fmt = fmt
         self.signed = fmt.islower()
+        self.fixed = fmt == "x"
 
     @contextmanager
-    def get_address(self, dst, long, signed, force=False):
-        if signed != self.fmt.islower():
-            raise AssembleError("HashMap variable has wrong signedness")
+    def get_address(self, dst, long, force=False):
         with self.ebpf.save_registers([i for i in range(6) if i != dst]), \
                 self.ebpf.get_stack(4) as stack:
             self.ebpf.append(Opcode.ST, 10, 0, stack, self.count)
             self.ebpf.r1 = self.ebpf.get_fd(self.fd)
             self.ebpf.r2 = self.ebpf.r10 + stack
             self.ebpf.call(FuncId.map_lookup_elem)
             with self.ebpf.r0 == 0:
@@ -74,15 +73,15 @@
     def __set__(self, ebpf, value):
         if ebpf.loaded:
             fd = ebpf.__dict__[self.name].fd
             update_elem(fd, pack("B", self.count),
                         pack("q" if self.fmt.islower() else "Q", value), 0)
             return
         with ebpf.save_registers([3]):
-            with value.get_address(3, True, self.fmt.islower(), True):
+            with value.get_address(3, True, True):
                 with ebpf.save_registers([0, 1, 2, 4, 5]), \
                         ebpf.get_stack(4) as stack:
                     ebpf.r1 = ebpf.get_fd(ebpf.__dict__[self.name].fd)
                     ebpf.append(Opcode.ST, 10, 0, stack, self.count)
                     ebpf.r2 = ebpf.r10 + stack
                     ebpf.r4 = 0
                     ebpf.call(FuncId.map_update_elem)
@@ -96,15 +95,16 @@
 
     def globalVar(self, fmt="I", default=0):
         self.count += 1
         ret = HashGlobalVarDesc(self.count, fmt, default)
         self.vars.append(ret)
         return ret
 
-    def init(self, ebpf):
-        fd = create_map(MapType.HASH, 1, 8, self.count)
+    def init(self, ebpf, fd):
+        if fd is None:
+            fd = create_map(MapType.HASH, 1, 8, self.count)
         for v in self.vars:
             getattr(ebpf, v.name).fd = fd
 
     def load(self, ebpf):
         for v in self.vars:
             setattr(ebpf, v.name, ebpf.__class__.__dict__[v.name].default)
```

### Comparing `ebpfcat-0.1.0/ebpfcat/serial.py` & `ebpfcat-0.4.1/ebpfcat/serial.py`

 * *Files identical despite different names*

