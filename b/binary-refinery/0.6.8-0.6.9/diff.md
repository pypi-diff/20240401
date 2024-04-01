# Comparing `tmp/binary-refinery-0.6.8.tar.gz` & `tmp/binary-refinery-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-3ww3hmkt/binary-refinery-0.6.8.tar", last modified: Wed May 31 10:28:49 2023, max compression
+gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-1xfd2szd/binary-refinery-0.6.9.tar", last modified: Wed Jun 21 11:18:14 2023, max compression
```

## Comparing `binary-refinery-0.6.8.tar` & `binary-refinery-0.6.9.tar`

### file list

```diff
@@ -1,383 +1,386 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/binary_refinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/__init__.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/data/rich.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59251 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/argformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/deobfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/dotnet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19591 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    34707 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/mscrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/murmur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/patterns/tlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/ripemd128.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/suffixtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/acefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/batch_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/pcode2code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/thirdparty/xxhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/lib/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/
--rw-r--r--   0 runner    (1001) docker     (123)    70717 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/blockwise/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/alu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/bitrev.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/byteswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/rev.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/rotl.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/rotr.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/shl.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/shr.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/blockwise/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/blz.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/bz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/jcalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzjb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/mscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/qlz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/szdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/compression/zl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/chacha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/chaskey.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/des.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/des3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/gost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/hc128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/isaac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc2.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc4mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rc6.py
--rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rijndael.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rncrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/rsakey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/salsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/secstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/tea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/vigenere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/xtea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/cipher/xxtea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/cryptographic.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/imphash.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/murmur.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/password_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/hash/xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/CryptDeriveKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/DESDerive.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/kblob.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/crypto/keyderive/unixcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/atbash.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b32.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b58.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/b85.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/cp1252.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/esc.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/htmlesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/ps1str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/recode.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/u16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/uuenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/encoding/wshenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/a3x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xt7z.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtasar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtcab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtcpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtgz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtnsis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtpyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xttar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/archive/xtzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/deserialize_php.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/dexstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/evtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/exe/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vaddr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vmemref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vsect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vsnip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/exe/vstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/hexload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/ifps.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/ifpsstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/java/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/jvdasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/java/jvstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/msi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/office/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/doctxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/officecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/vbapc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/vbastr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xlmdeobf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xlxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/office/xtvba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pcap_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/pe/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnblob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dncfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnfields.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/pemeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/peoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/perc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/pesig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pe/pestrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/pkcs7sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/stego.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/tnetmtm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/formats/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/malware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/malware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/malware/n40.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/chop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/cull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/eat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/ef.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iffp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/iffx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/min.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/mvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/mvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/meta/xfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/autoxor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/couple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/datefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/drp.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/misc/xkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/getattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/js/tuples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/securestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/typecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/ps1/uncurly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/char.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/obfuscation/vba/vba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_7z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/carve_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/defang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/dnsdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/mimewords.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/resplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/resub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/rex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/struct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/subfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/urlguards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/xtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/pattern/xtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/iemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10672 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/ppjscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/ppjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/sinks/ppxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/refinery/units/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/ccp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/clower.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/cupper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/snip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/termfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/refinery/units/strings/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 10:28:49.000000 binary-refinery-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-31 10:28:31.000000 binary-refinery-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/binary_refinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/binary_refinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/binary_refinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/binary_refinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/binary_refinery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/binary_refinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/binary_refinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/__init__.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/data/rich.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59251 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/argformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/deobfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/dex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/lib/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/dotnet/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/dotnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/dotnet/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/dotnet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19591 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34707 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/mscrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/murmur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/lib/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/patterns/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/ripemd128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/suffixtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/lib/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/thirdparty/acefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/thirdparty/batch_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/thirdparty/pcode2code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/thirdparty/xxhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/lib/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    70717 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/blockwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/alu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/bitrev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/bitsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/byteswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/rotl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/rotr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/shl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/shr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/blockwise/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/blz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/bz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/jcalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lzf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lzg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lzjb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/mscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/qlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/szdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/compression/zl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/chacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/chaskey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/des3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/gost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/hc128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/isaac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rc4mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rc6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rijndael.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rncrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/rsakey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/salsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/secstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/tea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/vigenere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/xtea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/cipher/xxtea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/cryptographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/imphash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/murmur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/password_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/hash/xxhash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/CryptDeriveKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/DESDerive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/kblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/pbkdf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/crypto/keyderive/unixcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/atbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/b32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/b58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/b85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/cp1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/esc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/htmlesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/ps1str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/recode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/u16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/uuenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/encoding/wshenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/a3x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/formats/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xt7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtasar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtcab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtcpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtgz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtnsis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtpyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xttar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/archive/xtzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/deserialize_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/dexstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/evtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/formats/exe/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/exe/vaddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/exe/vmemref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/exe/vsect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/exe/vsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/exe/vstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/hexload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/ifps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/ifpsstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/formats/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/java/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/java/jvdasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/java/jvstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/msi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/formats/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/doctxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/officecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/vbapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/vbastr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/xlmdeobf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/xlxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/xtdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/xtone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/xtrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/office/xtvba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pcap_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/formats/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dncfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnhdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/pemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/peoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/perc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/pesig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pe/pestrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/pkcs7sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/stego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/tnetmtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/formats/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/malware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/malware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/malware/n40.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/chop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/cull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/eat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/iff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/iffp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/iffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/iffx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/mvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/mvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/meta/xfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/autoxor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/couple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/datefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/misc/xkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/obfuscation/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/js/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/js/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/js/tuples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/b64convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/securestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/typecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/ps1/uncurly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/stringreverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/obfuscation/vba/vba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve_7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve_rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/carve_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/defang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/dnsdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/mimewords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/resplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/resub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/rex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/struct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/subfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/urlguards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/xtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/pattern/xtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/iemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/ppjscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/ppjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/sinks/ppxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/refinery/units/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/ccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/cfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/clower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/cswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/cupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/snip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/termfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/refinery/units/strings/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-21 11:18:14.000000 binary-refinery-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-21 11:17:59.000000 binary-refinery-0.6.9/setup.py
```

### Comparing `binary-refinery-0.6.8/LICENSE` & `binary-refinery-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/PKG-INFO` & `binary-refinery-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.8
+Version: 0.6.9
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.8/README.md` & `binary-refinery-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/binary_refinery.egg-info/PKG-INFO` & `binary-refinery-0.6.9/binary_refinery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.8
+Version: 0.6.9
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.8/binary_refinery.egg-info/SOURCES.txt` & `binary-refinery-0.6.9/binary_refinery.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 refinery/lib/thirdparty/pcode2code.py
 refinery/lib/thirdparty/xxhash.py
 refinery/units/__init__.py
 refinery/units/blockwise/__init__.py
 refinery/units/blockwise/add.py
 refinery/units/blockwise/alu.py
 refinery/units/blockwise/bitrev.py
+refinery/units/blockwise/bitsnip.py
 refinery/units/blockwise/byteswap.py
 refinery/units/blockwise/map.py
 refinery/units/blockwise/neg.py
 refinery/units/blockwise/pack.py
 refinery/units/blockwise/rev.py
 refinery/units/blockwise/rotl.py
 refinery/units/blockwise/rotr.py
@@ -280,17 +281,19 @@
 refinery/units/obfuscation/__init__.py
 refinery/units/obfuscation/js/__init__.py
 refinery/units/obfuscation/js/arrays.py
 refinery/units/obfuscation/js/getattr.py
 refinery/units/obfuscation/js/tuples.py
 refinery/units/obfuscation/ps1/__init__.py
 refinery/units/obfuscation/ps1/all.py
+refinery/units/obfuscation/ps1/b64convert.py
 refinery/units/obfuscation/ps1/brackets.py
 refinery/units/obfuscation/ps1/cases.py
 refinery/units/obfuscation/ps1/concat.py
+refinery/units/obfuscation/ps1/encodings.py
 refinery/units/obfuscation/ps1/escape.py
 refinery/units/obfuscation/ps1/format.py
 refinery/units/obfuscation/ps1/invoke.py
 refinery/units/obfuscation/ps1/securestring.py
 refinery/units/obfuscation/ps1/stringreplace.py
 refinery/units/obfuscation/ps1/typecast.py
 refinery/units/obfuscation/ps1/uncurly.py
```

### Comparing `binary-refinery-0.6.8/binary_refinery.egg-info/entry_points.txt` & `binary-refinery-0.6.9/binary_refinery.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 b58 = refinery.units.encoding.b58:b58.run
 b64 = refinery.units.encoding.b64:b64.run
 b85 = refinery.units.encoding.b85:b85.run
 base = refinery.units.encoding.base:base.run
 bat = refinery.units.formats.bat:bat.run
 binref = refinery.explore:explorer
 bitrev = refinery.units.blockwise.bitrev:bitrev.run
+bitsnip = refinery.units.blockwise.bitsnip:bitsnip.run
 blk224 = refinery.units.crypto.hash.cryptographic:blk224.run
 blk256 = refinery.units.crypto.hash.cryptographic:blk256.run
 blk384 = refinery.units.crypto.hash.cryptographic:blk384.run
 blk512 = refinery.units.crypto.hash.cryptographic:blk512.run
 blowfish = refinery.units.crypto.cipher.blowfish:blowfish.run
 blz = refinery.units.compression.blz:blz.run
 byteswap = refinery.units.blockwise.byteswap:byteswap.run
@@ -58,17 +59,19 @@
 decompress = refinery.units.compression.decompress:decompress.run
 dedup = refinery.units.meta.dedup:dedup.run
 defang = refinery.units.pattern.defang:defang.run
 deob-js-arrays = refinery.units.obfuscation.js.arrays:deob_js_arrays.run
 deob-js-getattr = refinery.units.obfuscation.js.getattr:deob_js_getattr.run
 deob-js-tuples = refinery.units.obfuscation.js.tuples:deob_js_tuples.run
 deob-ps1 = refinery.units.obfuscation.ps1.all:deob_ps1.run
+deob-ps1-b64convert = refinery.units.obfuscation.ps1.b64convert:deob_ps1_b64convert.run
 deob-ps1-brackets = refinery.units.obfuscation.ps1.brackets:deob_ps1_brackets.run
 deob-ps1-cases = refinery.units.obfuscation.ps1.cases:deob_ps1_cases.run
 deob-ps1-concat = refinery.units.obfuscation.ps1.concat:deob_ps1_concat.run
+deob-ps1-encodings = refinery.units.obfuscation.ps1.encodings:deob_ps1_encodings.run
 deob-ps1-escape = refinery.units.obfuscation.ps1.escape:deob_ps1_escape.run
 deob-ps1-format = refinery.units.obfuscation.ps1.format:deob_ps1_format.run
 deob-ps1-invoke = refinery.units.obfuscation.ps1.invoke:deob_ps1_invoke.run
 deob-ps1-secstr = refinery.units.obfuscation.ps1.securestring:deob_ps1_secstr.run
 deob-ps1-stringreplace = refinery.units.obfuscation.ps1.stringreplace:deob_ps1_stringreplace.run
 deob-ps1-typecast = refinery.units.obfuscation.ps1.typecast:deob_ps1_typecast.run
 deob-ps1-uncurly = refinery.units.obfuscation.ps1.uncurly:deob_ps1_uncurly.run
```

### Comparing `binary-refinery-0.6.8/binary_refinery.egg-info/requires.txt` & `binary-refinery-0.6.9/binary_refinery.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -5,56 +5,56 @@
 pefile
 pycryptodomex
 pyelftools
 setuptools
 toml
 wheel
 python-magic
-pycdlib
-python-registry
+pyperclip
 decompyle3
-capstone
-pyonenote
+chardet
+olefile
 XLMMacroDeobfuscator
-xlrd2
-PyPDF2>=3.0.0
-asn1crypto
+capstone
+msoffcrypto-tool
+pyxlsb2
+LnkParse3
 openpyxl
-chardet
+PyPDF2>=3.0.0
 javaobj-py3>=0.4.0.1
-LnkParse3
-uncompyle6
-pyxlsb2
-xdis
 cabarchive
-olefile
+pyonenote
+pycdlib
 py7zr
+uncompyle6
 phpserialize
-pyperclip
 extract-msg
-msoffcrypto-tool
 Pillow
+asn1crypto
+xdis
+xlrd2
+python-registry
 
 [add]
 numpy
 
 [all]
-pypcapkit[scapy]<0.16.0
-capstone
-pyzipper
-oletools
-intervaltree
 numpy
+python-evtx
+chardet
+mitmproxy
+oletools
+jsbeautifier
+capstone
 angr
 colorama
+pyzipper
+intervaltree
+pypcapkit[scapy]<0.16.0
 unicorn
-python-evtx
-jsbeautifier
-mitmproxy
-chardet
 
 [alu]
 numpy
 
 [asm]
 angr
 
@@ -127,23 +127,23 @@
 [vbastr]
 oletools
 
 [vmemref]
 angr
 
 [vstack]
-unicorn
-intervaltree
 capstone
+intervaltree
+unicorn
 
 [xor]
 numpy
 
 [xtrtf]
 oletools
 
 [xtvba]
 oletools
 
 [xtzip]
-chardet
 pyzipper
+chardet
```

### Comparing `binary-refinery-0.6.8/refinery/__init__.pkl` & `binary-refinery-0.6.9/refinery/__init__.pkl`

 * *Files 3% similar despite different names*

```diff
@@ -3,929 +3,943 @@
 00000020: 6974 732e 626c 6f63 6b77 6973 652e 6164  its.blockwise.ad
 00000030: 6471 0258 0300 0000 616c 7571 0358 1c00  dq.X....aluq.X..
 00000040: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
 00000050: 2e62 6c6f 636b 7769 7365 2e61 6c75 7104  .blockwise.aluq.
 00000060: 5806 0000 0062 6974 7265 7671 0558 1f00  X....bitrevq.X..
 00000070: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
 00000080: 2e62 6c6f 636b 7769 7365 2e62 6974 7265  .blockwise.bitre
-00000090: 7671 0658 0800 0000 6279 7465 7377 6170  vq.X....byteswap
-000000a0: 7107 5821 0000 0072 6566 696e 6572 792e  q.X!...refinery.
-000000b0: 756e 6974 732e 626c 6f63 6b77 6973 652e  units.blockwise.
-000000c0: 6279 7465 7377 6170 7108 5803 0000 006d  byteswapq.X....m
-000000d0: 6170 7109 581c 0000 0072 6566 696e 6572  apq.X....refiner
-000000e0: 792e 756e 6974 732e 626c 6f63 6b77 6973  y.units.blockwis
-000000f0: 652e 6d61 7071 0a58 0300 0000 6e65 6771  e.mapq.X....negq
-00000100: 0b58 1c00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00000110: 6e69 7473 2e62 6c6f 636b 7769 7365 2e6e  nits.blockwise.n
-00000120: 6567 710c 5804 0000 0070 6163 6b71 0d58  egq.X....packq.X
-00000130: 1d00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00000140: 7473 2e62 6c6f 636b 7769 7365 2e70 6163  ts.blockwise.pac
-00000150: 6b71 0e58 0300 0000 7265 7671 0f58 1c00  kq.X....revq.X..
-00000160: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000170: 2e62 6c6f 636b 7769 7365 2e72 6576 7110  .blockwise.revq.
-00000180: 5804 0000 0072 6f74 6c71 1158 1d00 0000  X....rotlq.X....
-00000190: 7265 6669 6e65 7279 2e75 6e69 7473 2e62  refinery.units.b
-000001a0: 6c6f 636b 7769 7365 2e72 6f74 6c71 1258  lockwise.rotlq.X
-000001b0: 0400 0000 726f 7472 7113 581d 0000 0072  ....rotrq.X....r
-000001c0: 6566 696e 6572 792e 756e 6974 732e 626c  efinery.units.bl
-000001d0: 6f63 6b77 6973 652e 726f 7472 7114 5803  ockwise.rotrq.X.
-000001e0: 0000 0073 686c 7115 581c 0000 0072 6566  ...shlq.X....ref
-000001f0: 696e 6572 792e 756e 6974 732e 626c 6f63  inery.units.bloc
-00000200: 6b77 6973 652e 7368 6c71 1658 0300 0000  kwise.shlq.X....
-00000210: 7368 7271 1758 1c00 0000 7265 6669 6e65  shrq.X....refine
-00000220: 7279 2e75 6e69 7473 2e62 6c6f 636b 7769  ry.units.blockwi
-00000230: 7365 2e73 6872 7118 5803 0000 0073 7562  se.shrq.X....sub
-00000240: 7119 581c 0000 0072 6566 696e 6572 792e  q.X....refinery.
-00000250: 756e 6974 732e 626c 6f63 6b77 6973 652e  units.blockwise.
-00000260: 7375 6271 1a58 0900 0000 7465 726d 696e  subq.X....termin
-00000270: 6174 6571 1b58 2200 0000 7265 6669 6e65  ateq.X"...refine
-00000280: 7279 2e75 6e69 7473 2e62 6c6f 636b 7769  ry.units.blockwi
-00000290: 7365 2e74 6572 6d69 6e61 7465 711c 5803  se.terminateq.X.
-000002a0: 0000 0078 6f72 711d 581c 0000 0072 6566  ...xorq.X....ref
-000002b0: 696e 6572 792e 756e 6974 732e 626c 6f63  inery.units.bloc
-000002c0: 6b77 6973 652e 786f 7271 1e58 0500 0000  kwise.xorq.X....
-000002d0: 6170 6c69 6271 1f58 1d00 0000 7265 6669  aplibq.X....refi
-000002e0: 6e65 7279 2e75 6e69 7473 2e63 6f6d 7072  nery.units.compr
-000002f0: 6573 7369 6f6e 2e61 7071 2058 0300 0000  ession.apq X....
-00000300: 626c 7a71 2158 1e00 0000 7265 6669 6e65  blzq!X....refine
-00000310: 7279 2e75 6e69 7473 2e63 6f6d 7072 6573  ry.units.compres
-00000320: 7369 6f6e 2e62 6c7a 7122 5803 0000 0062  sion.blzq"X....b
-00000330: 7a32 7123 581e 0000 0072 6566 696e 6572  z2q#X....refiner
-00000340: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
-00000350: 696f 6e2e 627a 3271 2458 0a00 0000 6465  ion.bz2q$X....de
-00000360: 636f 6d70 7265 7373 7125 5825 0000 0072  compressq%X%...r
-00000370: 6566 696e 6572 792e 756e 6974 732e 636f  efinery.units.co
-00000380: 6d70 7265 7373 696f 6e2e 6465 636f 6d70  mpression.decomp
-00000390: 7265 7373 7126 5805 0000 006a 6361 6c67  ressq&X....jcalg
-000003a0: 7127 5820 0000 0072 6566 696e 6572 792e  q'X ...refinery.
-000003b0: 756e 6974 732e 636f 6d70 7265 7373 696f  units.compressio
-000003c0: 6e2e 6a63 616c 6771 2858 0400 0000 6c7a  n.jcalgq(X....lz
-000003d0: 6d61 7129 581d 0000 0072 6566 696e 6572  maq)X....refiner
-000003e0: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
-000003f0: 696f 6e2e 6c7a 712a 5803 0000 006c 7a34  ion.lzq*X....lz4
-00000400: 712b 581e 0000 0072 6566 696e 6572 792e  q+X....refinery.
-00000410: 756e 6974 732e 636f 6d70 7265 7373 696f  units.compressio
-00000420: 6e2e 6c7a 3471 2c58 0300 0000 6c7a 6671  n.lz4q,X....lzfq
-00000430: 2d58 1e00 0000 7265 6669 6e65 7279 2e75  -X....refinery.u
-00000440: 6e69 7473 2e63 6f6d 7072 6573 7369 6f6e  nits.compression
-00000450: 2e6c 7a66 712e 5803 0000 006c 7a67 712f  .lzfq.X....lzgq/
-00000460: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00000470: 6974 732e 636f 6d70 7265 7373 696f 6e2e  its.compression.
-00000480: 6c7a 6771 3058 0400 0000 6c7a 6970 7131  lzgq0X....lzipq1
-00000490: 581f 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000004a0: 6974 732e 636f 6d70 7265 7373 696f 6e2e  its.compression.
-000004b0: 6c7a 6970 7132 5804 0000 006c 7a6a 6271  lzipq2X....lzjbq
-000004c0: 3358 1f00 0000 7265 6669 6e65 7279 2e75  3X....refinery.u
-000004d0: 6e69 7473 2e63 6f6d 7072 6573 7369 6f6e  nits.compression
-000004e0: 2e6c 7a6a 6271 3458 0500 0000 6c7a 6e74  .lzjbq4X....lznt
-000004f0: 3171 3558 2000 0000 7265 6669 6e65 7279  1q5X ...refinery
-00000500: 2e75 6e69 7473 2e63 6f6d 7072 6573 7369  .units.compressi
-00000510: 6f6e 2e6c 7a6e 7431 7136 5803 0000 006c  on.lznt1q6X....l
-00000520: 7a6f 7137 581e 0000 0072 6566 696e 6572  zoq7X....refiner
-00000530: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
-00000540: 696f 6e2e 6c7a 6f71 3858 0400 0000 6d73  ion.lzoq8X....ms
-00000550: 6366 7139 581f 0000 0072 6566 696e 6572  cfq9X....refiner
-00000560: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
-00000570: 696f 6e2e 6d73 6366 713a 5803 0000 0071  ion.mscfq:X....q
-00000580: 6c7a 713b 581e 0000 0072 6566 696e 6572  lzq;X....refiner
-00000590: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
-000005a0: 696f 6e2e 716c 7a71 3c58 0400 0000 737a  ion.qlzq<X....sz
-000005b0: 6464 713d 581f 0000 0072 6566 696e 6572  ddq=X....refiner
-000005c0: 792e 756e 6974 732e 636f 6d70 7265 7373  y.units.compress
-000005d0: 696f 6e2e 737a 6464 713e 5802 0000 007a  ion.szddq>X....z
-000005e0: 6c71 3f58 1d00 0000 7265 6669 6e65 7279  lq?X....refinery
-000005f0: 2e75 6e69 7473 2e63 6f6d 7072 6573 7369  .units.compressi
-00000600: 6f6e 2e7a 6c71 4058 0300 0000 6165 7371  on.zlq@X....aesq
-00000610: 4158 2000 0000 7265 6669 6e65 7279 2e75  AX ...refinery.u
-00000620: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
-00000630: 6572 2e61 6573 7142 5808 0000 0062 6c6f  er.aesqBX....blo
-00000640: 7766 6973 6871 4358 2500 0000 7265 6669  wfishqCX%...refi
-00000650: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
-00000660: 6f2e 6369 7068 6572 2e62 6c6f 7766 6973  o.cipher.blowfis
-00000670: 6871 4458 0800 0000 6361 6d65 6c6c 6961  hqDX....camellia
-00000680: 7145 5825 0000 0072 6566 696e 6572 792e  qEX%...refinery.
-00000690: 756e 6974 732e 6372 7970 746f 2e63 6970  units.crypto.cip
-000006a0: 6865 722e 6361 6d65 6c6c 6961 7146 5804  her.camelliaqFX.
-000006b0: 0000 0063 6173 7471 4758 2100 0000 7265  ...castqGX!...re
-000006c0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-000006d0: 7074 6f2e 6369 7068 6572 2e63 6173 7471  pto.cipher.castq
-000006e0: 4858 0600 0000 6368 6163 6861 7149 5823  HX....chachaqIX#
+00000090: 7671 0658 0700 0000 6269 7473 6e69 7071  vq.X....bitsnipq
+000000a0: 0758 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
+000000b0: 6e69 7473 2e62 6c6f 636b 7769 7365 2e62  nits.blockwise.b
+000000c0: 6974 736e 6970 7108 5808 0000 0062 7974  itsnipq.X....byt
+000000d0: 6573 7761 7071 0958 2100 0000 7265 6669  eswapq.X!...refi
+000000e0: 6e65 7279 2e75 6e69 7473 2e62 6c6f 636b  nery.units.block
+000000f0: 7769 7365 2e62 7974 6573 7761 7071 0a58  wise.byteswapq.X
+00000100: 0300 0000 6d61 7071 0b58 1c00 0000 7265  ....mapq.X....re
+00000110: 6669 6e65 7279 2e75 6e69 7473 2e62 6c6f  finery.units.blo
+00000120: 636b 7769 7365 2e6d 6170 710c 5803 0000  ckwise.mapq.X...
+00000130: 006e 6567 710d 581c 0000 0072 6566 696e  .negq.X....refin
+00000140: 6572 792e 756e 6974 732e 626c 6f63 6b77  ery.units.blockw
+00000150: 6973 652e 6e65 6771 0e58 0400 0000 7061  ise.negq.X....pa
+00000160: 636b 710f 581d 0000 0072 6566 696e 6572  ckq.X....refiner
+00000170: 792e 756e 6974 732e 626c 6f63 6b77 6973  y.units.blockwis
+00000180: 652e 7061 636b 7110 5803 0000 0072 6576  e.packq.X....rev
+00000190: 7111 581c 0000 0072 6566 696e 6572 792e  q.X....refinery.
+000001a0: 756e 6974 732e 626c 6f63 6b77 6973 652e  units.blockwise.
+000001b0: 7265 7671 1258 0400 0000 726f 746c 7113  revq.X....rotlq.
+000001c0: 581d 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000001d0: 6974 732e 626c 6f63 6b77 6973 652e 726f  its.blockwise.ro
+000001e0: 746c 7114 5804 0000 0072 6f74 7271 1558  tlq.X....rotrq.X
+000001f0: 1d00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00000200: 7473 2e62 6c6f 636b 7769 7365 2e72 6f74  ts.blockwise.rot
+00000210: 7271 1658 0300 0000 7368 6c71 1758 1c00  rq.X....shlq.X..
+00000220: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00000230: 2e62 6c6f 636b 7769 7365 2e73 686c 7118  .blockwise.shlq.
+00000240: 5803 0000 0073 6872 7119 581c 0000 0072  X....shrq.X....r
+00000250: 6566 696e 6572 792e 756e 6974 732e 626c  efinery.units.bl
+00000260: 6f63 6b77 6973 652e 7368 7271 1a58 0300  ockwise.shrq.X..
+00000270: 0000 7375 6271 1b58 1c00 0000 7265 6669  ..subq.X....refi
+00000280: 6e65 7279 2e75 6e69 7473 2e62 6c6f 636b  nery.units.block
+00000290: 7769 7365 2e73 7562 711c 5809 0000 0074  wise.subq.X....t
+000002a0: 6572 6d69 6e61 7465 711d 5822 0000 0072  erminateq.X"...r
+000002b0: 6566 696e 6572 792e 756e 6974 732e 626c  efinery.units.bl
+000002c0: 6f63 6b77 6973 652e 7465 726d 696e 6174  ockwise.terminat
+000002d0: 6571 1e58 0300 0000 786f 7271 1f58 1c00  eq.X....xorq.X..
+000002e0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000002f0: 2e62 6c6f 636b 7769 7365 2e78 6f72 7120  .blockwise.xorq 
+00000300: 5805 0000 0061 706c 6962 7121 581d 0000  X....aplibq!X...
+00000310: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00000320: 636f 6d70 7265 7373 696f 6e2e 6170 7122  compression.apq"
+00000330: 5803 0000 0062 6c7a 7123 581e 0000 0072  X....blzq#X....r
+00000340: 6566 696e 6572 792e 756e 6974 732e 636f  efinery.units.co
+00000350: 6d70 7265 7373 696f 6e2e 626c 7a71 2458  mpression.blzq$X
+00000360: 0300 0000 627a 3271 2558 1e00 0000 7265  ....bz2q%X....re
+00000370: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
+00000380: 7072 6573 7369 6f6e 2e62 7a32 7126 580a  pression.bz2q&X.
+00000390: 0000 0064 6563 6f6d 7072 6573 7371 2758  ...decompressq'X
+000003a0: 2500 0000 7265 6669 6e65 7279 2e75 6e69  %...refinery.uni
+000003b0: 7473 2e63 6f6d 7072 6573 7369 6f6e 2e64  ts.compression.d
+000003c0: 6563 6f6d 7072 6573 7371 2858 0500 0000  ecompressq(X....
+000003d0: 6a63 616c 6771 2958 2000 0000 7265 6669  jcalgq)X ...refi
+000003e0: 6e65 7279 2e75 6e69 7473 2e63 6f6d 7072  nery.units.compr
+000003f0: 6573 7369 6f6e 2e6a 6361 6c67 712a 5804  ession.jcalgq*X.
+00000400: 0000 006c 7a6d 6171 2b58 1d00 0000 7265  ...lzmaq+X....re
+00000410: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
+00000420: 7072 6573 7369 6f6e 2e6c 7a71 2c58 0300  pression.lzq,X..
+00000430: 0000 6c7a 3471 2d58 1e00 0000 7265 6669  ..lz4q-X....refi
+00000440: 6e65 7279 2e75 6e69 7473 2e63 6f6d 7072  nery.units.compr
+00000450: 6573 7369 6f6e 2e6c 7a34 712e 5803 0000  ession.lz4q.X...
+00000460: 006c 7a66 712f 581e 0000 0072 6566 696e  .lzfq/X....refin
+00000470: 6572 792e 756e 6974 732e 636f 6d70 7265  ery.units.compre
+00000480: 7373 696f 6e2e 6c7a 6671 3058 0300 0000  ssion.lzfq0X....
+00000490: 6c7a 6771 3158 1e00 0000 7265 6669 6e65  lzgq1X....refine
+000004a0: 7279 2e75 6e69 7473 2e63 6f6d 7072 6573  ry.units.compres
+000004b0: 7369 6f6e 2e6c 7a67 7132 5804 0000 006c  sion.lzgq2X....l
+000004c0: 7a69 7071 3358 1f00 0000 7265 6669 6e65  zipq3X....refine
+000004d0: 7279 2e75 6e69 7473 2e63 6f6d 7072 6573  ry.units.compres
+000004e0: 7369 6f6e 2e6c 7a69 7071 3458 0400 0000  sion.lzipq4X....
+000004f0: 6c7a 6a62 7135 581f 0000 0072 6566 696e  lzjbq5X....refin
+00000500: 6572 792e 756e 6974 732e 636f 6d70 7265  ery.units.compre
+00000510: 7373 696f 6e2e 6c7a 6a62 7136 5805 0000  ssion.lzjbq6X...
+00000520: 006c 7a6e 7431 7137 5820 0000 0072 6566  .lznt1q7X ...ref
+00000530: 696e 6572 792e 756e 6974 732e 636f 6d70  inery.units.comp
+00000540: 7265 7373 696f 6e2e 6c7a 6e74 3171 3858  ression.lznt1q8X
+00000550: 0300 0000 6c7a 6f71 3958 1e00 0000 7265  ....lzoq9X....re
+00000560: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
+00000570: 7072 6573 7369 6f6e 2e6c 7a6f 713a 5804  pression.lzoq:X.
+00000580: 0000 006d 7363 6671 3b58 1f00 0000 7265  ...mscfq;X....re
+00000590: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
+000005a0: 7072 6573 7369 6f6e 2e6d 7363 6671 3c58  pression.mscfq<X
+000005b0: 0300 0000 716c 7a71 3d58 1e00 0000 7265  ....qlzq=X....re
+000005c0: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
+000005d0: 7072 6573 7369 6f6e 2e71 6c7a 713e 5804  pression.qlzq>X.
+000005e0: 0000 0073 7a64 6471 3f58 1f00 0000 7265  ...szddq?X....re
+000005f0: 6669 6e65 7279 2e75 6e69 7473 2e63 6f6d  finery.units.com
+00000600: 7072 6573 7369 6f6e 2e73 7a64 6471 4058  pression.szddq@X
+00000610: 0200 0000 7a6c 7141 581d 0000 0072 6566  ....zlqAX....ref
+00000620: 696e 6572 792e 756e 6974 732e 636f 6d70  inery.units.comp
+00000630: 7265 7373 696f 6e2e 7a6c 7142 5803 0000  ression.zlqBX...
+00000640: 0061 6573 7143 5820 0000 0072 6566 696e  .aesqCX ...refin
+00000650: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00000660: 2e63 6970 6865 722e 6165 7371 4458 0800  .cipher.aesqDX..
+00000670: 0000 626c 6f77 6669 7368 7145 5825 0000  ..blowfishqEX%..
+00000680: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00000690: 6372 7970 746f 2e63 6970 6865 722e 626c  crypto.cipher.bl
+000006a0: 6f77 6669 7368 7146 5808 0000 0063 616d  owfishqFX....cam
+000006b0: 656c 6c69 6171 4758 2500 0000 7265 6669  elliaqGX%...refi
+000006c0: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+000006d0: 6f2e 6369 7068 6572 2e63 616d 656c 6c69  o.cipher.camelli
+000006e0: 6171 4858 0400 0000 6361 7374 7149 5821  aqHX....castqIX!
 000006f0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
 00000700: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000710: 6368 6163 6861 714a 5808 0000 0063 6861  chachaqJX....cha
-00000720: 6368 6132 3071 4b68 4a58 0700 0000 6368  cha20qKhJX....ch
-00000730: 6173 6b65 7971 4c58 2400 0000 7265 6669  askeyqLX$...refi
-00000740: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
-00000750: 6f2e 6369 7068 6572 2e63 6861 736b 6579  o.cipher.chaskey
-00000760: 714d 5803 0000 0064 6573 714e 5820 0000  qMX....desqNX ..
+00000710: 6361 7374 714a 5806 0000 0063 6861 6368  castqJX....chach
+00000720: 6171 4b58 2300 0000 7265 6669 6e65 7279  aqKX#...refinery
+00000730: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
+00000740: 7068 6572 2e63 6861 6368 6171 4c58 0800  pher.chachaqLX..
+00000750: 0000 6368 6163 6861 3230 714d 684c 5807  ..chacha20qMhLX.
+00000760: 0000 0063 6861 736b 6579 714e 5824 0000  ...chaskeyqNX$..
 00000770: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000780: 6372 7970 746f 2e63 6970 6865 722e 6465  crypto.cipher.de
-00000790: 7371 4f58 0400 0000 6465 7333 7150 5821  sqOX....des3qPX!
-000007a0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000007b0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-000007c0: 6465 7333 7151 5804 0000 0067 6f73 7471  des3qQX....gostq
-000007d0: 5258 2100 0000 7265 6669 6e65 7279 2e75  RX!...refinery.u
-000007e0: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
-000007f0: 6572 2e67 6f73 7471 5358 0500 0000 6863  er.gostqSX....hc
-00000800: 3132 3871 5458 2200 0000 7265 6669 6e65  128qTX"...refine
-00000810: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000820: 6369 7068 6572 2e68 6331 3238 7155 5805  cipher.hc128qUX.
-00000830: 0000 0069 7361 6163 7156 5822 0000 0072  ...isaacqVX"...r
+00000780: 6372 7970 746f 2e63 6970 6865 722e 6368  crypto.cipher.ch
+00000790: 6173 6b65 7971 4f58 0300 0000 6465 7371  askeyqOX....desq
+000007a0: 5058 2000 0000 7265 6669 6e65 7279 2e75  PX ...refinery.u
+000007b0: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
+000007c0: 6572 2e64 6573 7151 5804 0000 0064 6573  er.desqQX....des
+000007d0: 3371 5258 2100 0000 7265 6669 6e65 7279  3qRX!...refinery
+000007e0: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
+000007f0: 7068 6572 2e64 6573 3371 5358 0400 0000  pher.des3qSX....
+00000800: 676f 7374 7154 5821 0000 0072 6566 696e  gostqTX!...refin
+00000810: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00000820: 2e63 6970 6865 722e 676f 7374 7155 5805  .cipher.gostqUX.
+00000830: 0000 0068 6331 3238 7156 5822 0000 0072  ...hc128qVX"...r
 00000840: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
-00000850: 7970 746f 2e63 6970 6865 722e 6973 6161  ypto.cipher.isaa
-00000860: 6371 5758 0600 0000 7261 6262 6974 7158  cqWX....rabbitqX
-00000870: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
-00000880: 6974 732e 6372 7970 746f 2e63 6970 6865  its.crypto.ciphe
-00000890: 722e 7261 6262 6974 7159 5803 0000 0072  r.rabbitqYX....r
-000008a0: 6332 715a 5820 0000 0072 6566 696e 6572  c2qZX ...refiner
-000008b0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-000008c0: 6970 6865 722e 7263 3271 5b58 0300 0000  ipher.rc2q[X....
-000008d0: 7263 3471 5c58 2000 0000 7265 6669 6e65  rc4q\X ...refine
-000008e0: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-000008f0: 6369 7068 6572 2e72 6334 715d 5806 0000  cipher.rc4q]X...
-00000900: 0072 6334 6d6f 6471 5e58 2300 0000 7265  .rc4modq^X#...re
-00000910: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-00000920: 7074 6f2e 6369 7068 6572 2e72 6334 6d6f  pto.cipher.rc4mo
-00000930: 6471 5f58 0300 0000 7263 3571 6058 2000  dq_X....rc5q`X .
-00000940: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000950: 2e63 7279 7074 6f2e 6369 7068 6572 2e72  .crypto.cipher.r
-00000960: 6335 7161 5803 0000 0072 6336 7162 5820  c5qaX....rc6qbX 
-00000970: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00000980: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000990: 7263 3671 6358 0800 0000 7269 6a6e 6461  rc6qcX....rijnda
-000009a0: 656c 7164 5825 0000 0072 6566 696e 6572  elqdX%...refiner
-000009b0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-000009c0: 6970 6865 722e 7269 6a6e 6461 656c 7165  ipher.rijndaelqe
-000009d0: 5807 0000 0072 6e63 7279 7074 7166 5824  X....rncryptqfX$
-000009e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000009f0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000a00: 726e 6372 7970 7471 6758 0300 0000 726f  rncryptqgX....ro
-00000a10: 7471 6858 2000 0000 7265 6669 6e65 7279  tqhX ...refinery
+00000850: 7970 746f 2e63 6970 6865 722e 6863 3132  ypto.cipher.hc12
+00000860: 3871 5758 0500 0000 6973 6161 6371 5858  8qWX....isaacqXX
+00000870: 2200 0000 7265 6669 6e65 7279 2e75 6e69  "...refinery.uni
+00000880: 7473 2e63 7279 7074 6f2e 6369 7068 6572  ts.crypto.cipher
+00000890: 2e69 7361 6163 7159 5806 0000 0072 6162  .isaacqYX....rab
+000008a0: 6269 7471 5a58 2300 0000 7265 6669 6e65  bitqZX#...refine
+000008b0: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+000008c0: 6369 7068 6572 2e72 6162 6269 7471 5b58  cipher.rabbitq[X
+000008d0: 0300 0000 7263 3271 5c58 2000 0000 7265  ....rc2q\X ...re
+000008e0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+000008f0: 7074 6f2e 6369 7068 6572 2e72 6332 715d  pto.cipher.rc2q]
+00000900: 5803 0000 0072 6334 715e 5820 0000 0072  X....rc4q^X ...r
+00000910: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
+00000920: 7970 746f 2e63 6970 6865 722e 7263 3471  ypto.cipher.rc4q
+00000930: 5f58 0600 0000 7263 346d 6f64 7160 5823  _X....rc4modq`X#
+00000940: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00000950: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
+00000960: 7263 346d 6f64 7161 5803 0000 0072 6335  rc4modqaX....rc5
+00000970: 7162 5820 0000 0072 6566 696e 6572 792e  qbX ...refinery.
+00000980: 756e 6974 732e 6372 7970 746f 2e63 6970  units.crypto.cip
+00000990: 6865 722e 7263 3571 6358 0300 0000 7263  her.rc5qcX....rc
+000009a0: 3671 6458 2000 0000 7265 6669 6e65 7279  6qdX ...refinery
+000009b0: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
+000009c0: 7068 6572 2e72 6336 7165 5808 0000 0072  pher.rc6qeX....r
+000009d0: 696a 6e64 6165 6c71 6658 2500 0000 7265  ijndaelqfX%...re
+000009e0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+000009f0: 7074 6f2e 6369 7068 6572 2e72 696a 6e64  pto.cipher.rijnd
+00000a00: 6165 6c71 6758 0700 0000 726e 6372 7970  aelqgX....rncryp
+00000a10: 7471 6858 2400 0000 7265 6669 6e65 7279  tqhX$...refinery
 00000a20: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
-00000a30: 7068 6572 2e72 6f74 7169 5803 0000 0072  pher.rotqiX....r
-00000a40: 7361 716a 5820 0000 0072 6566 696e 6572  saqjX ...refiner
-00000a50: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-00000a60: 6970 6865 722e 7273 6171 6b58 0600 0000  ipher.rsaqkX....
-00000a70: 7273 616b 6579 716c 5823 0000 0072 6566  rsakeyqlX#...ref
-00000a80: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
-00000a90: 746f 2e63 6970 6865 722e 7273 616b 6579  to.cipher.rsakey
-00000aa0: 716d 5805 0000 0073 616c 7361 716e 5822  qmX....salsaqnX"
-00000ab0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00000ac0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000ad0: 7361 6c73 6171 6f58 0700 0000 7361 6c73  salsaqoX....sals
-00000ae0: 6132 3071 7068 6f58 0400 0000 7365 616c  a20qphoX....seal
-00000af0: 7171 5821 0000 0072 6566 696e 6572 792e  qqX!...refinery.
-00000b00: 756e 6974 732e 6372 7970 746f 2e63 6970  units.crypto.cip
-00000b10: 6865 722e 7365 616c 7172 5806 0000 0073  her.sealqrX....s
-00000b20: 6563 7374 7271 7358 2300 0000 7265 6669  ecstrqsX#...refi
+00000a30: 7068 6572 2e72 6e63 7279 7074 7169 5803  pher.rncryptqiX.
+00000a40: 0000 0072 6f74 716a 5820 0000 0072 6566  ...rotqjX ...ref
+00000a50: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
+00000a60: 746f 2e63 6970 6865 722e 726f 7471 6b58  to.cipher.rotqkX
+00000a70: 0300 0000 7273 6171 6c58 2000 0000 7265  ....rsaqlX ...re
+00000a80: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000a90: 7074 6f2e 6369 7068 6572 2e72 7361 716d  pto.cipher.rsaqm
+00000aa0: 5806 0000 0072 7361 6b65 7971 6e58 2300  X....rsakeyqnX#.
+00000ab0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00000ac0: 2e63 7279 7074 6f2e 6369 7068 6572 2e72  .crypto.cipher.r
+00000ad0: 7361 6b65 7971 6f58 0500 0000 7361 6c73  sakeyqoX....sals
+00000ae0: 6171 7058 2200 0000 7265 6669 6e65 7279  aqpX"...refinery
+00000af0: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
+00000b00: 7068 6572 2e73 616c 7361 7171 5807 0000  pher.salsaqqX...
+00000b10: 0073 616c 7361 3230 7172 6871 5804 0000  .salsa20qrhqX...
+00000b20: 0073 6561 6c71 7358 2100 0000 7265 6669  .sealqsX!...refi
 00000b30: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
-00000b40: 6f2e 6369 7068 6572 2e73 6563 7374 7271  o.cipher.secstrq
-00000b50: 7458 0700 0000 7365 7270 656e 7471 7558  tX....serpentquX
-00000b60: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
-00000b70: 7473 2e63 7279 7074 6f2e 6369 7068 6572  ts.crypto.cipher
-00000b80: 2e73 6572 7065 6e74 7176 5803 0000 0074  .serpentqvX....t
-00000b90: 6561 7177 5820 0000 0072 6566 696e 6572  eaqwX ...refiner
+00000b40: 6f2e 6369 7068 6572 2e73 6561 6c71 7458  o.cipher.sealqtX
+00000b50: 0600 0000 7365 6373 7472 7175 5823 0000  ....secstrquX#..
+00000b60: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00000b70: 6372 7970 746f 2e63 6970 6865 722e 7365  crypto.cipher.se
+00000b80: 6373 7472 7176 5807 0000 0073 6572 7065  cstrqvX....serpe
+00000b90: 6e74 7177 5824 0000 0072 6566 696e 6572  ntqwX$...refiner
 00000ba0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-00000bb0: 6970 6865 722e 7465 6171 7858 0800 0000  ipher.teaqxX....
-00000bc0: 7669 6765 6e65 7265 7179 5825 0000 0072  vigenereqyX%...r
-00000bd0: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
-00000be0: 7970 746f 2e63 6970 6865 722e 7669 6765  ypto.cipher.vige
-00000bf0: 6e65 7265 717a 5804 0000 0078 7465 6171  nereqzX....xteaq
-00000c00: 7b58 2100 0000 7265 6669 6e65 7279 2e75  {X!...refinery.u
-00000c10: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
-00000c20: 6572 2e78 7465 6171 7c58 0500 0000 7878  er.xteaq|X....xx
-00000c30: 7465 6171 7d58 2200 0000 7265 6669 6e65  teaq}X"...refine
-00000c40: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000c50: 6369 7068 6572 2e78 7874 6561 717e 5807  cipher.xxteaq~X.
-00000c60: 0000 0061 646c 6572 3332 717f 5824 0000  ...adler32q.X$..
-00000c70: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000c80: 6372 7970 746f 2e68 6173 682e 6368 6563  crypto.hash.chec
-00000c90: 6b73 756d 7371 8058 0500 0000 6372 6333  ksumsq.X....crc3
-00000ca0: 3271 8168 8058 0600 0000 626c 6b32 3234  2q.h.X....blk224
-00000cb0: 7182 5828 0000 0072 6566 696e 6572 792e  q.X(...refinery.
-00000cc0: 756e 6974 732e 6372 7970 746f 2e68 6173  units.crypto.has
-00000cd0: 682e 6372 7970 746f 6772 6170 6869 6371  h.cryptographicq
-00000ce0: 8358 0600 0000 626c 6b32 3536 7184 6883  .X....blk256q.h.
-00000cf0: 5806 0000 0062 6c6b 3338 3471 8568 8358  X....blk384q.h.X
-00000d00: 0600 0000 626c 6b35 3132 7186 6883 5803  ....blk512q.h.X.
-00000d10: 0000 006d 6432 7187 6883 5803 0000 006d  ...md2q.h.X....m
-00000d20: 6434 7188 6883 5803 0000 006d 6435 7189  d4q.h.X....md5q.
-00000d30: 6883 5809 0000 0072 6970 656d 6431 3238  h.X....ripemd128
-00000d40: 718a 6883 5809 0000 0072 6970 656d 6431  q.h.X....ripemd1
-00000d50: 3630 718b 6883 5804 0000 0073 6861 3171  60q.h.X....sha1q
-00000d60: 8c68 8358 0600 0000 7368 6132 3234 718d  .h.X....sha224q.
-00000d70: 6883 5806 0000 0073 6861 3235 3671 8e68  h.X....sha256q.h
-00000d80: 8358 0600 0000 7368 6133 3834 718f 6883  .X....sha384q.h.
-00000d90: 5806 0000 0073 6861 3531 3271 9068 8358  X....sha512q.h.X
-00000da0: 0700 0000 696d 7068 6173 6871 9158 2200  ....imphashq.X".
-00000db0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000dc0: 2e63 7279 7074 6f2e 6861 7368 2e69 6d70  .crypto.hash.imp
-00000dd0: 6861 7368 7192 5809 0000 006d 6d68 3132  hashq.X....mmh12
-00000de0: 3878 3332 7193 5821 0000 0072 6566 696e  8x32q.X!...refin
-00000df0: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
-00000e00: 2e68 6173 682e 6d75 726d 7572 7194 5809  .hash.murmurq.X.
-00000e10: 0000 006d 6d68 3132 3878 3634 7195 6894  ...mmh128x64q.h.
-00000e20: 5805 0000 006d 6d68 3332 7196 6894 5804  X....mmh32q.h.X.
-00000e30: 0000 006e 746c 6d71 9758 2a00 0000 7265  ...ntlmq.X*...re
-00000e40: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-00000e50: 7074 6f2e 6861 7368 2e70 6173 7377 6f72  pto.hash.passwor
-00000e60: 645f 6861 7368 6573 7198 5803 0000 0078  d_hashesq.X....x
-00000e70: 7868 7199 5821 0000 0072 6566 696e 6572  xhq.X!...refiner
-00000e80: 792e 756e 6974 732e 6372 7970 746f 2e68  y.units.crypto.h
-00000e90: 6173 682e 7878 6861 7368 719a 580e 0000  ash.xxhashq.X...
-00000ea0: 0043 7279 7074 4465 7269 7665 4b65 7971  .CryptDeriveKeyq
-00000eb0: 9b58 2e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00000ec0: 6e69 7473 2e63 7279 7074 6f2e 6b65 7964  nits.crypto.keyd
-00000ed0: 6572 6976 652e 4372 7970 7444 6572 6976  erive.CryptDeriv
-00000ee0: 654b 6579 719c 5809 0000 0044 4553 4465  eKeyq.X....DESDe
-00000ef0: 7269 7665 719d 5829 0000 0072 6566 696e  riveq.X)...refin
-00000f00: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
-00000f10: 2e6b 6579 6465 7269 7665 2e44 4553 4465  .keyderive.DESDe
-00000f20: 7269 7665 719e 5813 0000 0050 6173 7377  riveq.X....Passw
-00000f30: 6f72 6444 6572 6976 6542 7974 6573 719f  ordDeriveBytesq.
-00000f40: 5833 0000 0072 6566 696e 6572 792e 756e  X3...refinery.un
-00000f50: 6974 732e 6372 7970 746f 2e6b 6579 6465  its.crypto.keyde
-00000f60: 7269 7665 2e50 6173 7377 6f72 6444 6572  rive.PasswordDer
-00000f70: 6976 6542 7974 6573 71a0 5804 0000 0048  iveBytesq.X....H
-00000f80: 4b44 4671 a158 2400 0000 7265 6669 6e65  KDFq.X$...refine
-00000f90: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000fa0: 6b65 7964 6572 6976 652e 686b 6466 71a2  keyderive.hkdfq.
-00000fb0: 5804 0000 0068 6d61 6371 a358 2400 0000  X....hmacq.X$...
-00000fc0: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000fd0: 7279 7074 6f2e 6b65 7964 6572 6976 652e  rypto.keyderive.
-00000fe0: 686d 6163 71a4 5805 0000 006b 626c 6f62  hmacq.X....kblob
-00000ff0: 71a5 5825 0000 0072 6566 696e 6572 792e  q.X%...refinery.
-00001000: 756e 6974 732e 6372 7970 746f 2e6b 6579  units.crypto.key
-00001010: 6465 7269 7665 2e6b 626c 6f62 71a6 5806  derive.kblobq.X.
-00001020: 0000 0070 626b 6466 3171 a758 2600 0000  ...pbkdf1q.X&...
-00001030: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00001040: 7279 7074 6f2e 6b65 7964 6572 6976 652e  rypto.keyderive.
-00001050: 7062 6b64 6631 71a8 5806 0000 0070 626b  pbkdf1q.X....pbk
-00001060: 6466 3271 a958 2600 0000 7265 6669 6e65  df2q.X&...refine
-00001070: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00001080: 6b65 7964 6572 6976 652e 7062 6b64 6632  keyderive.pbkdf2
-00001090: 71aa 5806 0000 0075 6372 7970 7471 ab58  q.X....ucryptq.X
-000010a0: 2900 0000 7265 6669 6e65 7279 2e75 6e69  )...refinery.uni
-000010b0: 7473 2e63 7279 7074 6f2e 6b65 7964 6572  ts.crypto.keyder
-000010c0: 6976 652e 756e 6978 6372 7970 7471 ac58  ive.unixcryptq.X
-000010d0: 0600 0000 6174 6261 7368 71ad 581e 0000  ....atbashq.X...
-000010e0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000010f0: 656e 636f 6469 6e67 2e61 7462 6173 6871  encoding.atbashq
-00001100: ae58 0300 0000 6233 3271 af58 1b00 0000  .X....b32q.X....
-00001110: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-00001120: 6e63 6f64 696e 672e 6233 3271 b058 0300  ncoding.b32q.X..
-00001130: 0000 6235 3871 b158 1b00 0000 7265 6669  ..b58q.X....refi
-00001140: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
-00001150: 696e 672e 6235 3871 b258 0300 0000 6236  ing.b58q.X....b6
-00001160: 3471 b358 1b00 0000 7265 6669 6e65 7279  4q.X....refinery
-00001170: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
-00001180: 6236 3471 b458 0300 0000 6238 3571 b558  b64q.X....b85q.X
-00001190: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000011a0: 7473 2e65 6e63 6f64 696e 672e 6238 3571  ts.encoding.b85q
-000011b0: b658 0400 0000 6261 7365 71b7 581c 0000  .X....baseq.X...
-000011c0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000011d0: 656e 636f 6469 6e67 2e62 6173 6571 b858  encoding.baseq.X
-000011e0: 0600 0000 6370 3132 3532 71b9 581e 0000  ....cp1252q.X...
-000011f0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001200: 656e 636f 6469 6e67 2e63 7031 3235 3271  encoding.cp1252q
-00001210: ba58 0300 0000 6573 6371 bb58 1b00 0000  .X....escq.X....
-00001220: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-00001230: 6e63 6f64 696e 672e 6573 6371 bc58 0300  ncoding.escq.X..
-00001240: 0000 6865 7871 bd58 1b00 0000 7265 6669  ..hexq.X....refi
-00001250: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
-00001260: 696e 672e 6865 7871 be58 0700 0000 6874  ing.hexq.X....ht
-00001270: 6d6c 6573 6371 bf58 1f00 0000 7265 6669  mlescq.X....refi
-00001280: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
-00001290: 696e 672e 6874 6d6c 6573 6371 c058 0700  ing.htmlescq.X..
-000012a0: 0000 6e65 7462 696f 7371 c158 1f00 0000  ..netbiosq.X....
-000012b0: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-000012c0: 6e63 6f64 696e 672e 6e65 7462 696f 7371  ncoding.netbiosq
-000012d0: c258 0600 0000 7073 3173 7472 71c3 581e  .X....ps1strq.X.
-000012e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000012f0: 732e 656e 636f 6469 6e67 2e70 7331 7374  s.encoding.ps1st
-00001300: 7271 c458 0600 0000 7265 636f 6465 71c5  rq.X....recodeq.
-00001310: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00001320: 6974 732e 656e 636f 6469 6e67 2e72 6563  its.encoding.rec
-00001330: 6f64 6571 c658 0300 0000 7531 3671 c758  odeq.X....u16q.X
-00001340: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00001350: 7473 2e65 6e63 6f64 696e 672e 7531 3671  ts.encoding.u16q
-00001360: c858 0300 0000 7572 6c71 c958 1b00 0000  .X....urlq.X....
-00001370: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
-00001380: 6e63 6f64 696e 672e 7572 6c71 ca58 0500  ncoding.urlq.X..
-00001390: 0000 7575 656e 6371 cb58 1d00 0000 7265  ..uuencq.X....re
-000013a0: 6669 6e65 7279 2e75 6e69 7473 2e65 6e63  finery.units.enc
-000013b0: 6f64 696e 672e 7575 656e 6371 cc58 0600  oding.uuencq.X..
-000013c0: 0000 7773 6865 6e63 71cd 581e 0000 0072  ..wshencq.X....r
-000013d0: 6566 696e 6572 792e 756e 6974 732e 656e  efinery.units.en
-000013e0: 636f 6469 6e67 2e77 7368 656e 6371 ce58  coding.wshencq.X
-000013f0: 0300 0000 6133 7871 cf58 1a00 0000 7265  ....a3xq.X....re
-00001400: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-00001410: 6d61 7473 2e61 3378 71d0 5802 0000 0078  mats.a3xq.X....x
-00001420: 7471 d158 2100 0000 7265 6669 6e65 7279  tq.X!...refinery
-00001430: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
-00001440: 7263 6869 7665 2e78 7471 d258 0400 0000  rchive.xtq.X....
-00001450: 7874 377a 71d3 5823 0000 0072 6566 696e  xt7zq.X#...refin
-00001460: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001470: 732e 6172 6368 6976 652e 7874 377a 71d4  s.archive.xt7zq.
-00001480: 5805 0000 0078 7461 6365 71d5 5824 0000  X....xtaceq.X$..
-00001490: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000014a0: 666f 726d 6174 732e 6172 6368 6976 652e  formats.archive.
-000014b0: 7874 6163 6571 d658 0600 0000 7874 6173  xtaceq.X....xtas
-000014c0: 6172 71d7 5825 0000 0072 6566 696e 6572  arq.X%...refiner
-000014d0: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-000014e0: 6172 6368 6976 652e 7874 6173 6172 71d8  archive.xtasarq.
-000014f0: 5805 0000 0078 7463 6162 71d9 5824 0000  X....xtcabq.X$..
-00001500: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001510: 666f 726d 6174 732e 6172 6368 6976 652e  formats.archive.
-00001520: 7874 6361 6271 da58 0600 0000 7874 6370  xtcabq.X....xtcp
-00001530: 696f 71db 5825 0000 0072 6566 696e 6572  ioq.X%...refiner
-00001540: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001550: 6172 6368 6976 652e 7874 6370 696f 71dc  archive.xtcpioq.
-00001560: 5804 0000 0078 7467 7a71 dd58 2300 0000  X....xtgzq.X#...
-00001570: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-00001580: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
-00001590: 7467 7a71 de58 0500 0000 7874 6973 6f71  tgzq.X....xtisoq
-000015a0: df58 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
-000015b0: 6e69 7473 2e66 6f72 6d61 7473 2e61 7263  nits.formats.arc
-000015c0: 6869 7665 2e78 7469 736f 71e0 5805 0000  hive.xtisoq.X...
-000015d0: 0078 7469 7373 71e1 5824 0000 0072 6566  .xtissq.X$...ref
-000015e0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-000015f0: 6174 732e 6172 6368 6976 652e 7874 6973  ats.archive.xtis
-00001600: 7371 e258 0600 0000 7874 6e6f 6465 71e3  sq.X....xtnodeq.
-00001610: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
-00001620: 6974 732e 666f 726d 6174 732e 6172 6368  its.formats.arch
-00001630: 6976 652e 7874 6e6f 6465 71e4 5806 0000  ive.xtnodeq.X...
-00001640: 0078 746e 7369 7371 e558 2500 0000 7265  .xtnsisq.X%...re
-00001650: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-00001660: 6d61 7473 2e61 7263 6869 7665 2e78 746e  mats.archive.xtn
-00001670: 7369 7371 e658 0500 0000 7874 7079 6971  sisq.X....xtpyiq
-00001680: e758 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
-00001690: 6e69 7473 2e66 6f72 6d61 7473 2e61 7263  nits.formats.arc
-000016a0: 6869 7665 2e78 7470 7969 71e8 5805 0000  hive.xtpyiq.X...
-000016b0: 0078 7474 6172 71e9 5824 0000 0072 6566  .xttarq.X$...ref
-000016c0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-000016d0: 6174 732e 6172 6368 6976 652e 7874 7461  ats.archive.xtta
-000016e0: 7271 ea58 0500 0000 7874 7a69 7071 eb58  rq.X....xtzipq.X
-000016f0: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
-00001700: 7473 2e66 6f72 6d61 7473 2e61 7263 6869  ts.formats.archi
-00001710: 7665 2e78 747a 6970 71ec 5803 0000 0062  ve.xtzipq.X....b
-00001720: 6174 71ed 581a 0000 0072 6566 696e 6572  atq.X....refiner
+00000bb0: 6970 6865 722e 7365 7270 656e 7471 7858  ipher.serpentqxX
+00000bc0: 0300 0000 7465 6171 7958 2000 0000 7265  ....teaqyX ...re
+00000bd0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000be0: 7074 6f2e 6369 7068 6572 2e74 6561 717a  pto.cipher.teaqz
+00000bf0: 5808 0000 0076 6967 656e 6572 6571 7b58  X....vigenereq{X
+00000c00: 2500 0000 7265 6669 6e65 7279 2e75 6e69  %...refinery.uni
+00000c10: 7473 2e63 7279 7074 6f2e 6369 7068 6572  ts.crypto.cipher
+00000c20: 2e76 6967 656e 6572 6571 7c58 0400 0000  .vigenereq|X....
+00000c30: 7874 6561 717d 5821 0000 0072 6566 696e  xteaq}X!...refin
+00000c40: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00000c50: 2e63 6970 6865 722e 7874 6561 717e 5805  .cipher.xteaq~X.
+00000c60: 0000 0078 7874 6561 717f 5822 0000 0072  ...xxteaq.X"...r
+00000c70: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
+00000c80: 7970 746f 2e63 6970 6865 722e 7878 7465  ypto.cipher.xxte
+00000c90: 6171 8058 0700 0000 6164 6c65 7233 3271  aq.X....adler32q
+00000ca0: 8158 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
+00000cb0: 6e69 7473 2e63 7279 7074 6f2e 6861 7368  nits.crypto.hash
+00000cc0: 2e63 6865 636b 7375 6d73 7182 5805 0000  .checksumsq.X...
+00000cd0: 0063 7263 3332 7183 6882 5806 0000 0062  .crc32q.h.X....b
+00000ce0: 6c6b 3232 3471 8458 2800 0000 7265 6669  lk224q.X(...refi
+00000cf0: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+00000d00: 6f2e 6861 7368 2e63 7279 7074 6f67 7261  o.hash.cryptogra
+00000d10: 7068 6963 7185 5806 0000 0062 6c6b 3235  phicq.X....blk25
+00000d20: 3671 8668 8558 0600 0000 626c 6b33 3834  6q.h.X....blk384
+00000d30: 7187 6885 5806 0000 0062 6c6b 3531 3271  q.h.X....blk512q
+00000d40: 8868 8558 0300 0000 6d64 3271 8968 8558  .h.X....md2q.h.X
+00000d50: 0300 0000 6d64 3471 8a68 8558 0300 0000  ....md4q.h.X....
+00000d60: 6d64 3571 8b68 8558 0900 0000 7269 7065  md5q.h.X....ripe
+00000d70: 6d64 3132 3871 8c68 8558 0900 0000 7269  md128q.h.X....ri
+00000d80: 7065 6d64 3136 3071 8d68 8558 0400 0000  pemd160q.h.X....
+00000d90: 7368 6131 718e 6885 5806 0000 0073 6861  sha1q.h.X....sha
+00000da0: 3232 3471 8f68 8558 0600 0000 7368 6132  224q.h.X....sha2
+00000db0: 3536 7190 6885 5806 0000 0073 6861 3338  56q.h.X....sha38
+00000dc0: 3471 9168 8558 0600 0000 7368 6135 3132  4q.h.X....sha512
+00000dd0: 7192 6885 5807 0000 0069 6d70 6861 7368  q.h.X....imphash
+00000de0: 7193 5822 0000 0072 6566 696e 6572 792e  q.X"...refinery.
+00000df0: 756e 6974 732e 6372 7970 746f 2e68 6173  units.crypto.has
+00000e00: 682e 696d 7068 6173 6871 9458 0900 0000  h.imphashq.X....
+00000e10: 6d6d 6831 3238 7833 3271 9558 2100 0000  mmh128x32q.X!...
+00000e20: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000e30: 7279 7074 6f2e 6861 7368 2e6d 7572 6d75  rypto.hash.murmu
+00000e40: 7271 9658 0900 0000 6d6d 6831 3238 7836  rq.X....mmh128x6
+00000e50: 3471 9768 9658 0500 0000 6d6d 6833 3271  4q.h.X....mmh32q
+00000e60: 9868 9658 0400 0000 6e74 6c6d 7199 582a  .h.X....ntlmq.X*
+00000e70: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00000e80: 732e 6372 7970 746f 2e68 6173 682e 7061  s.crypto.hash.pa
+00000e90: 7373 776f 7264 5f68 6173 6865 7371 9a58  ssword_hashesq.X
+00000ea0: 0300 0000 7878 6871 9b58 2100 0000 7265  ....xxhq.X!...re
+00000eb0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000ec0: 7074 6f2e 6861 7368 2e78 7868 6173 6871  pto.hash.xxhashq
+00000ed0: 9c58 0e00 0000 4372 7970 7444 6572 6976  .X....CryptDeriv
+00000ee0: 654b 6579 719d 582e 0000 0072 6566 696e  eKeyq.X....refin
+00000ef0: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00000f00: 2e6b 6579 6465 7269 7665 2e43 7279 7074  .keyderive.Crypt
+00000f10: 4465 7269 7665 4b65 7971 9e58 0900 0000  DeriveKeyq.X....
+00000f20: 4445 5344 6572 6976 6571 9f58 2900 0000  DESDeriveq.X)...
+00000f30: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000f40: 7279 7074 6f2e 6b65 7964 6572 6976 652e  rypto.keyderive.
+00000f50: 4445 5344 6572 6976 6571 a058 1300 0000  DESDeriveq.X....
+00000f60: 5061 7373 776f 7264 4465 7269 7665 4279  PasswordDeriveBy
+00000f70: 7465 7371 a158 3300 0000 7265 6669 6e65  tesq.X3...refine
+00000f80: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00000f90: 6b65 7964 6572 6976 652e 5061 7373 776f  keyderive.Passwo
+00000fa0: 7264 4465 7269 7665 4279 7465 7371 a258  rdDeriveBytesq.X
+00000fb0: 0400 0000 484b 4446 71a3 5824 0000 0072  ....HKDFq.X$...r
+00000fc0: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
+00000fd0: 7970 746f 2e6b 6579 6465 7269 7665 2e68  ypto.keyderive.h
+00000fe0: 6b64 6671 a458 0400 0000 686d 6163 71a5  kdfq.X....hmacq.
+00000ff0: 5824 0000 0072 6566 696e 6572 792e 756e  X$...refinery.un
+00001000: 6974 732e 6372 7970 746f 2e6b 6579 6465  its.crypto.keyde
+00001010: 7269 7665 2e68 6d61 6371 a658 0500 0000  rive.hmacq.X....
+00001020: 6b62 6c6f 6271 a758 2500 0000 7265 6669  kblobq.X%...refi
+00001030: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+00001040: 6f2e 6b65 7964 6572 6976 652e 6b62 6c6f  o.keyderive.kblo
+00001050: 6271 a858 0600 0000 7062 6b64 6631 71a9  bq.X....pbkdf1q.
+00001060: 5826 0000 0072 6566 696e 6572 792e 756e  X&...refinery.un
+00001070: 6974 732e 6372 7970 746f 2e6b 6579 6465  its.crypto.keyde
+00001080: 7269 7665 2e70 626b 6466 3171 aa58 0600  rive.pbkdf1q.X..
+00001090: 0000 7062 6b64 6632 71ab 5826 0000 0072  ..pbkdf2q.X&...r
+000010a0: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
+000010b0: 7970 746f 2e6b 6579 6465 7269 7665 2e70  ypto.keyderive.p
+000010c0: 626b 6466 3271 ac58 0600 0000 7563 7279  bkdf2q.X....ucry
+000010d0: 7074 71ad 5829 0000 0072 6566 696e 6572  ptq.X)...refiner
+000010e0: 792e 756e 6974 732e 6372 7970 746f 2e6b  y.units.crypto.k
+000010f0: 6579 6465 7269 7665 2e75 6e69 7863 7279  eyderive.unixcry
+00001100: 7074 71ae 5806 0000 0061 7462 6173 6871  ptq.X....atbashq
+00001110: af58 1e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00001120: 6e69 7473 2e65 6e63 6f64 696e 672e 6174  nits.encoding.at
+00001130: 6261 7368 71b0 5803 0000 0062 3332 71b1  bashq.X....b32q.
+00001140: 581b 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00001150: 6974 732e 656e 636f 6469 6e67 2e62 3332  its.encoding.b32
+00001160: 71b2 5803 0000 0062 3538 71b3 581b 0000  q.X....b58q.X...
+00001170: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001180: 656e 636f 6469 6e67 2e62 3538 71b4 5803  encoding.b58q.X.
+00001190: 0000 0062 3634 71b5 581b 0000 0072 6566  ...b64q.X....ref
+000011a0: 696e 6572 792e 756e 6974 732e 656e 636f  inery.units.enco
+000011b0: 6469 6e67 2e62 3634 71b6 5803 0000 0062  ding.b64q.X....b
+000011c0: 3835 71b7 581b 0000 0072 6566 696e 6572  85q.X....refiner
+000011d0: 792e 756e 6974 732e 656e 636f 6469 6e67  y.units.encoding
+000011e0: 2e62 3835 71b8 5804 0000 0062 6173 6571  .b85q.X....baseq
+000011f0: b958 1c00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00001200: 6e69 7473 2e65 6e63 6f64 696e 672e 6261  nits.encoding.ba
+00001210: 7365 71ba 5806 0000 0063 7031 3235 3271  seq.X....cp1252q
+00001220: bb58 1e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00001230: 6e69 7473 2e65 6e63 6f64 696e 672e 6370  nits.encoding.cp
+00001240: 3132 3532 71bc 5803 0000 0065 7363 71bd  1252q.X....escq.
+00001250: 581b 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00001260: 6974 732e 656e 636f 6469 6e67 2e65 7363  its.encoding.esc
+00001270: 71be 5803 0000 0068 6578 71bf 581b 0000  q.X....hexq.X...
+00001280: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001290: 656e 636f 6469 6e67 2e68 6578 71c0 5807  encoding.hexq.X.
+000012a0: 0000 0068 746d 6c65 7363 71c1 581f 0000  ...htmlescq.X...
+000012b0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000012c0: 656e 636f 6469 6e67 2e68 746d 6c65 7363  encoding.htmlesc
+000012d0: 71c2 5807 0000 006e 6574 6269 6f73 71c3  q.X....netbiosq.
+000012e0: 581f 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000012f0: 6974 732e 656e 636f 6469 6e67 2e6e 6574  its.encoding.net
+00001300: 6269 6f73 71c4 5806 0000 0070 7331 7374  biosq.X....ps1st
+00001310: 7271 c558 1e00 0000 7265 6669 6e65 7279  rq.X....refinery
+00001320: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
+00001330: 7073 3173 7472 71c6 5806 0000 0072 6563  ps1strq.X....rec
+00001340: 6f64 6571 c758 1e00 0000 7265 6669 6e65  odeq.X....refine
+00001350: 7279 2e75 6e69 7473 2e65 6e63 6f64 696e  ry.units.encodin
+00001360: 672e 7265 636f 6465 71c8 5803 0000 0075  g.recodeq.X....u
+00001370: 3136 71c9 581b 0000 0072 6566 696e 6572  16q.X....refiner
+00001380: 792e 756e 6974 732e 656e 636f 6469 6e67  y.units.encoding
+00001390: 2e75 3136 71ca 5803 0000 0075 726c 71cb  .u16q.X....urlq.
+000013a0: 581b 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000013b0: 6974 732e 656e 636f 6469 6e67 2e75 726c  its.encoding.url
+000013c0: 71cc 5805 0000 0075 7565 6e63 71cd 581d  q.X....uuencq.X.
+000013d0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000013e0: 732e 656e 636f 6469 6e67 2e75 7565 6e63  s.encoding.uuenc
+000013f0: 71ce 5806 0000 0077 7368 656e 6371 cf58  q.X....wshencq.X
+00001400: 1e00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00001410: 7473 2e65 6e63 6f64 696e 672e 7773 6865  ts.encoding.wshe
+00001420: 6e63 71d0 5803 0000 0061 3378 71d1 581a  ncq.X....a3xq.X.
+00001430: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001440: 732e 666f 726d 6174 732e 6133 7871 d258  s.formats.a3xq.X
+00001450: 0200 0000 7874 71d3 5821 0000 0072 6566  ....xtq.X!...ref
+00001460: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+00001470: 6174 732e 6172 6368 6976 652e 7874 71d4  ats.archive.xtq.
+00001480: 5804 0000 0078 7437 7a71 d558 2300 0000  X....xt7zq.X#...
+00001490: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+000014a0: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
+000014b0: 7437 7a71 d658 0500 0000 7874 6163 6571  t7zq.X....xtaceq
+000014c0: d758 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
+000014d0: 6e69 7473 2e66 6f72 6d61 7473 2e61 7263  nits.formats.arc
+000014e0: 6869 7665 2e78 7461 6365 71d8 5806 0000  hive.xtaceq.X...
+000014f0: 0078 7461 7361 7271 d958 2500 0000 7265  .xtasarq.X%...re
+00001500: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00001510: 6d61 7473 2e61 7263 6869 7665 2e78 7461  mats.archive.xta
+00001520: 7361 7271 da58 0500 0000 7874 6361 6271  sarq.X....xtcabq
+00001530: db58 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
+00001540: 6e69 7473 2e66 6f72 6d61 7473 2e61 7263  nits.formats.arc
+00001550: 6869 7665 2e78 7463 6162 71dc 5806 0000  hive.xtcabq.X...
+00001560: 0078 7463 7069 6f71 dd58 2500 0000 7265  .xtcpioq.X%...re
+00001570: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00001580: 6d61 7473 2e61 7263 6869 7665 2e78 7463  mats.archive.xtc
+00001590: 7069 6f71 de58 0400 0000 7874 677a 71df  pioq.X....xtgzq.
+000015a0: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
+000015b0: 6974 732e 666f 726d 6174 732e 6172 6368  its.formats.arch
+000015c0: 6976 652e 7874 677a 71e0 5805 0000 0078  ive.xtgzq.X....x
+000015d0: 7469 736f 71e1 5824 0000 0072 6566 696e  tisoq.X$...refin
+000015e0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+000015f0: 732e 6172 6368 6976 652e 7874 6973 6f71  s.archive.xtisoq
+00001600: e258 0500 0000 7874 6973 7371 e358 2400  .X....xtissq.X$.
+00001610: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00001620: 2e66 6f72 6d61 7473 2e61 7263 6869 7665  .formats.archive
+00001630: 2e78 7469 7373 71e4 5806 0000 0078 746e  .xtissq.X....xtn
+00001640: 6f64 6571 e558 2500 0000 7265 6669 6e65  odeq.X%...refine
+00001650: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00001660: 2e61 7263 6869 7665 2e78 746e 6f64 6571  .archive.xtnodeq
+00001670: e658 0600 0000 7874 6e73 6973 71e7 5825  .X....xtnsisq.X%
+00001680: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001690: 732e 666f 726d 6174 732e 6172 6368 6976  s.formats.archiv
+000016a0: 652e 7874 6e73 6973 71e8 5805 0000 0078  e.xtnsisq.X....x
+000016b0: 7470 7969 71e9 5824 0000 0072 6566 696e  tpyiq.X$...refin
+000016c0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+000016d0: 732e 6172 6368 6976 652e 7874 7079 6971  s.archive.xtpyiq
+000016e0: ea58 0500 0000 7874 7461 7271 eb58 2400  .X....xttarq.X$.
+000016f0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00001700: 2e66 6f72 6d61 7473 2e61 7263 6869 7665  .formats.archive
+00001710: 2e78 7474 6172 71ec 5805 0000 0078 747a  .xttarq.X....xtz
+00001720: 6970 71ed 5824 0000 0072 6566 696e 6572  ipq.X$...refiner
 00001730: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001740: 6261 7471 ee58 0300 0000 6373 7671 ef58  batq.X....csvq.X
-00001750: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00001760: 7473 2e66 6f72 6d61 7473 2e63 7376 71f0  ts.formats.csvq.
-00001770: 5805 0000 0064 7370 6870 71f1 5826 0000  X....dsphpq.X&..
-00001780: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001790: 666f 726d 6174 732e 6465 7365 7269 616c  formats.deserial
-000017a0: 697a 655f 7068 7071 f258 0600 0000 6465  ize_phpq.X....de
-000017b0: 7873 7472 71f3 581d 0000 0072 6566 696e  xstrq.X....refin
-000017c0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-000017d0: 732e 6465 7873 7472 71f4 5806 0000 0078  s.dexstrq.X....x
-000017e0: 746d 6169 6c71 f558 1c00 0000 7265 6669  tmailq.X....refi
-000017f0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-00001800: 7473 2e65 6d61 696c 71f6 5804 0000 0065  ts.emailq.X....e
-00001810: 7674 7871 f758 1b00 0000 7265 6669 6e65  vtxq.X....refine
-00001820: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-00001830: 2e65 7674 7871 f858 0500 0000 7661 6464  .evtxq.X....vadd
-00001840: 7271 f958 2000 0000 7265 6669 6e65 7279  rq.X ...refinery
-00001850: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e65  .units.formats.e
-00001860: 7865 2e76 6164 6472 71fa 5807 0000 0076  xe.vaddrq.X....v
-00001870: 6d65 6d72 6566 71fb 5822 0000 0072 6566  memrefq.X"...ref
+00001740: 6172 6368 6976 652e 7874 7a69 7071 ee58  archive.xtzipq.X
+00001750: 0300 0000 6261 7471 ef58 1a00 0000 7265  ....batq.X....re
+00001760: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00001770: 6d61 7473 2e62 6174 71f0 5803 0000 0063  mats.batq.X....c
+00001780: 7376 71f1 581a 0000 0072 6566 696e 6572  svq.X....refiner
+00001790: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+000017a0: 6373 7671 f258 0500 0000 6473 7068 7071  csvq.X....dsphpq
+000017b0: f358 2600 0000 7265 6669 6e65 7279 2e75  .X&...refinery.u
+000017c0: 6e69 7473 2e66 6f72 6d61 7473 2e64 6573  nits.formats.des
+000017d0: 6572 6961 6c69 7a65 5f70 6870 71f4 5806  erialize_phpq.X.
+000017e0: 0000 0064 6578 7374 7271 f558 1d00 0000  ...dexstrq.X....
+000017f0: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001800: 6f72 6d61 7473 2e64 6578 7374 7271 f658  ormats.dexstrq.X
+00001810: 0600 0000 7874 6d61 696c 71f7 581c 0000  ....xtmailq.X...
+00001820: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001830: 666f 726d 6174 732e 656d 6169 6c71 f858  formats.emailq.X
+00001840: 0400 0000 6576 7478 71f9 581b 0000 0072  ....evtxq.X....r
+00001850: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001860: 726d 6174 732e 6576 7478 71fa 5805 0000  rmats.evtxq.X...
+00001870: 0076 6164 6472 71fb 5820 0000 0072 6566  .vaddrq.X ...ref
 00001880: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-00001890: 6174 732e 6578 652e 766d 656d 7265 6671  ats.exe.vmemrefq
-000018a0: fc58 0500 0000 7673 6563 7471 fd58 2000  .X....vsectq.X .
+00001890: 6174 732e 6578 652e 7661 6464 7271 fc58  ats.exe.vaddrq.X
+000018a0: 0700 0000 766d 656d 7265 6671 fd58 2200  ....vmemrefq.X".
 000018b0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000018c0: 2e66 6f72 6d61 7473 2e65 7865 2e76 7365  .formats.exe.vse
-000018d0: 6374 71fe 5805 0000 0076 736e 6970 71ff  ctq.X....vsnipq.
-000018e0: 5820 0000 0072 6566 696e 6572 792e 756e  X ...refinery.un
-000018f0: 6974 732e 666f 726d 6174 732e 6578 652e  its.formats.exe.
-00001900: 7673 6e69 7072 0001 0000 5806 0000 0076  vsnipr....X....v
-00001910: 7374 6163 6b72 0101 0000 5821 0000 0072  stackr....X!...r
-00001920: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001930: 726d 6174 732e 6578 652e 7673 7461 636b  rmats.exe.vstack
-00001940: 7202 0100 0058 0700 0000 6865 786c 6f61  r....X....hexloa
-00001950: 6472 0301 0000 581e 0000 0072 6566 696e  dr....X....refin
-00001960: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001970: 732e 6865 786c 6f61 6472 0401 0000 5806  s.hexloadr....X.
-00001980: 0000 0078 7468 746d 6c72 0501 0000 581b  ...xthtmlr....X.
-00001990: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000019a0: 732e 666f 726d 6174 732e 6874 6d6c 7206  s.formats.htmlr.
-000019b0: 0100 0058 0c00 0000 6874 7470 7265 7370  ...X....httpresp
-000019c0: 6f6e 7365 7207 0100 0058 2300 0000 7265  onser....X#...re
+000018c0: 2e66 6f72 6d61 7473 2e65 7865 2e76 6d65  .formats.exe.vme
+000018d0: 6d72 6566 71fe 5805 0000 0076 7365 6374  mrefq.X....vsect
+000018e0: 71ff 5820 0000 0072 6566 696e 6572 792e  q.X ...refinery.
+000018f0: 756e 6974 732e 666f 726d 6174 732e 6578  units.formats.ex
+00001900: 652e 7673 6563 7472 0001 0000 5805 0000  e.vsectr....X...
+00001910: 0076 736e 6970 7201 0100 0058 2000 0000  .vsnipr....X ...
+00001920: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001930: 6f72 6d61 7473 2e65 7865 2e76 736e 6970  ormats.exe.vsnip
+00001940: 7202 0100 0058 0600 0000 7673 7461 636b  r....X....vstack
+00001950: 7203 0100 0058 2100 0000 7265 6669 6e65  r....X!...refine
+00001960: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00001970: 2e65 7865 2e76 7374 6163 6b72 0401 0000  .exe.vstackr....
+00001980: 5807 0000 0068 6578 6c6f 6164 7205 0100  X....hexloadr...
+00001990: 0058 1e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000019a0: 6e69 7473 2e66 6f72 6d61 7473 2e68 6578  nits.formats.hex
+000019b0: 6c6f 6164 7206 0100 0058 0600 0000 7874  loadr....X....xt
+000019c0: 6874 6d6c 7207 0100 0058 1b00 0000 7265  htmlr....X....re
 000019d0: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-000019e0: 6d61 7473 2e68 7474 7072 6573 706f 6e73  mats.httprespons
-000019f0: 6572 0801 0000 5804 0000 0069 6670 7372  er....X....ifpsr
-00001a00: 0901 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
+000019e0: 6d61 7473 2e68 746d 6c72 0801 0000 580c  mats.htmlr....X.
+000019f0: 0000 0068 7474 7072 6573 706f 6e73 6572  ...httpresponser
+00001a00: 0901 0000 5823 0000 0072 6566 696e 6572  ....X#...refiner
 00001a10: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001a20: 6966 7073 720a 0100 0058 0700 0000 6966  ifpsr....X....if
-00001a30: 7073 7374 7272 0b01 0000 581e 0000 0072  psstrr....X....r
-00001a40: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001a50: 726d 6174 732e 6966 7073 7374 7272 0c01  rmats.ifpsstrr..
-00001a60: 0000 5806 0000 0064 736a 6176 6172 0d01  ..X....dsjavar..
-00001a70: 0000 5827 0000 0072 6566 696e 6572 792e  ..X'...refinery.
-00001a80: 756e 6974 732e 666f 726d 6174 732e 6a61  units.formats.ja
-00001a90: 7661 2e64 6573 6572 6961 6c69 7a65 720e  va.deserializer.
-00001aa0: 0100 0058 0600 0000 6a76 6461 736d 720f  ...X....jvdasmr.
-00001ab0: 0100 0058 2200 0000 7265 6669 6e65 7279  ...X"...refinery
-00001ac0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e6a  .units.formats.j
-00001ad0: 6176 612e 6a76 6461 736d 7210 0100 0058  ava.jvdasmr....X
-00001ae0: 0500 0000 6a76 7374 7272 1101 0000 5821  ....jvstrr....X!
+00001a20: 6874 7470 7265 7370 6f6e 7365 720a 0100  httpresponser...
+00001a30: 0058 0400 0000 6966 7073 720b 0100 0058  .X....ifpsr....X
+00001a40: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00001a50: 7473 2e66 6f72 6d61 7473 2e69 6670 7372  ts.formats.ifpsr
+00001a60: 0c01 0000 5807 0000 0069 6670 7373 7472  ....X....ifpsstr
+00001a70: 720d 0100 0058 1e00 0000 7265 6669 6e65  r....X....refine
+00001a80: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00001a90: 2e69 6670 7373 7472 720e 0100 0058 0600  .ifpsstrr....X..
+00001aa0: 0000 6473 6a61 7661 720f 0100 0058 2700  ..dsjavar....X'.
+00001ab0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00001ac0: 2e66 6f72 6d61 7473 2e6a 6176 612e 6465  .formats.java.de
+00001ad0: 7365 7269 616c 697a 6572 1001 0000 5806  serializer....X.
+00001ae0: 0000 006a 7664 6173 6d72 1101 0000 5822  ...jvdasmr....X"
 00001af0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
 00001b00: 732e 666f 726d 6174 732e 6a61 7661 2e6a  s.formats.java.j
-00001b10: 7673 7472 7212 0100 0058 0300 0000 786a  vstrr....X....xj
-00001b20: 3072 1301 0000 581b 0000 0072 6566 696e  0r....X....refin
-00001b30: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001b40: 732e 6a73 6f6e 7214 0100 0058 0300 0000  s.jsonr....X....
-00001b50: 786a 6c72 1501 0000 6a14 0100 0058 0600  xjlr....j....X..
-00001b60: 0000 7874 6a73 6f6e 7216 0100 006a 1401  ..xtjsonr....j..
-00001b70: 0000 5803 0000 006c 6e6b 7217 0100 0058  ..X....lnkr....X
-00001b80: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00001b90: 7473 2e66 6f72 6d61 7473 2e6c 6e6b 7218  ts.formats.lnkr.
-00001ba0: 0100 0058 0700 0000 6d73 6770 6163 6b72  ...X....msgpackr
-00001bb0: 1901 0000 581e 0000 0072 6566 696e 6572  ....X....refiner
-00001bc0: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001bd0: 6d73 6770 6163 6b72 1a01 0000 5805 0000  msgpackr....X...
-00001be0: 0078 746d 7369 721b 0100 0058 1a00 0000  .xtmsir....X....
-00001bf0: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-00001c00: 6f72 6d61 7473 2e6d 7369 721c 0100 0058  ormats.msir....X
-00001c10: 0600 0000 646f 6374 7874 721d 0100 0058  ....doctxtr....X
-00001c20: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
-00001c30: 7473 2e66 6f72 6d61 7473 2e6f 6666 6963  ts.formats.offic
-00001c40: 652e 646f 6374 7874 721e 0100 0058 0b00  e.doctxtr....X..
-00001c50: 0000 6f66 6669 6365 6372 7970 7472 1f01  ..officecryptr..
-00001c60: 0000 5829 0000 0072 6566 696e 6572 792e  ..X)...refinery.
-00001c70: 756e 6974 732e 666f 726d 6174 732e 6f66  units.formats.of
-00001c80: 6669 6365 2e6f 6666 6963 6563 7279 7074  fice.officecrypt
-00001c90: 7220 0100 0058 0500 0000 7662 6170 6372  r ...X....vbapcr
-00001ca0: 2101 0000 5823 0000 0072 6566 696e 6572  !...X#...refiner
-00001cb0: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001cc0: 6f66 6669 6365 2e76 6261 7063 7222 0100  office.vbapcr"..
-00001cd0: 0058 0600 0000 7662 6173 7472 7223 0100  .X....vbastrr#..
-00001ce0: 0058 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
-00001cf0: 6e69 7473 2e66 6f72 6d61 7473 2e6f 6666  nits.formats.off
-00001d00: 6963 652e 7662 6173 7472 7224 0100 0058  ice.vbastrr$...X
-00001d10: 0800 0000 786c 6d64 656f 6266 7225 0100  ....xlmdeobfr%..
-00001d20: 0058 2600 0000 7265 6669 6e65 7279 2e75  .X&...refinery.u
-00001d30: 6e69 7473 2e66 6f72 6d61 7473 2e6f 6666  nits.formats.off
-00001d40: 6963 652e 786c 6d64 656f 6266 7226 0100  ice.xlmdeobfr&..
-00001d50: 0058 0500 0000 786c 7874 7272 2701 0000  .X....xlxtrr'...
-00001d60: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
-00001d70: 6974 732e 666f 726d 6174 732e 6f66 6669  its.formats.offi
-00001d80: 6365 2e78 6c78 7472 7228 0100 0058 0500  ce.xlxtrr(...X..
-00001d90: 0000 7874 646f 6372 2901 0000 5823 0000  ..xtdocr)...X#..
-00001da0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001db0: 666f 726d 6174 732e 6f66 6669 6365 2e78  formats.office.x
-00001dc0: 7464 6f63 722a 0100 0058 0500 0000 7874  tdocr*...X....xt
-00001dd0: 6f6e 6572 2b01 0000 5823 0000 0072 6566  oner+...X#...ref
-00001de0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-00001df0: 6174 732e 6f66 6669 6365 2e78 746f 6e65  ats.office.xtone
-00001e00: 722c 0100 0058 0500 0000 7874 7274 6672  r,...X....xtrtfr
-00001e10: 2d01 0000 5823 0000 0072 6566 696e 6572  -...X#...refiner
-00001e20: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001e30: 6f66 6669 6365 2e78 7472 7466 722e 0100  office.xtrtfr...
-00001e40: 0058 0500 0000 7874 7662 6172 2f01 0000  .X....xtvbar/...
-00001e50: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
-00001e60: 6974 732e 666f 726d 6174 732e 6f66 6669  its.formats.offi
-00001e70: 6365 2e78 7476 6261 7230 0100 0058 0400  ce.xtvbar0...X..
-00001e80: 0000 7063 6170 7231 0100 0058 1b00 0000  ..pcapr1...X....
+00001b10: 7664 6173 6d72 1201 0000 5805 0000 006a  vdasmr....X....j
+00001b20: 7673 7472 7213 0100 0058 2100 0000 7265  vstrr....X!...re
+00001b30: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00001b40: 6d61 7473 2e6a 6176 612e 6a76 7374 7272  mats.java.jvstrr
+00001b50: 1401 0000 5803 0000 0078 6a30 7215 0100  ....X....xj0r...
+00001b60: 0058 1b00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00001b70: 6e69 7473 2e66 6f72 6d61 7473 2e6a 736f  nits.formats.jso
+00001b80: 6e72 1601 0000 5803 0000 0078 6a6c 7217  nr....X....xjlr.
+00001b90: 0100 006a 1601 0000 5806 0000 0078 746a  ...j....X....xtj
+00001ba0: 736f 6e72 1801 0000 6a16 0100 0058 0300  sonr....j....X..
+00001bb0: 0000 6c6e 6b72 1901 0000 581a 0000 0072  ..lnkr....X....r
+00001bc0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001bd0: 726d 6174 732e 6c6e 6b72 1a01 0000 5807  rmats.lnkr....X.
+00001be0: 0000 006d 7367 7061 636b 721b 0100 0058  ...msgpackr....X
+00001bf0: 1e00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00001c00: 7473 2e66 6f72 6d61 7473 2e6d 7367 7061  ts.formats.msgpa
+00001c10: 636b 721c 0100 0058 0500 0000 7874 6d73  ckr....X....xtms
+00001c20: 6972 1d01 0000 581a 0000 0072 6566 696e  ir....X....refin
+00001c30: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001c40: 732e 6d73 6972 1e01 0000 5806 0000 0064  s.msir....X....d
+00001c50: 6f63 7478 7472 1f01 0000 5824 0000 0072  octxtr....X$...r
+00001c60: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001c70: 726d 6174 732e 6f66 6669 6365 2e64 6f63  rmats.office.doc
+00001c80: 7478 7472 2001 0000 580b 0000 006f 6666  txtr ...X....off
+00001c90: 6963 6563 7279 7074 7221 0100 0058 2900  icecryptr!...X).
+00001ca0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00001cb0: 2e66 6f72 6d61 7473 2e6f 6666 6963 652e  .formats.office.
+00001cc0: 6f66 6669 6365 6372 7970 7472 2201 0000  officecryptr"...
+00001cd0: 5805 0000 0076 6261 7063 7223 0100 0058  X....vbapcr#...X
+00001ce0: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
+00001cf0: 7473 2e66 6f72 6d61 7473 2e6f 6666 6963  ts.formats.offic
+00001d00: 652e 7662 6170 6372 2401 0000 5806 0000  e.vbapcr$...X...
+00001d10: 0076 6261 7374 7272 2501 0000 5824 0000  .vbastrr%...X$..
+00001d20: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001d30: 666f 726d 6174 732e 6f66 6669 6365 2e76  formats.office.v
+00001d40: 6261 7374 7272 2601 0000 5808 0000 0078  bastrr&...X....x
+00001d50: 6c6d 6465 6f62 6672 2701 0000 5826 0000  lmdeobfr'...X&..
+00001d60: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001d70: 666f 726d 6174 732e 6f66 6669 6365 2e78  formats.office.x
+00001d80: 6c6d 6465 6f62 6672 2801 0000 5805 0000  lmdeobfr(...X...
+00001d90: 0078 6c78 7472 7229 0100 0058 2300 0000  .xlxtrr)...X#...
+00001da0: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001db0: 6f72 6d61 7473 2e6f 6666 6963 652e 786c  ormats.office.xl
+00001dc0: 7874 7272 2a01 0000 5805 0000 0078 7464  xtrr*...X....xtd
+00001dd0: 6f63 722b 0100 0058 2300 0000 7265 6669  ocr+...X#...refi
+00001de0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00001df0: 7473 2e6f 6666 6963 652e 7874 646f 6372  ts.office.xtdocr
+00001e00: 2c01 0000 5805 0000 0078 746f 6e65 722d  ,...X....xtoner-
+00001e10: 0100 0058 2300 0000 7265 6669 6e65 7279  ...X#...refinery
+00001e20: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e6f  .units.formats.o
+00001e30: 6666 6963 652e 7874 6f6e 6572 2e01 0000  ffice.xtoner....
+00001e40: 5805 0000 0078 7472 7466 722f 0100 0058  X....xtrtfr/...X
+00001e50: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
+00001e60: 7473 2e66 6f72 6d61 7473 2e6f 6666 6963  ts.formats.offic
+00001e70: 652e 7874 7274 6672 3001 0000 5805 0000  e.xtrtfr0...X...
+00001e80: 0078 7476 6261 7231 0100 0058 2300 0000  .xtvbar1...X#...
 00001e90: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-00001ea0: 6f72 6d61 7473 2e70 6361 7072 3201 0000  ormats.pcapr2...
-00001eb0: 5809 0000 0070 6361 705f 6874 7470 7233  X....pcap_httpr3
-00001ec0: 0100 0058 2000 0000 7265 6669 6e65 7279  ...X ...refinery
-00001ed0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
-00001ee0: 6361 705f 6874 7470 7234 0100 0058 0500  cap_httpr4...X..
-00001ef0: 0000 7874 7064 6672 3501 0000 581a 0000  ..xtpdfr5...X...
-00001f00: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001f10: 666f 726d 6174 732e 7064 6672 3601 0000  formats.pdfr6...
-00001f20: 5806 0000 0064 6e62 6c6f 6272 3701 0000  X....dnblobr7...
-00001f30: 5827 0000 0072 6566 696e 6572 792e 756e  X'...refinery.un
-00001f40: 6974 732e 666f 726d 6174 732e 7065 2e64  its.formats.pe.d
-00001f50: 6f74 6e65 742e 646e 626c 6f62 7238 0100  otnet.dnblobr8..
-00001f60: 0058 0500 0000 646e 6366 7872 3901 0000  .X....dncfxr9...
-00001f70: 5826 0000 0072 6566 696e 6572 792e 756e  X&...refinery.un
-00001f80: 6974 732e 666f 726d 6174 732e 7065 2e64  its.formats.pe.d
-00001f90: 6f74 6e65 742e 646e 6366 7872 3a01 0000  otnet.dncfxr:...
-00001fa0: 5804 0000 0064 6e64 7372 3b01 0000 5825  X....dndsr;...X%
-00001fb0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00001fc0: 732e 666f 726d 6174 732e 7065 2e64 6f74  s.formats.pe.dot
-00001fd0: 6e65 742e 646e 6473 723c 0100 0058 0800  net.dndsr<...X..
-00001fe0: 0000 646e 6669 656c 6473 723d 0100 0058  ..dnfieldsr=...X
-00001ff0: 2900 0000 7265 6669 6e65 7279 2e75 6e69  )...refinery.uni
-00002000: 7473 2e66 6f72 6d61 7473 2e70 652e 646f  ts.formats.pe.do
-00002010: 746e 6574 2e64 6e66 6965 6c64 7372 3e01  tnet.dnfieldsr>.
-00002020: 0000 5805 0000 0064 6e68 6472 723f 0100  ..X....dnhdrr?..
-00002030: 0058 2600 0000 7265 6669 6e65 7279 2e75  .X&...refinery.u
-00002040: 6e69 7473 2e66 6f72 6d61 7473 2e70 652e  nits.formats.pe.
-00002050: 646f 746e 6574 2e64 6e68 6472 7240 0100  dotnet.dnhdrr@..
-00002060: 0058 0400 0000 646e 6d72 7241 0100 0058  .X....dnmrrA...X
-00002070: 2500 0000 7265 6669 6e65 7279 2e75 6e69  %...refinery.uni
-00002080: 7473 2e66 6f72 6d61 7473 2e70 652e 646f  ts.formats.pe.do
-00002090: 746e 6574 2e64 6e6d 7272 4201 0000 5804  tnet.dnmrrB...X.
-000020a0: 0000 0064 6e72 6372 4301 0000 5825 0000  ...dnrcrC...X%..
-000020b0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000020c0: 666f 726d 6174 732e 7065 2e64 6f74 6e65  formats.pe.dotne
-000020d0: 742e 646e 7263 7244 0100 0058 0500 0000  t.dnrcrD...X....
-000020e0: 646e 7374 7272 4501 0000 5826 0000 0072  dnstrrE...X&...r
-000020f0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00002100: 726d 6174 732e 7065 2e64 6f74 6e65 742e  rmats.pe.dotnet.
-00002110: 646e 7374 7272 4601 0000 5806 0000 0070  dnstrrF...X....p
-00002120: 656d 6574 6172 4701 0000 5820 0000 0072  emetarG...X ...r
-00002130: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00002140: 726d 6174 732e 7065 2e70 656d 6574 6172  rmats.pe.pemetar
-00002150: 4801 0000 5809 0000 0070 656f 7665 726c  H...X....peoverl
-00002160: 6179 7249 0100 0058 2300 0000 7265 6669  ayrI...X#...refi
-00002170: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-00002180: 7473 2e70 652e 7065 6f76 6572 6c61 7972  ts.pe.peoverlayr
-00002190: 4a01 0000 5804 0000 0070 6572 6372 4b01  J...X....percrK.
-000021a0: 0000 581e 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00001ea0: 6f72 6d61 7473 2e6f 6666 6963 652e 7874  ormats.office.xt
+00001eb0: 7662 6172 3201 0000 5804 0000 0070 6361  vbar2...X....pca
+00001ec0: 7072 3301 0000 581b 0000 0072 6566 696e  pr3...X....refin
+00001ed0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001ee0: 732e 7063 6170 7234 0100 0058 0900 0000  s.pcapr4...X....
+00001ef0: 7063 6170 5f68 7474 7072 3501 0000 5820  pcap_httpr5...X 
+00001f00: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001f10: 732e 666f 726d 6174 732e 7063 6170 5f68  s.formats.pcap_h
+00001f20: 7474 7072 3601 0000 5805 0000 0078 7470  ttpr6...X....xtp
+00001f30: 6466 7237 0100 0058 1a00 0000 7265 6669  dfr7...X....refi
+00001f40: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00001f50: 7473 2e70 6466 7238 0100 0058 0600 0000  ts.pdfr8...X....
+00001f60: 646e 626c 6f62 7239 0100 0058 2700 0000  dnblobr9...X'...
+00001f70: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001f80: 6f72 6d61 7473 2e70 652e 646f 746e 6574  ormats.pe.dotnet
+00001f90: 2e64 6e62 6c6f 6272 3a01 0000 5805 0000  .dnblobr:...X...
+00001fa0: 0064 6e63 6678 723b 0100 0058 2600 0000  .dncfxr;...X&...
+00001fb0: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001fc0: 6f72 6d61 7473 2e70 652e 646f 746e 6574  ormats.pe.dotnet
+00001fd0: 2e64 6e63 6678 723c 0100 0058 0400 0000  .dncfxr<...X....
+00001fe0: 646e 6473 723d 0100 0058 2500 0000 7265  dndsr=...X%...re
+00001ff0: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00002000: 6d61 7473 2e70 652e 646f 746e 6574 2e64  mats.pe.dotnet.d
+00002010: 6e64 7372 3e01 0000 5808 0000 0064 6e66  ndsr>...X....dnf
+00002020: 6965 6c64 7372 3f01 0000 5829 0000 0072  ieldsr?...X)...r
+00002030: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00002040: 726d 6174 732e 7065 2e64 6f74 6e65 742e  rmats.pe.dotnet.
+00002050: 646e 6669 656c 6473 7240 0100 0058 0500  dnfieldsr@...X..
+00002060: 0000 646e 6864 7272 4101 0000 5826 0000  ..dnhdrrA...X&..
+00002070: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002080: 666f 726d 6174 732e 7065 2e64 6f74 6e65  formats.pe.dotne
+00002090: 742e 646e 6864 7272 4201 0000 5804 0000  t.dnhdrrB...X...
+000020a0: 0064 6e6d 7272 4301 0000 5825 0000 0072  .dnmrrC...X%...r
+000020b0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+000020c0: 726d 6174 732e 7065 2e64 6f74 6e65 742e  rmats.pe.dotnet.
+000020d0: 646e 6d72 7244 0100 0058 0400 0000 646e  dnmrrD...X....dn
+000020e0: 7263 7245 0100 0058 2500 0000 7265 6669  rcrE...X%...refi
+000020f0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00002100: 7473 2e70 652e 646f 746e 6574 2e64 6e72  ts.pe.dotnet.dnr
+00002110: 6372 4601 0000 5805 0000 0064 6e73 7472  crF...X....dnstr
+00002120: 7247 0100 0058 2600 0000 7265 6669 6e65  rG...X&...refine
+00002130: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00002140: 2e70 652e 646f 746e 6574 2e64 6e73 7472  .pe.dotnet.dnstr
+00002150: 7248 0100 0058 0600 0000 7065 6d65 7461  rH...X....pemeta
+00002160: 7249 0100 0058 2000 0000 7265 6669 6e65  rI...X ...refine
+00002170: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00002180: 2e70 652e 7065 6d65 7461 724a 0100 0058  .pe.pemetarJ...X
+00002190: 0900 0000 7065 6f76 6572 6c61 7972 4b01  ....peoverlayrK.
+000021a0: 0000 5823 0000 0072 6566 696e 6572 792e  ..X#...refinery.
 000021b0: 756e 6974 732e 666f 726d 6174 732e 7065  units.formats.pe
-000021c0: 2e70 6572 6372 4c01 0000 5805 0000 0070  .percrL...X....p
-000021d0: 6573 6967 724d 0100 0058 1f00 0000 7265  esigrM...X....re
-000021e0: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-000021f0: 6d61 7473 2e70 652e 7065 7369 6772 4e01  mats.pe.pesigrN.
-00002200: 0000 5807 0000 0070 6573 7472 6970 724f  ..X....pestriprO
-00002210: 0100 0058 2100 0000 7265 6669 6e65 7279  ...X!...refinery
-00002220: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
-00002230: 652e 7065 7374 7269 7072 5001 0000 5805  e.pestriprP...X.
-00002240: 0000 0070 6b63 7337 7251 0100 0058 1c00  ...pkcs7rQ...X..
-00002250: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002260: 2e66 6f72 6d61 7473 2e70 6b63 7337 7252  .formats.pkcs7rR
-00002270: 0100 0058 0800 0000 706b 6373 3773 6967  ...X....pkcs7sig
-00002280: 7253 0100 0058 1f00 0000 7265 6669 6e65  rS...X....refine
-00002290: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-000022a0: 2e70 6b63 7337 7369 6772 5401 0000 5805  .pkcs7sigrT...X.
-000022b0: 0000 0073 7465 676f 7255 0100 0058 1c00  ...stegorU...X..
-000022c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000022d0: 2e66 6f72 6d61 7473 2e73 7465 676f 7256  .formats.stegorV
-000022e0: 0100 0058 0700 0000 746e 6574 6d74 6d72  ...X....tnetmtmr
-000022f0: 5701 0000 581e 0000 0072 6566 696e 6572  W...X....refiner
-00002300: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00002310: 746e 6574 6d74 6d72 5801 0000 5806 0000  tnetmtmrX...X...
-00002320: 0077 696e 7265 6772 5901 0000 581d 0000  .winregrY...X...
-00002330: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002340: 666f 726d 6174 732e 7769 6e72 6567 725a  formats.winregrZ
-00002350: 0100 0058 0500 0000 7874 786d 6c72 5b01  ...X....xtxmlr[.
-00002360: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002370: 756e 6974 732e 666f 726d 6174 732e 786d  units.formats.xm
-00002380: 6c72 5c01 0000 5803 0000 006e 3430 725d  lr\...X....n40r]
-00002390: 0100 0058 1a00 0000 7265 6669 6e65 7279  ...X....refinery
-000023a0: 2e75 6e69 7473 2e6d 616c 7761 7265 2e6e  .units.malware.n
-000023b0: 3430 725e 0100 0058 0400 0000 6368 6f70  40r^...X....chop
-000023c0: 725f 0100 0058 1800 0000 7265 6669 6e65  r_...X....refine
-000023d0: 7279 2e75 6e69 7473 2e6d 6574 612e 6368  ry.units.meta.ch
-000023e0: 6f70 7260 0100 0058 0200 0000 636d 7261  opr`...X....cmra
-000023f0: 0100 0058 1600 0000 7265 6669 6e65 7279  ...X....refinery
-00002400: 2e75 6e69 7473 2e6d 6574 612e 636d 7262  .units.meta.cmrb
-00002410: 0100 0058 0400 0000 6375 6c6c 7263 0100  ...X....cullrc..
-00002420: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00002430: 6e69 7473 2e6d 6574 612e 6375 6c6c 7264  nits.meta.cullrd
-00002440: 0100 0058 0500 0000 6465 6475 7072 6501  ...X....dedupre.
-00002450: 0000 5819 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002460: 756e 6974 732e 6d65 7461 2e64 6564 7570  units.meta.dedup
-00002470: 7266 0100 0058 0300 0000 6561 7472 6701  rf...X....eatrg.
-00002480: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002490: 756e 6974 732e 6d65 7461 2e65 6174 7268  units.meta.eatrh
-000024a0: 0100 0058 0200 0000 6566 7269 0100 0058  ...X....efri...X
-000024b0: 1600 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000024c0: 7473 2e6d 6574 612e 6566 726a 0100 0058  ts.meta.efrj...X
-000024d0: 0400 0000 656d 6974 726b 0100 0058 1800  ....emitrk...X..
-000024e0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000024f0: 2e6d 6574 612e 656d 6974 726c 0100 0058  .meta.emitrl...X
-00002500: 0500 0000 6772 6f75 7072 6d01 0000 5819  ....grouprm...X.
-00002510: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002520: 732e 6d65 7461 2e67 726f 7570 726e 0100  s.meta.grouprn..
-00002530: 0058 0700 0000 6772 6f75 7062 7972 6f01  .X....groupbyro.
-00002540: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002550: 756e 6974 732e 6d65 7461 2e67 726f 7570  units.meta.group
-00002560: 6279 7270 0100 0058 0300 0000 6966 6672  byrp...X....iffr
-00002570: 7101 0000 5817 0000 0072 6566 696e 6572  q...X....refiner
-00002580: 792e 756e 6974 732e 6d65 7461 2e69 6666  y.units.meta.iff
-00002590: 7272 0100 0058 0400 0000 6966 6670 7273  rr...X....iffprs
-000025a0: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
-000025b0: 2e75 6e69 7473 2e6d 6574 612e 6966 6670  .units.meta.iffp
-000025c0: 7274 0100 0058 0400 0000 6966 6673 7275  rt...X....iffsru
-000025d0: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
-000025e0: 2e75 6e69 7473 2e6d 6574 612e 6966 6673  .units.meta.iffs
-000025f0: 7276 0100 0058 0400 0000 6966 6678 7277  rv...X....iffxrw
-00002600: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
-00002610: 2e75 6e69 7473 2e6d 6574 612e 6966 6678  .units.meta.iffx
-00002620: 7278 0100 0058 0400 0000 6d61 785f 7279  rx...X....max_ry
-00002630: 0100 0058 1700 0000 7265 6669 6e65 7279  ...X....refinery
-00002640: 2e75 6e69 7473 2e6d 6574 612e 6d61 7872  .units.meta.maxr
-00002650: 7a01 0000 5804 0000 006d 696e 5f72 7b01  z...X....min_r{.
-00002660: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002670: 756e 6974 732e 6d65 7461 2e6d 696e 727c  units.meta.minr|
-00002680: 0100 0058 0300 0000 6d76 6372 7d01 0000  ...X....mvcr}...
-00002690: 5817 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000026a0: 6974 732e 6d65 7461 2e6d 7663 727e 0100  its.meta.mvcr~..
-000026b0: 0058 0300 0000 6d76 6772 7f01 0000 5817  .X....mvgr....X.
-000026c0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000026d0: 732e 6d65 7461 2e6d 7667 7280 0100 0058  s.meta.mvgr....X
-000026e0: 0300 0000 7061 6472 8101 0000 5817 0000  ....padr....X...
-000026f0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002700: 6d65 7461 2e70 6164 7282 0100 0058 0400  meta.padr....X..
-00002710: 0000 7069 636b 7283 0100 0058 1800 0000  ..pickr....X....
-00002720: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002730: 6574 612e 7069 636b 7284 0100 0058 0300  eta.pickr....X..
-00002740: 0000 706f 7072 8501 0000 5817 0000 0072  ..popr....X....r
-00002750: 6566 696e 6572 792e 756e 6974 732e 6d65  efinery.units.me
-00002760: 7461 2e70 6f70 7286 0100 0058 0400 0000  ta.popr....X....
-00002770: 7075 7368 7287 0100 0058 1800 0000 7265  pushr....X....re
-00002780: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-00002790: 612e 7075 7368 7288 0100 0058 0300 0000  a.pushr....X....
-000027a0: 7075 7472 8901 0000 5817 0000 0072 6566  putr....X....ref
-000027b0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-000027c0: 2e70 7574 728a 0100 0058 0500 0000 7175  .putr....X....qu
-000027d0: 6575 6572 8b01 0000 5819 0000 0072 6566  euer....X....ref
-000027e0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-000027f0: 2e71 7565 7565 728c 0100 0058 0600 0000  .queuer....X....
-00002800: 7265 6475 6365 728d 0100 0058 1a00 0000  reducer....X....
-00002810: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002820: 6574 612e 7265 6475 6365 728e 0100 0058  eta.reducer....X
-00002830: 0500 0000 7363 6f70 6572 8f01 0000 5819  ....scoper....X.
-00002840: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002850: 732e 6d65 7461 2e73 636f 7065 7290 0100  s.meta.scoper...
-00002860: 0058 0300 0000 7365 7072 9101 0000 5817  .X....sepr....X.
-00002870: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002880: 732e 6d65 7461 2e73 6570 7292 0100 0058  s.meta.sepr....X
-00002890: 0600 0000 736f 7274 6564 7293 0100 0058  ....sortedr....X
-000028a0: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000028b0: 7473 2e6d 6574 612e 736f 7274 6564 7294  ts.meta.sortedr.
-000028c0: 0100 0058 0400 0000 7377 6170 7295 0100  ...X....swapr...
-000028d0: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000028e0: 6e69 7473 2e6d 6574 612e 7377 6170 7296  nits.meta.swapr.
-000028f0: 0100 0058 0900 0000 7472 616e 7370 6f73  ...X....transpos
-00002900: 6572 9701 0000 581d 0000 0072 6566 696e  er....X....refin
-00002910: 6572 792e 756e 6974 732e 6d65 7461 2e74  ery.units.meta.t
-00002920: 7261 6e73 706f 7365 7298 0100 0058 0400  ransposer....X..
-00002930: 0000 7866 6363 7299 0100 0058 1800 0000  ..xfccr....X....
-00002940: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002950: 6574 612e 7866 6363 729a 0100 0058 0700  eta.xfccr....X..
-00002960: 0000 6175 746f 786f 7272 9b01 0000 581b  ..autoxorr....X.
-00002970: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002980: 732e 6d69 7363 2e61 7574 6f78 6f72 729c  s.misc.autoxorr.
-00002990: 0100 0058 0600 0000 636f 7570 6c65 729d  ...X....coupler.
-000029a0: 0100 0058 1a00 0000 7265 6669 6e65 7279  ...X....refinery
-000029b0: 2e75 6e69 7473 2e6d 6973 632e 636f 7570  .units.misc.coup
-000029c0: 6c65 729e 0100 0058 0700 0000 6461 7465  ler....X....date
-000029d0: 6669 7872 9f01 0000 581b 0000 0072 6566  fixr....X....ref
-000029e0: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
-000029f0: 2e64 6174 6566 6978 72a0 0100 0058 0300  .datefixr....X..
-00002a00: 0000 6472 7072 a101 0000 5817 0000 0072  ..drpr....X....r
-00002a10: 6566 696e 6572 792e 756e 6974 732e 6d69  efinery.units.mi
-00002a20: 7363 2e64 7270 72a2 0100 0058 0300 0000  sc.drpr....X....
-00002a30: 6e6f 7072 a301 0000 5817 0000 0072 6566  nopr....X....ref
-00002a40: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
-00002a50: 2e6e 6f70 72a4 0100 0058 0600 0000 7572  .nopr....X....ur
-00002a60: 6c66 6978 72a5 0100 0058 1a00 0000 7265  lfixr....X....re
-00002a70: 6669 6e65 7279 2e75 6e69 7473 2e6d 6973  finery.units.mis
-00002a80: 632e 7572 6c66 6978 72a6 0100 0058 0400  c.urlfixr....X..
-00002a90: 0000 786b 6579 72a7 0100 0058 1800 0000  ..xkeyr....X....
-00002aa0: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002ab0: 6973 632e 786b 6579 72a8 0100 0058 0e00  isc.xkeyr....X..
-00002ac0: 0000 6465 6f62 5f6a 735f 6172 7261 7973  ..deob_js_arrays
-00002ad0: 72a9 0100 0058 2400 0000 7265 6669 6e65  r....X$...refine
-00002ae0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
-00002af0: 7469 6f6e 2e6a 732e 6172 7261 7973 72aa  tion.js.arraysr.
-00002b00: 0100 0058 0f00 0000 6465 6f62 5f6a 735f  ...X....deob_js_
-00002b10: 6765 7461 7474 7272 ab01 0000 5825 0000  getattrr....X%..
-00002b20: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002b30: 6f62 6675 7363 6174 696f 6e2e 6a73 2e67  obfuscation.js.g
-00002b40: 6574 6174 7472 72ac 0100 0058 0e00 0000  etattrr....X....
-00002b50: 6465 6f62 5f6a 735f 7475 706c 6573 72ad  deob_js_tuplesr.
-00002b60: 0100 0058 2400 0000 7265 6669 6e65 7279  ...X$...refinery
-00002b70: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002b80: 6f6e 2e6a 732e 7475 706c 6573 72ae 0100  on.js.tuplesr...
-00002b90: 0058 0800 0000 6465 6f62 5f70 7331 72af  .X....deob_ps1r.
-00002ba0: 0100 0058 2200 0000 7265 6669 6e65 7279  ...X"...refinery
-00002bb0: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002bc0: 6f6e 2e70 7331 2e61 6c6c 72b0 0100 0058  on.ps1.allr....X
-00002bd0: 1100 0000 6465 6f62 5f70 7331 5f62 7261  ....deob_ps1_bra
-00002be0: 636b 6574 7372 b101 0000 5827 0000 0072  cketsr....X'...r
-00002bf0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002c00: 6675 7363 6174 696f 6e2e 7073 312e 6272  fuscation.ps1.br
-00002c10: 6163 6b65 7473 72b2 0100 0058 0e00 0000  acketsr....X....
-00002c20: 6465 6f62 5f70 7331 5f63 6173 6573 72b3  deob_ps1_casesr.
-00002c30: 0100 0058 2400 0000 7265 6669 6e65 7279  ...X$...refinery
-00002c40: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002c50: 6f6e 2e70 7331 2e63 6173 6573 72b4 0100  on.ps1.casesr...
-00002c60: 0058 0f00 0000 6465 6f62 5f70 7331 5f63  .X....deob_ps1_c
-00002c70: 6f6e 6361 7472 b501 0000 5825 0000 0072  oncatr....X%...r
-00002c80: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002c90: 6675 7363 6174 696f 6e2e 7073 312e 636f  fuscation.ps1.co
-00002ca0: 6e63 6174 72b6 0100 0058 0f00 0000 6465  ncatr....X....de
-00002cb0: 6f62 5f70 7331 5f65 7363 6170 6572 b701  ob_ps1_escaper..
-00002cc0: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
-00002cd0: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-00002ce0: 6e2e 7073 312e 6573 6361 7065 72b8 0100  n.ps1.escaper...
-00002cf0: 0058 0f00 0000 6465 6f62 5f70 7331 5f66  .X....deob_ps1_f
-00002d00: 6f72 6d61 7472 b901 0000 5825 0000 0072  ormatr....X%...r
-00002d10: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002d20: 6675 7363 6174 696f 6e2e 7073 312e 666f  fuscation.ps1.fo
-00002d30: 726d 6174 72ba 0100 0058 0f00 0000 6465  rmatr....X....de
-00002d40: 6f62 5f70 7331 5f69 6e76 6f6b 6572 bb01  ob_ps1_invoker..
-00002d50: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
-00002d60: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-00002d70: 6e2e 7073 312e 696e 766f 6b65 72bc 0100  n.ps1.invoker...
-00002d80: 0058 0f00 0000 6465 6f62 5f70 7331 5f73  .X....deob_ps1_s
-00002d90: 6563 7374 7272 bd01 0000 582b 0000 0072  ecstrr....X+...r
-00002da0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002db0: 6675 7363 6174 696f 6e2e 7073 312e 7365  fuscation.ps1.se
-00002dc0: 6375 7265 7374 7269 6e67 72be 0100 0058  curestringr....X
-00002dd0: 1600 0000 6465 6f62 5f70 7331 5f73 7472  ....deob_ps1_str
-00002de0: 696e 6772 6570 6c61 6365 72bf 0100 0058  ingreplacer....X
-00002df0: 2c00 0000 7265 6669 6e65 7279 2e75 6e69  ,...refinery.uni
-00002e00: 7473 2e6f 6266 7573 6361 7469 6f6e 2e70  ts.obfuscation.p
-00002e10: 7331 2e73 7472 696e 6772 6570 6c61 6365  s1.stringreplace
-00002e20: 72c0 0100 0058 1100 0000 6465 6f62 5f70  r....X....deob_p
-00002e30: 7331 5f74 7970 6563 6173 7472 c101 0000  s1_typecastr....
-00002e40: 5827 0000 0072 6566 696e 6572 792e 756e  X'...refinery.un
-00002e50: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00002e60: 7073 312e 7479 7065 6361 7374 72c2 0100  ps1.typecastr...
-00002e70: 0058 1000 0000 6465 6f62 5f70 7331 5f75  .X....deob_ps1_u
-00002e80: 6e63 7572 6c79 72c3 0100 0058 2600 0000  ncurlyr....X&...
-00002e90: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
-00002ea0: 6266 7573 6361 7469 6f6e 2e70 7331 2e75  bfuscation.ps1.u
-00002eb0: 6e63 7572 6c79 72c4 0100 0058 0800 0000  ncurlyr....X....
-00002ec0: 6465 6f62 5f76 6261 72c5 0100 0058 2200  deob_vbar....X".
-00002ed0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002ee0: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
-00002ef0: 2e61 6c6c 72c6 0100 0058 1300 0000 6465  .allr....X....de
-00002f00: 6f62 5f76 6261 5f61 7269 7468 6d65 7469  ob_vba_arithmeti
-00002f10: 6372 c701 0000 5829 0000 0072 6566 696e  cr....X)...refin
-00002f20: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00002f30: 6174 696f 6e2e 7662 612e 6172 6974 686d  ation.vba.arithm
-00002f40: 6574 6963 72c8 0100 0058 1100 0000 6465  eticr....X....de
-00002f50: 6f62 5f76 6261 5f62 7261 636b 6574 7372  ob_vba_bracketsr
-00002f60: c901 0000 5827 0000 0072 6566 696e 6572  ....X'...refiner
+000021c0: 2e70 656f 7665 726c 6179 724c 0100 0058  .peoverlayrL...X
+000021d0: 0400 0000 7065 7263 724d 0100 0058 1e00  ....percrM...X..
+000021e0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000021f0: 2e66 6f72 6d61 7473 2e70 652e 7065 7263  .formats.pe.perc
+00002200: 724e 0100 0058 0500 0000 7065 7369 6772  rN...X....pesigr
+00002210: 4f01 0000 581f 0000 0072 6566 696e 6572  O...X....refiner
+00002220: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00002230: 7065 2e70 6573 6967 7250 0100 0058 0700  pe.pesigrP...X..
+00002240: 0000 7065 7374 7269 7072 5101 0000 5821  ..pestriprQ...X!
+00002250: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002260: 732e 666f 726d 6174 732e 7065 2e70 6573  s.formats.pe.pes
+00002270: 7472 6970 7252 0100 0058 0500 0000 706b  triprR...X....pk
+00002280: 6373 3772 5301 0000 581c 0000 0072 6566  cs7rS...X....ref
+00002290: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+000022a0: 6174 732e 706b 6373 3772 5401 0000 5808  ats.pkcs7rT...X.
+000022b0: 0000 0070 6b63 7337 7369 6772 5501 0000  ...pkcs7sigrU...
+000022c0: 581f 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000022d0: 6974 732e 666f 726d 6174 732e 706b 6373  its.formats.pkcs
+000022e0: 3773 6967 7256 0100 0058 0500 0000 7374  7sigrV...X....st
+000022f0: 6567 6f72 5701 0000 581c 0000 0072 6566  egorW...X....ref
+00002300: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+00002310: 6174 732e 7374 6567 6f72 5801 0000 5807  ats.stegorX...X.
+00002320: 0000 0074 6e65 746d 746d 7259 0100 0058  ...tnetmtmrY...X
+00002330: 1e00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00002340: 7473 2e66 6f72 6d61 7473 2e74 6e65 746d  ts.formats.tnetm
+00002350: 746d 725a 0100 0058 0600 0000 7769 6e72  tmrZ...X....winr
+00002360: 6567 725b 0100 0058 1d00 0000 7265 6669  egr[...X....refi
+00002370: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00002380: 7473 2e77 696e 7265 6772 5c01 0000 5805  ts.winregr\...X.
+00002390: 0000 0078 7478 6d6c 725d 0100 0058 1a00  ...xtxmlr]...X..
+000023a0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000023b0: 2e66 6f72 6d61 7473 2e78 6d6c 725e 0100  .formats.xmlr^..
+000023c0: 0058 0300 0000 6e34 3072 5f01 0000 581a  .X....n40r_...X.
+000023d0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000023e0: 732e 6d61 6c77 6172 652e 6e34 3072 6001  s.malware.n40r`.
+000023f0: 0000 5804 0000 0063 686f 7072 6101 0000  ..X....chopra...
+00002400: 5818 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00002410: 6974 732e 6d65 7461 2e63 686f 7072 6201  its.meta.choprb.
+00002420: 0000 5802 0000 0063 6d72 6301 0000 5816  ..X....cmrc...X.
+00002430: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002440: 732e 6d65 7461 2e63 6d72 6401 0000 5804  s.meta.cmrd...X.
+00002450: 0000 0063 756c 6c72 6501 0000 5818 0000  ...cullre...X...
+00002460: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002470: 6d65 7461 2e63 756c 6c72 6601 0000 5805  meta.cullrf...X.
+00002480: 0000 0064 6564 7570 7267 0100 0058 1900  ...deduprg...X..
+00002490: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000024a0: 2e6d 6574 612e 6465 6475 7072 6801 0000  .meta.deduprh...
+000024b0: 5803 0000 0065 6174 7269 0100 0058 1700  X....eatri...X..
+000024c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000024d0: 2e6d 6574 612e 6561 7472 6a01 0000 5802  .meta.eatrj...X.
+000024e0: 0000 0065 6672 6b01 0000 5816 0000 0072  ...efrk...X....r
+000024f0: 6566 696e 6572 792e 756e 6974 732e 6d65  efinery.units.me
+00002500: 7461 2e65 6672 6c01 0000 5804 0000 0065  ta.efrl...X....e
+00002510: 6d69 7472 6d01 0000 5818 0000 0072 6566  mitrm...X....ref
+00002520: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
+00002530: 2e65 6d69 7472 6e01 0000 5805 0000 0067  .emitrn...X....g
+00002540: 726f 7570 726f 0100 0058 1900 0000 7265  roupro...X....re
+00002550: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+00002560: 612e 6772 6f75 7072 7001 0000 5807 0000  a.grouprp...X...
+00002570: 0067 726f 7570 6279 7271 0100 0058 1b00  .groupbyrq...X..
+00002580: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002590: 2e6d 6574 612e 6772 6f75 7062 7972 7201  .meta.groupbyrr.
+000025a0: 0000 5803 0000 0069 6666 7273 0100 0058  ..X....iffrs...X
+000025b0: 1700 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+000025c0: 7473 2e6d 6574 612e 6966 6672 7401 0000  ts.meta.iffrt...
+000025d0: 5804 0000 0069 6666 7072 7501 0000 5818  X....iffpru...X.
+000025e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000025f0: 732e 6d65 7461 2e69 6666 7072 7601 0000  s.meta.iffprv...
+00002600: 5804 0000 0069 6666 7372 7701 0000 5818  X....iffsrw...X.
+00002610: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002620: 732e 6d65 7461 2e69 6666 7372 7801 0000  s.meta.iffsrx...
+00002630: 5804 0000 0069 6666 7872 7901 0000 5818  X....iffxry...X.
+00002640: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002650: 732e 6d65 7461 2e69 6666 7872 7a01 0000  s.meta.iffxrz...
+00002660: 5804 0000 006d 6178 5f72 7b01 0000 5817  X....max_r{...X.
+00002670: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002680: 732e 6d65 7461 2e6d 6178 727c 0100 0058  s.meta.maxr|...X
+00002690: 0400 0000 6d69 6e5f 727d 0100 0058 1700  ....min_r}...X..
+000026a0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000026b0: 2e6d 6574 612e 6d69 6e72 7e01 0000 5803  .meta.minr~...X.
+000026c0: 0000 006d 7663 727f 0100 0058 1700 0000  ...mvcr....X....
+000026d0: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
+000026e0: 6574 612e 6d76 6372 8001 0000 5803 0000  eta.mvcr....X...
+000026f0: 006d 7667 7281 0100 0058 1700 0000 7265  .mvgr....X....re
+00002700: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+00002710: 612e 6d76 6772 8201 0000 5803 0000 0070  a.mvgr....X....p
+00002720: 6164 7283 0100 0058 1700 0000 7265 6669  adr....X....refi
+00002730: 6e65 7279 2e75 6e69 7473 2e6d 6574 612e  nery.units.meta.
+00002740: 7061 6472 8401 0000 5804 0000 0070 6963  padr....X....pic
+00002750: 6b72 8501 0000 5818 0000 0072 6566 696e  kr....X....refin
+00002760: 6572 792e 756e 6974 732e 6d65 7461 2e70  ery.units.meta.p
+00002770: 6963 6b72 8601 0000 5803 0000 0070 6f70  ickr....X....pop
+00002780: 7287 0100 0058 1700 0000 7265 6669 6e65  r....X....refine
+00002790: 7279 2e75 6e69 7473 2e6d 6574 612e 706f  ry.units.meta.po
+000027a0: 7072 8801 0000 5804 0000 0070 7573 6872  pr....X....pushr
+000027b0: 8901 0000 5818 0000 0072 6566 696e 6572  ....X....refiner
+000027c0: 792e 756e 6974 732e 6d65 7461 2e70 7573  y.units.meta.pus
+000027d0: 6872 8a01 0000 5803 0000 0070 7574 728b  hr....X....putr.
+000027e0: 0100 0058 1700 0000 7265 6669 6e65 7279  ...X....refinery
+000027f0: 2e75 6e69 7473 2e6d 6574 612e 7075 7472  .units.meta.putr
+00002800: 8c01 0000 5805 0000 0071 7565 7565 728d  ....X....queuer.
+00002810: 0100 0058 1900 0000 7265 6669 6e65 7279  ...X....refinery
+00002820: 2e75 6e69 7473 2e6d 6574 612e 7175 6575  .units.meta.queu
+00002830: 6572 8e01 0000 5806 0000 0072 6564 7563  er....X....reduc
+00002840: 6572 8f01 0000 581a 0000 0072 6566 696e  er....X....refin
+00002850: 6572 792e 756e 6974 732e 6d65 7461 2e72  ery.units.meta.r
+00002860: 6564 7563 6572 9001 0000 5805 0000 0073  educer....X....s
+00002870: 636f 7065 7291 0100 0058 1900 0000 7265  coper....X....re
+00002880: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+00002890: 612e 7363 6f70 6572 9201 0000 5803 0000  a.scoper....X...
+000028a0: 0073 6570 7293 0100 0058 1700 0000 7265  .sepr....X....re
+000028b0: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+000028c0: 612e 7365 7072 9401 0000 5806 0000 0073  a.sepr....X....s
+000028d0: 6f72 7465 6472 9501 0000 581a 0000 0072  ortedr....X....r
+000028e0: 6566 696e 6572 792e 756e 6974 732e 6d65  efinery.units.me
+000028f0: 7461 2e73 6f72 7465 6472 9601 0000 5804  ta.sortedr....X.
+00002900: 0000 0073 7761 7072 9701 0000 5818 0000  ...swapr....X...
+00002910: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002920: 6d65 7461 2e73 7761 7072 9801 0000 5809  meta.swapr....X.
+00002930: 0000 0074 7261 6e73 706f 7365 7299 0100  ...transposer...
+00002940: 0058 1d00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00002950: 6e69 7473 2e6d 6574 612e 7472 616e 7370  nits.meta.transp
+00002960: 6f73 6572 9a01 0000 5804 0000 0078 6663  oser....X....xfc
+00002970: 6372 9b01 0000 5818 0000 0072 6566 696e  cr....X....refin
+00002980: 6572 792e 756e 6974 732e 6d65 7461 2e78  ery.units.meta.x
+00002990: 6663 6372 9c01 0000 5807 0000 0061 7574  fccr....X....aut
+000029a0: 6f78 6f72 729d 0100 0058 1b00 0000 7265  oxorr....X....re
+000029b0: 6669 6e65 7279 2e75 6e69 7473 2e6d 6973  finery.units.mis
+000029c0: 632e 6175 746f 786f 7272 9e01 0000 5806  c.autoxorr....X.
+000029d0: 0000 0063 6f75 706c 6572 9f01 0000 581a  ...coupler....X.
+000029e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000029f0: 732e 6d69 7363 2e63 6f75 706c 6572 a001  s.misc.coupler..
+00002a00: 0000 5807 0000 0064 6174 6566 6978 72a1  ..X....datefixr.
+00002a10: 0100 0058 1b00 0000 7265 6669 6e65 7279  ...X....refinery
+00002a20: 2e75 6e69 7473 2e6d 6973 632e 6461 7465  .units.misc.date
+00002a30: 6669 7872 a201 0000 5803 0000 0064 7270  fixr....X....drp
+00002a40: 72a3 0100 0058 1700 0000 7265 6669 6e65  r....X....refine
+00002a50: 7279 2e75 6e69 7473 2e6d 6973 632e 6472  ry.units.misc.dr
+00002a60: 7072 a401 0000 5803 0000 006e 6f70 72a5  pr....X....nopr.
+00002a70: 0100 0058 1700 0000 7265 6669 6e65 7279  ...X....refinery
+00002a80: 2e75 6e69 7473 2e6d 6973 632e 6e6f 7072  .units.misc.nopr
+00002a90: a601 0000 5806 0000 0075 726c 6669 7872  ....X....urlfixr
+00002aa0: a701 0000 581a 0000 0072 6566 696e 6572  ....X....refiner
+00002ab0: 792e 756e 6974 732e 6d69 7363 2e75 726c  y.units.misc.url
+00002ac0: 6669 7872 a801 0000 5804 0000 0078 6b65  fixr....X....xke
+00002ad0: 7972 a901 0000 5818 0000 0072 6566 696e  yr....X....refin
+00002ae0: 6572 792e 756e 6974 732e 6d69 7363 2e78  ery.units.misc.x
+00002af0: 6b65 7972 aa01 0000 580e 0000 0064 656f  keyr....X....deo
+00002b00: 625f 6a73 5f61 7272 6179 7372 ab01 0000  b_js_arraysr....
+00002b10: 5824 0000 0072 6566 696e 6572 792e 756e  X$...refinery.un
+00002b20: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002b30: 6a73 2e61 7272 6179 7372 ac01 0000 580f  js.arraysr....X.
+00002b40: 0000 0064 656f 625f 6a73 5f67 6574 6174  ...deob_js_getat
+00002b50: 7472 72ad 0100 0058 2500 0000 7265 6669  trr....X%...refi
+00002b60: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
+00002b70: 6361 7469 6f6e 2e6a 732e 6765 7461 7474  cation.js.getatt
+00002b80: 7272 ae01 0000 580e 0000 0064 656f 625f  rr....X....deob_
+00002b90: 6a73 5f74 7570 6c65 7372 af01 0000 5824  js_tuplesr....X$
+00002ba0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002bb0: 732e 6f62 6675 7363 6174 696f 6e2e 6a73  s.obfuscation.js
+00002bc0: 2e74 7570 6c65 7372 b001 0000 5808 0000  .tuplesr....X...
+00002bd0: 0064 656f 625f 7073 3172 b101 0000 5822  .deob_ps1r....X"
+00002be0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002bf0: 732e 6f62 6675 7363 6174 696f 6e2e 7073  s.obfuscation.ps
+00002c00: 312e 616c 6c72 b201 0000 5813 0000 0064  1.allr....X....d
+00002c10: 656f 625f 7073 315f 6236 3463 6f6e 7665  eob_ps1_b64conve
+00002c20: 7274 72b3 0100 0058 2900 0000 7265 6669  rtr....X)...refi
+00002c30: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
+00002c40: 6361 7469 6f6e 2e70 7331 2e62 3634 636f  cation.ps1.b64co
+00002c50: 6e76 6572 7472 b401 0000 5811 0000 0064  nvertr....X....d
+00002c60: 656f 625f 7073 315f 6272 6163 6b65 7473  eob_ps1_brackets
+00002c70: 72b5 0100 0058 2700 0000 7265 6669 6e65  r....X'...refine
+00002c80: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
+00002c90: 7469 6f6e 2e70 7331 2e62 7261 636b 6574  tion.ps1.bracket
+00002ca0: 7372 b601 0000 580e 0000 0064 656f 625f  sr....X....deob_
+00002cb0: 7073 315f 6361 7365 7372 b701 0000 5824  ps1_casesr....X$
+00002cc0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002cd0: 732e 6f62 6675 7363 6174 696f 6e2e 7073  s.obfuscation.ps
+00002ce0: 312e 6361 7365 7372 b801 0000 580f 0000  1.casesr....X...
+00002cf0: 0064 656f 625f 7073 315f 636f 6e63 6174  .deob_ps1_concat
+00002d00: 72b9 0100 0058 2500 0000 7265 6669 6e65  r....X%...refine
+00002d10: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
+00002d20: 7469 6f6e 2e70 7331 2e63 6f6e 6361 7472  tion.ps1.concatr
+00002d30: ba01 0000 5812 0000 0064 656f 625f 7073  ....X....deob_ps
+00002d40: 315f 656e 636f 6469 6e67 7372 bb01 0000  1_encodingsr....
+00002d50: 5828 0000 0072 6566 696e 6572 792e 756e  X(...refinery.un
+00002d60: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002d70: 7073 312e 656e 636f 6469 6e67 7372 bc01  ps1.encodingsr..
+00002d80: 0000 580f 0000 0064 656f 625f 7073 315f  ..X....deob_ps1_
+00002d90: 6573 6361 7065 72bd 0100 0058 2500 0000  escaper....X%...
+00002da0: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
+00002db0: 6266 7573 6361 7469 6f6e 2e70 7331 2e65  bfuscation.ps1.e
+00002dc0: 7363 6170 6572 be01 0000 580f 0000 0064  scaper....X....d
+00002dd0: 656f 625f 7073 315f 666f 726d 6174 72bf  eob_ps1_formatr.
+00002de0: 0100 0058 2500 0000 7265 6669 6e65 7279  ...X%...refinery
+00002df0: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
+00002e00: 6f6e 2e70 7331 2e66 6f72 6d61 7472 c001  on.ps1.formatr..
+00002e10: 0000 580f 0000 0064 656f 625f 7073 315f  ..X....deob_ps1_
+00002e20: 696e 766f 6b65 72c1 0100 0058 2500 0000  invoker....X%...
+00002e30: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
+00002e40: 6266 7573 6361 7469 6f6e 2e70 7331 2e69  bfuscation.ps1.i
+00002e50: 6e76 6f6b 6572 c201 0000 580f 0000 0064  nvoker....X....d
+00002e60: 656f 625f 7073 315f 7365 6373 7472 72c3  eob_ps1_secstrr.
+00002e70: 0100 0058 2b00 0000 7265 6669 6e65 7279  ...X+...refinery
+00002e80: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
+00002e90: 6f6e 2e70 7331 2e73 6563 7572 6573 7472  on.ps1.securestr
+00002ea0: 696e 6772 c401 0000 5816 0000 0064 656f  ingr....X....deo
+00002eb0: 625f 7073 315f 7374 7269 6e67 7265 706c  b_ps1_stringrepl
+00002ec0: 6163 6572 c501 0000 582c 0000 0072 6566  acer....X,...ref
+00002ed0: 696e 6572 792e 756e 6974 732e 6f62 6675  inery.units.obfu
+00002ee0: 7363 6174 696f 6e2e 7073 312e 7374 7269  scation.ps1.stri
+00002ef0: 6e67 7265 706c 6163 6572 c601 0000 5811  ngreplacer....X.
+00002f00: 0000 0064 656f 625f 7073 315f 7479 7065  ...deob_ps1_type
+00002f10: 6361 7374 72c7 0100 0058 2700 0000 7265  castr....X'...re
+00002f20: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
+00002f30: 7573 6361 7469 6f6e 2e70 7331 2e74 7970  uscation.ps1.typ
+00002f40: 6563 6173 7472 c801 0000 5810 0000 0064  ecastr....X....d
+00002f50: 656f 625f 7073 315f 756e 6375 726c 7972  eob_ps1_uncurlyr
+00002f60: c901 0000 5826 0000 0072 6566 696e 6572  ....X&...refiner
 00002f70: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
-00002f80: 696f 6e2e 7662 612e 6272 6163 6b65 7473  ion.vba.brackets
-00002f90: 72ca 0100 0058 1600 0000 6465 6f62 5f76  r....X....deob_v
-00002fa0: 6261 5f63 6861 725f 6675 6e63 7469 6f6e  ba_char_function
-00002fb0: 72cb 0100 0058 2300 0000 7265 6669 6e65  r....X#...refine
-00002fc0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
-00002fd0: 7469 6f6e 2e76 6261 2e63 6861 7272 cc01  tion.vba.charr..
-00002fe0: 0000 5811 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
-00002ff0: 636f 6d6d 656e 7473 72cd 0100 0058 2700  commentsr....X'.
-00003000: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00003010: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
-00003020: 2e63 6f6d 6d65 6e74 7372 ce01 0000 580f  .commentsr....X.
-00003030: 0000 0064 656f 625f 7662 615f 636f 6e63  ...deob_vba_conc
-00003040: 6174 72cf 0100 0058 2500 0000 7265 6669  atr....X%...refi
-00003050: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
-00003060: 6361 7469 6f6e 2e76 6261 2e63 6f6e 6361  cation.vba.conca
-00003070: 7472 d001 0000 5812 0000 0064 656f 625f  tr....X....deob_
-00003080: 7662 615f 636f 6e73 7461 6e74 7372 d101  vba_constantsr..
-00003090: 0000 5828 0000 0072 6566 696e 6572 792e  ..X(...refinery.
-000030a0: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-000030b0: 6e2e 7662 612e 636f 6e73 7461 6e74 7372  n.vba.constantsr
-000030c0: d201 0000 5818 0000 0064 656f 625f 7662  ....X....deob_vb
-000030d0: 615f 6475 6d6d 795f 7661 7269 6162 6c65  a_dummy_variable
-000030e0: 7372 d301 0000 5826 0000 0072 6566 696e  sr....X&...refin
-000030f0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00003100: 6174 696f 6e2e 7662 612e 6475 6d6d 6965  ation.vba.dummie
-00003110: 7372 d401 0000 5816 0000 0064 656f 625f  sr....X....deob_
-00003120: 7662 615f 7374 7269 6e67 7265 706c 6163  vba_stringreplac
-00003130: 6572 d501 0000 582c 0000 0072 6566 696e  er....X,...refin
-00003140: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00003150: 6174 696f 6e2e 7662 612e 7374 7269 6e67  ation.vba.string
-00003160: 7265 706c 6163 6572 d601 0000 5816 0000  replacer....X...
-00003170: 0064 656f 625f 7662 615f 7374 7269 6e67  .deob_vba_string
-00003180: 7265 7665 7273 6572 d701 0000 582c 0000  reverser....X,..
-00003190: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000031a0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
-000031b0: 7374 7269 6e67 7265 7665 7273 6572 d801  stringreverser..
-000031c0: 0000 5815 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
-000031d0: 6368 725f 6c69 7465 7261 6c73 72d9 0100  chr_literalsr...
-000031e0: 0058 2200 0000 7265 6669 6e65 7279 2e75  .X"...refinery.u
-000031f0: 6e69 7473 2e6f 6266 7573 6361 7469 6f6e  nits.obfuscation
-00003200: 2e76 6261 2e76 6261 72da 0100 0058 0500  .vba.vbar....X..
-00003210: 0000 6361 7276 6572 db01 0000 581c 0000  ..carver....X...
-00003220: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00003230: 7061 7474 6572 6e2e 6361 7276 6572 dc01  pattern.carver..
-00003240: 0000 5808 0000 0063 6172 7665 5f37 7a72  ..X....carve_7zr
-00003250: dd01 0000 581f 0000 0072 6566 696e 6572  ....X....refiner
-00003260: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
-00003270: 6361 7276 655f 377a 72de 0100 0058 0a00  carve_7zr....X..
-00003280: 0000 6361 7276 655f 6a73 6f6e 72df 0100  ..carve_jsonr...
-00003290: 0058 2100 0000 7265 6669 6e65 7279 2e75  .X!...refinery.u
-000032a0: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
-000032b0: 7665 5f6a 736f 6e72 e001 0000 5809 0000  ve_jsonr....X...
-000032c0: 0063 6172 7665 5f6c 6e6b 72e1 0100 0058  .carve_lnkr....X
-000032d0: 2000 0000 7265 6669 6e65 7279 2e75 6e69   ...refinery.uni
-000032e0: 7473 2e70 6174 7465 726e 2e63 6172 7665  ts.pattern.carve
-000032f0: 5f6c 6e6b 72e2 0100 0058 0800 0000 6361  _lnkr....X....ca
-00003300: 7276 655f 7065 72e3 0100 0058 1f00 0000  rve_per....X....
-00003310: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-00003320: 6174 7465 726e 2e63 6172 7665 5f70 6572  attern.carve_per
-00003330: e401 0000 5809 0000 0063 6172 7665 5f72  ....X....carve_r
-00003340: 7466 72e5 0100 0058 2000 0000 7265 6669  tfr....X ...refi
-00003350: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-00003360: 726e 2e63 6172 7665 5f72 7466 72e6 0100  rn.carve_rtfr...
-00003370: 0058 0900 0000 6361 7276 655f 786d 6c72  .X....carve_xmlr
-00003380: e701 0000 5820 0000 0072 6566 696e 6572  ....X ...refiner
-00003390: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
-000033a0: 6361 7276 655f 786d 6c72 e801 0000 5809  carve_xmlr....X.
-000033b0: 0000 0063 6172 7665 5f7a 6970 72e9 0100  ...carve_zipr...
-000033c0: 0058 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
-000033d0: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
-000033e0: 7665 5f7a 6970 72ea 0100 0058 0600 0000  ve_zipr....X....
-000033f0: 6465 6661 6e67 72eb 0100 0058 1d00 0000  defangr....X....
-00003400: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-00003410: 6174 7465 726e 2e64 6566 616e 6772 ec01  attern.defangr..
-00003420: 0000 5809 0000 0064 6e73 646f 6d61 696e  ..X....dnsdomain
-00003430: 72ed 0100 0058 2000 0000 7265 6669 6e65  r....X ...refine
-00003440: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-00003450: 2e64 6e73 646f 6d61 696e 72ee 0100 0058  .dnsdomainr....X
-00003460: 0900 0000 6d69 6d65 776f 7264 7372 ef01  ....mimewordsr..
-00003470: 0000 5820 0000 0072 6566 696e 6572 792e  ..X ...refinery.
-00003480: 756e 6974 732e 7061 7474 6572 6e2e 6d69  units.pattern.mi
-00003490: 6d65 776f 7264 7372 f001 0000 5807 0000  mewordsr....X...
-000034a0: 0072 6573 706c 6974 72f1 0100 0058 1e00  .resplitr....X..
-000034b0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000034c0: 2e70 6174 7465 726e 2e72 6573 706c 6974  .pattern.resplit
-000034d0: 72f2 0100 0058 0500 0000 7265 7375 6272  r....X....resubr
-000034e0: f301 0000 581c 0000 0072 6566 696e 6572  ....X....refiner
-000034f0: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
-00003500: 7265 7375 6272 f401 0000 5803 0000 0072  resubr....X....r
-00003510: 6578 72f5 0100 0058 1a00 0000 7265 6669  exr....X....refi
-00003520: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-00003530: 726e 2e72 6578 72f6 0100 0058 0600 0000  rn.rexr....X....
-00003540: 7374 7275 6374 72f7 0100 0058 2400 0000  structr....X$...
+00002f80: 696f 6e2e 7073 312e 756e 6375 726c 7972  ion.ps1.uncurlyr
+00002f90: ca01 0000 5808 0000 0064 656f 625f 7662  ....X....deob_vb
+00002fa0: 6172 cb01 0000 5822 0000 0072 6566 696e  ar....X"...refin
+00002fb0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+00002fc0: 6174 696f 6e2e 7662 612e 616c 6c72 cc01  ation.vba.allr..
+00002fd0: 0000 5813 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
+00002fe0: 6172 6974 686d 6574 6963 72cd 0100 0058  arithmeticr....X
+00002ff0: 2900 0000 7265 6669 6e65 7279 2e75 6e69  )...refinery.uni
+00003000: 7473 2e6f 6266 7573 6361 7469 6f6e 2e76  ts.obfuscation.v
+00003010: 6261 2e61 7269 7468 6d65 7469 6372 ce01  ba.arithmeticr..
+00003020: 0000 5811 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
+00003030: 6272 6163 6b65 7473 72cf 0100 0058 2700  bracketsr....X'.
+00003040: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003050: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
+00003060: 2e62 7261 636b 6574 7372 d001 0000 5816  .bracketsr....X.
+00003070: 0000 0064 656f 625f 7662 615f 6368 6172  ...deob_vba_char
+00003080: 5f66 756e 6374 696f 6e72 d101 0000 5823  _functionr....X#
+00003090: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000030a0: 732e 6f62 6675 7363 6174 696f 6e2e 7662  s.obfuscation.vb
+000030b0: 612e 6368 6172 72d2 0100 0058 1100 0000  a.charr....X....
+000030c0: 6465 6f62 5f76 6261 5f63 6f6d 6d65 6e74  deob_vba_comment
+000030d0: 7372 d301 0000 5827 0000 0072 6566 696e  sr....X'...refin
+000030e0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+000030f0: 6174 696f 6e2e 7662 612e 636f 6d6d 656e  ation.vba.commen
+00003100: 7473 72d4 0100 0058 0f00 0000 6465 6f62  tsr....X....deob
+00003110: 5f76 6261 5f63 6f6e 6361 7472 d501 0000  _vba_concatr....
+00003120: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
+00003130: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00003140: 7662 612e 636f 6e63 6174 72d6 0100 0058  vba.concatr....X
+00003150: 1200 0000 6465 6f62 5f76 6261 5f63 6f6e  ....deob_vba_con
+00003160: 7374 616e 7473 72d7 0100 0058 2800 0000  stantsr....X(...
+00003170: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
+00003180: 6266 7573 6361 7469 6f6e 2e76 6261 2e63  bfuscation.vba.c
+00003190: 6f6e 7374 616e 7473 72d8 0100 0058 1800  onstantsr....X..
+000031a0: 0000 6465 6f62 5f76 6261 5f64 756d 6d79  ..deob_vba_dummy
+000031b0: 5f76 6172 6961 626c 6573 72d9 0100 0058  _variablesr....X
+000031c0: 2600 0000 7265 6669 6e65 7279 2e75 6e69  &...refinery.uni
+000031d0: 7473 2e6f 6266 7573 6361 7469 6f6e 2e76  ts.obfuscation.v
+000031e0: 6261 2e64 756d 6d69 6573 72da 0100 0058  ba.dummiesr....X
+000031f0: 1600 0000 6465 6f62 5f76 6261 5f73 7472  ....deob_vba_str
+00003200: 696e 6772 6570 6c61 6365 72db 0100 0058  ingreplacer....X
+00003210: 2c00 0000 7265 6669 6e65 7279 2e75 6e69  ,...refinery.uni
+00003220: 7473 2e6f 6266 7573 6361 7469 6f6e 2e76  ts.obfuscation.v
+00003230: 6261 2e73 7472 696e 6772 6570 6c61 6365  ba.stringreplace
+00003240: 72dc 0100 0058 1600 0000 6465 6f62 5f76  r....X....deob_v
+00003250: 6261 5f73 7472 696e 6772 6576 6572 7365  ba_stringreverse
+00003260: 72dd 0100 0058 2c00 0000 7265 6669 6e65  r....X,...refine
+00003270: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
+00003280: 7469 6f6e 2e76 6261 2e73 7472 696e 6772  tion.vba.stringr
+00003290: 6576 6572 7365 72de 0100 0058 1500 0000  everser....X....
+000032a0: 6465 6f62 5f76 6261 5f63 6872 5f6c 6974  deob_vba_chr_lit
+000032b0: 6572 616c 7372 df01 0000 5822 0000 0072  eralsr....X"...r
+000032c0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
+000032d0: 6675 7363 6174 696f 6e2e 7662 612e 7662  fuscation.vba.vb
+000032e0: 6172 e001 0000 5805 0000 0063 6172 7665  ar....X....carve
+000032f0: 72e1 0100 0058 1c00 0000 7265 6669 6e65  r....X....refine
+00003300: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
+00003310: 2e63 6172 7665 72e2 0100 0058 0800 0000  .carver....X....
+00003320: 6361 7276 655f 377a 72e3 0100 0058 1f00  carve_7zr....X..
+00003330: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003340: 2e70 6174 7465 726e 2e63 6172 7665 5f37  .pattern.carve_7
+00003350: 7a72 e401 0000 580a 0000 0063 6172 7665  zr....X....carve
+00003360: 5f6a 736f 6e72 e501 0000 5821 0000 0072  _jsonr....X!...r
+00003370: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
+00003380: 7474 6572 6e2e 6361 7276 655f 6a73 6f6e  ttern.carve_json
+00003390: 72e6 0100 0058 0900 0000 6361 7276 655f  r....X....carve_
+000033a0: 6c6e 6b72 e701 0000 5820 0000 0072 6566  lnkr....X ...ref
+000033b0: 696e 6572 792e 756e 6974 732e 7061 7474  inery.units.patt
+000033c0: 6572 6e2e 6361 7276 655f 6c6e 6b72 e801  ern.carve_lnkr..
+000033d0: 0000 5808 0000 0063 6172 7665 5f70 6572  ..X....carve_per
+000033e0: e901 0000 581f 0000 0072 6566 696e 6572  ....X....refiner
+000033f0: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+00003400: 6361 7276 655f 7065 72ea 0100 0058 0900  carve_per....X..
+00003410: 0000 6361 7276 655f 7274 6672 eb01 0000  ..carve_rtfr....
+00003420: 5820 0000 0072 6566 696e 6572 792e 756e  X ...refinery.un
+00003430: 6974 732e 7061 7474 6572 6e2e 6361 7276  its.pattern.carv
+00003440: 655f 7274 6672 ec01 0000 5809 0000 0063  e_rtfr....X....c
+00003450: 6172 7665 5f78 6d6c 72ed 0100 0058 2000  arve_xmlr....X .
+00003460: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003470: 2e70 6174 7465 726e 2e63 6172 7665 5f78  .pattern.carve_x
+00003480: 6d6c 72ee 0100 0058 0900 0000 6361 7276  mlr....X....carv
+00003490: 655f 7a69 7072 ef01 0000 5820 0000 0072  e_zipr....X ...r
+000034a0: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
+000034b0: 7474 6572 6e2e 6361 7276 655f 7a69 7072  ttern.carve_zipr
+000034c0: f001 0000 5806 0000 0064 6566 616e 6772  ....X....defangr
+000034d0: f101 0000 581d 0000 0072 6566 696e 6572  ....X....refiner
+000034e0: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+000034f0: 6465 6661 6e67 72f2 0100 0058 0900 0000  defangr....X....
+00003500: 646e 7364 6f6d 6169 6e72 f301 0000 5820  dnsdomainr....X 
+00003510: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003520: 732e 7061 7474 6572 6e2e 646e 7364 6f6d  s.pattern.dnsdom
+00003530: 6169 6e72 f401 0000 5809 0000 006d 696d  ainr....X....mim
+00003540: 6577 6f72 6473 72f5 0100 0058 2000 0000  ewordsr....X ...
 00003550: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-00003560: 6174 7465 726e 2e73 7472 7563 745f 7061  attern.struct_pa
-00003570: 7273 6572 72f8 0100 0058 0800 0000 7375  rserr....X....su
-00003580: 6266 696c 6573 72f9 0100 0058 1f00 0000  bfilesr....X....
-00003590: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-000035a0: 6174 7465 726e 2e73 7562 6669 6c65 7372  attern.subfilesr
-000035b0: fa01 0000 5809 0000 0075 726c 6775 6172  ....X....urlguar
-000035c0: 6473 72fb 0100 0058 2000 0000 7265 6669  dsr....X ...refi
-000035d0: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-000035e0: 726e 2e75 726c 6775 6172 6473 72fc 0100  rn.urlguardsr...
-000035f0: 0058 0300 0000 7874 7072 fd01 0000 581a  .X....xtpr....X.
-00003600: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00003610: 732e 7061 7474 6572 6e2e 7874 7072 fe01  s.pattern.xtpr..
-00003620: 0000 5803 0000 0078 7477 72ff 0100 0058  ..X....xtwr....X
-00003630: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00003640: 7473 2e70 6174 7465 726e 2e78 7477 7200  ts.pattern.xtwr.
-00003650: 0200 0058 0300 0000 6173 6d72 0102 0000  ...X....asmr....
-00003660: 5818 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00003670: 6974 732e 7369 6e6b 732e 6173 6d72 0202  its.sinks.asmr..
-00003680: 0000 5804 0000 0064 756d 7072 0302 0000  ..X....dumpr....
-00003690: 5819 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000036a0: 6974 732e 7369 6e6b 732e 6475 6d70 7204  its.sinks.dumpr.
-000036b0: 0200 0058 0500 0000 6965 6d61 7072 0502  ...X....iemapr..
-000036c0: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
-000036d0: 756e 6974 732e 7369 6e6b 732e 6965 6d61  units.sinks.iema
-000036e0: 7072 0602 0000 5804 0000 0070 6565 6b72  pr....X....peekr
-000036f0: 0702 0000 5819 0000 0072 6566 696e 6572  ....X....refiner
-00003700: 792e 756e 6974 732e 7369 6e6b 732e 7065  y.units.sinks.pe
-00003710: 656b 7208 0200 0058 0900 0000 7070 6a73  ekr....X....ppjs
-00003720: 6372 6970 7472 0902 0000 581e 0000 0072  criptr....X....r
-00003730: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
-00003740: 6e6b 732e 7070 6a73 6372 6970 7472 0a02  nks.ppjscriptr..
-00003750: 0000 5806 0000 0070 706a 736f 6e72 0b02  ..X....ppjsonr..
-00003760: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00003770: 756e 6974 732e 7369 6e6b 732e 7070 6a73  units.sinks.ppjs
-00003780: 6f6e 720c 0200 0058 0500 0000 7070 786d  onr....X....ppxm
-00003790: 6c72 0d02 0000 581a 0000 0072 6566 696e  lr....X....refin
-000037a0: 6572 792e 756e 6974 732e 7369 6e6b 732e  ery.units.sinks.
-000037b0: 7070 786d 6c72 0e02 0000 5803 0000 0063  ppxmlr....X....c
-000037c0: 6361 720f 0200 0058 1a00 0000 7265 6669  car....X....refi
-000037d0: 6e65 7279 2e75 6e69 7473 2e73 7472 696e  nery.units.strin
-000037e0: 6773 2e63 6361 7210 0200 0058 0300 0000  gs.ccar....X....
-000037f0: 6363 7072 1102 0000 581a 0000 0072 6566  ccpr....X....ref
-00003800: 696e 6572 792e 756e 6974 732e 7374 7269  inery.units.stri
-00003810: 6e67 732e 6363 7072 1202 0000 5804 0000  ngs.ccpr....X...
-00003820: 0063 666d 7472 1302 0000 581b 0000 0072  .cfmtr....X....r
-00003830: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
-00003840: 7269 6e67 732e 6366 6d74 7214 0200 0058  rings.cfmtr....X
-00003850: 0600 0000 636c 6f77 6572 7215 0200 0058  ....clowerr....X
-00003860: 1d00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00003870: 7473 2e73 7472 696e 6773 2e63 6c6f 7765  ts.strings.clowe
-00003880: 7272 1602 0000 5805 0000 0063 7377 6170  rr....X....cswap
-00003890: 7217 0200 0058 1c00 0000 7265 6669 6e65  r....X....refine
-000038a0: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
-000038b0: 2e63 7377 6170 7218 0200 0058 0600 0000  .cswapr....X....
-000038c0: 6375 7070 6572 7219 0200 0058 1d00 0000  cupperr....X....
-000038d0: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
-000038e0: 7472 696e 6773 2e63 7570 7065 7272 1a02  trings.cupperr..
-000038f0: 0000 5803 0000 0072 6570 721b 0200 0058  ..X....repr....X
-00003900: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00003910: 7473 2e73 7472 696e 6773 2e72 6570 721c  ts.strings.repr.
-00003920: 0200 0058 0400 0000 7265 706c 721d 0200  ...X....replr...
-00003930: 0058 1b00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00003940: 6e69 7473 2e73 7472 696e 6773 2e72 6570  nits.strings.rep
-00003950: 6c72 1e02 0000 5804 0000 0073 6e69 7072  lr....X....snipr
-00003960: 1f02 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
-00003970: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
-00003980: 736e 6970 7220 0200 0058 0700 0000 7374  snipr ...X....st
-00003990: 7265 7463 6872 2102 0000 581e 0000 0072  retchr!...X....r
-000039a0: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
-000039b0: 7269 6e67 732e 7374 7265 7463 6872 2202  rings.stretchr".
-000039c0: 0000 5807 0000 0074 6572 6d66 6974 7223  ..X....termfitr#
-000039d0: 0200 0058 1e00 0000 7265 6669 6e65 7279  ...X....refinery
-000039e0: 2e75 6e69 7473 2e73 7472 696e 6773 2e74  .units.strings.t
-000039f0: 6572 6d66 6974 7224 0200 0058 0400 0000  ermfitr$...X....
-00003a00: 7472 696d 7225 0200 0058 1b00 0000 7265  trimr%...X....re
-00003a10: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
-00003a20: 696e 6773 2e74 7269 6d72 2602 0000 752e  ings.trimr&...u.
+00003560: 6174 7465 726e 2e6d 696d 6577 6f72 6473  attern.mimewords
+00003570: 72f6 0100 0058 0700 0000 7265 7370 6c69  r....X....respli
+00003580: 7472 f701 0000 581e 0000 0072 6566 696e  tr....X....refin
+00003590: 6572 792e 756e 6974 732e 7061 7474 6572  ery.units.patter
+000035a0: 6e2e 7265 7370 6c69 7472 f801 0000 5805  n.resplitr....X.
+000035b0: 0000 0072 6573 7562 72f9 0100 0058 1c00  ...resubr....X..
+000035c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000035d0: 2e70 6174 7465 726e 2e72 6573 7562 72fa  .pattern.resubr.
+000035e0: 0100 0058 0300 0000 7265 7872 fb01 0000  ...X....rexr....
+000035f0: 581a 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00003600: 6974 732e 7061 7474 6572 6e2e 7265 7872  its.pattern.rexr
+00003610: fc01 0000 5806 0000 0073 7472 7563 7472  ....X....structr
+00003620: fd01 0000 5824 0000 0072 6566 696e 6572  ....X$...refiner
+00003630: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+00003640: 7374 7275 6374 5f70 6172 7365 7272 fe01  struct_parserr..
+00003650: 0000 5808 0000 0073 7562 6669 6c65 7372  ..X....subfilesr
+00003660: ff01 0000 581f 0000 0072 6566 696e 6572  ....X....refiner
+00003670: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+00003680: 7375 6266 696c 6573 7200 0200 0058 0900  subfilesr....X..
+00003690: 0000 7572 6c67 7561 7264 7372 0102 0000  ..urlguardsr....
+000036a0: 5820 0000 0072 6566 696e 6572 792e 756e  X ...refinery.un
+000036b0: 6974 732e 7061 7474 6572 6e2e 7572 6c67  its.pattern.urlg
+000036c0: 7561 7264 7372 0202 0000 5803 0000 0078  uardsr....X....x
+000036d0: 7470 7203 0200 0058 1a00 0000 7265 6669  tpr....X....refi
+000036e0: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
+000036f0: 726e 2e78 7470 7204 0200 0058 0300 0000  rn.xtpr....X....
+00003700: 7874 7772 0502 0000 581a 0000 0072 6566  xtwr....X....ref
+00003710: 696e 6572 792e 756e 6974 732e 7061 7474  inery.units.patt
+00003720: 6572 6e2e 7874 7772 0602 0000 5803 0000  ern.xtwr....X...
+00003730: 0061 736d 7207 0200 0058 1800 0000 7265  .asmr....X....re
+00003740: 6669 6e65 7279 2e75 6e69 7473 2e73 696e  finery.units.sin
+00003750: 6b73 2e61 736d 7208 0200 0058 0400 0000  ks.asmr....X....
+00003760: 6475 6d70 7209 0200 0058 1900 0000 7265  dumpr....X....re
+00003770: 6669 6e65 7279 2e75 6e69 7473 2e73 696e  finery.units.sin
+00003780: 6b73 2e64 756d 7072 0a02 0000 5805 0000  ks.dumpr....X...
+00003790: 0069 656d 6170 720b 0200 0058 1a00 0000  .iemapr....X....
+000037a0: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
+000037b0: 696e 6b73 2e69 656d 6170 720c 0200 0058  inks.iemapr....X
+000037c0: 0400 0000 7065 656b 720d 0200 0058 1900  ....peekr....X..
+000037d0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000037e0: 2e73 696e 6b73 2e70 6565 6b72 0e02 0000  .sinks.peekr....
+000037f0: 5809 0000 0070 706a 7363 7269 7074 720f  X....ppjscriptr.
+00003800: 0200 0058 1e00 0000 7265 6669 6e65 7279  ...X....refinery
+00003810: 2e75 6e69 7473 2e73 696e 6b73 2e70 706a  .units.sinks.ppj
+00003820: 7363 7269 7074 7210 0200 0058 0600 0000  scriptr....X....
+00003830: 7070 6a73 6f6e 7211 0200 0058 1b00 0000  ppjsonr....X....
+00003840: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
+00003850: 696e 6b73 2e70 706a 736f 6e72 1202 0000  inks.ppjsonr....
+00003860: 5805 0000 0070 7078 6d6c 7213 0200 0058  X....ppxmlr....X
+00003870: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00003880: 7473 2e73 696e 6b73 2e70 7078 6d6c 7214  ts.sinks.ppxmlr.
+00003890: 0200 0058 0300 0000 6363 6172 1502 0000  ...X....ccar....
+000038a0: 581a 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000038b0: 6974 732e 7374 7269 6e67 732e 6363 6172  its.strings.ccar
+000038c0: 1602 0000 5803 0000 0063 6370 7217 0200  ....X....ccpr...
+000038d0: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000038e0: 6e69 7473 2e73 7472 696e 6773 2e63 6370  nits.strings.ccp
+000038f0: 7218 0200 0058 0400 0000 6366 6d74 7219  r....X....cfmtr.
+00003900: 0200 0058 1b00 0000 7265 6669 6e65 7279  ...X....refinery
+00003910: 2e75 6e69 7473 2e73 7472 696e 6773 2e63  .units.strings.c
+00003920: 666d 7472 1a02 0000 5806 0000 0063 6c6f  fmtr....X....clo
+00003930: 7765 7272 1b02 0000 581d 0000 0072 6566  werr....X....ref
+00003940: 696e 6572 792e 756e 6974 732e 7374 7269  inery.units.stri
+00003950: 6e67 732e 636c 6f77 6572 721c 0200 0058  ngs.clowerr....X
+00003960: 0500 0000 6373 7761 7072 1d02 0000 581c  ....cswapr....X.
+00003970: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003980: 732e 7374 7269 6e67 732e 6373 7761 7072  s.strings.cswapr
+00003990: 1e02 0000 5806 0000 0063 7570 7065 7272  ....X....cupperr
+000039a0: 1f02 0000 581d 0000 0072 6566 696e 6572  ....X....refiner
+000039b0: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
+000039c0: 6375 7070 6572 7220 0200 0058 0300 0000  cupperr ...X....
+000039d0: 7265 7072 2102 0000 581a 0000 0072 6566  repr!...X....ref
+000039e0: 696e 6572 792e 756e 6974 732e 7374 7269  inery.units.stri
+000039f0: 6e67 732e 7265 7072 2202 0000 5804 0000  ngs.repr"...X...
+00003a00: 0072 6570 6c72 2302 0000 581b 0000 0072  .replr#...X....r
+00003a10: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
+00003a20: 7269 6e67 732e 7265 706c 7224 0200 0058  rings.replr$...X
+00003a30: 0400 0000 736e 6970 7225 0200 0058 1b00  ....snipr%...X..
+00003a40: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003a50: 2e73 7472 696e 6773 2e73 6e69 7072 2602  .strings.snipr&.
+00003a60: 0000 5807 0000 0073 7472 6574 6368 7227  ..X....stretchr'
+00003a70: 0200 0058 1e00 0000 7265 6669 6e65 7279  ...X....refinery
+00003a80: 2e75 6e69 7473 2e73 7472 696e 6773 2e73  .units.strings.s
+00003a90: 7472 6574 6368 7228 0200 0058 0700 0000  tretchr(...X....
+00003aa0: 7465 726d 6669 7472 2902 0000 581e 0000  termfitr)...X...
+00003ab0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00003ac0: 7374 7269 6e67 732e 7465 726d 6669 7472  strings.termfitr
+00003ad0: 2a02 0000 5804 0000 0074 7269 6d72 2b02  *...X....trimr+.
+00003ae0: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00003af0: 756e 6974 732e 7374 7269 6e67 732e 7472  units.strings.tr
+00003b00: 696d 722c 0200 0075 2e                   imr,...u.
```

### Comparing `binary-refinery-0.6.8/refinery/__init__.py` & `binary-refinery-0.6.9/refinery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 1. `refinery.lib.frame`: framing syntax for working on lists of binary chunks
 2. `refinery.lib.argformats`: the multibin syntax for refinery arguments
 3. `refinery.lib.meta`: defining and using metadata variables within frames
 4. `refinery.units`: writing custom units, add command-line arguments, and how to use refinery
    units within Python code.
 """
-__version__ = '0.6.8'
+__version__ = '0.6.9'
 __distribution__ = 'binary-refinery'
 
 from typing import Dict, List, Optional, Type
 from importlib import resources
 from datetime import datetime
 
 import pickle
```

### Comparing `binary-refinery-0.6.8/refinery/data/rich.json` & `binary-refinery-0.6.9/refinery/data/rich.json`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/explore.py` & `binary-refinery-0.6.9/refinery/explore.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/argformats.py` & `binary-refinery-0.6.9/refinery/lib/argformats.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/argparser.py` & `binary-refinery-0.6.9/refinery/lib/argparser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/chunks.py` & `binary-refinery-0.6.9/refinery/lib/chunks.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/crypto.py` & `binary-refinery-0.6.9/refinery/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/decompression.py` & `binary-refinery-0.6.9/refinery/lib/decompression.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/decorators.py` & `binary-refinery-0.6.9/refinery/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/deobfuscation.py` & `binary-refinery-0.6.9/refinery/lib/deobfuscation.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/dex.py` & `binary-refinery-0.6.9/refinery/lib/dex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/dotnet/deserialize.py` & `binary-refinery-0.6.9/refinery/lib/dotnet/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/dotnet/header.py` & `binary-refinery-0.6.9/refinery/lib/dotnet/header.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/dotnet/resources.py` & `binary-refinery-0.6.9/refinery/lib/dotnet/resources.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/dotnet/types.py` & `binary-refinery-0.6.9/refinery/lib/dotnet/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/environment.py` & `binary-refinery-0.6.9/refinery/lib/environment.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/executable.py` & `binary-refinery-0.6.9/refinery/lib/executable.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/frame.py` & `binary-refinery-0.6.9/refinery/lib/frame.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/inline.py` & `binary-refinery-0.6.9/refinery/lib/inline.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/java.py` & `binary-refinery-0.6.9/refinery/lib/java.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/json.py` & `binary-refinery-0.6.9/refinery/lib/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/loader.py` & `binary-refinery-0.6.9/refinery/lib/loader.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/magic.py` & `binary-refinery-0.6.9/refinery/lib/magic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/meta.py` & `binary-refinery-0.6.9/refinery/lib/meta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/mime.py` & `binary-refinery-0.6.9/refinery/lib/mime.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/mscrypto.py` & `binary-refinery-0.6.9/refinery/lib/mscrypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/murmur.py` & `binary-refinery-0.6.9/refinery/lib/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/patterns/__init__.py` & `binary-refinery-0.6.9/refinery/lib/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/patterns/tlds.py` & `binary-refinery-0.6.9/refinery/lib/patterns/tlds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/powershell.py` & `binary-refinery-0.6.9/refinery/lib/powershell.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/ripemd128.py` & `binary-refinery-0.6.9/refinery/lib/ripemd128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/serpent.py` & `binary-refinery-0.6.9/refinery/lib/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/structures.py` & `binary-refinery-0.6.9/refinery/lib/structures.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/suffixtree.py` & `binary-refinery-0.6.9/refinery/lib/suffixtree.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/thirdparty/acefile.py` & `binary-refinery-0.6.9/refinery/lib/thirdparty/acefile.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/thirdparty/batch_interpreter.py` & `binary-refinery-0.6.9/refinery/lib/thirdparty/batch_interpreter.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/thirdparty/pcode2code.py` & `binary-refinery-0.6.9/refinery/lib/thirdparty/pcode2code.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/thirdparty/xxhash.py` & `binary-refinery-0.6.9/refinery/lib/thirdparty/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/tools.py` & `binary-refinery-0.6.9/refinery/lib/tools.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/types.py` & `binary-refinery-0.6.9/refinery/lib/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/vfs.py` & `binary-refinery-0.6.9/refinery/lib/vfs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/lib/xml.py` & `binary-refinery-0.6.9/refinery/lib/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/__init__.py` & `binary-refinery-0.6.9/refinery/units/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/__init__.py` & `binary-refinery-0.6.9/refinery/units/blockwise/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/alu.py` & `binary-refinery-0.6.9/refinery/units/blockwise/alu.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,19 @@
     """
     The arithmetic-logical unit. It allows you to specify a custom Python expression where the following
     variables are allowed:
 
     - the variable `A`: same as `V[0]`
     - the variable `B`: current block
     - the variable `N`: number of bytes in the input
-    - the variable `I`: current index in the input
-    - the variable `S`: an optional seed value for an internal state
+    - the variable `K`: current index in the input
+    - the variable `S`: the internal state value
     - the variable `V`: the vector of arguments
+    - the variable `I`: function that casts to a signed int in current precision
+    - the variable `U`: function that casts to unsigned int in current precision
 
     Each block of the input is replaced by the value of this expression. Additionally, it is possible to
     specify prologue and epilogue expressions which are used to update the state variable `S` before and
     after the update of each block, respectively.
     """
 
     @staticmethod
@@ -108,18 +110,29 @@
             seed = PythonExpression(seed, 'N', constants=metavars(data))
         if callable(seed):
             seed = seed(context, N=len(data))
         self._index.init(self.fmask)
         prologue = self.args.prologue.expression
         epilogue = self.args.epilogue.expression
         operator = self.args.operator.expression
-        context.update(N=len(data), S=seed)
+
+        def toUINT(n) -> int:
+            return int(n) & self.fmask
+
+        def toSINT(n) -> int:
+            n = toUINT(n)
+            if n >> (self.fbits - 1):
+                return -((~n + 1) & self.fmask)
+            else:
+                return n
+
+        context.update(N=len(data), S=seed, I=toSINT, U=toUINT)
 
         def operate(block, index, *args):
-            context.update(I=index, B=block, V=args)
+            context.update(K=index, B=block, V=args)
             if args:
                 context['A'] = args[0]
             context['S'] = eval(prologue, None, context)
             context['B'] = eval(operator, None, context)
             context['S'] = eval(epilogue, None, context)
             return context['B']
```

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/bitrev.py` & `binary-refinery-0.6.9/refinery/units/blockwise/bitrev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/byteswap.py` & `binary-refinery-0.6.9/refinery/units/blockwise/byteswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/map.py` & `binary-refinery-0.6.9/refinery/units/blockwise/map.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/pack.py` & `binary-refinery-0.6.9/refinery/units/blockwise/pack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/rev.py` & `binary-refinery-0.6.9/refinery/units/blockwise/rev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/terminate.py` & `binary-refinery-0.6.9/refinery/units/blockwise/terminate.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/blockwise/xor.py` & `binary-refinery-0.6.9/refinery/units/blockwise/xor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/ap.py` & `binary-refinery-0.6.9/refinery/units/compression/ap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/blz.py` & `binary-refinery-0.6.9/refinery/units/compression/blz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/bz2.py` & `binary-refinery-0.6.9/refinery/units/compression/bz2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/decompress.py` & `binary-refinery-0.6.9/refinery/units/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/jcalg.py` & `binary-refinery-0.6.9/refinery/units/compression/jcalg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lz.py` & `binary-refinery-0.6.9/refinery/units/compression/lz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lz4.py` & `binary-refinery-0.6.9/refinery/units/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lzf.py` & `binary-refinery-0.6.9/refinery/units/compression/lzf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lzg.py` & `binary-refinery-0.6.9/refinery/units/compression/lzg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lzip.py` & `binary-refinery-0.6.9/refinery/units/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lzjb.py` & `binary-refinery-0.6.9/refinery/units/compression/lzjb.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lznt1.py` & `binary-refinery-0.6.9/refinery/units/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/lzo.py` & `binary-refinery-0.6.9/refinery/units/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/mscf.py` & `binary-refinery-0.6.9/refinery/units/compression/mscf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/qlz.py` & `binary-refinery-0.6.9/refinery/units/compression/qlz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/szdd.py` & `binary-refinery-0.6.9/refinery/units/compression/szdd.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/compression/zl.py` & `binary-refinery-0.6.9/refinery/units/compression/zl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/__init__.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/camellia.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/camellia.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/chacha.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/chacha.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/chaskey.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/chaskey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/gost.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/gost.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/hc128.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/hc128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/isaac.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/isaac.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rabbit.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rabbit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc2.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rc2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc4.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rc4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc4mod.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rc4mod.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc5.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rc5.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rc6.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rc6.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rijndael.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rijndael.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rncrypt.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rncrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rot.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rot.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rsa.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/rsakey.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/rsakey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/salsa.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/salsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/seal.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/seal.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/secstr.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/secstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/serpent.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/tea.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/tea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/vigenere.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/vigenere.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/xtea.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/xtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/cipher/xxtea.py` & `binary-refinery-0.6.9/refinery/units/crypto/cipher/xxtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/hash/__init__.py` & `binary-refinery-0.6.9/refinery/units/crypto/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/hash/checksums.py` & `binary-refinery-0.6.9/refinery/units/crypto/hash/checksums.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/hash/cryptographic.py` & `binary-refinery-0.6.9/refinery/units/crypto/hash/cryptographic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/hash/imphash.py` & `binary-refinery-0.6.9/refinery/units/crypto/hash/imphash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/hash/murmur.py` & `binary-refinery-0.6.9/refinery/units/crypto/hash/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/hash/xxhash.py` & `binary-refinery-0.6.9/refinery/units/crypto/hash/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/CryptDeriveKey.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/CryptDeriveKey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/DESDerive.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/DESDerive.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/PasswordDeriveBytes.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/PasswordDeriveBytes.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/__init__.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/kblob.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/kblob.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf1.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/pbkdf1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/pbkdf2.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/crypto/keyderive/unixcrypt.py` & `binary-refinery-0.6.9/refinery/units/crypto/keyderive/unixcrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/atbash.py` & `binary-refinery-0.6.9/refinery/units/encoding/atbash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/b32.py` & `binary-refinery-0.6.9/refinery/units/encoding/b32.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/b64.py` & `binary-refinery-0.6.9/refinery/units/encoding/b64.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/base.py` & `binary-refinery-0.6.9/refinery/units/encoding/base.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/esc.py` & `binary-refinery-0.6.9/refinery/units/encoding/esc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/hex.py` & `binary-refinery-0.6.9/refinery/units/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/netbios.py` & `binary-refinery-0.6.9/refinery/units/encoding/netbios.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/ps1str.py` & `binary-refinery-0.6.9/refinery/units/encoding/ps1str.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/recode.py` & `binary-refinery-0.6.9/refinery/units/encoding/recode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/url.py` & `binary-refinery-0.6.9/refinery/units/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/uuenc.py` & `binary-refinery-0.6.9/refinery/units/encoding/uuenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/encoding/wshenc.py` & `binary-refinery-0.6.9/refinery/units/encoding/wshenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/__init__.py` & `binary-refinery-0.6.9/refinery/units/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/a3x.py` & `binary-refinery-0.6.9/refinery/units/formats/a3x.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/__init__.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xt.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xt7z.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xt7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtace.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtasar.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtasar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtcab.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtcab.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtcpio.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtcpio.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtgz.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtgz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtiso.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtiso.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtiss.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtiss.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtnode.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtnode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtnsis.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtnsis.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtpyi.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtpyi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xttar.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xttar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/archive/xtzip.py` & `binary-refinery-0.6.9/refinery/units/formats/archive/xtzip.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,28 +76,30 @@
                     if not password:
                         raise RuntimeError('archive is password-protected')
                     else:
                         raise RuntimeError(F'invalid password: {password.decode(self.codec)}') from E
             if info.filename:
                 if info.is_dir():
                     continue
-            try:
-                date = datetime(*info.date_time)
-            except Exception:
-                date = None
 
             # courtesy of https://stackoverflow.com/a/37773438/9130824
             filename = info.filename
             if info.flag_bits & ZIP_FILENAME_UTF8_FLAG == 0:
                 filename_bytes = filename.encode('437')
                 try:
                     guessed_encoding = self._chardet.detect(filename_bytes)['encoding']
                 except ImportError:
                     guessed_encoding = None
                 guessed_encoding = guessed_encoding or 'cp1252'
                 filename = filename_bytes.decode(guessed_encoding, 'replace')
 
+            try:
+                date = datetime(*info.date_time)
+            except Exception as e:
+                self.log_info(F'{e!s} - unable to determine date from tuple {info.date_time} for: {filename}')
+                date = None
+
             yield self._pack(filename, date, xt)
 
     @classmethod
     def handles(cls, data: bytearray) -> Optional[bool]:
         return data.rfind(ZipEndOfCentralDirectory.SIGNATURE) > 0
```

### Comparing `binary-refinery-0.6.8/refinery/units/formats/bat.py` & `binary-refinery-0.6.9/refinery/units/formats/bat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/csv.py` & `binary-refinery-0.6.9/refinery/units/formats/csv.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/deserialize_php.py` & `binary-refinery-0.6.9/refinery/units/formats/deserialize_php.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/email.py` & `binary-refinery-0.6.9/refinery/units/formats/email.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/evtx.py` & `binary-refinery-0.6.9/refinery/units/formats/evtx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/exe/vaddr.py` & `binary-refinery-0.6.9/refinery/units/formats/exe/vaddr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/exe/vmemref.py` & `binary-refinery-0.6.9/refinery/units/formats/exe/vmemref.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/exe/vsect.py` & `binary-refinery-0.6.9/refinery/units/formats/exe/vsect.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/exe/vsnip.py` & `binary-refinery-0.6.9/refinery/units/formats/exe/vsnip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/exe/vstack.py` & `binary-refinery-0.6.9/refinery/units/formats/exe/vstack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import List, TYPE_CHECKING
 
 from refinery.units import Arg, Unit
 from refinery.lib.executable import align, Arch, Executable
 from refinery.lib.types import INF
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 if TYPE_CHECKING:
     from typing import Tuple, Optional, Iterator
     from capstone import Cs
     from unicorn import Uc
     from intervaltree import IntervalTree, Interval
 
 
 @dataclass
 class EmuState:
     executable: Executable
     writes: IntervalTree
+    address: int
     disassembler: Optional[Cs] = None
     waiting: int = 0
+    callstack: List[int] = field(default_factory=list)
+    retaddr: Optional[int] = None
+    stop: Optional[int] = None
+    previous_address: int = 0
+    sp_register: int = 0
+    stack_ceiling: int = 0
 
     def disassemble(self, address: int, size: int):
         if self.disassembler is None:
             return None
         try:
             pos = self.executable.location_from_address(address).physical.position
             end = pos + size
             return next(self.disassembler.disasm(
                 bytes(self.executable.data[pos:end]), address, 1))
         except Exception:
             return None
 
+    def fmt(self, address: int) -> str:
+        return F'0x{address:0{self.executable.pointer_size//4}X}'
+
 
 class vstack(Unit):
     """
     The unit emulates instructions at a given address in the input executable (PE/ELF/MachO) and
     extracts data patches that are written to the stack during emulation. Emulation is halted as
     soon as a certain number of instructions has not performed any memory writes, or when an error
     occurs.
@@ -60,29 +70,31 @@
     @Unit.Requires('capstone')
     def _capstone():
         import capstone
         return capstone
 
     def __init__(
         self,
-        address: Arg.Number(metavar='address', help='Specify the (virtual) address of a stack string instruction sequence.'),
+        address: Arg.Number(metavar='start', help='Specify the (virtual) address of a stack string instruction sequence.'),
+        stop: Arg.Number(metavar='stop', help='Optional: Stop when reaching this address.') = None,
         base: Arg.Number('-b', metavar='ADDR', help='Optionally specify a custom base address B.') = None,
-        min: Arg.Number('-n', help='Minimum size of a memory patch, default is {default}.') = 10,
+        min: Arg.Number('-n', help='Minimum size of a memory patch, default is {default}.') = 5,
         max: Arg.Number('-m', help='Maximum size of a memory patch, default is {default}.') = INF,
-        halt_after: Arg.Number('-a', help=(
-            'When this many instructions did not write to memory, emulation is halted. The default is {default}.')) = 5,
+        wait: Arg.Number('-w', help=(
+            'When this many instructions did not write to memory, emulation is halted. The default is {default}.')) = 10,
         stack_size: Arg.Number('-s', help='Optionally specify the stack size. The default is 0x{default:X}.') = 0x10000,
         block_size: Arg.Number('-k', help='Standard memory block size for the emulator, 0x{default:X} by default.') = 0x1000,
     ):
         super().__init__(
             address=address,
+            stop=stop,
             base=base,
             min=min,
             max=max,
-            halt_after=halt_after,
+            wait=wait,
             stack_size=stack_size,
             block_size=block_size,
         )
 
     def _find_stack_location(self, exe: Executable):
         stack_size = self.args.stack_size
         memory_max = 1 << exe.pointer_size
@@ -108,28 +120,30 @@
         image = memoryview(data)
 
         if self.log_debug():
             disassembler = self._capstone.Cs(*self._cs_arch(arch))
         else:
             disassembler = None
 
-        state = EmuState(exe, tree, disassembler)
-
-        emulator.mem_map(stack_addr, stack_size * 3)
-        emulator.reg_write({
+        sp = {
             Arch.X8632   : uc.x86_const.UC_X86_REG_ESP,
             Arch.X8664   : uc.x86_const.UC_X86_REG_RSP,
             Arch.ARM32   : uc.arm_const.UC_ARM_REG_SP,
             Arch.ARM32   : uc.arm_const.UC_ARM_REG_SP,
             Arch.MIPS16  : uc.mips_const.UC_MIPS_REG_SP,
             Arch.MIPS32  : uc.mips_const.UC_MIPS_REG_SP,
             Arch.MIPS64  : uc.mips_const.UC_MIPS_REG_SP,
             Arch.SPARC32 : uc.sparc_const.UC_SPARC_REG_SP,
             Arch.SPARC64 : uc.sparc_const.UC_SPARC_REG_SP,
-        }[arch], stack_addr + 2 * stack_size)
+        }[arch]
+
+        state = EmuState(exe, tree, address, disassembler,
+            stop=self.args.stop, sp_register=sp)
+        emulator.mem_map(stack_addr, stack_size * 3)
+        emulator.reg_write(sp, stack_addr + 2 * stack_size)
 
         if arch is Arch.X8632:
             for reg in [
                 uc.x86_const.UC_X86_REG_EAX,
                 uc.x86_const.UC_X86_REG_EBX,
                 uc.x86_const.UC_X86_REG_ECX,
                 uc.x86_const.UC_X86_REG_EDX,
@@ -187,26 +201,45 @@
         it: Iterator[Interval] = iter(tree)
         for interval in it:
             size = interval.end - interval.begin - 1
             if size > self.args.max:
                 continue
             if size < self.args.min:
                 continue
-            self.log_info(F'memory patch at 0x{interval.begin:0{exe.pointer_size//4}X} of size {size}')
+            self.log_info(F'memory patch at {state.fmt(interval.begin)} of size {size}')
             yield emulator.mem_read(interval.begin, size)
 
     def _hook_mem_write(self, emu: Uc, access: int, address: int, size: int, value: int, state: EmuState):
+        mask = (1 << (size * 8)) - 1
+        unsigned_value = value & mask
+        depth = len(state.callstack)
+
+        if unsigned_value == state.address:
+            callstack = state.callstack
+            if not callstack:
+                state.stack_ceiling = emu.reg_read(state.sp_register)
+            state.retaddr = unsigned_value
+            callstack.append(unsigned_value)
+        else:
+            state.retaddr = None
+
+        if state.stack_ceiling > 0 and address in range(state.stack_ceiling - 0x200, state.stack_ceiling):
+            return
+
         state.waiting = 0
         state.writes.addi(address, address + size + 1)
         state.writes.merge_overlaps()
 
         def info():
-            mask = (1 << (size * 8)) - 1
-            data = (value & mask).to_bytes(size, state.executable.byte_order().value).hex().upper()
-            return F'memory write to 0x{address:0{state.executable.pointer_size//4}X}: {data}'
+            data = unsigned_value.to_bytes(size, state.executable.byte_order().value).hex().upper()
+            indent = '\x20' * 4 * depth
+            return (
+                F'emulating [wait={state.waiting:02d}] {indent}{state.fmt(state.previous_address)}: '
+                F'{state.fmt(address)} <- {data}')
+
         self.log_info(info)
 
     def _hook_insn_error(self, emu: Uc, state: EmuState):
         self.log_debug('aborting emulation; instruction error')
         emu.emu_stop()
         return False
 
@@ -215,29 +248,53 @@
             R'aborting emulation; access error '
             F'at 0x{address:0{state.executable.pointer_size//4}X}; '
             F'value={value:0{size*2}X}; code={access}')
         emu.emu_stop()
         return False
 
     def _hook_code(self, emu: Uc, address: int, size: int, state: EmuState):
+        if address == state.stop:
+            emu.emu_stop()
+            return False
         try:
             waiting = state.waiting
+            callstack = state.callstack
+            depth = len(callstack)
+            state.previous_address = state.address
+
+            if address != state.address:
+                if depth and address == callstack[-1]:
+                    depth -= 1
+                    state.callstack.pop()
+                    if depth == 0:
+                        state.stack_ceiling = 0
+                state.address = address
+            elif state.retaddr is not None:
+                # The present address was moved to the stack but we did not branch.
+                # This is not quite accurate, of course: We could be calling the
+                # next instruction. However, that sort of code is usually not really
+                # a function call anyway, but rather a way to get the IP.
+                callstack.pop()
+                state.retaddr = None
 
-            if waiting > self.args.halt_after:
+            if waiting > self.args.wait:
                 emu.emu_stop()
                 return False
-            state.waiting += 1
+            if not depth:
+                state.waiting += 1
+            state.address += size
 
             def debug_message():
                 instruction = state.disassemble(address, size)
+                indent = '\x20' * 4 * depth
                 if instruction:
                     instruction = F'{instruction.mnemonic} {instruction.op_str}'
                 else:
                     instruction = '<DISASSEMBLER FAILURE>'
-                return F'emulating [wait={waiting:02d}] 0x{address:0{state.executable.pointer_size//4}X}: {instruction}'
+                return F'emulating [wait={waiting:02d}] {indent}0x{address:0{state.executable.pointer_size//4}X}: {instruction}'
 
             self.log_debug(debug_message)
 
         except KeyboardInterrupt:
             emu.emu_stop()
             return False
```

### Comparing `binary-refinery-0.6.8/refinery/units/formats/hexload.py` & `binary-refinery-0.6.9/refinery/units/formats/hexload.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/html.py` & `binary-refinery-0.6.9/refinery/units/formats/html.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/httpresponse.py` & `binary-refinery-0.6.9/refinery/units/formats/httpresponse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/ifps.py` & `binary-refinery-0.6.9/refinery/units/formats/ifps.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/ifpsstr.py` & `binary-refinery-0.6.9/refinery/units/formats/ifpsstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/java/deserialize.py` & `binary-refinery-0.6.9/refinery/units/formats/java/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/java/jvdasm.py` & `binary-refinery-0.6.9/refinery/units/formats/java/jvdasm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/json.py` & `binary-refinery-0.6.9/refinery/units/formats/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/lnk.py` & `binary-refinery-0.6.9/refinery/units/formats/lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/msgpack.py` & `binary-refinery-0.6.9/refinery/units/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/msi.py` & `binary-refinery-0.6.9/refinery/units/formats/msi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/doctxt.py` & `binary-refinery-0.6.9/refinery/units/formats/office/doctxt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/officecrypt.py` & `binary-refinery-0.6.9/refinery/units/formats/office/officecrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/vbapc.py` & `binary-refinery-0.6.9/refinery/units/formats/office/vbapc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/vbastr.py` & `binary-refinery-0.6.9/refinery/units/formats/office/vbastr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/xlmdeobf.py` & `binary-refinery-0.6.9/refinery/units/formats/office/xlmdeobf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/xlxtr.py` & `binary-refinery-0.6.9/refinery/units/formats/office/xlxtr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/xtdoc.py` & `binary-refinery-0.6.9/refinery/units/formats/office/xtdoc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/xtone.py` & `binary-refinery-0.6.9/refinery/units/formats/office/xtone.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/xtrtf.py` & `binary-refinery-0.6.9/refinery/units/formats/office/xtrtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/office/xtvba.py` & `binary-refinery-0.6.9/refinery/units/formats/office/xtvba.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pcap.py` & `binary-refinery-0.6.9/refinery/units/formats/pcap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pcap_http.py` & `binary-refinery-0.6.9/refinery/units/formats/pcap_http.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pdf.py` & `binary-refinery-0.6.9/refinery/units/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/__init__.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,20 @@
         for s in pe.sections
     ), default=0) or 0
 
     memdump_value = memdump and max((
         s.VirtualAddress + s.Misc_VirtualSize
         for s in pe.sections
     ), default=0) or 0
-    cert_entry = pe.OPTIONAL_HEADER.DATA_DIRECTORY[
-        IMAGE_DIRECTORY_ENTRY_SECURITY]
+
+    try:
+        cert_entry = pe.OPTIONAL_HEADER.DATA_DIRECTORY[IMAGE_DIRECTORY_ENTRY_SECURITY]
+    except IndexError:
+        cert_entry = None
+        certificate = False
 
     if directories:
         directories_value = max((
             pe.get_offset_from_rva(d.VirtualAddress) + d.Size
             for d in pe.OPTIONAL_HEADER.DATA_DIRECTORY
             if d.name != 'IMAGE_DIRECTORY_ENTRY_SECURITY'
         ), default=0)
```

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/__init__.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dncfx.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dncfx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnds.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnfields.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnfields.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnhdr.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnhdr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnmr.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnmr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnrc.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnrc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/dotnet/dnstr.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/dotnet/dnstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/pemeta.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/pemeta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/peoverlay.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/peoverlay.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/perc.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/perc.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 from typing import Tuple
 
 import enum
 import pefile
 import re
 import struct
+import json
 
 from refinery.units.formats import UnpackResult, PathExtractorUnit, Arg
 from refinery.lib.structures import Struct, StructReader
 
 
 class RSRC(enum.IntEnum):
     CURSOR        = 0x01  # noqa
@@ -101,19 +102,38 @@
                 path = '/'.join(str(p) for p in (*parts, identifier))
                 extract = None
                 if self.args.pretty:
                     if parts[0] is RSRC.BITMAP:
                         extract = self._handle_bitmap(pe, rva, size)
                     elif parts[0] is RSRC.ICON:
                         extract = self._handle_icon(pe, parts, rva, size)
+                    elif parts[0] is RSRC.STRING:
+                        extract = self._handle_strings(pe, parts, rva, size)
                 if extract is None:
                     def extract(pe=pe):
                         return pe.get_data(rva, size)
                 yield UnpackResult(path, extract, offset=pe.get_offset_from_rva(rva))
 
+    def _handle_strings(self, pe: pefile.PE, parts: Tuple[RSRC, int, int], rva: int, size: int):
+        def extract(pe=pe):
+            self.log_debug(parts)
+            base = (parts[1] - 1) << 4
+            reader = StructReader(pe.get_data(rva, size))
+            table = {}
+            index = 0
+            while not reader.eof:
+                string = reader.read_exactly(reader.u16() * 2)
+                if not string:
+                    break
+                key = F'{base+index:04X}'
+                table[key] = string.decode('utf-16le')
+                index += 1
+            return json.dumps(table, indent=4).encode(self.codec)
+        return extract
+
     def _handle_bitmap(self, pe: pefile.PE, rva: int, size: int):
         def extract(pe=pe):
             bitmap = pe.get_data(rva, size)
             total = (len(bitmap) + 14).to_bytes(4, 'little')
             return B'BM' + total + B'\0\0\0\0\x36\0\0\0' + bitmap
         return extract
```

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/pesig.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/pesig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pe/pestrip.py` & `binary-refinery-0.6.9/refinery/units/formats/pe/pestrip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pkcs7.py` & `binary-refinery-0.6.9/refinery/units/formats/pkcs7.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/pkcs7sig.py` & `binary-refinery-0.6.9/refinery/units/formats/pkcs7sig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/stego.py` & `binary-refinery-0.6.9/refinery/units/formats/stego.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     b = 2
     a = 3
 
 
 class stego(Unit):
     """
     Decodes the RGBA (red/green/blue/alpha) values of the pixels of a given image file and outputs
-    these values as bytes. Each row of the image is transformed and output as and individual chunk.
+    these values as bytes. Each row of the image is transformed and output as an individual chunk.
     """
     def __init__(
         self,
         transpose: Arg.Switch('-t', help='Return the columns of the image rather than the rows.'),
         parts: Arg('parts', nargs='?', type=str, help=(
             'A string containing any ordering of the letters R, G, B, and A (case-insensitive). '
             'These pixel components will be extracted from every pixel in the given order. The '
```

### Comparing `binary-refinery-0.6.8/refinery/units/formats/tnetmtm.py` & `binary-refinery-0.6.9/refinery/units/formats/tnetmtm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/winreg.py` & `binary-refinery-0.6.9/refinery/units/formats/winreg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/formats/xml.py` & `binary-refinery-0.6.9/refinery/units/formats/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/malware/n40.py` & `binary-refinery-0.6.9/refinery/units/malware/n40.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/__init__.py` & `binary-refinery-0.6.9/refinery/units/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/chop.py` & `binary-refinery-0.6.9/refinery/units/meta/chop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/cm.py` & `binary-refinery-0.6.9/refinery/units/meta/cm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/cull.py` & `binary-refinery-0.6.9/refinery/units/meta/cull.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/dedup.py` & `binary-refinery-0.6.9/refinery/units/meta/dedup.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/eat.py` & `binary-refinery-0.6.9/refinery/units/meta/eat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/ef.py` & `binary-refinery-0.6.9/refinery/units/meta/ef.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/emit.py` & `binary-refinery-0.6.9/refinery/units/meta/emit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/group.py` & `binary-refinery-0.6.9/refinery/units/meta/group.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/groupby.py` & `binary-refinery-0.6.9/refinery/units/meta/groupby.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/iff.py` & `binary-refinery-0.6.9/refinery/units/meta/iff.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/iffp.py` & `binary-refinery-0.6.9/refinery/units/meta/iffp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/iffs.py` & `binary-refinery-0.6.9/refinery/units/meta/iffs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/iffx.py` & `binary-refinery-0.6.9/refinery/units/meta/iffx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/max.py` & `binary-refinery-0.6.9/refinery/units/meta/max.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/min.py` & `binary-refinery-0.6.9/refinery/units/meta/min.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/mvc.py` & `binary-refinery-0.6.9/refinery/units/meta/mvc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/mvg.py` & `binary-refinery-0.6.9/refinery/units/meta/mvg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/pad.py` & `binary-refinery-0.6.9/refinery/units/meta/pad.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/pick.py` & `binary-refinery-0.6.9/refinery/units/meta/pick.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/pop.py` & `binary-refinery-0.6.9/refinery/units/meta/pop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/push.py` & `binary-refinery-0.6.9/refinery/units/meta/push.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/put.py` & `binary-refinery-0.6.9/refinery/units/meta/put.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/queue.py` & `binary-refinery-0.6.9/refinery/units/meta/queue.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/reduce.py` & `binary-refinery-0.6.9/refinery/units/meta/reduce.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/scope.py` & `binary-refinery-0.6.9/refinery/units/meta/scope.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/sep.py` & `binary-refinery-0.6.9/refinery/units/meta/sep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/sorted.py` & `binary-refinery-0.6.9/refinery/units/meta/sorted.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/swap.py` & `binary-refinery-0.6.9/refinery/units/meta/swap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/transpose.py` & `binary-refinery-0.6.9/refinery/units/meta/transpose.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/meta/xfcc.py` & `binary-refinery-0.6.9/refinery/units/meta/xfcc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/misc/autoxor.py` & `binary-refinery-0.6.9/refinery/units/misc/autoxor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/misc/couple.py` & `binary-refinery-0.6.9/refinery/units/misc/couple.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/misc/datefix.py` & `binary-refinery-0.6.9/refinery/units/misc/datefix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/misc/drp.py` & `binary-refinery-0.6.9/refinery/units/misc/drp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/misc/nop.py` & `binary-refinery-0.6.9/refinery/units/misc/nop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/misc/urlfix.py` & `binary-refinery-0.6.9/refinery/units/misc/urlfix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/misc/xkey.py` & `binary-refinery-0.6.9/refinery/units/misc/xkey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/__init__.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/js/arrays.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/js/arrays.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/js/getattr.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/js/getattr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/js/tuples.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/js/tuples.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/__init__.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/all.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/all.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 from .escape import deob_ps1_escape
 from .cases import deob_ps1_cases
 from .format import deob_ps1_format
 from .typecast import deob_ps1_typecast
 from .stringreplace import deob_ps1_stringreplace
 from .uncurly import deob_ps1_uncurly
 from .invoke import deob_ps1_invoke
+from .b64convert import deob_ps1_b64convert
+from .encodings import deob_ps1_encodings
 
 
 class deob_ps1(IterativeDeobfuscator):
 
     _SUBUNITS = [sub() for sub in [
         deob_ps1_escape,
         deob_ps1_cases,
         deob_ps1_brackets,
         deob_ps1_format,
         deob_ps1_typecast,
         deob_ps1_stringreplace,
+        deob_ps1_b64convert,
+        deob_ps1_encodings,
         deob_ps1_concat,
         deob_ps1_invoke,
         deob_ps1_uncurly
     ]]
 
     def deobfuscate(self, data):
         for u in self._SUBUNITS:
```

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/brackets.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/cases.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/cases.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/concat.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/format.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/format.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/invoke.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/invoke.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/securestring.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/securestring.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/stringreplace.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/typecast.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/typecast.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/ps1/uncurly.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/ps1/uncurly.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/all.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/arithmetic.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/arithmetic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/brackets.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/char.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/char.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/concat.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/constants.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/constants.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/dummies.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/dummies.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreplace.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/obfuscation/vba/stringreverse.py` & `binary-refinery-0.6.9/refinery/units/obfuscation/vba/stringreverse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/__init__.py` & `binary-refinery-0.6.9/refinery/units/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve_7z.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve_7z.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,18 +36,23 @@
     def process(self, data: bytearray):
         cursor = 0
         mv = memoryview(data)
         while True:
             start = data.find(self.HEADER_SIGNATURE, cursor)
             if start < cursor:
                 break
+            self.log_debug(F'found header at offset: 0x{start:08X}')
             try:
                 mf = MemoryFileRecorder(mv[start:])
+                self.log_debug('attempting to read archive')
                 archive = self._py7zr.SevenZipFile(mf)
+                self.log_debug('attempting to test archive')
                 success = archive.test() is not False
-            except Exception:
+            except Exception as error:
+                self.log_debug('parsing archive failed:', error)
                 success = False
             if success:
+                self.log_info(F'identified archive of size 0x{mf.max_cursor:08X} at offset 0x{start:08X}')
                 cursor = start + mf.max_cursor
                 yield self.labelled(mv[start:cursor], offset=start)
             else:
-                cursor += 5
+                cursor = start + 5
```

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve_json.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
             if end is None:
                 continue
             try:
                 if not json.loads(data[start:end]):
                     continue
             except json.JSONDecodeError:
                 continue
+            except UnicodeDecodeError:
+                continue
             self.cursor = end + 1
             return start, data[start:end]
 
     @classmethod
     def find_end(cls, data: bytearray, start: int):
         token = data[start]
         scope = bytearray()
```

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve_lnk.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve_lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve_pe.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve_pe.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve_rtf.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve_rtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve_xml.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve_xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/carve_zip.py` & `binary-refinery-0.6.9/refinery/units/pattern/carve_zip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/defang.py` & `binary-refinery-0.6.9/refinery/units/pattern/defang.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/dnsdomain.py` & `binary-refinery-0.6.9/refinery/units/pattern/dnsdomain.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/mimewords.py` & `binary-refinery-0.6.9/refinery/units/pattern/mimewords.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/resplit.py` & `binary-refinery-0.6.9/refinery/units/pattern/resplit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/resub.py` & `binary-refinery-0.6.9/refinery/units/pattern/resub.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/rex.py` & `binary-refinery-0.6.9/refinery/units/pattern/rex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/struct_parser.py` & `binary-refinery-0.6.9/refinery/units/pattern/struct_parser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/subfiles.py` & `binary-refinery-0.6.9/refinery/units/pattern/subfiles.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/urlguards.py` & `binary-refinery-0.6.9/refinery/units/pattern/urlguards.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/xtp.py` & `binary-refinery-0.6.9/refinery/units/pattern/xtp.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,14 +111,15 @@
         'azure.com'               : 1,
         'baidu.com'               : 2,
         'bootstrapcdn.com'        : 2,
         'cdnjs.cloudflare.com'    : 4,
         'comodo.net'              : 1,
         'comodoca.com'            : 1,
         'curl.haxx.se'            : 1,
+        'curl.se'                 : 1,
         'digicert.com'            : 1,
         'dublincore.org'          : 1,
         'fontawesome.com'         : 1,
         'facebook.com'            : 4,
         'github.com'              : 3,
         'globalsign.com'          : 1,
         'globalsign.net'          : 1,
@@ -250,14 +251,16 @@
                 self.log_info(F'excluding indicator because domain {hl} is whitelisted')
                 return None
             if name in {
                 indicators.hostname.name,
                 indicators.domain.name,
                 indicators.subdomain.name
             }:
+                if data[pos - 1] in b'/\\' and self.args.filter >= 2:
+                    return None
                 hostparts = host.split('.')
                 if self.args.filter >= 2:
                     if not all(p.isdigit() for p in hostparts) and all(len(p) < 4 for p in hostparts):
                         self.log_info(value)
                         self.log_info('excluding host with too many short parts')
                         return None
                 if self.args.filter >= 3:
@@ -303,32 +306,41 @@
                 ix += 1
             return None if at - ix < 3 else value[ix:]
         elif name == indicators.path.name:
             if len(value) < 8:
                 return None
             if len(value) > 16 and len(re.findall(RB'\\x\d\d', value)) > len(value) // 10:
                 return None
+            try:
+                path_string = value.decode(self.codec)
+            except Exception:
+                return None
+            try:
+                path = Path(path_string)
+            except Exception as E:
+                self.log_debug(F'error parsing path "{path}": {E!s}')
+                return None
+            path_likeness = sum(v for v, x in [
+                (1, path.suffix),
+                (1, path_string.startswith('/')),
+                (2, path_string.startswith('%')),
+                (2, path_string.startswith('\\\\')),
+                (2, path_string[1:3] == ':\\'),
+            ] if x)
+            if path_likeness < min(self.args.filter, 2):
+                return None
             if self.args.filter >= 2:
-                try:
-                    path = value.decode(self.codec)
-                except Exception:
-                    return None
-                try:
-                    path = Path(path)
-                except Exception as E:
-                    self.log_debug(F'error parsing path "{path}": {E!s}')
-                    return None
                 for k, part in enumerate(path.parts):
                     if not k:
                         drive, colon, slash = part.partition(':')
                         if colon and len(drive) == 1 and len(slash) <= 1:
                             continue
                         if part[0] == part[~0] == '%':
                             continue
-                    if LetterWeights.Path(part) < 0.6:
+                    if LetterWeights.Path(part) < 0.4 + (min(self.args.filter, 5) * 0.1):
                         return None
         return value
 
     def process(self, data):
         whitelist = set()
 
         def check(match: re.Match):
```

### Comparing `binary-refinery-0.6.8/refinery/units/pattern/xtw.py` & `binary-refinery-0.6.9/refinery/units/pattern/xtw.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/__init__.py` & `binary-refinery-0.6.9/refinery/units/sinks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,16 @@
     separator = metrics.hex_char_spacer
     hex_width = metrics.hex_column_width
     addr_width = metrics.address_width
     columns = metrics.hex_columns
     hexformat = metrics.hex_char_format
     printable = range(0x21, 0x7F)
 
-    from colorama import Fore as FG, Style as S
+    from colorama import Fore as FG
+    color_reset = FG.RESET
 
     if columns <= 0:
         raise RuntimeError('Requested width is too small.')
 
     view = memoryview(data)
     step = columns * metrics.block_size
     previous = None
@@ -96,45 +97,46 @@
             elif repetitions > 0:
                 format = ' {} repetitions'
                 message = format.format(repetitions)
                 pad = (hex_width * columns - len(format) + 1) // 2
                 pad = pad - len(message) + len(format)
                 line = ' ' * pad + message
                 if colorize:
-                    line = F'{FG.LIGHTBLACK_EX}{line}{S.RESET_ALL}'
+                    line = F'{FG.LIGHTBLACK_EX}{line}{color_reset}'
                 if addr_width:
                     line = F'{".":.>{addr_width}}{metrics.hex_addr_spacer}{line}'
                 yield line
                 skipped += repetitions - 1
                 repetitions = 0
 
         if metrics.line_count and lno - skipped >= metrics.line_count:
             break
 
         blocks = chunks.unpack(chunk, metrics.block_size, metrics.big_endian)
 
         if not colorize:
+            color_prefix = ''
             dump = separator.join(hexformat.format(b) for b in blocks)
             ascii_preview = re.sub(B'[^!-~]', B'.', chunk).decode('ascii')
             line = (
                 F'{dump:<{hex_width*columns-len(separator)}}'
                 F'{metrics.txt_separator}{ascii_preview:<{columns}}'
             )
         else:
             def byte_color(value: int):
                 if not value:
                     return FG.LIGHTBLACK_EX
-                elif value in B'\x20\t\n\r\v\f':
-                    return FG.LIGHTYELLOW_EX
+                elif value in B'\x20\t\n\r':
+                    return FG.CYAN
                 elif value not in printable:
                     return FG.LIGHTRED_EX
                 else:
-                    return S.RESET_ALL
+                    return color_reset
+            color_prefix = current_color = color_reset
             with io.StringIO() as _hex, io.StringIO() as _asc:
-                current_color = S.RESET_ALL
                 block_size = metrics.block_size
                 prefix = metrics.hex_char_prefix
                 remaining_hex_width = hex_width * columns - len(separator)
                 for k, b in enumerate(chunk):
                     if k % block_size == 0:
                         if k != 0:
                             _hex.write(separator)
@@ -146,21 +148,21 @@
                     if color != current_color:
                         _hex.write(color)
                         _asc.write(color)
                         current_color = color
                     _hex.write(F'{b:02X}')
                     remaining_hex_width -= 2
                     _asc.write(chr(b) if b in printable else '.')
-                _hex.write(S.RESET_ALL)
+                _hex.write(color_reset)
                 _hex.write(' ' * remaining_hex_width)
-                _asc.write(S.RESET_ALL)
+                _asc.write(color_reset)
                 line = F'{_hex.getvalue()}{metrics.txt_separator}{_asc.getvalue():<{columns}}'
 
         if addr_width:
-            line = F'{lno*columns:0{addr_width}X}: {line}'
+            line = F'{color_prefix}{lno*columns:0{addr_width}X}: {line}'
 
         yield line
 
         if not metrics.expand:
             previous = chunk
```

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/asm.py` & `binary-refinery-0.6.9/refinery/units/sinks/asm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/dump.py` & `binary-refinery-0.6.9/refinery/units/sinks/dump.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/iemap.py` & `binary-refinery-0.6.9/refinery/units/sinks/iemap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/peek.py` & `binary-refinery-0.6.9/refinery/units/sinks/peek.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,14 @@
     @HexViewer.Requires('colorama')
     def _colorama():
         import colorama
         return colorama
 
     def process(self, data):
         colorize = not self.args.gray and not self.args.stdout
-        if os.name == 'nt' and not self.isatty:
-            # coloring stderr does not work properly in Windows when stdout is redirected:
-            # https://github.com/tartley/colorama/issues/200
-            colorize = False
         lines = self._peeklines(data, colorize)
 
         if self.args.stdout:
             for line in lines:
                 yield line.encode(self.codec)
             return
```

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/ppjscript.py` & `binary-refinery-0.6.9/refinery/units/sinks/ppjscript.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/ppjson.py` & `binary-refinery-0.6.9/refinery/units/sinks/ppjson.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/sinks/ppxml.py` & `binary-refinery-0.6.9/refinery/units/sinks/ppxml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/cfmt.py` & `binary-refinery-0.6.9/refinery/units/strings/cfmt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/cswap.py` & `binary-refinery-0.6.9/refinery/units/strings/cswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/rep.py` & `binary-refinery-0.6.9/refinery/units/strings/rep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/repl.py` & `binary-refinery-0.6.9/refinery/units/strings/repl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/snip.py` & `binary-refinery-0.6.9/refinery/units/strings/snip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/stretch.py` & `binary-refinery-0.6.9/refinery/units/strings/stretch.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/termfit.py` & `binary-refinery-0.6.9/refinery/units/strings/termfit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/refinery/units/strings/trim.py` & `binary-refinery-0.6.9/refinery/units/strings/trim.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.8/setup.py` & `binary-refinery-0.6.9/setup.py`

 * *Files identical despite different names*

