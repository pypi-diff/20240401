# Comparing `tmp/pi_heif-0.9.2.tar.gz` & `tmp/pi_heif-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi_heif-0.9.2.tar", last modified: Wed Jan 18 10:47:05 2023, max compression
+gzip compressed data, was "pi_heif-0.9.3.tar", last modified: Sun Jan 22 22:58:27 2023, max compression
```

## Comparing `pi_heif-0.9.2.tar` & `pi_heif-0.9.3.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.112211 pi_heif-0.9.2/
--rw-r--r--   0 runner     (501) staff       (20)    22327 2023-01-18 10:45:07.000000 pi_heif-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner     (501) staff       (20)    11357 2023-01-18 10:45:07.000000 pi_heif-0.9.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      570 2023-01-18 10:45:08.000000 pi_heif-0.9.2/LICENSES_bundled.txt
--rw-r--r--   0 runner     (501) staff       (20)      378 2023-01-18 10:45:08.000000 pi_heif-0.9.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     5413 2023-01-18 10:47:05.112435 pi_heif-0.9.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3772 2023-01-18 10:45:08.000000 pi_heif-0.9.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.027400 pi_heif-0.9.2/examples/
--rw-r--r--   0 runner     (501) staff       (20)      870 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/heif_add_del_thumbnails.py
--rw-r--r--   0 runner     (501) staff       (20)      757 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/heif_create_sequence.py
--rw-r--r--   0 runner     (501) staff       (20)     3138 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/heif_dump_info.py
--rw-r--r--   0 runner     (501) staff       (20)      666 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/heif_enumerate.py
--rw-r--r--   0 runner     (501) staff       (20)      548 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/heif_remove_image.py
--rw-r--r--   0 runner     (501) staff       (20)      679 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/heif_save.py
--rw-r--r--   0 runner     (501) staff       (20)      971 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/pillow_add_del_thumbnails.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/pillow_create_sequence.py
--rw-r--r--   0 runner     (501) staff       (20)     2083 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/pillow_dump_info.py
--rw-r--r--   0 runner     (501) staff       (20)      658 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/pillow_enumerate.py
--rw-r--r--   0 runner     (501) staff       (20)      740 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/pillow_remove_image.py
--rw-r--r--   0 runner     (501) staff       (20)      544 2023-01-18 10:45:07.000000 pi_heif-0.9.2/examples/pillow_save.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.028966 pi_heif-0.9.2/libheif/
--rw-r--r--   0 runner     (501) staff       (20)     2943 2023-01-18 10:45:08.000000 pi_heif-0.9.2/libheif/build.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.012979 pi_heif-0.9.2/libheif/linux/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.029639 pi_heif-0.9.2/libheif/linux/aom-musl/
--rw-r--r--   0 runner     (501) staff       (20)     2356 2023-01-18 10:45:07.000000 pi_heif-0.9.2/libheif/linux/aom-musl/fix-stack-size-e53da0b-2.patch
--rw-r--r--   0 runner     (501) staff       (20)    10688 2023-01-18 10:45:07.000000 pi_heif-0.9.2/libheif/linux_build_libs.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.030226 pi_heif-0.9.2/libheif/macos/
--rw-r--r--   0 runner     (501) staff       (20)      660 2023-01-18 10:45:08.000000 pi_heif-0.9.2/libheif/macos/libheif.rb
--rw-r--r--   0 runner     (501) staff       (20)    50392 2023-01-18 10:45:07.000000 pi_heif-0.9.2/libheif/public_api.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.013621 pi_heif-0.9.2/libheif/windows/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.030733 pi_heif-0.9.2/libheif/windows/mingw-w64-libheif/
--rw-r--r--   0 runner     (501) staff       (20)     1798 2023-01-18 10:45:08.000000 pi_heif-0.9.2/libheif/windows/mingw-w64-libheif/PKGBUILD
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.039202 pi_heif-0.9.2/pi_heif/
--rw-r--r--   0 runner     (501) staff       (20)      138 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pi_heif/AvifImagePlugin.py
--rw-r--r--   0 runner     (501) staff       (20)      137 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pi_heif/HeifImagePlugin.py
--rw-r--r--   0 runner     (501) staff       (20)      600 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pi_heif/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2102 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/_lib_info.py
--rw-r--r--   0 runner     (501) staff       (20)     3818 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/_libheif_ctx.py
--rw-r--r--   0 runner     (501) staff       (20)       50 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/_version.py
--rw-r--r--   0 runner     (501) staff       (20)     7696 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pi_heif/as_plugin.py
--rw-r--r--   0 runner     (501) staff       (20)     3568 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/constants.py
--rw-r--r--   0 runner     (501) staff       (20)     1246 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/error.py
--rw-r--r--   0 runner     (501) staff       (20)    34153 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/heif.py
--rw-r--r--   0 runner     (501) staff       (20)    18421 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pi_heif/helpers.c
--rw-r--r--   0 runner     (501) staff       (20)     2740 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pi_heif/helpers.h
--rw-r--r--   0 runner     (501) staff       (20)     4256 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/misc.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/options.py
--rw-r--r--   0 runner     (501) staff       (20)    12565 2023-01-18 10:45:08.000000 pi_heif-0.9.2/pi_heif/private.py
--rw-r--r--   0 runner     (501) staff       (20)     3434 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pi_heif/thumbnails.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.042136 pi_heif-0.9.2/pi_heif.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5413 2023-01-18 10:47:04.000000 pi_heif-0.9.2/pi_heif.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3798 2023-01-18 10:47:05.000000 pi_heif-0.9.2/pi_heif.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-18 10:47:04.000000 pi_heif-0.9.2/pi_heif.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-18 10:47:04.000000 pi_heif-0.9.2/pi_heif.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      119 2023-01-18 10:47:04.000000 pi_heif-0.9.2/pi_heif.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       22 2023-01-18 10:47:04.000000 pi_heif-0.9.2/pi_heif.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1984 2023-01-18 10:45:07.000000 pi_heif-0.9.2/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1611 2023-01-18 10:47:05.113371 pi_heif-0.9.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      804 2023-01-18 10:45:08.000000 pi_heif-0.9.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.050422 pi_heif-0.9.2/tests/
--rw-r--r--   0 runner     (501) staff       (20)     4696 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/basic_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1148 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8154 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/helpers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.016588 pi_heif-0.9.2/tests/images/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.061004 pi_heif-0.9.2/tests/images/heif/
--rw-r--r--   0 runner     (501) staff       (20)      436 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/L_10.avif
--rw-r--r--   0 runner     (501) staff       (20)     1071 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/L_10.heif
--rw-r--r--   0 runner     (501) staff       (20)      490 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/L_12.avif
--rw-r--r--   0 runner     (501) staff       (20)     1193 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/L_12.heif
--rw-r--r--   0 runner     (501) staff       (20)     5867 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGBA_10.avif
--rw-r--r--   0 runner     (501) staff       (20)     7371 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGBA_10.heif
--rw-r--r--   0 runner     (501) staff       (20)     8355 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGBA_12.avif
--rw-r--r--   0 runner     (501) staff       (20)    10246 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGBA_12.heif
--rw-r--r--   0 runner     (501) staff       (20)   204222 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGB_10.avif
--rw-r--r--   0 runner     (501) staff       (20)   123409 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGB_10.heif
--rw-r--r--   0 runner     (501) staff       (20)   288926 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGB_12.avif
--rw-r--r--   0 runner     (501) staff       (20)   208858 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/RGB_12.heif
--rw-r--r--   0 runner     (501) staff       (20)    15881 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/xmp.heif
--rw-r--r--   0 runner     (501) staff       (20)    22074 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif/zPug_3.heic
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.063538 pi_heif-0.9.2/tests/images/heif_corrupted/
--rw-r--r--   0 runner     (501) staff       (20)    31207 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_corrupted/corrupted.avif
--rw-r--r--   0 runner     (501) staff       (20)     4785 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_corrupted/corrupted.heic
--rw-r--r--   0 runner     (501) staff       (20)    28851 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_corrupted/corrupted.hif
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_corrupted/empty.heic
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.074329 pi_heif-0.9.2/tests/images/heif_other/
--rw-r--r--   0 runner     (501) staff       (20)   792052 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/arrow.heic
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.095755 pi_heif-0.9.2/tests/images/heif_other/avif/
--rw-r--r--   0 runner     (501) staff       (20)    20131 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/LICENSE.txt
--rw-r--r--   0 runner     (501) staff       (20)      174 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/README.txt
--rw-r--r--   0 runner     (501) staff       (20)    83040 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.avif
--rw-r--r--   0 runner     (501) staff       (20)    71882 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.monochrome.avif
--rw-r--r--   0 runner     (501) staff       (20)    80743 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.avif
--rw-r--r--   0 runner     (501) staff       (20)    69856 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.monochrome.avif
--rw-r--r--   0 runner     (501) staff       (20)    97436 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile1.10bpc.yuv444.avif
--rw-r--r--   0 runner     (501) staff       (20)    95375 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile1.8bpc.yuv444.avif
--rw-r--r--   0 runner     (501) staff       (20)    89097 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.avif
--rw-r--r--   0 runner     (501) staff       (20)    71878 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.monochrome.avif
--rw-r--r--   0 runner     (501) staff       (20)    84078 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.avif
--rw-r--r--   0 runner     (501) staff       (20)    73014 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.monochrome.avif
--rw-r--r--   0 runner     (501) staff       (20)    90198 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.avif
--rw-r--r--   0 runner     (501) staff       (20)    73014 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.monochrome.avif
--rw-r--r--   0 runner     (501) staff       (20)    98800 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.avif
--rw-r--r--   0 runner     (501) staff       (20)    73014 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.monochrome.avif
--rw-r--r--   0 runner     (501) staff       (20)    86782 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.avif
--rw-r--r--   0 runner     (501) staff       (20)    69852 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.monochrome.avif
--rw-r--r--   0 runner     (501) staff       (20)  2641920 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/cat.hif
--rw-r--r--   0 runner     (501) staff       (20)   156055 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/empty_icc.heic
--rw-r--r--   0 runner     (501) staff       (20)   126947 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/invalid_id.heic
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.101608 pi_heif-0.9.2/tests/images/heif_other/nokia/
--rw-r--r--   0 runner     (501) staff       (20)      119 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/nokia/COPYRIGHT.txt
--rw-r--r--   0 runner     (501) staff       (20)       71 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/nokia/README.txt
--rw-r--r--   0 runner     (501) staff       (20)   443075 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/nokia/alpha.heic
--rw-r--r--   0 runner     (501) staff       (20)   470071 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_other/nokia/bird_burst.heic
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.103610 pi_heif-0.9.2/tests/images/heif_truncated/
--rw-r--r--   0 runner     (501) staff       (20)  1148758 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/heif_truncated/truncated.heic
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-18 10:47:05.111782 pi_heif-0.9.2/tests/images/non_heif/
--rw-r--r--   0 runner     (501) staff       (20)      302 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/L_16.png
--rw-r--r--   0 runner     (501) staff       (20)     6874 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/RGBA_16.png
--rw-r--r--   0 runner     (501) staff       (20)     3974 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/RGB_16.png
--rw-r--r--   0 runner     (501) staff       (20)    85539 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/chi.gif
--rw-r--r--   0 runner     (501) staff       (20)     3510 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/xmp.jpeg
--rw-r--r--   0 runner     (501) staff       (20)      526 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/xmp.png
--rw-r--r--   0 runner     (501) staff       (20)     3298 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/xmp.tiff
--rw-r--r--   0 runner     (501) staff       (20)      492 2023-01-18 10:45:07.000000 pi_heif-0.9.2/tests/images/non_heif/xmp.webp
--rw-r--r--   0 runner     (501) staff       (20)     3462 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/leaks_test.py
--rw-r--r--   0 runner     (501) staff       (20)     8915 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/metadata_etc_test.py
--rw-r--r--   0 runner     (501) staff       (20)     7866 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/metadata_exif_test.py
--rw-r--r--   0 runner     (501) staff       (20)     4316 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/metadata_xmp_test.py
--rw-r--r--   0 runner     (501) staff       (20)     4427 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/mode_convert_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1938 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/numpy_test.py
--rw-r--r--   0 runner     (501) staff       (20)     4257 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/opencv_test.py
--rw-r--r--   0 runner     (501) staff       (20)     3911 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/options_test.py
--rw-r--r--   0 runner     (501) staff       (20)     7797 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/orientation_test.py
--rw-r--r--   0 runner     (501) staff       (20)    15014 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/read_test.py
--rw-r--r--   0 runner     (501) staff       (20)    11654 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/thumbnails_test.py
--rw-r--r--   0 runner     (501) staff       (20)    16221 2023-01-18 10:45:08.000000 pi_heif-0.9.2/tests/write_test.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.115440 pi_heif-0.9.3/
+-rw-r--r--   0 runner     (501) staff       (20)    22606 2023-01-22 22:56:10.000000 pi_heif-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner     (501) staff       (20)    11357 2023-01-22 22:56:10.000000 pi_heif-0.9.3/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      570 2023-01-22 22:56:10.000000 pi_heif-0.9.3/LICENSES_bundled.txt
+-rw-r--r--   0 runner     (501) staff       (20)      378 2023-01-22 22:56:11.000000 pi_heif-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     5413 2023-01-22 22:58:27.115678 pi_heif-0.9.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3772 2023-01-22 22:56:10.000000 pi_heif-0.9.3/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:26.998928 pi_heif-0.9.3/examples/
+-rw-r--r--   0 runner     (501) staff       (20)      870 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/heif_add_del_thumbnails.py
+-rw-r--r--   0 runner     (501) staff       (20)      757 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/heif_create_sequence.py
+-rw-r--r--   0 runner     (501) staff       (20)     3138 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/heif_dump_info.py
+-rw-r--r--   0 runner     (501) staff       (20)      666 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/heif_enumerate.py
+-rw-r--r--   0 runner     (501) staff       (20)      548 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/heif_remove_image.py
+-rw-r--r--   0 runner     (501) staff       (20)      679 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/heif_save.py
+-rw-r--r--   0 runner     (501) staff       (20)      971 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/pillow_add_del_thumbnails.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/pillow_create_sequence.py
+-rw-r--r--   0 runner     (501) staff       (20)     2083 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/pillow_dump_info.py
+-rw-r--r--   0 runner     (501) staff       (20)      658 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/pillow_enumerate.py
+-rw-r--r--   0 runner     (501) staff       (20)      740 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/pillow_remove_image.py
+-rw-r--r--   0 runner     (501) staff       (20)      544 2023-01-22 22:56:10.000000 pi_heif-0.9.3/examples/pillow_save.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.000917 pi_heif-0.9.3/libheif/
+-rw-r--r--   0 runner     (501) staff       (20)     2943 2023-01-22 22:56:11.000000 pi_heif-0.9.3/libheif/build.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:26.980575 pi_heif-0.9.3/libheif/linux/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.001740 pi_heif-0.9.3/libheif/linux/aom-musl/
+-rw-r--r--   0 runner     (501) staff       (20)     2356 2023-01-22 22:56:10.000000 pi_heif-0.9.3/libheif/linux/aom-musl/fix-stack-size-e53da0b-2.patch
+-rw-r--r--   0 runner     (501) staff       (20)    10688 2023-01-22 22:56:10.000000 pi_heif-0.9.3/libheif/linux_build_libs.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.002344 pi_heif-0.9.3/libheif/macos/
+-rw-r--r--   0 runner     (501) staff       (20)      660 2023-01-22 22:56:10.000000 pi_heif-0.9.3/libheif/macos/libheif.rb
+-rw-r--r--   0 runner     (501) staff       (20)    50392 2023-01-22 22:56:10.000000 pi_heif-0.9.3/libheif/public_api.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:26.981400 pi_heif-0.9.3/libheif/windows/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.002949 pi_heif-0.9.3/libheif/windows/mingw-w64-libheif/
+-rw-r--r--   0 runner     (501) staff       (20)     1798 2023-01-22 22:56:10.000000 pi_heif-0.9.3/libheif/windows/mingw-w64-libheif/PKGBUILD
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.014635 pi_heif-0.9.3/pi_heif/
+-rw-r--r--   0 runner     (501) staff       (20)      138 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pi_heif/AvifImagePlugin.py
+-rw-r--r--   0 runner     (501) staff       (20)      137 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pi_heif/HeifImagePlugin.py
+-rw-r--r--   0 runner     (501) staff       (20)      600 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pi_heif/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2102 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/_lib_info.py
+-rw-r--r--   0 runner     (501) staff       (20)     3818 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/_libheif_ctx.py
+-rw-r--r--   0 runner     (501) staff       (20)       50 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)     7696 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pi_heif/as_plugin.py
+-rw-r--r--   0 runner     (501) staff       (20)     3568 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)     1246 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/error.py
+-rw-r--r--   0 runner     (501) staff       (20)    34153 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/heif.py
+-rw-r--r--   0 runner     (501) staff       (20)    18421 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pi_heif/helpers.c
+-rw-r--r--   0 runner     (501) staff       (20)     2740 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pi_heif/helpers.h
+-rw-r--r--   0 runner     (501) staff       (20)     5058 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/misc.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/options.py
+-rw-r--r--   0 runner     (501) staff       (20)    12565 2023-01-22 22:56:11.000000 pi_heif-0.9.3/pi_heif/private.py
+-rw-r--r--   0 runner     (501) staff       (20)     3434 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pi_heif/thumbnails.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.018467 pi_heif-0.9.3/pi_heif.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5413 2023-01-22 22:58:26.000000 pi_heif-0.9.3/pi_heif.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3838 2023-01-22 22:58:26.000000 pi_heif-0.9.3/pi_heif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-22 22:58:26.000000 pi_heif-0.9.3/pi_heif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-22 22:58:26.000000 pi_heif-0.9.3/pi_heif.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      119 2023-01-22 22:58:26.000000 pi_heif-0.9.3/pi_heif.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       22 2023-01-22 22:58:26.000000 pi_heif-0.9.3/pi_heif.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2009 2023-01-22 22:56:10.000000 pi_heif-0.9.3/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1611 2023-01-22 22:58:27.116727 pi_heif-0.9.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      804 2023-01-22 22:56:11.000000 pi_heif-0.9.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.030848 pi_heif-0.9.3/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     4696 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/basic_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1148 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8154 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/helpers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:26.984822 pi_heif-0.9.3/tests/images/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.049330 pi_heif-0.9.3/tests/images/heif/
+-rw-r--r--   0 runner     (501) staff       (20)      436 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/L_10.avif
+-rw-r--r--   0 runner     (501) staff       (20)     1071 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/L_10.heif
+-rw-r--r--   0 runner     (501) staff       (20)      490 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/L_12.avif
+-rw-r--r--   0 runner     (501) staff       (20)     1193 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/L_12.heif
+-rw-r--r--   0 runner     (501) staff       (20)     5867 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGBA_10.avif
+-rw-r--r--   0 runner     (501) staff       (20)     7371 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGBA_10.heif
+-rw-r--r--   0 runner     (501) staff       (20)     8355 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGBA_12.avif
+-rw-r--r--   0 runner     (501) staff       (20)    10246 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGBA_12.heif
+-rw-r--r--   0 runner     (501) staff       (20)   204222 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGB_10.avif
+-rw-r--r--   0 runner     (501) staff       (20)   123409 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGB_10.heif
+-rw-r--r--   0 runner     (501) staff       (20)   288926 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGB_12.avif
+-rw-r--r--   0 runner     (501) staff       (20)   208858 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/RGB_12.heif
+-rw-r--r--   0 runner     (501) staff       (20)    15881 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/xmp.heif
+-rw-r--r--   0 runner     (501) staff       (20)    22074 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif/zPug_3.heic
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.052785 pi_heif-0.9.3/tests/images/heif_corrupted/
+-rw-r--r--   0 runner     (501) staff       (20)    31207 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_corrupted/corrupted.avif
+-rw-r--r--   0 runner     (501) staff       (20)     4785 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_corrupted/corrupted.heic
+-rw-r--r--   0 runner     (501) staff       (20)    28851 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_corrupted/corrupted.hif
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_corrupted/empty.heic
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.072388 pi_heif-0.9.3/tests/images/heif_other/
+-rw-r--r--   0 runner     (501) staff       (20)   792052 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/arrow.heic
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.093485 pi_heif-0.9.3/tests/images/heif_other/avif/
+-rw-r--r--   0 runner     (501) staff       (20)    20131 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/LICENSE.txt
+-rw-r--r--   0 runner     (501) staff       (20)      174 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/README.txt
+-rw-r--r--   0 runner     (501) staff       (20)    83040 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.avif
+-rw-r--r--   0 runner     (501) staff       (20)    71882 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.monochrome.avif
+-rw-r--r--   0 runner     (501) staff       (20)    80743 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.avif
+-rw-r--r--   0 runner     (501) staff       (20)    69856 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.monochrome.avif
+-rw-r--r--   0 runner     (501) staff       (20)    97436 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile1.10bpc.yuv444.avif
+-rw-r--r--   0 runner     (501) staff       (20)    95375 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile1.8bpc.yuv444.avif
+-rw-r--r--   0 runner     (501) staff       (20)    89097 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.avif
+-rw-r--r--   0 runner     (501) staff       (20)    71878 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.monochrome.avif
+-rw-r--r--   0 runner     (501) staff       (20)    84078 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.avif
+-rw-r--r--   0 runner     (501) staff       (20)    73014 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.monochrome.avif
+-rw-r--r--   0 runner     (501) staff       (20)    90198 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.avif
+-rw-r--r--   0 runner     (501) staff       (20)    73014 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.monochrome.avif
+-rw-r--r--   0 runner     (501) staff       (20)    98800 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.avif
+-rw-r--r--   0 runner     (501) staff       (20)    73014 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.monochrome.avif
+-rw-r--r--   0 runner     (501) staff       (20)    86782 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.avif
+-rw-r--r--   0 runner     (501) staff       (20)    69852 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.monochrome.avif
+-rw-r--r--   0 runner     (501) staff       (20)  2641920 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/cat.hif
+-rw-r--r--   0 runner     (501) staff       (20)   156055 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/empty_icc.heic
+-rw-r--r--   0 runner     (501) staff       (20)   126947 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/invalid_id.heic
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.098394 pi_heif-0.9.3/tests/images/heif_other/nokia/
+-rw-r--r--   0 runner     (501) staff       (20)      119 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/nokia/COPYRIGHT.txt
+-rw-r--r--   0 runner     (501) staff       (20)       71 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/nokia/README.txt
+-rw-r--r--   0 runner     (501) staff       (20)   443075 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/nokia/alpha.heic
+-rw-r--r--   0 runner     (501) staff       (20)   470071 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/nokia/bird_burst.heic
+-rw-r--r--   0 runner     (501) staff       (20)     1477 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_other/xmp_latin1.heic
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.100920 pi_heif-0.9.3/tests/images/heif_truncated/
+-rw-r--r--   0 runner     (501) staff       (20)  1148758 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/heif_truncated/truncated.heic
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-22 22:58:27.114728 pi_heif-0.9.3/tests/images/non_heif/
+-rw-r--r--   0 runner     (501) staff       (20)      302 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/L_16.png
+-rw-r--r--   0 runner     (501) staff       (20)     6874 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/RGBA_16.png
+-rw-r--r--   0 runner     (501) staff       (20)     3974 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/RGB_16.png
+-rw-r--r--   0 runner     (501) staff       (20)    85539 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/chi.gif
+-rw-r--r--   0 runner     (501) staff       (20)     3510 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/xmp.jpeg
+-rw-r--r--   0 runner     (501) staff       (20)      526 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/xmp.png
+-rw-r--r--   0 runner     (501) staff       (20)     3298 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/xmp.tiff
+-rw-r--r--   0 runner     (501) staff       (20)      492 2023-01-22 22:56:10.000000 pi_heif-0.9.3/tests/images/non_heif/xmp.webp
+-rw-r--r--   0 runner     (501) staff       (20)     3462 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/leaks_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     8915 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/metadata_etc_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     7866 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/metadata_exif_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     4787 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/metadata_xmp_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     4427 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/mode_convert_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1938 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/numpy_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     4257 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/opencv_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     3995 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/options_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     7797 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/orientation_test.py
+-rw-r--r--   0 runner     (501) staff       (20)    15014 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/read_test.py
+-rw-r--r--   0 runner     (501) staff       (20)    11654 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/thumbnails_test.py
+-rw-r--r--   0 runner     (501) staff       (20)    16221 2023-01-22 22:56:11.000000 pi_heif-0.9.3/tests/write_test.py
```

### Comparing `pi_heif-0.9.2/CHANGELOG.md` & `pi_heif-0.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 _# Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.9.3 - 2023-01-22]
+
+### Fixed
+
+Two bugs in XMP metadata handling that were causing exceptions. All versions were affected.
+Thanks to @eeyrw for pointing out such a problem.
+
+- Handling XMP data with `zero` byte at the end. #69
+- Handling XMP data in `latin1` encoding. #69
+
 ## [0.9.2 - 2023-01-18]
 
 ### Changed
 
 - libheif updated from `1.14.0` to `1.14.2`
 
 ## [0.9.1 - 2023-01-02]
```

### Comparing `pi_heif-0.9.2/LICENSE` & `pi_heif-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/LICENSES_bundled.txt` & `pi_heif-0.9.3/LICENSES_bundled.txt`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/PKG-INFO` & `pi_heif-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi_heif
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python interface for libheif library
 Home-page: https://github.com/bigcat88/pillow_heif
 Author: Alexander Piskun
 Author-email: bigcat88@users.noreply.github.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pillow-heif.readthedocs.io
 Project-URL: Source, https://github.com/bigcat88/pillow_heif
```

### Comparing `pi_heif-0.9.2/README.md` & `pi_heif-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/heif_add_del_thumbnails.py` & `pi_heif-0.9.3/examples/heif_add_del_thumbnails.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/heif_create_sequence.py` & `pi_heif-0.9.3/examples/heif_create_sequence.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/heif_dump_info.py` & `pi_heif-0.9.3/examples/heif_dump_info.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/heif_enumerate.py` & `pi_heif-0.9.3/examples/heif_enumerate.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/heif_remove_image.py` & `pi_heif-0.9.3/examples/heif_remove_image.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/heif_save.py` & `pi_heif-0.9.3/examples/heif_save.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/pillow_add_del_thumbnails.py` & `pi_heif-0.9.3/examples/pillow_add_del_thumbnails.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/pillow_create_sequence.py` & `pi_heif-0.9.3/examples/pillow_create_sequence.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/pillow_dump_info.py` & `pi_heif-0.9.3/examples/pillow_dump_info.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/pillow_enumerate.py` & `pi_heif-0.9.3/examples/pillow_enumerate.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/pillow_remove_image.py` & `pi_heif-0.9.3/examples/pillow_remove_image.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/examples/pillow_save.py` & `pi_heif-0.9.3/examples/pillow_save.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/libheif/build.py` & `pi_heif-0.9.3/libheif/build.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/libheif/linux/aom-musl/fix-stack-size-e53da0b-2.patch` & `pi_heif-0.9.3/libheif/linux/aom-musl/fix-stack-size-e53da0b-2.patch`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/libheif/linux_build_libs.py` & `pi_heif-0.9.3/libheif/linux_build_libs.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/libheif/macos/libheif.rb` & `pi_heif-0.9.3/libheif/macos/libheif.rb`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/libheif/public_api.h` & `pi_heif-0.9.3/libheif/public_api.h`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/libheif/windows/mingw-w64-libheif/PKGBUILD` & `pi_heif-0.9.3/libheif/windows/mingw-w64-libheif/PKGBUILD`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/__init__.py` & `pi_heif-0.9.3/pi_heif/__init__.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/_lib_info.py` & `pi_heif-0.9.3/pi_heif/_lib_info.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/_libheif_ctx.py` & `pi_heif-0.9.3/pi_heif/_libheif_ctx.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/as_plugin.py` & `pi_heif-0.9.3/pi_heif/as_plugin.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/constants.py` & `pi_heif-0.9.3/pi_heif/constants.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/error.py` & `pi_heif-0.9.3/pi_heif/error.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/heif.py` & `pi_heif-0.9.3/pi_heif/heif.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/helpers.c` & `pi_heif-0.9.3/pi_heif/helpers.c`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/helpers.h` & `pi_heif-0.9.3/pi_heif/helpers.h`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/misc.py` & `pi_heif-0.9.3/pi_heif/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,22 +47,35 @@
                     p_value = 6 + pointer + 8
                     new_orientation = pack(endian_mark + "H", orientation)
                     info["exif"] = info["exif"][:p_value] + new_orientation + info["exif"][p_value + 2 :]
                     break
         except Exception:  # noqa # pylint: disable=broad-except
             pass
     if info.get("xmp", None):
-        xmp_data = info["xmp"].decode("utf-8")
-        match = re.search(r'tiff:Orientation(="|>)([0-9])', xmp_data)
-        if match:
-            if original_orientation is None and int(match[2]) != 1:
-                original_orientation = int(match[2])
-            xmp_data = re.sub(r'tiff:Orientation="([0-9])"', "", xmp_data)
-            xmp_data = re.sub(r"<tiff:Orientation>([0-9])</tiff:Orientation>", "", xmp_data)
-            info["xmp"] = xmp_data.encode("utf-8")
+        xmp_data = info["xmp"].rsplit(b"\x00", 1)
+        if xmp_data[0]:
+            decoded_xmp_data = None
+            for encoding in ("utf-8", "latin1"):
+                try:
+                    decoded_xmp_data = xmp_data[0].decode(encoding)
+                    break
+                except Exception:  # noqa # pylint: disable=broad-except
+                    pass
+            if decoded_xmp_data:
+                _original_orientation = 1
+                match = re.search(r'tiff:Orientation(="|>)([0-9])', decoded_xmp_data)
+                if match:
+                    _original_orientation = int(match[2])
+                    if original_orientation is None and _original_orientation != 1:
+                        original_orientation = _original_orientation
+                    decoded_xmp_data = re.sub(r'tiff:Orientation="([0-9])"', "", decoded_xmp_data)
+                    decoded_xmp_data = re.sub(r"<tiff:Orientation>([0-9])</tiff:Orientation>", "", decoded_xmp_data)
+                # should encode in "utf-8" anyway, as `defusedxml` do not work with `latin1` encoding.
+                if encoding != "utf-8" or _original_orientation != 1:
+                    info["xmp"] = b"".join([decoded_xmp_data.encode("utf-8"), b"\x00" if len(xmp_data) > 1 else b""])
     return original_orientation
 
 
 def get_file_mimetype(fp) -> str:
     """Gets the MIME type of the HEIF(or AVIF) object.`
 
     :param fp: A filename (string), pathlib.Path object, file object or bytes.
```

### Comparing `pi_heif-0.9.2/pi_heif/options.py` & `pi_heif-0.9.3/pi_heif/options.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/private.py` & `pi_heif-0.9.3/pi_heif/private.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif/thumbnails.py` & `pi_heif-0.9.3/pi_heif/thumbnails.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/pi_heif.egg-info/PKG-INFO` & `pi_heif-0.9.3/pi_heif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-heif
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python interface for libheif library
 Home-page: https://github.com/bigcat88/pillow_heif
 Author: Alexander Piskun
 Author-email: bigcat88@users.noreply.github.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pillow-heif.readthedocs.io
 Project-URL: Source, https://github.com/bigcat88/pillow_heif
```

### Comparing `pi_heif-0.9.2/pi_heif.egg-info/SOURCES.txt` & `pi_heif-0.9.3/pi_heif.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 tests/images/heif_corrupted/corrupted.heic
 tests/images/heif_corrupted/corrupted.hif
 tests/images/heif_corrupted/empty.heic
 tests/images/heif_other/arrow.heic
 tests/images/heif_other/cat.hif
 tests/images/heif_other/empty_icc.heic
 tests/images/heif_other/invalid_id.heic
+tests/images/heif_other/xmp_latin1.heic
 tests/images/heif_other/avif/LICENSE.txt
 tests/images/heif_other/avif/README.txt
 tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.avif
 tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.monochrome.avif
 tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.avif
 tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.monochrome.avif
 tests/images/heif_other/avif/fox.profile1.10bpc.yuv444.avif
```

### Comparing `pi_heif-0.9.2/pyproject.toml` & `pi_heif-0.9.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 [tool.isort]
 profile = "black"
 
 [tool.pylint]
 master.py-version = "3.7"
 master.extension-pkg-allow-list = ["_pillow_heif_cffi"]
 design.max-attributes = 9
-design.max-locals = 16
+design.max-branches = 14
+design.max-locals = 18
 design.max-returns = 8
 basic.good-names = [
     "a", "b", "c", "d", "e", "f", "i", "j", "k", "v",
     "ex", "_", "fp", "im", "HeifImagePlugin", "AvifImagePlugin",
 ]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
```

### Comparing `pi_heif-0.9.2/setup.cfg` & `pi_heif-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/setup.py` & `pi_heif-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/basic_test.py` & `pi_heif-0.9.3/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/dataset.py` & `pi_heif-0.9.3/tests/dataset.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/helpers.py` & `pi_heif-0.9.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/L_10.heif` & `pi_heif-0.9.3/tests/images/heif/L_10.heif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/L_12.heif` & `pi_heif-0.9.3/tests/images/heif/L_12.heif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGBA_10.avif` & `pi_heif-0.9.3/tests/images/heif/RGBA_10.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGBA_10.heif` & `pi_heif-0.9.3/tests/images/heif/RGBA_10.heif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGBA_12.avif` & `pi_heif-0.9.3/tests/images/heif/RGBA_12.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGBA_12.heif` & `pi_heif-0.9.3/tests/images/heif/RGBA_12.heif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGB_10.avif` & `pi_heif-0.9.3/tests/images/heif/RGB_10.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGB_10.heif` & `pi_heif-0.9.3/tests/images/heif/RGB_10.heif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGB_12.avif` & `pi_heif-0.9.3/tests/images/heif/RGB_12.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/RGB_12.heif` & `pi_heif-0.9.3/tests/images/heif/RGB_12.heif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/xmp.heif` & `pi_heif-0.9.3/tests/images/heif/xmp.heif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif/zPug_3.heic` & `pi_heif-0.9.3/tests/images/heif/zPug_3.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_corrupted/corrupted.avif` & `pi_heif-0.9.3/tests/images/heif_corrupted/corrupted.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_corrupted/corrupted.heic` & `pi_heif-0.9.3/tests/images/heif_corrupted/corrupted.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_corrupted/corrupted.hif` & `pi_heif-0.9.3/tests/images/heif_corrupted/corrupted.hif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/arrow.heic` & `pi_heif-0.9.3/tests/images/heif_other/arrow.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/LICENSE.txt` & `pi_heif-0.9.3/tests/images/heif_other/avif/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.monochrome.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.10bpc.yuv420.monochrome.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.monochrome.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile0.8bpc.yuv420.monochrome.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile1.10bpc.yuv444.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile1.10bpc.yuv444.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile1.8bpc.yuv444.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile1.8bpc.yuv444.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.monochrome.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.10bpc.yuv422.monochrome.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.monochrome.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv420.monochrome.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.monochrome.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv422.monochrome.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.monochrome.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.12bpc.yuv444.monochrome.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.monochrome.avif` & `pi_heif-0.9.3/tests/images/heif_other/avif/fox.profile2.8bpc.yuv422.monochrome.avif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/cat.hif` & `pi_heif-0.9.3/tests/images/heif_other/cat.hif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/empty_icc.heic` & `pi_heif-0.9.3/tests/images/heif_other/empty_icc.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/invalid_id.heic` & `pi_heif-0.9.3/tests/images/heif_other/invalid_id.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/nokia/alpha.heic` & `pi_heif-0.9.3/tests/images/heif_other/nokia/alpha.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_other/nokia/bird_burst.heic` & `pi_heif-0.9.3/tests/images/heif_other/nokia/bird_burst.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/heif_truncated/truncated.heic` & `pi_heif-0.9.3/tests/images/heif_truncated/truncated.heic`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/non_heif/RGBA_16.png` & `pi_heif-0.9.3/tests/images/non_heif/RGBA_16.png`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/non_heif/RGB_16.png` & `pi_heif-0.9.3/tests/images/non_heif/RGB_16.png`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/non_heif/chi.gif` & `pi_heif-0.9.3/tests/images/non_heif/chi.gif`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/non_heif/xmp.jpeg` & `pi_heif-0.9.3/tests/images/non_heif/xmp.jpeg`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/non_heif/xmp.png` & `pi_heif-0.9.3/tests/images/non_heif/xmp.png`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/images/non_heif/xmp.tiff` & `pi_heif-0.9.3/tests/images/non_heif/xmp.tiff`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/leaks_test.py` & `pi_heif-0.9.3/tests/leaks_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/metadata_etc_test.py` & `pi_heif-0.9.3/tests/metadata_etc_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/metadata_exif_test.py` & `pi_heif-0.9.3/tests/metadata_exif_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/metadata_xmp_test.py` & `pi_heif-0.9.3/tests/metadata_xmp_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,23 +48,23 @@
     out_heif_no_xmp = BytesIO()
     out_heif = BytesIO()
     im = Image.new("RGB", (15, 15), 0)
     # filling `xmp` during save.
     im.save(out_heif, format="HEIF", xmp=xmp_data)
     assert "xmp" not in im.info or im.info["xmp"] is None
     im_heif = Image.open(out_heif)
-    assert im_heif.info["xmp"]
+    assert im_heif.info["xmp"] == xmp_data
     # filling `info["xmp"]` before save.
     im.info["xmp"] = xmp_data
     im.save(out_heif, format="HEIF")
     im_heif = Image.open(out_heif)
-    assert im_heif.info["xmp"]
+    assert im_heif.info["xmp"] == xmp_data
     # setting `xmp` to `None` during save.
     im_heif.save(out_heif_no_xmp, format="HEIF", xmp=None)
-    assert im_heif.info["xmp"]
+    assert im_heif.info["xmp"] == xmp_data
     im_heif_no_xmp = Image.open(out_heif_no_xmp)
     assert "xmp" not in im_heif_no_xmp.info or im_heif_no_xmp.info["xmp"] is None
     # filling `info["xmp"]` with `None` before save.
     im_heif.info["xmp"] = None
     im_heif.save(out_heif_no_xmp, format="HEIF")
     im_heif_no_xmp = Image.open(out_heif_no_xmp)
     assert "xmp" not in im_heif_no_xmp.info or im_heif_no_xmp.info["xmp"] is None
@@ -81,29 +81,39 @@
     out_heif_no_xmp = BytesIO()
     out_heif = BytesIO()
     # test filling `xmp` during save.
     im_heif = pi_heif.from_pillow(Image.new("RGB", (15, 15), 0))
     im_heif.save(out_heif, xmp=xmp_data)
     assert "xmp" not in im_heif.info or im_heif.info["xmp"] is None
     im_heif = pi_heif.open_heif(out_heif)
-    assert im_heif.info["xmp"]
+    assert im_heif.info["xmp"] == xmp_data
     # test filling `info["xmp"]` before save.
     im_heif = pi_heif.from_pillow(Image.new("RGB", (15, 15), 0))
     im_heif.info["xmp"] = xmp_data
     im_heif.save(out_heif)
     im_heif = pi_heif.open_heif(out_heif)
-    assert im_heif.info["xmp"]
+    assert im_heif.info["xmp"] == xmp_data
     # setting `xmp` to `None` during save.
     im_heif.save(out_heif_no_xmp, xmp=None)
-    assert im_heif.info["xmp"]
+    assert im_heif.info["xmp"] == xmp_data
     im_heif_no_xmp = pi_heif.open_heif(out_heif_no_xmp)
     assert "xmp" not in im_heif_no_xmp.info or im_heif_no_xmp.info["xmp"] is None
     # filling `info["xmp"]` with `None` before save.
     im_heif.info["xmp"] = None
     im_heif.save(out_heif_no_xmp)
     im_heif_no_xmp = pi_heif.open_heif(out_heif_no_xmp)
     assert "xmp" not in im_heif_no_xmp.info or im_heif_no_xmp.info["xmp"] is None
     # removing `info["xmp"]` before save.
     im_heif.info.pop("xmp")
     im_heif.save(out_heif_no_xmp)
     im_heif_no_xmp = pi_heif.open_heif(out_heif_no_xmp)
     assert "xmp" not in im_heif_no_xmp.info or im_heif_no_xmp.info["xmp"] is None
+
+
+@pytest.mark.skipif(not helpers.hevc_enc(), reason="Requires HEVC encoder.")
+def test_heif_xmp_latin1_with_zero_byte():
+    im = Image.open("images/heif_other/xmp_latin1.heic")
+    out_heif = BytesIO()
+    im.save(out_heif, format="HEIF")
+    out_im = Image.open(out_heif)
+    assert im.getxmp() == out_im.getxmp()  # noqa
+    assert out_im.info["xmp"][-1] == 0  # check null byte not to get lost
```

### Comparing `pi_heif-0.9.2/tests/mode_convert_test.py` & `pi_heif-0.9.3/tests/mode_convert_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/numpy_test.py` & `pi_heif-0.9.3/tests/numpy_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/opencv_test.py` & `pi_heif-0.9.3/tests/opencv_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/options_test.py` & `pi_heif-0.9.3/tests/options_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 from io import SEEK_END, BytesIO
 from time import perf_counter
 
 import pytest
 from helpers import aom_enc, create_heif, hevc_enc
 from PIL import Image
 
@@ -71,23 +72,24 @@
         assert out_buf_1_q10.seek(0, SEEK_END) < out_buf_3_q30.seek(0, SEEK_END)
     finally:
         options.QUALITY = None
 
 
 @pytest.mark.skipif(os.cpu_count() < 2, reason="Requires at least a processor with two cores.")
 @pytest.mark.skipif(os.getenv("TEST_DECODE_THREADS", "1") == "0", reason="TEST_DECODE_THREADS set to `0`")
+@pytest.mark.skipif(sys.maxsize <= 2147483647, reason="Run test only on 64 bit CPU.")
 def test_decode_threads():
     test_image = "images/heif_other/arrow.heic"  # not all images can be decoded using more than one thread
     # As we do not know real performance of hardware, measure relative
     try:
         options.DECODE_THREADS = 1
         start_time_one_thread = perf_counter()
         open_heif(test_image, convert_hdr_to_8bit=False).load()
         total_time_one_thread = perf_counter() - start_time_one_thread
-        options.DECODE_THREADS = os.cpu_count()
+        options.DECODE_THREADS = 2
         start_time_multiply_threads = perf_counter()
         open_heif(test_image, convert_hdr_to_8bit=False).load()
         total_time_multiply_threads = perf_counter() - start_time_multiply_threads
         # decoding in multiply threads should be faster at least by 12%
         assert total_time_one_thread > total_time_multiply_threads * 1.12
     finally:
         options.DECODE_THREADS = 4
```

### Comparing `pi_heif-0.9.2/tests/orientation_test.py` & `pi_heif-0.9.3/tests/orientation_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/read_test.py` & `pi_heif-0.9.3/tests/read_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/thumbnails_test.py` & `pi_heif-0.9.3/tests/thumbnails_test.py`

 * *Files identical despite different names*

### Comparing `pi_heif-0.9.2/tests/write_test.py` & `pi_heif-0.9.3/tests/write_test.py`

 * *Files identical despite different names*

