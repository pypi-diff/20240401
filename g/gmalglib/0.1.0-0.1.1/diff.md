# Comparing `tmp/gmalglib-0.1.0.tar.gz` & `tmp/gmalglib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.1.0.tar", last modified: Mon Apr  1 11:17:34 2024, max compression
+gzip compressed data, was "gmalglib-0.1.1.tar", last modified: Mon Apr  1 11:52:41 2024, max compression
```

## Comparing `gmalglib-0.1.0.tar` & `gmalglib-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:34.361993 gmalglib-0.1.0/
--rw-rw-rw-   0        0        0      926 2024-04-01 11:17:34.360745 gmalglib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-01 11:14:50.000000 gmalglib-0.1.0/README.en.md
--rw-rw-rw-   0        0        0      342 2024-04-01 11:14:36.000000 gmalglib-0.1.0/README.md
--rw-rw-rw-   0        0        0      808 2024-04-01 09:41:32.000000 gmalglib-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 11:17:34.361993 gmalglib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      242 2024-04-01 10:01:19.000000 gmalglib-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:34.354061 gmalglib-0.1.0/sm3/
--rw-rw-rw-   0        0        0     6139 2024-04-01 09:26:31.000000 gmalglib-0.1.0/sm3/sm3.c
--rw-rw-rw-   0        0        0      578 2024-04-01 05:16:43.000000 gmalglib-0.1.0/sm3/sm3.h
--rw-rw-rw-   0        0        0     4094 2024-04-01 09:58:53.000000 gmalglib-0.1.0/sm3/sm3module.c
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:34.347931 gmalglib-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:34.355393 gmalglib-0.1.0/src/gmalglib/
--rw-rw-rw-   0        0        0       44 2024-04-01 10:39:29.000000 gmalglib-0.1.0/src/gmalglib/__init__.py
--rw-rw-rw-   0        0        0      701 2024-04-01 10:43:40.000000 gmalglib-0.1.0/src/gmalglib/sm3.pyi
-drwxrwxrwx   0        0        0        0 2024-04-01 11:17:34.359696 gmalglib-0.1.0/src/gmalglib.egg-info/
--rw-rw-rw-   0        0        0      926 2024-04-01 11:17:34.000000 gmalglib-0.1.0/src/gmalglib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-01 11:17:34.000000 gmalglib-0.1.0/src/gmalglib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 11:17:34.000000 gmalglib-0.1.0/src/gmalglib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 11:17:34.000000 gmalglib-0.1.0/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:52:41.989993 gmalglib-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 11:52:35.000000 gmalglib-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 11:52:41.989993 gmalglib-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 11:52:35.000000 gmalglib-0.1.1/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 11:52:35.000000 gmalglib-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-01 11:52:35.000000 gmalglib-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:52:41.989993 gmalglib-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 11:52:35.000000 gmalglib-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:52:41.989993 gmalglib-0.1.1/sm3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-01 11:52:35.000000 gmalglib-0.1.1/sm3/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-01 11:52:35.000000 gmalglib-0.1.1/sm3/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-01 11:52:35.000000 gmalglib-0.1.1/sm3/sm3module.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:52:41.985993 gmalglib-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:52:41.989993 gmalglib-0.1.1/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 11:52:35.000000 gmalglib-0.1.1/src/gmalglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 11:52:35.000000 gmalglib-0.1.1/src/gmalglib/sm3.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:52:41.989993 gmalglib-0.1.1/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 11:52:41.000000 gmalglib-0.1.1/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 11:52:41.000000 gmalglib-0.1.1/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:52:41.000000 gmalglib-0.1.1/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 11:52:41.000000 gmalglib-0.1.1/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.1.0/PKG-INFO` & `gmalglib-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1
-Name: gmalglib
-Version: 0.1.0
-Summary: GM algorithms C extension for python.
-Author-email: ww-rm <ww-rm@qq.com>
-Project-URL: Homepage, https://github.com/ww-rm/gmalglib
-Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
-Project-URL: Documentation, https://gmalglib.readthedocs.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# gmalglib
-
-[![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
-[![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
+Metadata-Version: 2.1
+Name: gmalglib
+Version: 0.1.1
+Summary: GM algorithms C extension for python.
+Author-email: ww-rm <ww-rm@qq.com>
+Project-URL: Homepage, https://github.com/ww-rm/gmalglib
+Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
+Project-URL: Documentation, https://gmalglib.readthedocs.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security :: Cryptography
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# gmalglib
+
+[![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
+[![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
```

### Comparing `gmalglib-0.1.0/sm3/sm3.c` & `gmalglib-0.1.1/sm3/sm3.c`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-#include <stdint.h>
-#include "sm3.h"
-
-static const
-uint32_t ROL_T_TABLE[64] = {
-    0x79cc4519, 0xf3988a32, 0xe7311465, 0xce6228cb, 0x9cc45197, 0x3988a32f, 0x7311465e, 0xe6228cbc,
-    0xcc451979, 0x988a32f3, 0x311465e7, 0x6228cbce, 0xc451979c, 0x88a32f39, 0x11465e73, 0x228cbce6,
-    0x9d8a7a87, 0x3b14f50f, 0x7629ea1e, 0xec53d43c, 0xd8a7a879, 0xb14f50f3, 0x629ea1e7, 0xc53d43ce,
-    0x8a7a879d, 0x14f50f3b, 0x29ea1e76, 0x53d43cec, 0xa7a879d8, 0x4f50f3b1, 0x9ea1e762, 0x3d43cec5,
-    0x7a879d8a, 0xf50f3b14, 0xea1e7629, 0xd43cec53, 0xa879d8a7, 0x50f3b14f, 0xa1e7629e, 0x43cec53d,
-    0x879d8a7a, 0x0f3b14f5, 0x1e7629ea, 0x3cec53d4, 0x79d8a7a8, 0xf3b14f50, 0xe7629ea1, 0xcec53d43,
-    0x9d8a7a87, 0x3b14f50f, 0x7629ea1e, 0xec53d43c, 0xd8a7a879, 0xb14f50f3, 0x629ea1e7, 0xc53d43ce,
-    0x8a7a879d, 0x14f50f3b, 0x29ea1e76, 0x53d43cec, 0xa7a879d8, 0x4f50f3b1, 0x9ea1e762, 0x3d43cec5,
-};
-
-static const
-uint32_t INIT_TABLE[8] = {
-    0x7380166f, 0x4914b2b9, 0x172442d7, 0xda8a0600, 0xa96f30bc, 0x163138aa, 0xe38dee4d, 0xb0fb0e4e
-};
-
-static inline
-uint32_t ROL(uint32_t X, uint32_t count)
-{
-    return (X << count) | (X >> (32 - count));
-}
-
-static inline
-uint32_t FROM_BE(const uint8_t* bytes)
-{
-    return (((uint32_t)bytes[0]) << 24) | (((uint32_t)bytes[1]) << 16) | (((uint32_t)bytes[2]) << 8) | (((uint32_t)bytes[3]));
-}
-
-static inline
-void TO_BE(uint32_t word, uint8_t* bytes)
-{
-    bytes[0] = (uint8_t)(word >> 24);
-    bytes[1] = (uint8_t)(word >> 16);
-    bytes[2] = (uint8_t)(word >> 8);
-    bytes[3] = (uint8_t)(word);
-}
-
-static inline
-uint32_t T(uint32_t i)
-{
-    return i <= 15 ? 0x79cc4519 : 0x7a879d8a;
-}
-
-static inline
-uint32_t FF(uint32_t i, uint32_t X, uint32_t Y, uint32_t Z)
-{
-    return i <= 15 ? (X ^ Y ^ Z) : ((X & Y) | (X & Z) | (Y & Z));
-}
-
-static inline
-uint32_t GG(uint32_t i, uint32_t X, uint32_t Y, uint32_t Z)
-{
-    return i <= 15 ? (X ^ Y ^ Z) : ((X & Y) | (~X & Z));
-}
-
-static inline
-uint32_t P0(uint32_t X)
-{
-    return X ^ ROL(X, 9) ^ ROL(X, 17);
-}
-
-static inline
-uint32_t P1(uint32_t X)
-{
-    return X ^ ROL(X, 15) ^ ROL(X, 23);
-}
-
-static inline
-void Expand(const uint8_t* B, uint32_t* W1, uint32_t* W2)
-{
-    uint32_t i;
-    for (i = 0; i < 16; i++)
-    {
-        W1[i] = FROM_BE(B + i * 4);
-    }
-    for (i = 16; i < 68; i++)
-    {
-        W1[i] = P1(W1[i - 16] ^ W1[i - 9] ^ ROL(W1[i - 3], 15)) ^ ROL(W1[i - 13], 7) ^ W1[i - 6];
-    }
-    for (i = 0; i < 64; i++)
-    {
-        W2[i] = W1[i] ^ W1[i + 4];
-    }
-}
-
-static inline
-void Compress(const uint32_t* W1, const uint32_t* W2, uint32_t* V)
-{
-    uint32_t i;
-    uint32_t A = V[0];
-    uint32_t B = V[1];
-    uint32_t C = V[2];
-    uint32_t D = V[3];
-    uint32_t E = V[4];
-    uint32_t F = V[5];
-    uint32_t G = V[6];
-    uint32_t H = V[7];
-    uint32_t SS1, SS2, TT1, TT2;
-
-    for (i = 0; i < 64; i++)
-    {
-        SS1 = ROL((ROL(A, 12) + E + ROL_T_TABLE[i]), 7);
-        SS2 = SS1 ^ ROL(A, 12);
-        TT1 = (FF(i, A, B, C) + D + SS2 + W2[i]);
-        TT2 = (GG(i, E, F, G) + H + SS1 + W1[i]);
-        D = C;
-        C = ROL(B, 9);
-        B = A;
-        A = TT1;
-        H = G;
-        G = ROL(F, 19);
-        F = E;
-        E = P0(TT2);
-    }
-
-    V[0] ^= A;
-    V[1] ^= B;
-    V[2] ^= C;
-    V[3] ^= D;
-    V[4] ^= E;
-    V[5] ^= F;
-    V[6] ^= G;
-    V[7] ^= H;
-}
-
-static inline
-void ExpandAndCompress(const uint8_t* B, uint32_t* V)
-{
-    uint32_t W1[68];
-    uint32_t W2[64];
-    Expand(B, W1, W2);
-    Compress(W1, W2, V);
-}
-
-void SM3_Init(SM3* self)
-{
-    uint32_t i;
-    for (i = 0; i < 8; i++)
-    {
-        self->value[i] = INIT_TABLE[i];
-    }
-    for (i = 0; i < 64; i++)
-    {
-        self->msg_buffer[i] = 0;
-    }
-    self->msg_buffer_length = 0;
-    self->msg_bitlen = 0;
-}
-
-int SM3_Update(SM3* self, const uint8_t* data, uint64_t data_len)
-{
-    uint64_t data_idx;
-    if ((data_len >> 61) || self->msg_bitlen + (data_len << 3) < self->msg_bitlen)
-    {
-        return SM3_ERR_OVERFLOW;
-    }
-
-    data_idx = 0;
-    if (self->msg_buffer_length > 0)
-    {
-        while (data_idx < data_len && self->msg_buffer_length < 64)
-        {
-            self->msg_buffer[self->msg_buffer_length++] = data[data_idx++];
-        }
-
-        if (self->msg_buffer_length >= 64)
-        {
-            ExpandAndCompress(self->msg_buffer, self->value);
-            self->msg_buffer_length = 0;
-        }
-    }
-
-    while (data_idx + 63 < data_len)
-    {
-        ExpandAndCompress(data + data_idx, self->value);
-        data_idx += 64;
-    }
-
-    while (data_idx < data_len)
-    {
-        self->msg_buffer[self->msg_buffer_length++] = data[data_idx++];
-    }
-
-    self->msg_bitlen += (data_len << 3);
-
-    return 0;
-}
-
-void SM3_Digest(SM3* self, uint8_t* digest)
-{
-    uint32_t i;
-    uint32_t value[8];
-    uint8_t msg_buffer[64];
-    uint64_t msg_buffer_length = self->msg_buffer_length;
-
-    for (i = 0; i < 8; i++)
-    {
-        value[i] = self->value[i];
-    }
-    for (i = 0; i < msg_buffer_length; i++)
-    {
-        msg_buffer[i] = self->msg_buffer[i];
-    }
-
-    msg_buffer[msg_buffer_length++] = 0x80;
-
-    if (msg_buffer_length > 56)
-    {
-        while (msg_buffer_length < 64)
-        {
-            msg_buffer[msg_buffer_length++] = 0x00;
-        }
-        ExpandAndCompress(msg_buffer, value);
-        msg_buffer_length = 0;
-    }
-
-    while (msg_buffer_length < 56)
-    {
-        msg_buffer[msg_buffer_length++] = 0x00;
-    }
-
-    msg_buffer[56] = (uint8_t)(self->msg_bitlen >> 56);
-    msg_buffer[57] = (uint8_t)(self->msg_bitlen >> 48);
-    msg_buffer[58] = (uint8_t)(self->msg_bitlen >> 40);
-    msg_buffer[59] = (uint8_t)(self->msg_bitlen >> 32);
-    msg_buffer[60] = (uint8_t)(self->msg_bitlen >> 24);
-    msg_buffer[61] = (uint8_t)(self->msg_bitlen >> 16);
-    msg_buffer[62] = (uint8_t)(self->msg_bitlen >> 8);
-    msg_buffer[63] = (uint8_t)(self->msg_bitlen);
-    ExpandAndCompress(msg_buffer, value);
-
-    for (i = 0; i < 8; i++)
-    {
-        TO_BE(value[i], digest + i * 4);
-    }
-}
+#include <stdint.h>
+#include "sm3.h"
+
+static const
+uint32_t ROL_T_TABLE[64] = {
+    0x79cc4519, 0xf3988a32, 0xe7311465, 0xce6228cb, 0x9cc45197, 0x3988a32f, 0x7311465e, 0xe6228cbc,
+    0xcc451979, 0x988a32f3, 0x311465e7, 0x6228cbce, 0xc451979c, 0x88a32f39, 0x11465e73, 0x228cbce6,
+    0x9d8a7a87, 0x3b14f50f, 0x7629ea1e, 0xec53d43c, 0xd8a7a879, 0xb14f50f3, 0x629ea1e7, 0xc53d43ce,
+    0x8a7a879d, 0x14f50f3b, 0x29ea1e76, 0x53d43cec, 0xa7a879d8, 0x4f50f3b1, 0x9ea1e762, 0x3d43cec5,
+    0x7a879d8a, 0xf50f3b14, 0xea1e7629, 0xd43cec53, 0xa879d8a7, 0x50f3b14f, 0xa1e7629e, 0x43cec53d,
+    0x879d8a7a, 0x0f3b14f5, 0x1e7629ea, 0x3cec53d4, 0x79d8a7a8, 0xf3b14f50, 0xe7629ea1, 0xcec53d43,
+    0x9d8a7a87, 0x3b14f50f, 0x7629ea1e, 0xec53d43c, 0xd8a7a879, 0xb14f50f3, 0x629ea1e7, 0xc53d43ce,
+    0x8a7a879d, 0x14f50f3b, 0x29ea1e76, 0x53d43cec, 0xa7a879d8, 0x4f50f3b1, 0x9ea1e762, 0x3d43cec5,
+};
+
+static const
+uint32_t INIT_TABLE[8] = {
+    0x7380166f, 0x4914b2b9, 0x172442d7, 0xda8a0600, 0xa96f30bc, 0x163138aa, 0xe38dee4d, 0xb0fb0e4e
+};
+
+static inline
+uint32_t ROL(uint32_t X, uint32_t count)
+{
+    return (X << count) | (X >> (32 - count));
+}
+
+static inline
+uint32_t FROM_BE(const uint8_t* bytes)
+{
+    return (((uint32_t)bytes[0]) << 24) | (((uint32_t)bytes[1]) << 16) | (((uint32_t)bytes[2]) << 8) | (((uint32_t)bytes[3]));
+}
+
+static inline
+void TO_BE(uint32_t word, uint8_t* bytes)
+{
+    bytes[0] = (uint8_t)(word >> 24);
+    bytes[1] = (uint8_t)(word >> 16);
+    bytes[2] = (uint8_t)(word >> 8);
+    bytes[3] = (uint8_t)(word);
+}
+
+static inline
+uint32_t T(uint32_t i)
+{
+    return i <= 15 ? 0x79cc4519 : 0x7a879d8a;
+}
+
+static inline
+uint32_t FF(uint32_t i, uint32_t X, uint32_t Y, uint32_t Z)
+{
+    return i <= 15 ? (X ^ Y ^ Z) : ((X & Y) | (X & Z) | (Y & Z));
+}
+
+static inline
+uint32_t GG(uint32_t i, uint32_t X, uint32_t Y, uint32_t Z)
+{
+    return i <= 15 ? (X ^ Y ^ Z) : ((X & Y) | (~X & Z));
+}
+
+static inline
+uint32_t P0(uint32_t X)
+{
+    return X ^ ROL(X, 9) ^ ROL(X, 17);
+}
+
+static inline
+uint32_t P1(uint32_t X)
+{
+    return X ^ ROL(X, 15) ^ ROL(X, 23);
+}
+
+static inline
+void Expand(const uint8_t* B, uint32_t* W1, uint32_t* W2)
+{
+    uint32_t i;
+    for (i = 0; i < 16; i++)
+    {
+        W1[i] = FROM_BE(B + i * 4);
+    }
+    for (i = 16; i < 68; i++)
+    {
+        W1[i] = P1(W1[i - 16] ^ W1[i - 9] ^ ROL(W1[i - 3], 15)) ^ ROL(W1[i - 13], 7) ^ W1[i - 6];
+    }
+    for (i = 0; i < 64; i++)
+    {
+        W2[i] = W1[i] ^ W1[i + 4];
+    }
+}
+
+static inline
+void Compress(const uint32_t* W1, const uint32_t* W2, uint32_t* V)
+{
+    uint32_t i;
+    uint32_t A = V[0];
+    uint32_t B = V[1];
+    uint32_t C = V[2];
+    uint32_t D = V[3];
+    uint32_t E = V[4];
+    uint32_t F = V[5];
+    uint32_t G = V[6];
+    uint32_t H = V[7];
+    uint32_t SS1, SS2, TT1, TT2;
+
+    for (i = 0; i < 64; i++)
+    {
+        SS1 = ROL((ROL(A, 12) + E + ROL_T_TABLE[i]), 7);
+        SS2 = SS1 ^ ROL(A, 12);
+        TT1 = (FF(i, A, B, C) + D + SS2 + W2[i]);
+        TT2 = (GG(i, E, F, G) + H + SS1 + W1[i]);
+        D = C;
+        C = ROL(B, 9);
+        B = A;
+        A = TT1;
+        H = G;
+        G = ROL(F, 19);
+        F = E;
+        E = P0(TT2);
+    }
+
+    V[0] ^= A;
+    V[1] ^= B;
+    V[2] ^= C;
+    V[3] ^= D;
+    V[4] ^= E;
+    V[5] ^= F;
+    V[6] ^= G;
+    V[7] ^= H;
+}
+
+static inline
+void ExpandAndCompress(const uint8_t* B, uint32_t* V)
+{
+    uint32_t W1[68];
+    uint32_t W2[64];
+    Expand(B, W1, W2);
+    Compress(W1, W2, V);
+}
+
+void SM3_Init(SM3* self)
+{
+    uint32_t i;
+    for (i = 0; i < 8; i++)
+    {
+        self->value[i] = INIT_TABLE[i];
+    }
+    for (i = 0; i < 64; i++)
+    {
+        self->msg_buffer[i] = 0;
+    }
+    self->msg_buffer_length = 0;
+    self->msg_bitlen = 0;
+}
+
+int SM3_Update(SM3* self, const uint8_t* data, uint64_t data_len)
+{
+    uint64_t data_idx;
+    if ((data_len >> 61) || self->msg_bitlen + (data_len << 3) < self->msg_bitlen)
+    {
+        return SM3_ERR_OVERFLOW;
+    }
+
+    data_idx = 0;
+    if (self->msg_buffer_length > 0)
+    {
+        while (data_idx < data_len && self->msg_buffer_length < 64)
+        {
+            self->msg_buffer[self->msg_buffer_length++] = data[data_idx++];
+        }
+
+        if (self->msg_buffer_length >= 64)
+        {
+            ExpandAndCompress(self->msg_buffer, self->value);
+            self->msg_buffer_length = 0;
+        }
+    }
+
+    while (data_idx + 63 < data_len)
+    {
+        ExpandAndCompress(data + data_idx, self->value);
+        data_idx += 64;
+    }
+
+    while (data_idx < data_len)
+    {
+        self->msg_buffer[self->msg_buffer_length++] = data[data_idx++];
+    }
+
+    self->msg_bitlen += (data_len << 3);
+
+    return 0;
+}
+
+void SM3_Digest(SM3* self, uint8_t* digest)
+{
+    uint32_t i;
+    uint32_t value[8];
+    uint8_t msg_buffer[64];
+    uint64_t msg_buffer_length = self->msg_buffer_length;
+
+    for (i = 0; i < 8; i++)
+    {
+        value[i] = self->value[i];
+    }
+    for (i = 0; i < msg_buffer_length; i++)
+    {
+        msg_buffer[i] = self->msg_buffer[i];
+    }
+
+    msg_buffer[msg_buffer_length++] = 0x80;
+
+    if (msg_buffer_length > 56)
+    {
+        while (msg_buffer_length < 64)
+        {
+            msg_buffer[msg_buffer_length++] = 0x00;
+        }
+        ExpandAndCompress(msg_buffer, value);
+        msg_buffer_length = 0;
+    }
+
+    while (msg_buffer_length < 56)
+    {
+        msg_buffer[msg_buffer_length++] = 0x00;
+    }
+
+    msg_buffer[56] = (uint8_t)(self->msg_bitlen >> 56);
+    msg_buffer[57] = (uint8_t)(self->msg_bitlen >> 48);
+    msg_buffer[58] = (uint8_t)(self->msg_bitlen >> 40);
+    msg_buffer[59] = (uint8_t)(self->msg_bitlen >> 32);
+    msg_buffer[60] = (uint8_t)(self->msg_bitlen >> 24);
+    msg_buffer[61] = (uint8_t)(self->msg_bitlen >> 16);
+    msg_buffer[62] = (uint8_t)(self->msg_bitlen >> 8);
+    msg_buffer[63] = (uint8_t)(self->msg_bitlen);
+    ExpandAndCompress(msg_buffer, value);
+
+    for (i = 0; i < 8; i++)
+    {
+        TO_BE(value[i], digest + i * 4);
+    }
+}
```

### Comparing `gmalglib-0.1.0/sm3/sm3.h` & `gmalglib-0.1.1/sm3/sm3.h`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#ifndef GMALGLIB_SM3_H
-#define GMALGLIB_SM3_H
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#include <stdint.h>
-
-#define SM3_MAX_MSG_BITLEN      0xffffffffffffffffULL  // (1 << 64 - 1)
-
-#define SM3_ERR_OVERFLOW        -1
-
-typedef struct _SM3 {
-    uint32_t value[8];
-    uint8_t msg_buffer[64];
-    uint64_t msg_buffer_length;
-    uint64_t msg_bitlen;
-} SM3;
-
-void SM3_Init(SM3* self);
-
-int SM3_Update(SM3* self, const uint8_t* data, uint64_t data_len);
-
-void SM3_Digest(SM3* self, uint8_t* digest);
-
-#ifdef __cplusplus
-}
-#endif
-#endif // !GMALGLIB_SM3_H
+#ifndef GMALGLIB_SM3_H
+#define GMALGLIB_SM3_H
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include <stdint.h>
+
+#define SM3_MAX_MSG_BITLEN      0xffffffffffffffffULL  // (1 << 64 - 1)
+
+#define SM3_ERR_OVERFLOW        -1
+
+typedef struct _SM3 {
+    uint32_t value[8];
+    uint8_t msg_buffer[64];
+    uint64_t msg_buffer_length;
+    uint64_t msg_bitlen;
+} SM3;
+
+void SM3_Init(SM3* self);
+
+int SM3_Update(SM3* self, const uint8_t* data, uint64_t data_len);
+
+void SM3_Digest(SM3* self, uint8_t* digest);
+
+#ifdef __cplusplus
+}
+#endif
+#endif // !GMALGLIB_SM3_H
```

### Comparing `gmalglib-0.1.0/sm3/sm3module.c` & `gmalglib-0.1.1/sm3/sm3module.c`

 * *Files 17% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-#define PY_SSIZE_T_CLEAN
-
-#include <Python.h>
-#include "sm3.h"
-
-typedef struct _PySM3Object {
-    PyObject_HEAD
-    SM3 sm3;
-} PySM3Object;
-
-static int PySM3_init(PySM3Object* self, PyObject* args, PyObject* kwargs);
-static PyObject* PySM3_update(PySM3Object* self, PyObject* args, PyObject* kwargs);
-static PyObject* PySM3_digest(PySM3Object* self, PyObject* Py_UNUSED(args));
-static PyObject* PySM3_reset(PySM3Object* self, PyObject* Py_UNUSED(args));
-static PyObject* PySM3_copy(PySM3Object* self, PyObject* Py_UNUSED(args));
-
-static PyMethodDef py_methods_def_SM3[] = {
-    {"update", (PyCFunction)PySM3_update, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("Update internal state with data stream.")},
-    {"digest", (PyCFunction)PySM3_digest, METH_NOARGS, PyDoc_STR("Get digest.")},
-    {"reset", (PyCFunction)PySM3_reset, METH_NOARGS, PyDoc_STR("Reset internal state to empty.")},
-    {"copy", (PyCFunction)PySM3_copy, METH_NOARGS, PyDoc_STR("Copy state to a new object.")},
-    {NULL}
-};
-
-static PyTypeObject py_type_SM3 = {
-    .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name = "sm3.SM3",
-    .tp_doc = PyDoc_STR("SM3 Object"),
-    .tp_basicsize = sizeof(PySM3Object),
-    .tp_itemsize = 0,
-    .tp_flags = Py_TPFLAGS_DEFAULT,
-    .tp_new = PyType_GenericNew,
-    .tp_init = (initproc)PySM3_init,
-    .tp_methods = py_methods_def_SM3,
-};
-
-static PyModuleDef py_module_def_sm3 = {
-    .m_base = PyModuleDef_HEAD_INIT,
-    .m_name = "sm3",
-    .m_doc = PyDoc_STR("SM3 Algorithm Implemented in C"),
-    .m_size = 0,
-};
-
-static int PySM3_init(PySM3Object* self, PyObject* args, PyObject* kwargs)
-{
-    char* keys[] = { "data", NULL };
-    Py_buffer py_buffer_data = { 0 };
-    int ret = 0;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*:__init__", keys, &py_buffer_data))
-        return -1;
-
-    SM3_Init(&self->sm3);
-
-    ret = SM3_Update(&self->sm3, py_buffer_data.buf, py_buffer_data.len);
-    PyBuffer_Release(&py_buffer_data);
-
-    if (ret == SM3_ERR_OVERFLOW)
-    {
-        PyErr_SetString(PyExc_OverflowError, "Data too long.");
-        return -1;
-    }
-    return 0;
-}
-
-static PyObject* PySM3_update(PySM3Object* self, PyObject* args, PyObject* kwargs)
-{
-    char* keys[] = { "data", NULL };
-    Py_buffer py_buffer_data = { 0 };
-    int ret = 0;
-
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:update", keys, &py_buffer_data))
-        return NULL;
-
-    ret = SM3_Update(&self->sm3, py_buffer_data.buf, py_buffer_data.len);
-    PyBuffer_Release(&py_buffer_data);
-
-    if (ret == SM3_ERR_OVERFLOW)
-    {
-        PyErr_SetString(PyExc_OverflowError, "Data too long.");
-        return NULL;
-    }
-
-    Py_RETURN_NONE;
-}
-
-static PyObject* PySM3_digest(PySM3Object* self, PyObject* Py_UNUSED(args))
-{
-    uint8_t digest[32] = { 0 };
-    SM3_Digest(&self->sm3, digest);
-
-    return PyBytes_FromStringAndSize(digest, 32);
-}
-
-static PyObject* PySM3_reset(PySM3Object* self, PyObject* Py_UNUSED(args))
-{
-    SM3_Init(&self->sm3);
-    Py_RETURN_NONE;
-}
-
-static PyObject* PySM3_copy(PySM3Object* self, PyObject* Py_UNUSED(args))
-{
-    PySM3Object* other = PyObject_New(PySM3Object, &py_type_SM3);
-    if (!other)
-        return NULL;
-
-    other->sm3 = self->sm3;
-    return (PyObject*)other;
-}
-
-PyMODINIT_FUNC PyInit_sm3() {
-    PyObject* py_module = NULL;
-    PyObject* py_long_const_1 = NULL;
-
-    if (PyType_Ready(&py_type_SM3) < 0)
-        return NULL;
-
-    py_module = PyModule_Create(&py_module_def_sm3);
-    if (!py_module)
-        goto F0;
-
-    Py_INCREF(&py_type_SM3);
-    if (PyModule_AddObject(py_module, "SM3", (PyObject*)&py_type_SM3) < 0)
-        goto F1;
-
-    py_long_const_1 = PyLong_FromUnsignedLongLong(SM3_MAX_MSG_BITLEN);
-    if (!py_long_const_1)
-        goto F1;
-
-    if (PyModule_AddObject(py_module, "SM3_MAX_MSG_BITLEN", py_long_const_1) < 0)
-        goto F2;
-
-    return py_module;
-
-F2:
-    Py_DECREF(py_long_const_1);
-F1:
-    Py_DECREF(&py_type_SM3);
-    Py_DECREF(py_module);
-F0:    
-    return NULL;
-}
+#define PY_SSIZE_T_CLEAN
+
+#include <Python.h>
+#include "sm3.h"
+
+typedef struct _PySM3Object {
+    PyObject_HEAD
+    SM3 sm3;
+} PySM3Object;
+
+static int PySM3_init(PySM3Object* self, PyObject* args, PyObject* kwargs);
+static PyObject* PySM3_update(PySM3Object* self, PyObject* args, PyObject* kwargs);
+static PyObject* PySM3_digest(PySM3Object* self, PyObject* Py_UNUSED(args));
+static PyObject* PySM3_reset(PySM3Object* self, PyObject* Py_UNUSED(args));
+static PyObject* PySM3_copy(PySM3Object* self, PyObject* Py_UNUSED(args));
+
+static PyMethodDef py_methods_def_SM3[] = {
+    {"update", (PyCFunction)PySM3_update, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("Update internal state with data stream.")},
+    {"digest", (PyCFunction)PySM3_digest, METH_NOARGS, PyDoc_STR("Get digest.")},
+    {"reset", (PyCFunction)PySM3_reset, METH_NOARGS, PyDoc_STR("Reset internal state to empty.")},
+    {"copy", (PyCFunction)PySM3_copy, METH_NOARGS, PyDoc_STR("Copy state to a new object.")},
+    {NULL}
+};
+
+static PyTypeObject py_type_SM3 = {
+    .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_name = "sm3.SM3",
+    .tp_doc = PyDoc_STR("SM3 Object"),
+    .tp_basicsize = sizeof(PySM3Object),
+    .tp_itemsize = 0,
+    .tp_flags = Py_TPFLAGS_DEFAULT,
+    .tp_new = PyType_GenericNew,
+    .tp_init = (initproc)PySM3_init,
+    .tp_methods = py_methods_def_SM3,
+};
+
+static PyModuleDef py_module_def_sm3 = {
+    .m_base = PyModuleDef_HEAD_INIT,
+    .m_name = "sm3",
+    .m_doc = PyDoc_STR("SM3 Algorithm Implemented in C"),
+    .m_size = 0,
+};
+
+static int PySM3_init(PySM3Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "data", NULL };
+    Py_buffer py_buffer_data = { 0 };
+    int ret = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|y*:__init__", keys, &py_buffer_data))
+        return -1;
+
+    SM3_Init(&self->sm3);
+
+    ret = SM3_Update(&self->sm3, py_buffer_data.buf, py_buffer_data.len);
+    PyBuffer_Release(&py_buffer_data);
+
+    if (ret == SM3_ERR_OVERFLOW)
+    {
+        PyErr_SetString(PyExc_OverflowError, "Data too long.");
+        return -1;
+    }
+    return 0;
+}
+
+static PyObject* PySM3_update(PySM3Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "data", NULL };
+    Py_buffer py_buffer_data = { 0 };
+    int ret = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:update", keys, &py_buffer_data))
+        return NULL;
+
+    ret = SM3_Update(&self->sm3, py_buffer_data.buf, py_buffer_data.len);
+    PyBuffer_Release(&py_buffer_data);
+
+    if (ret == SM3_ERR_OVERFLOW)
+    {
+        PyErr_SetString(PyExc_OverflowError, "Data too long.");
+        return NULL;
+    }
+
+    Py_RETURN_NONE;
+}
+
+static PyObject* PySM3_digest(PySM3Object* self, PyObject* Py_UNUSED(args))
+{
+    uint8_t digest[32] = { 0 };
+    SM3_Digest(&self->sm3, digest);
+
+    return PyBytes_FromStringAndSize((char*)digest, 32);
+}
+
+static PyObject* PySM3_reset(PySM3Object* self, PyObject* Py_UNUSED(args))
+{
+    SM3_Init(&self->sm3);
+    Py_RETURN_NONE;
+}
+
+static PyObject* PySM3_copy(PySM3Object* self, PyObject* Py_UNUSED(args))
+{
+    PySM3Object* other = PyObject_New(PySM3Object, &py_type_SM3);
+    if (!other)
+        return NULL;
+
+    other->sm3 = self->sm3;
+    return (PyObject*)other;
+}
+
+PyMODINIT_FUNC PyInit_sm3() {
+    PyObject* py_module = NULL;
+    PyObject* py_long_const_1 = NULL;
+
+    if (PyType_Ready(&py_type_SM3) < 0)
+        return NULL;
+
+    py_module = PyModule_Create(&py_module_def_sm3);
+    if (!py_module)
+        goto F0;
+
+    Py_INCREF(&py_type_SM3);
+    if (PyModule_AddObject(py_module, "SM3", (PyObject*)&py_type_SM3) < 0)
+        goto F1;
+
+    py_long_const_1 = PyLong_FromUnsignedLongLong(SM3_MAX_MSG_BITLEN);
+    if (!py_long_const_1)
+        goto F1;
+
+    if (PyModule_AddObject(py_module, "SM3_MAX_MSG_BITLEN", py_long_const_1) < 0)
+        goto F2;
+
+    return py_module;
+
+F2:
+    Py_DECREF(py_long_const_1);
+F1:
+    Py_DECREF(&py_type_SM3);
+    Py_DECREF(py_module);
+F0:    
+    return NULL;
+}
```

### Comparing `gmalglib-0.1.0/src/gmalglib/sm3.pyi` & `gmalglib-0.1.1/src/gmalglib/sm3.pyi`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-SM3_MAX_MSG_BITLEN: int
-
-
-class SM3:
-    """SM3 Algorithm."""
-
-    def __init__(self, data: bytes = b"") -> None:
-        """SM3 Algorithm.
-
-        Args:
-            data: Initial data.
-        """
-
-    def update(self, data: bytes) -> None:
-        """Update state.
-
-        Args:
-            data: Bytes data.
-        """
-
-    def digest(self) -> bytes:
-        """Get digest.
-
-        Returns:
-            digest: Digest in bytes.
-        """
-
-    def reset(self) -> None:
-        """Reset internal state."""
-
-    def copy(self) -> SM3:
-        """Copy a new SM3 object with identical state.
-
-        Returns:
-            sm3_obj: A new SM3 object.
-        """
+SM3_MAX_MSG_BITLEN: int
+
+
+class SM3:
+    """SM3 Algorithm."""
+
+    def __init__(self, data: bytes = b"") -> None:
+        """SM3 Algorithm.
+
+        Args:
+            data: Initial data.
+        """
+
+    def update(self, data: bytes) -> None:
+        """Update state.
+
+        Args:
+            data: Bytes data.
+        """
+
+    def digest(self) -> bytes:
+        """Get digest.
+
+        Returns:
+            digest: Digest in bytes.
+        """
+
+    def reset(self) -> None:
+        """Reset internal state."""
+
+    def copy(self) -> SM3:
+        """Copy a new SM3 object with identical state.
+
+        Returns:
+            sm3_obj: A new SM3 object.
+        """
```

### Comparing `gmalglib-0.1.0/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.1.1/src/gmalglib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1
-Name: gmalglib
-Version: 0.1.0
-Summary: GM algorithms C extension for python.
-Author-email: ww-rm <ww-rm@qq.com>
-Project-URL: Homepage, https://github.com/ww-rm/gmalglib
-Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
-Project-URL: Documentation, https://gmalglib.readthedocs.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# gmalglib
-
-[![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
-[![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
+Metadata-Version: 2.1
+Name: gmalglib
+Version: 0.1.1
+Summary: GM algorithms C extension for python.
+Author-email: ww-rm <ww-rm@qq.com>
+Project-URL: Homepage, https://github.com/ww-rm/gmalglib
+Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
+Project-URL: Documentation, https://gmalglib.readthedocs.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security :: Cryptography
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# gmalglib
+
+[![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
+[![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
```

