# Comparing `tmp/viaconstructor-0.6.5.tar.gz` & `tmp/viaconstructor-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viaconstructor-0.6.5.tar", last modified: Thu Feb  1 14:48:36 2024, max compression
+gzip compressed data, was "viaconstructor-0.6.6.tar", last modified: Mon Apr  1 19:41:55 2024, max compression
```

## Comparing `viaconstructor-0.6.5.tar` & `viaconstructor-0.6.6.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.218563 viaconstructor-0.6.5/
--rwxr-xr-x   0 root         (0) root         (0)    35147 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      194 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3885 2024-02-01 14:48:36.218563 viaconstructor-0.6.5/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3624 2023-04-08 23:55:39.000000 viaconstructor-0.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.150564 viaconstructor-0.6.5/bin/
--rwxr-xr-x   0 root         (0) root         (0)       36 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/bin/dxfpreview
--rwxr-xr-x   0 root         (0) root         (0)       38 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/bin/gcodepreview
--rwxr-xr-x   0 root         (0) root         (0)       42 2022-08-17 21:04:13.000000 viaconstructor-0.6.5/bin/viaconstructor
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.164564 viaconstructor-0.6.5/dxfpreview/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/dxfpreview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/dxfpreview/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     4131 2022-08-22 19:23:27.000000 viaconstructor-0.6.5/dxfpreview/dxfpreview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.169564 viaconstructor-0.6.5/gcodepreview/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/gcodepreview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       96 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/gcodepreview/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     3630 2022-08-03 19:17:04.000000 viaconstructor-0.6.5/gcodepreview/gcodepreview.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-01 14:48:36.218563 viaconstructor-0.6.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1232 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.186564 viaconstructor-0.6.5/viaconstructor/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/viaconstructor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.5/viaconstructor/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)    50759 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/calc.py
--rwxr-xr-x   0 root         (0) root         (0)    24883 2023-04-02 20:48:58.000000 viaconstructor-0.6.5/viaconstructor/draw2d.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-03-26 08:12:36.000000 viaconstructor-0.6.5/viaconstructor/dxfcolors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.099564 viaconstructor-0.6.5/viaconstructor/ext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.189564 viaconstructor-0.6.5/viaconstructor/ext/HersheyFonts/
--rw-r--r--   0 root         (0) root         (0)    91220 2022-08-22 17:54:34.000000 viaconstructor-0.6.5/viaconstructor/ext/HersheyFonts/HersheyFonts.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-08-22 17:54:34.000000 viaconstructor-0.6.5/viaconstructor/ext/HersheyFonts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      101 2022-08-22 17:54:34.000000 viaconstructor-0.6.5/viaconstructor/ext/HersheyFonts/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.190564 viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/
--rw-r--r--   0 root         (0) root         (0)       39 2022-08-22 18:47:24.000000 viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8813 2023-03-23 17:27:32.000000 viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/cavaliercontours.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.193564 viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/lib/
--rwxr-xr-x   0 root         (0) root         (0)   872112 2023-03-23 17:27:32.000000 viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
--rwxr-xr-x   0 root         (0) root         (0)  1383488 2023-03-23 17:27:32.000000 viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.196564 viaconstructor-0.6.5/viaconstructor/ext/meshcut/
--rw-r--r--   0 root         (0) root         (0)    12866 2022-08-22 19:00:32.000000 viaconstructor-0.6.5/viaconstructor/ext/meshcut/meshcut.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.198563 viaconstructor-0.6.5/viaconstructor/ext/stl/
--rw-r--r--   0 root         (0) root         (0)      321 2022-08-22 19:01:54.000000 viaconstructor-0.6.5/viaconstructor/ext/stl/__about__.py
--rw-r--r--   0 root         (0) root         (0)      375 2022-08-22 19:01:54.000000 viaconstructor-0.6.5/viaconstructor/ext/stl/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22397 2022-08-22 19:01:54.000000 viaconstructor-0.6.5/viaconstructor/ext/stl/base.py
--rw-r--r--   0 root         (0) root         (0)     3277 2022-08-22 19:01:54.000000 viaconstructor-0.6.5/viaconstructor/ext/stl/main.py
--rw-r--r--   0 root         (0) root         (0)       55 2022-08-22 19:01:54.000000 viaconstructor-0.6.5/viaconstructor/ext/stl/mesh.py
--rw-r--r--   0 root         (0) root         (0)    15642 2022-08-22 19:01:54.000000 viaconstructor-0.6.5/viaconstructor/ext/stl/stl.py
--rw-r--r--   0 root         (0) root         (0)      541 2022-08-22 19:01:54.000000 viaconstructor-0.6.5/viaconstructor/ext/stl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.203564 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/
--rw-r--r--   0 root         (0) root         (0)     1097 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14309 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/bezier.py
--rw-r--r--   0 root         (0) root         (0)    18496 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/document.py
--rw-r--r--   0 root         (0) root         (0)     2026 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/misctools.py
--rw-r--r--   0 root         (0) root         (0)     3939 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/parser.py
--rw-r--r--   0 root         (0) root         (0)   133535 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/path.py
--rw-r--r--   0 root         (0) root         (0)    18991 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/paths2svg.py
--rw-r--r--   0 root         (0) root         (0)     2473 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/polytools.py
--rw-r--r--   0 root         (0) root         (0)     7642 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/smoothing.py
--rw-r--r--   0 root         (0) root         (0)     7089 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/svg_io_sax.py
--rw-r--r--   0 root         (0) root         (0)    11331 2022-08-22 18:57:05.000000 viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/svg_to_paths.py
--rwxr-xr-x   0 root         (0) root         (0)    53077 2023-04-11 15:48:53.000000 viaconstructor-0.6.5/viaconstructor/gldraw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.211563 viaconstructor-0.6.5/viaconstructor/icons/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-03-30 20:02:43.000000 viaconstructor-0.6.5/viaconstructor/icons/camotics.png
--rw-r--r--   0 root         (0) root         (0)     2046 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/delete.png
--rwxr-xr-x   0 root         (0) root         (0)     2633 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/exit.png
--rw-r--r--   0 root         (0) root         (0)     1606 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/flip-x.png
--rw-r--r--   0 root         (0) root         (0)     1348 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/flip-y.png
--rw-r--r--   0 root         (0) root         (0)     2413 2023-04-04 16:17:31.000000 viaconstructor-0.6.5/viaconstructor/icons/fonts.png
--rw-r--r--   0 root         (0) root         (0)     3221 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/icons/gears.png
--rw-r--r--   0 root         (0) root         (0)    20293 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/load-setup-gcode.png
--rw-r--r--   0 root         (0) root         (0)    16209 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/load-setup.png
--rw-r--r--   0 root         (0) root         (0)     2237 2022-09-23 15:31:33.000000 viaconstructor-0.6.5/viaconstructor/icons/load-tooltable.png
--rw-r--r--   0 root         (0) root         (0)      523 2023-02-25 16:12:56.000000 viaconstructor-0.6.5/viaconstructor/icons/nesting.png
--rw-r--r--   0 root         (0) root         (0)     2237 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/open.png
--rw-r--r--   0 root         (0) root         (0)    11071 2023-03-30 20:02:43.000000 viaconstructor-0.6.5/viaconstructor/icons/openscad.png
--rw-r--r--   0 root         (0) root         (0)      912 2022-09-22 16:28:41.000000 viaconstructor-0.6.5/viaconstructor/icons/pause.png
--rw-r--r--   0 root         (0) root         (0)     1473 2022-09-20 19:38:29.000000 viaconstructor-0.6.5/viaconstructor/icons/play.png
--rw-r--r--   0 root         (0) root         (0)     2120 2023-03-27 15:46:36.000000 viaconstructor-0.6.5/viaconstructor/icons/redraw.png
--rw-r--r--   0 root         (0) root         (0)     1843 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/repair.png
--rw-r--r--   0 root         (0) root         (0)     2967 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/rotate.png
--rwxr-xr-x   0 root         (0) root         (0)    12941 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/save-gcode.png
--rw-r--r--   0 root         (0) root         (0)    16787 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/save-setup-as.png
--rwxr-xr-x   0 root         (0) root         (0)     3096 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/save-setup.png
--rw-r--r--   0 root         (0) root         (0)     3484 2022-09-23 15:31:33.000000 viaconstructor-0.6.5/viaconstructor/icons/save-tooltable.png
--rw-r--r--   0 root         (0) root         (0)     3196 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/save.png
--rw-r--r--   0 root         (0) root         (0)     1254 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/scale.png
--rw-r--r--   0 root         (0) root         (0)      291 2022-09-21 16:00:41.000000 viaconstructor-0.6.5/viaconstructor/icons/select.png
--rw-r--r--   0 root         (0) root         (0)     1759 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/start.png
--rw-r--r--   0 root         (0) root         (0)      729 2022-09-22 16:28:41.000000 viaconstructor-0.6.5/viaconstructor/icons/stop.png
--rw-r--r--   0 root         (0) root         (0)     1500 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/tab-selector.png
--rw-r--r--   0 root         (0) root         (0)     2496 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/view-2d.png
--rw-r--r--   0 root         (0) root         (0)     4342 2022-08-24 16:12:33.000000 viaconstructor-0.6.5/viaconstructor/icons/view-reset.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.214563 viaconstructor-0.6.5/viaconstructor/input_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6762 2023-04-12 16:19:12.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/brdread.py
--rwxr-xr-x   0 root         (0) root         (0)    26370 2023-04-14 11:57:42.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/dxfread.py
--rw-r--r--   0 root         (0) root         (0)     6793 2023-03-23 17:27:32.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/hpglread.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-03-26 08:12:36.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/imgread.py
--rw-r--r--   0 root         (0) root         (0)     7853 2023-04-07 10:50:08.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/stlread.py
--rwxr-xr-x   0 root         (0) root         (0)    10642 2023-03-26 08:12:36.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/svgread.py
--rw-r--r--   0 root         (0) root         (0)     9352 2024-01-09 19:28:37.000000 viaconstructor-0.6.5/viaconstructor/input_plugins/ttfread.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-03-23 17:27:32.000000 viaconstructor-0.6.5/viaconstructor/input_plugins_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.099564 viaconstructor-0.6.5/viaconstructor/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.099564 viaconstructor-0.6.5/viaconstructor/locales/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.215563 viaconstructor-0.6.5/viaconstructor/locales/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5083 2023-04-10 16:36:40.000000 viaconstructor-0.6.5/viaconstructor/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 root         (0) root         (0)     8633 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/locales/de/LC_MESSAGES/base.po
--rwxr-xr-x   0 root         (0) root         (0)    44035 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/machine_cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.216563 viaconstructor-0.6.5/viaconstructor/output_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.5/viaconstructor/output_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10499 2023-04-08 21:07:42.000000 viaconstructor-0.6.5/viaconstructor/output_plugins/gcode_grbl.py
--rw-r--r--   0 root         (0) root         (0)    10647 2023-04-08 21:07:27.000000 viaconstructor-0.6.5/viaconstructor/output_plugins/gcode_linuxcnc.py
--rw-r--r--   0 root         (0) root         (0)     7450 2023-04-08 21:06:43.000000 viaconstructor-0.6.5/viaconstructor/output_plugins/hpgl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.217563 viaconstructor-0.6.5/viaconstructor/preview_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.5/viaconstructor/preview_plugins/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10939 2023-04-11 15:48:53.000000 viaconstructor-0.6.5/viaconstructor/preview_plugins/gcode.py
--rw-r--r--   0 root         (0) root         (0)     9321 2023-04-02 20:48:58.000000 viaconstructor-0.6.5/viaconstructor/preview_plugins/hpgl.py
--rwxr-xr-x   0 root         (0) root         (0)    22521 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/setupdefaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.217563 viaconstructor-0.6.5/viaconstructor/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9012 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/tools/font.py
--rw-r--r--   0 root         (0) root         (0)     8771 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/tools/gear.py
--rw-r--r--   0 root         (0) root         (0)     2560 2023-02-25 16:12:56.000000 viaconstructor-0.6.5/viaconstructor/vc_types.py
--rwxr-xr-x   0 root         (0) root         (0)   126674 2024-02-01 14:48:19.000000 viaconstructor-0.6.5/viaconstructor/viaconstructor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 14:48:36.188563 viaconstructor-0.6.5/viaconstructor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3885 2024-02-01 14:48:35.000000 viaconstructor-0.6.5/viaconstructor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3690 2024-02-01 14:48:36.000000 viaconstructor-0.6.5/viaconstructor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 14:48:35.000000 viaconstructor-0.6.5/viaconstructor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2024-02-01 14:48:35.000000 viaconstructor-0.6.5/viaconstructor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-02-01 14:48:35.000000 viaconstructor-0.6.5/viaconstructor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/
+-rwxr-xr-x   0 root         (0) root         (0)    35147 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      194 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3624 2023-04-08 23:55:39.000000 viaconstructor-0.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.677492 viaconstructor-0.6.6/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       36 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/bin/dxfpreview
+-rwxr-xr-x   0 root         (0) root         (0)       38 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/bin/gcodepreview
+-rwxr-xr-x   0 root         (0) root         (0)       42 2022-08-17 21:04:13.000000 viaconstructor-0.6.6/bin/viaconstructor
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.677492 viaconstructor-0.6.6/dxfpreview/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/dxfpreview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/dxfpreview/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4131 2022-08-22 19:23:27.000000 viaconstructor-0.6.6/dxfpreview/dxfpreview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.678492 viaconstructor-0.6.6/gcodepreview/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/gcodepreview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       96 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/gcodepreview/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3630 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/gcodepreview/gcodepreview.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1232 2024-04-01 19:41:02.000000 viaconstructor-0.6.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.680492 viaconstructor-0.6.6/viaconstructor/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/viaconstructor/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.6/viaconstructor/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)    50759 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/calc.py
+-rwxr-xr-x   0 root         (0) root         (0)    24883 2023-04-02 20:48:58.000000 viaconstructor-0.6.6/viaconstructor/draw2d.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-03-26 08:12:36.000000 viaconstructor-0.6.6/viaconstructor/dxfcolors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.675492 viaconstructor-0.6.6/viaconstructor/ext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.681492 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/
+-rw-r--r--   0 root         (0) root         (0)    91220 2022-08-22 17:54:34.000000 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/HersheyFonts.py
+-rw-r--r--   0 root         (0) root         (0)       63 2022-08-22 17:54:34.000000 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      101 2022-08-22 17:54:34.000000 viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.681492 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/
+-rw-r--r--   0 root         (0) root         (0)       39 2022-08-22 18:47:24.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8813 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/cavaliercontours.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.683492 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/
+-rwxr-xr-x   0 root         (0) root         (0)   872112 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
+-rwxr-xr-x   0 root         (0) root         (0)  1383488 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.684491 viaconstructor-0.6.6/viaconstructor/ext/meshcut/
+-rw-r--r--   0 root         (0) root         (0)    12866 2022-08-22 19:00:32.000000 viaconstructor-0.6.6/viaconstructor/ext/meshcut/meshcut.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.685492 viaconstructor-0.6.6/viaconstructor/ext/stl/
+-rw-r--r--   0 root         (0) root         (0)      321 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/__about__.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22397 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/base.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/main.py
+-rw-r--r--   0 root         (0) root         (0)       55 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/stl.py
+-rw-r--r--   0 root         (0) root         (0)      541 2022-08-22 19:01:54.000000 viaconstructor-0.6.6/viaconstructor/ext/stl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.687492 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/
+-rw-r--r--   0 root         (0) root         (0)     1097 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14309 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/bezier.py
+-rw-r--r--   0 root         (0) root         (0)    18496 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/document.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/misctools.py
+-rw-r--r--   0 root         (0) root         (0)     3939 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/parser.py
+-rw-r--r--   0 root         (0) root         (0)   133535 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/path.py
+-rw-r--r--   0 root         (0) root         (0)    18991 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/paths2svg.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/polytools.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/smoothing.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_io_sax.py
+-rw-r--r--   0 root         (0) root         (0)    11331 2022-08-22 18:57:05.000000 viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_to_paths.py
+-rwxr-xr-x   0 root         (0) root         (0)    53077 2023-04-11 15:48:53.000000 viaconstructor-0.6.6/viaconstructor/gldraw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.691491 viaconstructor-0.6.6/viaconstructor/icons/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-03-30 20:02:43.000000 viaconstructor-0.6.6/viaconstructor/icons/camotics.png
+-rw-r--r--   0 root         (0) root         (0)     2046 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/delete.png
+-rwxr-xr-x   0 root         (0) root         (0)     2633 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/exit.png
+-rw-r--r--   0 root         (0) root         (0)     1606 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/flip-x.png
+-rw-r--r--   0 root         (0) root         (0)     1348 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/flip-y.png
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-04-04 16:17:31.000000 viaconstructor-0.6.6/viaconstructor/icons/fonts.png
+-rw-r--r--   0 root         (0) root         (0)     3221 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/icons/gears.png
+-rw-r--r--   0 root         (0) root         (0)    20293 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/load-setup-gcode.png
+-rw-r--r--   0 root         (0) root         (0)    16209 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/load-setup.png
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-09-23 15:31:33.000000 viaconstructor-0.6.6/viaconstructor/icons/load-tooltable.png
+-rw-r--r--   0 root         (0) root         (0)      523 2023-02-25 16:12:56.000000 viaconstructor-0.6.6/viaconstructor/icons/nesting.png
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/open.png
+-rw-r--r--   0 root         (0) root         (0)    11071 2023-03-30 20:02:43.000000 viaconstructor-0.6.6/viaconstructor/icons/openscad.png
+-rw-r--r--   0 root         (0) root         (0)      912 2022-09-22 16:28:41.000000 viaconstructor-0.6.6/viaconstructor/icons/pause.png
+-rw-r--r--   0 root         (0) root         (0)     1473 2022-09-20 19:38:29.000000 viaconstructor-0.6.6/viaconstructor/icons/play.png
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-03-27 15:46:36.000000 viaconstructor-0.6.6/viaconstructor/icons/redraw.png
+-rw-r--r--   0 root         (0) root         (0)     1843 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/repair.png
+-rw-r--r--   0 root         (0) root         (0)     2967 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/rotate.png
+-rwxr-xr-x   0 root         (0) root         (0)    12941 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-gcode.png
+-rw-r--r--   0 root         (0) root         (0)    16787 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-setup-as.png
+-rwxr-xr-x   0 root         (0) root         (0)     3096 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-setup.png
+-rw-r--r--   0 root         (0) root         (0)     3484 2022-09-23 15:31:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save-tooltable.png
+-rw-r--r--   0 root         (0) root         (0)     3196 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/save.png
+-rw-r--r--   0 root         (0) root         (0)     1254 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/scale.png
+-rw-r--r--   0 root         (0) root         (0)      291 2022-09-21 16:00:41.000000 viaconstructor-0.6.6/viaconstructor/icons/select.png
+-rw-r--r--   0 root         (0) root         (0)     1759 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/start.png
+-rw-r--r--   0 root         (0) root         (0)      729 2022-09-22 16:28:41.000000 viaconstructor-0.6.6/viaconstructor/icons/stop.png
+-rw-r--r--   0 root         (0) root         (0)     1500 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/tab-selector.png
+-rw-r--r--   0 root         (0) root         (0)     2496 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/view-2d.png
+-rw-r--r--   0 root         (0) root         (0)     4342 2022-08-24 16:12:33.000000 viaconstructor-0.6.6/viaconstructor/icons/view-reset.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.692492 viaconstructor-0.6.6/viaconstructor/input_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6762 2023-04-12 16:19:12.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/brdread.py
+-rwxr-xr-x   0 root         (0) root         (0)    26370 2023-04-14 11:57:42.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/dxfread.py
+-rw-r--r--   0 root         (0) root         (0)     6793 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/hpglread.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-03-26 08:12:36.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/imgread.py
+-rw-r--r--   0 root         (0) root         (0)     7853 2023-04-07 10:50:08.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/stlread.py
+-rwxr-xr-x   0 root         (0) root         (0)    10642 2023-03-26 08:12:36.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/svgread.py
+-rw-r--r--   0 root         (0) root         (0)     9352 2024-01-09 19:28:37.000000 viaconstructor-0.6.6/viaconstructor/input_plugins/ttfread.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-03-23 17:27:32.000000 viaconstructor-0.6.6/viaconstructor/input_plugins_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.676492 viaconstructor-0.6.6/viaconstructor/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.676492 viaconstructor-0.6.6/viaconstructor/locales/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.693492 viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-04-10 16:36:40.000000 viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 root         (0) root         (0)     8633 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.po
+-rwxr-xr-x   0 root         (0) root         (0)    44035 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/machine_cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.693492 viaconstructor-0.6.6/viaconstructor/output_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10499 2023-04-08 21:07:42.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_grbl.py
+-rw-r--r--   0 root         (0) root         (0)    10647 2023-04-08 21:07:27.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_linuxcnc.py
+-rw-r--r--   0 root         (0) root         (0)     7450 2023-04-08 21:06:43.000000 viaconstructor-0.6.6/viaconstructor/output_plugins/hpgl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/viaconstructor/preview_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.6/viaconstructor/preview_plugins/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10939 2023-04-11 15:48:53.000000 viaconstructor-0.6.6/viaconstructor/preview_plugins/gcode.py
+-rw-r--r--   0 root         (0) root         (0)     9321 2023-04-02 20:48:58.000000 viaconstructor-0.6.6/viaconstructor/preview_plugins/hpgl.py
+-rwxr-xr-x   0 root         (0) root         (0)    22521 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/setupdefaults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.694491 viaconstructor-0.6.6/viaconstructor/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9012 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/tools/font.py
+-rw-r--r--   0 root         (0) root         (0)     8791 2024-04-01 19:39:59.000000 viaconstructor-0.6.6/viaconstructor/tools/gear.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-02-25 16:12:56.000000 viaconstructor-0.6.6/viaconstructor/vc_types.py
+-rwxr-xr-x   0 root         (0) root         (0)   126674 2024-02-01 14:48:19.000000 viaconstructor-0.6.6/viaconstructor/viaconstructor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 19:41:55.681492 viaconstructor-0.6.6/viaconstructor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-01 19:41:55.000000 viaconstructor-0.6.6/viaconstructor.egg-info/top_level.txt
```

### Comparing `viaconstructor-0.6.5/LICENSE` & `viaconstructor-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/PKG-INFO` & `viaconstructor-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.5
+Version: 0.6.6
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.5/README.md` & `viaconstructor-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/dxfpreview/dxfpreview.py` & `viaconstructor-0.6.6/dxfpreview/dxfpreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/gcodepreview/gcodepreview.py` & `viaconstructor-0.6.6/gcodepreview/gcodepreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/setup.py` & `viaconstructor-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 from setuptools import setup
 
 
 setup(
     name='viaconstructor',
-    version='0.6.5',
+    version='0.6.6',
     author='Oliver Dippel',
     author_email='o.dippel@gmx.de',
     packages=['viaconstructor', 'viaconstructor.ext.cavaliercontours', 'viaconstructor.ext.HersheyFonts', 'viaconstructor.ext.meshcut', 'viaconstructor.ext.stl', 'viaconstructor.ext.svgpathtools', 'viaconstructor.input_plugins', 'viaconstructor.output_plugins', 'viaconstructor.preview_plugins', 'viaconstructor.tools', 'gcodepreview', 'dxfpreview'],
     package_data={'viaconstructor.ext.cavaliercontours': ['lib/libCavalierContours.x86_64-linux.so'], 'viaconstructor/ext/nest2D': ['nest2D.cpython-39-x86_64-linux-gnu.so']},
     scripts=['bin/viaconstructor','bin/gcodepreview','bin/dxfpreview'],
     url='https://github.com/multigcs/viaconstructor',
     license='LICENSE',
```

### Comparing `viaconstructor-0.6.5/viaconstructor/calc.py` & `viaconstructor-0.6.6/viaconstructor/calc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/draw2d.py` & `viaconstructor-0.6.6/viaconstructor/draw2d.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/dxfcolors.py` & `viaconstructor-0.6.6/viaconstructor/dxfcolors.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/HersheyFonts/HersheyFonts.py` & `viaconstructor-0.6.6/viaconstructor/ext/HersheyFonts/HersheyFonts.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/cavaliercontours.py` & `viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/cavaliercontours.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so` & `viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so` & `viaconstructor-0.6.6/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/meshcut/meshcut.py` & `viaconstructor-0.6.6/viaconstructor/ext/meshcut/meshcut.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/stl/base.py` & `viaconstructor-0.6.6/viaconstructor/ext/stl/base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/stl/main.py` & `viaconstructor-0.6.6/viaconstructor/ext/stl/main.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/stl/stl.py` & `viaconstructor-0.6.6/viaconstructor/ext/stl/stl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/stl/utils.py` & `viaconstructor-0.6.6/viaconstructor/ext/stl/utils.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/__init__.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/bezier.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/bezier.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/document.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/document.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/misctools.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/misctools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/parser.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/parser.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/path.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/path.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/paths2svg.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/paths2svg.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/polytools.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/polytools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/smoothing.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/smoothing.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/svg_io_sax.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_io_sax.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/ext/svgpathtools/svg_to_paths.py` & `viaconstructor-0.6.6/viaconstructor/ext/svgpathtools/svg_to_paths.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/gldraw.py` & `viaconstructor-0.6.6/viaconstructor/gldraw.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/camotics.png` & `viaconstructor-0.6.6/viaconstructor/icons/camotics.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/delete.png` & `viaconstructor-0.6.6/viaconstructor/icons/delete.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/exit.png` & `viaconstructor-0.6.6/viaconstructor/icons/exit.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/flip-x.png` & `viaconstructor-0.6.6/viaconstructor/icons/flip-x.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/flip-y.png` & `viaconstructor-0.6.6/viaconstructor/icons/flip-y.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/fonts.png` & `viaconstructor-0.6.6/viaconstructor/icons/fonts.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/gears.png` & `viaconstructor-0.6.6/viaconstructor/icons/gears.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/load-setup-gcode.png` & `viaconstructor-0.6.6/viaconstructor/icons/load-setup-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/load-setup.png` & `viaconstructor-0.6.6/viaconstructor/icons/load-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/load-tooltable.png` & `viaconstructor-0.6.6/viaconstructor/icons/load-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/nesting.png` & `viaconstructor-0.6.6/viaconstructor/icons/nesting.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/open.png` & `viaconstructor-0.6.6/viaconstructor/icons/open.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/openscad.png` & `viaconstructor-0.6.6/viaconstructor/icons/openscad.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/pause.png` & `viaconstructor-0.6.6/viaconstructor/icons/pause.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/play.png` & `viaconstructor-0.6.6/viaconstructor/icons/play.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/redraw.png` & `viaconstructor-0.6.6/viaconstructor/icons/redraw.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/repair.png` & `viaconstructor-0.6.6/viaconstructor/icons/repair.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/rotate.png` & `viaconstructor-0.6.6/viaconstructor/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/save-gcode.png` & `viaconstructor-0.6.6/viaconstructor/icons/save-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/save-setup-as.png` & `viaconstructor-0.6.6/viaconstructor/icons/save-setup-as.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/save-setup.png` & `viaconstructor-0.6.6/viaconstructor/icons/save-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/save-tooltable.png` & `viaconstructor-0.6.6/viaconstructor/icons/save-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/save.png` & `viaconstructor-0.6.6/viaconstructor/icons/save.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/scale.png` & `viaconstructor-0.6.6/viaconstructor/icons/scale.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/start.png` & `viaconstructor-0.6.6/viaconstructor/icons/start.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/stop.png` & `viaconstructor-0.6.6/viaconstructor/icons/stop.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/tab-selector.png` & `viaconstructor-0.6.6/viaconstructor/icons/tab-selector.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/view-2d.png` & `viaconstructor-0.6.6/viaconstructor/icons/view-2d.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/icons/view-reset.png` & `viaconstructor-0.6.6/viaconstructor/icons/view-reset.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins/brdread.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins/brdread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins/dxfread.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins/dxfread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins/hpglread.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins/hpglread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins/imgread.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins/imgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins/stlread.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins/stlread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins/svgread.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins/svgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins/ttfread.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins/ttfread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/input_plugins_base.py` & `viaconstructor-0.6.6/viaconstructor/input_plugins_base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/locales/de/LC_MESSAGES/base.mo` & `viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/locales/de/LC_MESSAGES/base.po` & `viaconstructor-0.6.6/viaconstructor/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/machine_cmd.py` & `viaconstructor-0.6.6/viaconstructor/machine_cmd.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/output_plugins/gcode_grbl.py` & `viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_grbl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/output_plugins/gcode_linuxcnc.py` & `viaconstructor-0.6.6/viaconstructor/output_plugins/gcode_linuxcnc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/output_plugins/hpgl.py` & `viaconstructor-0.6.6/viaconstructor/output_plugins/hpgl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/preview_plugins/gcode.py` & `viaconstructor-0.6.6/viaconstructor/preview_plugins/gcode.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/preview_plugins/hpgl.py` & `viaconstructor-0.6.6/viaconstructor/preview_plugins/hpgl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/setupdefaults.py` & `viaconstructor-0.6.6/viaconstructor/setupdefaults.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/tools/font.py` & `viaconstructor-0.6.6/viaconstructor/tools/font.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/tools/gear.py` & `viaconstructor-0.6.6/viaconstructor/tools/gear.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,15 @@
                     point[0] * scale + off_x,
                     point[1] * scale + off_y,
                 )
             )
             last = point
 
         square = QRect(
-            off_x - hole / 2 * scale,
-            off_y - hole / 2 * scale,
-            hole * scale,
-            hole * scale,
+            int(off_x - hole / 2 * scale),
+            int(off_y - hole / 2 * scale),
+            int(hole * scale),
+            int(hole * scale),
         )
         self.painter.drawEllipse(square)
 
         self.painter.end()
```

### Comparing `viaconstructor-0.6.5/viaconstructor/vc_types.py` & `viaconstructor-0.6.6/viaconstructor/vc_types.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor/viaconstructor.py` & `viaconstructor-0.6.6/viaconstructor/viaconstructor.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.5/viaconstructor.egg-info/PKG-INFO` & `viaconstructor-0.6.6/viaconstructor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.5
+Version: 0.6.6
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.5/viaconstructor.egg-info/SOURCES.txt` & `viaconstructor-0.6.6/viaconstructor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

