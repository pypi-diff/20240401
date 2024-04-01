# Comparing `tmp/omfit_classes-3.2024.13.2.tar.gz` & `tmp/omfit_classes-3.2024.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omfit_classes-3.2024.13.2.tar", last modified: Mon Apr  1 18:31:26 2024, max compression
+gzip compressed data, was "dist/omfit_classes-3.2024.9.2.tar", last modified: Fri Mar  8 20:50:57 2024, max compression
```

## Comparing `omfit_classes-3.2024.13.2.tar` & `omfit_classes-3.2024.9.2.tar`

### file list

```diff
@@ -1,723 +1,723 @@
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/
--rw-r--r--   0 fusionbot   (505) staff       (20)     1067 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/LICENSE.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)     1179 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/PKG-INFO
--rw-r--r--   0 fusionbot   (505) staff       (20)      942 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/README.rst
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/__init__.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/classes/
--rw-r--r--   0 fusionbot   (505) staff       (20)      290 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/classes/__init__.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    27149 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/externalImports.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/__init__.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/
--rw-r--r--   0 fusionbot   (505) staff       (20)   385815 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/LOM.png
--rw-r--r--   0 fusionbot   (505) staff       (20)     6335 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_font.bf
--rw-r--r--   0 fusionbot   (505) staff       (20)     3044 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_font.ttf
--rw-r--r--   0 fusionbot   (505) staff       (20)     2087 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)    56012 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo.pdf
--rw-r--r--   0 fusionbot   (505) staff       (20)     3187 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_color.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)    59634 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_color.pdf
--rw-r--r--   0 fusionbot   (505) staff       (20)     6504 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_olympics.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)   179267 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_olympics.pdf
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/__init__.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/autoX.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/autoY.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/bookmark.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     8760 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/colors.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/copy.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/crosshair.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1512 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/error.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      277 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/events.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/
--rw-r--r--   0 fusionbot   (505) staff       (20)    25832 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Humor-Sans.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    52836 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Bold.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    53512 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-BoldItalic.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    48220 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-ExtraLight.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    49204 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-ExtraLightItalic.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    49760 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Italic.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    48856 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Light.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    49552 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-LightItalic.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    49488 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Semi-BoldItalic.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    49272 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-SemiBold.ttf
--rwxr-xr-x   0 fusionbot   (505) staff       (20)    49008 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli.ttf
--rw-r--r--   0 fusionbot   (505) staff       (20)     2334 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/fonts.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/help.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     2507 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/info.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/legend.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/linked.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/mail.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)      631 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/matplotlib_backends.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/paste.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/pdf.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     5370 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/pin.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     2472 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/question.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/select.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/settings.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/storage.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/text.ppm
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/
--rw-r--r--   0 fusionbot   (505) staff       (20)      600 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/CreateImageLib.def
--rw-r--r--   0 fusionbot   (505) staff       (20)    41722 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/ImageLib.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/LICENSE
--rw-r--r--   0 fusionbot   (505) staff       (20)     6971 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/aquativo.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)   112011 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/images.tgz
--rw-r--r--   0 fusionbot   (505) staff       (20)       95 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/black/
--rw-r--r--   0 fusionbot   (505) staff       (20)     2123 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/black/LICENSE
--rw-r--r--   0 fusionbot   (505) staff       (20)     4066 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/black/black.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)      209 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/black/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/
--rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/LICENSE
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/
--rw-r--r--   0 fusionbot   (505) staff       (20)      315 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowdown-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      312 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowdown-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      313 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowdown.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      329 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowleft-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      327 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowleft-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      323 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowleft.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowright-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      327 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowright-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      324 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowright.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      309 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowup-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      313 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowup-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      314 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/arrowup.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      696 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/button-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      770 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/button-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      769 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/button-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      254 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/check-hc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/check-hu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      249 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/check-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      229 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/check-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1098 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/radio-hc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      626 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/radio-hu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      389 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/radio-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      401 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/radio-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      343 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/sb-thumb-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      316 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/sb-thumb.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      333 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/sb-vthumb-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      308 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/sb-vthumb.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      182 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/slider-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      182 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/slider.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      183 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/vslider-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      283 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/vslider.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     4714 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)      188 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/blue/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/
--rw-r--r--   0 fusionbot   (505) staff       (20)     2226 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/LICENSE
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/
--rw-r--r--   0 fusionbot   (505) staff       (20)      245 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      230 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      246 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      248 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      248 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      252 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      251 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      250 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      235 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      252 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      251 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      244 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      228 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      248 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      247 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       63 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/blank.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      661 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      590 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      656 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      519 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      394 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-pa.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      331 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-ac.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-au.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-dc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-du.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      331 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      332 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-pc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/check-pu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      100 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      527 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-ra.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      512 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-rd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      550 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-rf.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      533 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-rn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      402 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-rp.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      441 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      432 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      451 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      450 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      281 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/progress-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      304 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/progress-v.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      356 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-ac.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-au.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      362 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-dc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-du.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      359 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      359 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-pc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      225 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/radio-pu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      276 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-ha.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      263 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-hd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      278 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-hn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      278 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-hp.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      266 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-va.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      262 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-vd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      271 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-vn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      271 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-vp.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      474 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scale-ha.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      336 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scale-hd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      477 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scale-hn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      526 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scale-va.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      342 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scale-vd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      511 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scale-vn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       87 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scaletrough-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      111 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scaletrough-v.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sep-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sep-v.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       77 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/sizegrip.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      536 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tab-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      549 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tab-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      554 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      499 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      557 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      527 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      333 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-pa.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      509 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tree-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      519 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tree-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      528 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tree-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      420 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tree-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)    11637 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)      406 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/
--rw-r--r--   0 fusionbot   (505) staff       (20)     2226 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/LICENSE
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/
--rw-r--r--   0 fusionbot   (505) staff       (20)       70 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/arrow-optionmenu-disabled.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       79 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/arrow-optionmenu-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       79 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/arrow-optionmenu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1954 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-active-disabled.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1953 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-active-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      872 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-active.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1267 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-default.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     2001 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      138 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/check1.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      145 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/check2.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/combo-active.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/entry-active.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/entry-inactive.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/grip-horiz-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/grip-horiz.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       59 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/grip-vert-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       59 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/grip-vert.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      700 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/list-header-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      706 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/list-header.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/option1.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      363 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/option2.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      995 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/progressbar-horiz.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      966 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/progressbar-vert.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/scale-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      320 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/scale.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      651 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-horiz-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      673 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-horiz.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      666 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-vert-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      722 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-vert.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      542 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-down-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      555 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-down.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      555 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-left-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      556 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-left.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      555 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-right-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      560 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-right.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      542 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-up-prelight.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      549 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-up.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      544 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/tab-top-active.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      583 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/tab-top.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       97 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-horiz.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      664 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-progressbar-horiz.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      677 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-progressbar-vert.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      803 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-horiz.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      871 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-vert.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      133 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-vert.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     9054 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)      154 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/
--rw-r--r--   0 fusionbot   (505) staff       (20)      203 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/arrow-down-insens.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      200 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/arrow-down-prelight.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      202 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/arrow-down.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      128 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/arrow-up-small-insens.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      127 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/arrow-up-small-prelight.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      132 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/arrow-up-small.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      201 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/arrow-up.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      370 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/button-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      156 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/button-empty.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      365 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/button-hover.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      210 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/button-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      347 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/button.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      321 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/checkbox-checked-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      334 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/checkbox-checked.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      227 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/checkbox-unchecked-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      216 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/checkbox-unchecked.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      197 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/combo-entry-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      285 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/combo-entry-button-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      289 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/combo-entry-button-hover.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      203 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/combo-entry-button-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      274 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/combo-entry-button.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/combo-entry-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      236 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/combo-entry.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      221 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/down-background-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      183 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/down-background-disable.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/down-background-hover.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      218 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/down-background.png
--rw-r--r--   0 fusionbot   (505) staff       (20)       71 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/empty.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/entry-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      265 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/entry-border-bg.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      258 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/entry-border-disabled.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      202 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/focus.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      157 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/frame.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      264 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/labelframe.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      307 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/minus.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      264 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/notebook.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      148 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/null.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      294 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/plus.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      140 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/progressbar-horiz.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      141 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/progressbar-vert.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      588 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/radio-checked-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      667 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/radio-checked.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      476 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/radio-unchecked-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      567 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/radio-unchecked.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      181 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-horiz-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      183 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-horiz-insens.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      185 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-horiz-prelight.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      185 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-horiz.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      386 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-insensitive.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      385 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-prelight.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      177 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-vert-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      203 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-vert-insens.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      184 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-vert-prelight.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      184 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider-vert.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      338 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/slider.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      213 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/tab-top-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      227 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/tab-top-hover.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/tab-top.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      129 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/treeview.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      177 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-horizontal-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      177 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-horizontal.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      429 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-progressbar-horiz.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      405 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-progressbar-vert.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      429 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-progressbar.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      405 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-progressbar_v.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      143 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-scrollbar-horiz.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      142 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-scrollbar-vert.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      277 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-vertical-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      176 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/trough-vertical.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/up-background-active.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      195 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/up-background-disable.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/up-background-hover.png
--rw-r--r--   0 fusionbot   (505) staff       (20)      224 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/up-background.png
--rw-r--r--   0 fusionbot   (505) staff       (20)    14336 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)      441 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/
--rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/LICENSE
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/
--rw-r--r--   0 fusionbot   (505) staff       (20)      273 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowdown-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      258 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowdown-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      292 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowleft-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      272 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowleft-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      274 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowright-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      258 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowright-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      286 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowup-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      271 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/arrowup-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1266 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      896 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      881 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      625 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      859 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-s.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1110 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/cbox-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1076 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/cbox-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1097 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/cbox-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      434 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/check-c.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      423 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/check-u.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hsb-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hsb-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      401 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hsb-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      395 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hsb-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      119 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hsb-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      592 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hslider-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      579 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hslider-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/indicator-c.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       64 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/indicator-o.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1116 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/mbut-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       61 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/mbut-arrow-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1057 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/mbut-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1095 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/mbut-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      712 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/progress-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      713 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/progress-v.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      695 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/radio-c.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      686 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/radio-u.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      409 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/spinbox-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       56 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/spindown-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      207 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/spindown-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       56 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/spinup-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/spinup-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      871 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tab-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      383 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tab-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      878 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tab-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      907 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tbar-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      238 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tbar-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      927 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tbar-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tree-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      688 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tree-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      373 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vsb-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      240 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vsb-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      405 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vsb-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      399 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vsb-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      124 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vsb-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      587 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vslider-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      581 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vslider-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)    13334 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik_alt/
--rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik_alt/hsb-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik_alt/hsb-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      373 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik_alt/vsb-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      240 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik_alt/vsb-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      314 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/pkgIndex.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)      650 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/
--rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/LICENSE
--rw-r--r--   0 fusionbot   (505) staff       (20)      219 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/
--rw-r--r--   0 fusionbot   (505) staff       (20)       49 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrow-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       49 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrow-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      218 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowdown-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      225 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowdown-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      353 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowleft-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      242 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowleft-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowright-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      242 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowright-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      219 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowup-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/arrowup-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       88 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/border.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1209 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/button-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1221 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/button-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      302 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/button-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      141 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/check-hc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      145 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/check-hu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      198 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/check-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      197 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/check-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      144 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/check-pc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      320 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      453 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      463 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-f.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-fa.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      446 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      728 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-r.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      721 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-ra.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      111 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/entry-f.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      106 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/entry-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      446 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/hprogress-b.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      124 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/hprogress-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      139 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/hsb-g.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      348 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/hsb-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       85 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/hsb-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      319 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/hslider-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       63 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/hslider-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       99 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/notebook-c.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      376 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/notebook-ta.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      378 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/notebook-tn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      156 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/notebook-ts.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      120 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/radio-hc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      154 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/radio-hu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      208 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/radio-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      151 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/radio-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      121 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/radio-pc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      201 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spinbox-f.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      160 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spinbox-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      130 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spinbut-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       60 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spinbut-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      144 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spindown-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      189 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spindown-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      202 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spindown-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      147 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spinup-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      192 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spinup-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      206 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/spinup-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      691 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/tbutton-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       58 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/tbutton-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      450 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/tbutton-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      357 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/tree-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      227 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/tree-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      427 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/vprogress-b.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      146 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/vsb-g.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      220 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/vsb-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       80 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/vsb-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      208 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/vslider-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/vslider-t.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     9617 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/
--rw-r--r--   0 fusionbot   (505) staff       (20)     2226 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/LICENSE.ORIG
--rw-r--r--   0 fusionbot   (505) staff       (20)      396 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/pkgIndex.tcl
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/
--rw-r--r--   0 fusionbot   (505) staff       (20)      357 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowdown-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      361 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowdown-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowdown-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowdown-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowleft-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      569 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowleft-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      355 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowleft-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      356 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowleft-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowright-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      364 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowright-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowright-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      355 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowright-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      355 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowup-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      363 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowup-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      356 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowup-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowup-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       63 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/blank.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1026 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      734 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      742 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      996 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1441 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-s.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1022 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-sa.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      645 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/check-dc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      337 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/check-du.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      630 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/check-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      389 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/check-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      247 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      442 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-ra.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      451 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-rd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      672 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-rf.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      452 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-rn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      679 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-rp.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      381 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/comboarrow-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      389 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/comboarrow-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      381 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/comboarrow-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      381 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/comboarrow-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      743 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/progress-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      733 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/progress-v.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      630 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/radio-dc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      364 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/radio-du.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)     1035 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/radio-nc.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      564 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/radio-nu.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      221 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-ha.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      333 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-hd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-hn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-hp.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-va.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      335 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-vd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-vn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sbthumb-vp.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      369 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scale-ha.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      365 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scale-hd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scale-hn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      367 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scale-va.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      364 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scale-vd.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      367 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scale-vn.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      209 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scaletrough-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/scaletrough-v.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sep-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sep-v.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)       78 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/sizegrip.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      454 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/tab-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      409 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/tab-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      453 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-a.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      689 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      672 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      691 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      683 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-pa.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/tree-d.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      257 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/tree-h.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      362 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/tree-n.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)      363 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/tree-p.gif
--rw-r--r--   0 fusionbot   (505) staff       (20)    12159 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance.tcl
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/trash.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/unlinked.ppm
--rw-r--r--   0 fusionbot   (505) staff       (20)     2267 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/graphics/warning.gif
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/extras/styles/
--rw-r--r--   0 fusionbot   (505) staff       (20)      342 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/styles/DIII-D.mplstyle
--rw-r--r--   0 fusionbot   (505) staff       (20)      770 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/styles/DIII-D_beamer.mplstyle
--rw-r--r--   0 fusionbot   (505) staff       (20)      769 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/styles/DIII-D_beamer_half.mplstyle
--rw-r--r--   0 fusionbot   (505) staff       (20)      770 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/styles/DIII-D_beamer_multifig.mplstyle
--rw-r--r--   0 fusionbot   (505) staff       (20)      859 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/extras/styles/DIII-D_paper_one_of_two_columns.mplstyle
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/framework_guis/
--rw-r--r--   0 fusionbot   (505) staff       (20)     3423 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/developerModeGUI.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    44586 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/efitviewer_gui.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6805 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/efitviewer_settings.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)    18806 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/efitviewer_support_gui.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3147 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/imasActorGUI.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3703 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/imasGUI.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2121 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/latexGUI.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    10662 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/machine_mappings.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3399 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/moduleSetupGUI.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2316 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/namelistGUI.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     9715 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/preferencesGUI.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6189 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/spruceUpFigures.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     7835 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/framework_guis/styleGUI.py
--rwxr-xr-x   0 fusionbot   (505) staff       (20)     4448 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/
--rw-r--r--   0 fusionbot   (505) staff       (20)   304834 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/OMFITx.py
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/__init__.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    76415 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/adaptors.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    42383 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/atomic_elements.json
--rw-r--r--   0 fusionbot   (505) staff       (20)     9475 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/brainfuse.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     9710 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/brainfusetf.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2368 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/exceptions_omfit.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   144808 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/fluxSurface.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    12090 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/gapy.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     9302 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/harvest_lib.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    64521 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/namelist.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     4953 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_accome.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3673 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_ascii.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     4580 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_asciitable.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2346 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_aurora.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   212488 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_base.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    10776 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_bibtex.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    24974 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_boundary.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     5916 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_bout.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    12867 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_brainfuse.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6416 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_cdb.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    33174 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_chease.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2867 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_chombo.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6732 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_clusters.json
--rw-r--r--   0 fusionbot   (505) staff       (20)    10357 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_clusters.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    25698 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_coils.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6311 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_cotsim.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     7018 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_csv.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   140223 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_ctrl_analysis.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    31373 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_data.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     5059 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_dir.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    11301 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_dmp.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6926 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_efit.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    97543 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_efitviewer.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    75191 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_efund.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    14430 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_elite.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   181065 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_elm.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1594 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_environment.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6068 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_eped.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   348799 2024-04-01 18:31:14.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_eqdsk.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1759 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_error.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2435 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_execution_diagram.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1273 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_fastran.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    16304 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_focus.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     4212 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_formatter.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    54185 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gacode.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1428 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gaprofiles.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   133370 2024-04-01 18:31:14.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gapy.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    18819 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gato.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    12142 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_genray.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1728 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gingred.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    46693 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_github.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     4243 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gks.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2592 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gnuplot.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    57394 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_google_sheet.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    51592 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gpec.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1616 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_gptools.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    17339 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_harvest.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     8303 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_hdf5.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    48570 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_helena.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1507 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_idl.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     5034 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_idlSav.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     5022 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_ini.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    13082 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_interface.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     5481 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_ionorb.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     5154 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_jscope.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1774 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_jsolver.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     7459 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_json.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2877 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_kepler.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    29701 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_latex.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    92530 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_mars.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2352 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_matlab.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     6709 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_matrix.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    85242 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_mds.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1724 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_mmm.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3425 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_namelist.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    21157 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_nc.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    33491 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_nimrod.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    56023 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_oedge.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    19310 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_omas.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    53177 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_d3d.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    11705 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_east.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    12148 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_kstar.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   157087 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_utils.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   115393 2024-04-01 18:31:14.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_onetwo.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    49418 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_osborne.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    51257 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_patch.py
--rw-r--r--   0 fusionbot   (505) staff       (20)      784 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_path.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3078 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_pdb.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   116962 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_profiles.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    85704 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_python.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    33627 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_rabbit.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    39649 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_rdb.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2366 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_reviewplus.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   114264 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_solps.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3423 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_spider.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    98670 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_testing.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   107516 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_tglf.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   115550 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_thomson.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     7856 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_timcon.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    21853 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_toksearch.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     7617 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_toq.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    71812 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_transp.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    48768 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_trip3d.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    13791 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_tsc.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2695 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_uda.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    11728 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_uedge.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    18800 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_ufile.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2146 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_weblink.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3451 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_xml.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2822 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/omfit_yaml.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/GUIS/
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/GUIS/__init__.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/INPUTS/
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/INPUTS/__init__.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/LIB/
--rw-r--r--   0 fusionbot   (505) staff       (20)       15 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/LIB/OMFITlib_startup.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     2627 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/OMFITsave.txt
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/OUTPUTS/
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/OUTPUTS/__init__.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/PLOTS/
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/PLOTS/__init__.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/SCRIPTS/
--rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/SCRIPTS/__init__.py
--rw-r--r--   0 fusionbot   (505) staff       (20)      478 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/SettingsNamelist.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)     1589 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/help.rst
--rw-r--r--   0 fusionbot   (505) staff       (20)    41260 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettings.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)     7677 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettingsNamelist.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)       92 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettingsNamelistOSX.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)      141 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettingsNamelistUNIX.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)       89 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettingsOSX.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)       90 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettingsUNIX.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)    57188 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/sortedDict.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     1032 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/startup_choice.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    12200 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/startup_classes.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    55483 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/startup_framework.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   734548 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/uedge_common_map.json
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes/unix_os/
--rw-r--r--   0 fusionbot   (505) staff       (20)      139 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/unix_os/__init__.py
--rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/unix_os/path.py
--rw-r--r--   0 fusionbot   (505) staff       (20)      761 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/unix_os/setup.py
--rw-r--r--   0 fusionbot   (505) staff       (20)        3 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/unix_os/version
--rw-r--r--   0 fusionbot   (505) staff       (20)   158596 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/utils_base.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   128683 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/utils_fit.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   147207 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/utils_fusion.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   236581 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/utils_math.py
--rw-r--r--   0 fusionbot   (505) staff       (20)   166642 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/utils_plot.py
--rw-r--r--   0 fusionbot   (505) staff       (20)       10 2024-04-01 18:31:14.000000 omfit_classes-3.2024.13.2/omfit_classes/version
--rw-r--r--   0 fusionbot   (505) staff       (20)     3549 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_classes/zdata.py
-drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/omfit_classes.egg-info/
--rw-r--r--   0 fusionbot   (505) staff       (20)     1179 2024-04-01 18:31:24.000000 omfit_classes-3.2024.13.2/omfit_classes.egg-info/PKG-INFO
--rw-r--r--   0 fusionbot   (505) staff       (20)    32245 2024-04-01 18:31:25.000000 omfit_classes-3.2024.13.2/omfit_classes.egg-info/SOURCES.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)        1 2024-04-01 18:31:24.000000 omfit_classes-3.2024.13.2/omfit_classes.egg-info/dependency_links.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)       14 2024-04-01 18:31:24.000000 omfit_classes-3.2024.13.2/omfit_classes.egg-info/top_level.txt
--rw-r--r--   0 fusionbot   (505) staff       (20)   370599 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_gui.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     3236 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_halt.py
--rw-r--r--   0 fusionbot   (505) staff       (20)     4949 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_parse_args.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    83252 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_plot.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    12707 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_setup.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    83673 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/omfit_tree.py
--rw-r--r--   0 fusionbot   (505) staff       (20)       38 2024-04-01 18:31:26.000000 omfit_classes-3.2024.13.2/setup.cfg
--rw-r--r--   0 fusionbot   (505) staff       (20)     1314 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/setup.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    26589 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/utils.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    62680 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/utils_tk.py
--rw-r--r--   0 fusionbot   (505) staff       (20)    32777 2024-04-01 04:39:43.000000 omfit_classes-3.2024.13.2/utils_widgets.py
--rw-r--r--   0 fusionbot   (505) staff       (20)       10 2024-04-01 18:31:14.000000 omfit_classes-3.2024.13.2/version
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1067 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/LICENSE.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1178 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/PKG-INFO
+-rw-r--r--   0 fusionbot   (505) staff       (20)      942 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/README.rst
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/__init__.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/classes/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      290 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/classes/__init__.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    27149 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/externalImports.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/__init__.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/
+-rw-r--r--   0 fusionbot   (505) staff       (20)   385815 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/LOM.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6335 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_font.bf
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3044 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_font.ttf
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2087 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)    56012 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo.pdf
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3187 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_color.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)    59634 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_color.pdf
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6504 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_olympics.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)   179267 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_olympics.pdf
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/__init__.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/autoX.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/autoY.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/bookmark.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     8760 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/colors.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/copy.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/crosshair.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1512 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/error.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      277 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/events.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/
+-rw-r--r--   0 fusionbot   (505) staff       (20)    25832 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Humor-Sans.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    52836 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Bold.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    53512 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-BoldItalic.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    48220 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-ExtraLight.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    49204 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-ExtraLightItalic.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    49760 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Italic.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    48856 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Light.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    49552 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-LightItalic.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    49488 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Semi-BoldItalic.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    49272 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-SemiBold.ttf
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)    49008 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli.ttf
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2334 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/fonts.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/help.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2507 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/info.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/legend.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/linked.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/mail.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)      631 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/matplotlib_backends.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/paste.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/pdf.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     5370 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/pin.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2472 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/question.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/select.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/settings.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/storage.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/text.ppm
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      600 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/CreateImageLib.def
+-rw-r--r--   0 fusionbot   (505) staff       (20)    41722 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/ImageLib.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/LICENSE
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6971 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/aquativo.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)   112011 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/images.tgz
+-rw-r--r--   0 fusionbot   (505) staff       (20)       95 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/black/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2123 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/black/LICENSE
+-rw-r--r--   0 fusionbot   (505) staff       (20)     4066 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/black/black.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)      209 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/black/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/LICENSE
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      315 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowdown-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      312 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowdown-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      313 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowdown.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      329 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowleft-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      327 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowleft-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      323 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowleft.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowright-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      327 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowright-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      324 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowright.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      309 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowup-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      313 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowup-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      314 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/arrowup.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      696 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/button-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      770 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/button-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      769 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/button-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      254 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/check-hc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/check-hu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      249 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/check-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      229 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/check-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1098 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/radio-hc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      626 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/radio-hu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      389 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/radio-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      401 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/radio-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      343 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/sb-thumb-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      316 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/sb-thumb.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      333 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/sb-vthumb-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      308 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/sb-vthumb.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      182 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/slider-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      182 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/slider.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      183 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/vslider-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      283 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/vslider.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     4714 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)      188 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/blue/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2226 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/LICENSE
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      245 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      230 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      246 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      248 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowdown-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      248 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      252 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      251 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowleft-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      250 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      235 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      252 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      251 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowright-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      244 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      228 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      248 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      247 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/arrowup-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       63 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/blank.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      661 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      590 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      656 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      519 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      394 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-pa.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      331 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-ac.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-au.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-dc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-du.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      331 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      332 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-pc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       96 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/check-pu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      100 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      527 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-ra.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      512 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-rd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      550 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-rf.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      533 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-rn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      402 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-rp.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      441 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      432 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      451 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      450 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/comboarrow-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      281 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/progress-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      304 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/progress-v.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      356 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-ac.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-au.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      362 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-dc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-du.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      359 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      359 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-pc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      225 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/radio-pu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      276 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-ha.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      263 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-hd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      278 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-hn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      278 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-hp.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      266 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-va.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      262 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-vd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      271 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-vn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      271 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sbthumb-vp.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      474 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scale-ha.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      336 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scale-hd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      477 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scale-hn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      526 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scale-va.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      342 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scale-vd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      511 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scale-vn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       87 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scaletrough-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      111 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scaletrough-v.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sep-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sep-v.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       77 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/sizegrip.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      536 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tab-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      549 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tab-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      554 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      499 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      557 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      527 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      333 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-pa.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      509 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tree-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      519 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tree-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      528 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tree-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      420 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tree-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)    11637 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)      406 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2226 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/LICENSE
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/
+-rw-r--r--   0 fusionbot   (505) staff       (20)       70 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/arrow-optionmenu-disabled.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       79 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/arrow-optionmenu-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       79 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/arrow-optionmenu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1954 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-active-disabled.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1953 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-active-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      872 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-active.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1267 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-default.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2001 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      138 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/check1.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      145 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/check2.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/combo-active.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/entry-active.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/entry-inactive.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/grip-horiz-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/grip-horiz.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       59 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/grip-vert-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       59 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/grip-vert.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      700 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/list-header-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      706 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/list-header.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/option1.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      363 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/option2.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      995 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/progressbar-horiz.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      966 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/progressbar-vert.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/scale-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      320 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/scale.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      651 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-horiz-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      673 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-horiz.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      666 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-vert-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      722 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-vert.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      542 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-down-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      555 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-down.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      555 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-left-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      556 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-left.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      555 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-right-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      560 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-right.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      542 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-up-prelight.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      549 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-up.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      544 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/tab-top-active.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      583 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/tab-top.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       97 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-horiz.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      664 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-progressbar-horiz.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      677 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-progressbar-vert.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      803 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-horiz.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      871 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-vert.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      133 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-vert.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     9054 2024-03-08 19:19:03.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)      154 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      203 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/arrow-down-insens.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      200 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/arrow-down-prelight.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      202 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/arrow-down.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      128 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/arrow-up-small-insens.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      127 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/arrow-up-small-prelight.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      132 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/arrow-up-small.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      201 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/arrow-up.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      370 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/button-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      156 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/button-empty.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      365 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/button-hover.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      210 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/button-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      347 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/button.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      321 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/checkbox-checked-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      334 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/checkbox-checked.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      227 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/checkbox-unchecked-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      216 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/checkbox-unchecked.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      197 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/combo-entry-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      285 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/combo-entry-button-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      289 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/combo-entry-button-hover.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      203 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/combo-entry-button-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      274 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/combo-entry-button.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/combo-entry-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      236 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/combo-entry.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      221 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/down-background-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      183 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/down-background-disable.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/down-background-hover.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      218 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/down-background.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)       71 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/empty.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      223 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/entry-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      265 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/entry-border-bg.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      258 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/entry-border-disabled.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      202 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/focus.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      157 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/frame.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      264 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/labelframe.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      307 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/minus.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      264 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/notebook.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      148 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/null.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      294 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/plus.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      140 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/progressbar-horiz.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      141 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/progressbar-vert.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      588 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/radio-checked-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      667 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/radio-checked.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      476 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/radio-unchecked-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      567 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/radio-unchecked.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      181 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-horiz-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      183 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-horiz-insens.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      185 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-horiz-prelight.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      185 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-horiz.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      386 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-insensitive.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      385 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-prelight.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      177 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-vert-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      203 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-vert-insens.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      184 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-vert-prelight.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      184 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider-vert.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      338 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/slider.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      213 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/tab-top-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      227 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/tab-top-hover.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/tab-top.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      129 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/treeview.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      177 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-horizontal-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      177 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-horizontal.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      429 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-progressbar-horiz.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      405 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-progressbar-vert.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      429 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-progressbar.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      405 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-progressbar_v.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      143 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-scrollbar-horiz.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      142 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-scrollbar-vert.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      277 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-vertical-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      176 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/trough-vertical.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      234 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/up-background-active.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      195 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/up-background-disable.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/up-background-hover.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)      224 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/up-background.png
+-rw-r--r--   0 fusionbot   (505) staff       (20)    14336 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)      441 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/LICENSE
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      273 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowdown-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      258 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowdown-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      292 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowleft-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      272 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowleft-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      274 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowright-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      258 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowright-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      286 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowup-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      271 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/arrowup-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1266 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      896 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      881 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      625 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      859 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-s.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1110 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/cbox-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1076 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/cbox-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1097 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/cbox-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      434 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/check-c.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      423 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/check-u.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hsb-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hsb-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      401 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hsb-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      395 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hsb-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      119 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hsb-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      592 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hslider-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      579 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hslider-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/indicator-c.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       64 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/indicator-o.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1116 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/mbut-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       61 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/mbut-arrow-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1057 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/mbut-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1095 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/mbut-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      712 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/progress-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      713 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/progress-v.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      695 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/radio-c.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      686 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/radio-u.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      409 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/spinbox-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       56 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/spindown-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      207 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/spindown-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       56 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/spinup-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      190 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/spinup-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      871 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tab-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      383 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tab-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      878 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tab-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      907 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tbar-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      238 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tbar-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      927 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tbar-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tree-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      688 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tree-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      373 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vsb-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      240 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vsb-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      405 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vsb-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      399 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vsb-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      124 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vsb-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      587 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vslider-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      581 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vslider-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)    13334 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik_alt/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik_alt/hsb-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik_alt/hsb-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      373 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik_alt/vsb-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      240 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik_alt/vsb-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      314 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/pkgIndex.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)      650 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2147 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/LICENSE
+-rw-r--r--   0 fusionbot   (505) staff       (20)      219 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/
+-rw-r--r--   0 fusionbot   (505) staff       (20)       49 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrow-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       49 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrow-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      218 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowdown-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      225 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowdown-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      353 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowleft-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      242 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowleft-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowright-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      242 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowright-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      219 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowup-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/arrowup-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       88 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/border.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1209 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/button-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1221 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/button-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      302 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/button-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      141 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/check-hc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      145 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/check-hu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      198 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/check-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      197 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/check-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      144 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/check-pc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      320 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      453 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      463 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-f.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-fa.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      446 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      728 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-r.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      721 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-ra.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      111 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/entry-f.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      106 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/entry-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      446 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/hprogress-b.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      124 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/hprogress-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      139 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/hsb-g.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      348 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/hsb-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       85 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/hsb-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      319 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/hslider-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       63 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/hslider-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       99 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/notebook-c.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      376 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/notebook-ta.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      378 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/notebook-tn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      156 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/notebook-ts.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      120 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/radio-hc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      154 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/radio-hu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      208 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/radio-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      151 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/radio-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      121 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/radio-pc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      201 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spinbox-f.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      160 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spinbox-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      130 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spinbut-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       60 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spinbut-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      144 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spindown-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      189 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spindown-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      202 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spindown-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      147 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spinup-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      192 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spinup-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      206 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/spinup-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      691 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/tbutton-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       58 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/tbutton-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      450 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/tbutton-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      357 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/tree-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      227 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/tree-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      427 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/vprogress-b.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      146 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/vsb-g.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      220 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/vsb-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       80 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/vsb-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      208 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/vslider-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       67 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/vslider-t.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     9617 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2226 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/LICENSE.ORIG
+-rw-r--r--   0 fusionbot   (505) staff       (20)      396 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/pkgIndex.tcl
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      357 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowdown-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      361 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowdown-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowdown-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowdown-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowleft-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      569 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowleft-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      355 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowleft-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      356 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowleft-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowright-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      364 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowright-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      354 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowright-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      355 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowright-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      355 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowup-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      363 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowup-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      356 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowup-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      358 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowup-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       63 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/blank.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1026 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      734 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      742 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      996 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1441 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-s.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1022 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-sa.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      645 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/check-dc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      337 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/check-du.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      630 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/check-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      389 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/check-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      247 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      442 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-ra.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      451 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-rd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      672 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-rf.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      452 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-rn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      679 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-rp.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      381 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/comboarrow-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      389 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/comboarrow-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      381 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/comboarrow-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      381 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/comboarrow-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      743 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/progress-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      733 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/progress-v.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      630 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/radio-dc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      364 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/radio-du.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1035 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/radio-nc.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      564 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/radio-nu.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      221 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-ha.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      333 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-hd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-hn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-hp.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      226 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-va.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      335 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-vd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-vn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      330 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sbthumb-vp.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      369 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scale-ha.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      365 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scale-hd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scale-hn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      367 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scale-va.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      364 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scale-vd.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      367 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scale-vn.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      209 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scaletrough-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      233 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/scaletrough-v.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sep-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       40 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sep-v.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)       78 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/sizegrip.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      454 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/tab-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      409 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/tab-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      453 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-a.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      689 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      672 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      691 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      683 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-pa.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      366 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/tree-d.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      257 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/tree-h.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      362 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/tree-n.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)      363 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/tree-p.gif
+-rw-r--r--   0 fusionbot   (505) staff       (20)    12159 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance.tcl
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/trash.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1741 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/unlinked.ppm
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2267 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/graphics/warning.gif
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/extras/styles/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      342 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/styles/DIII-D.mplstyle
+-rw-r--r--   0 fusionbot   (505) staff       (20)      770 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/styles/DIII-D_beamer.mplstyle
+-rw-r--r--   0 fusionbot   (505) staff       (20)      769 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/styles/DIII-D_beamer_half.mplstyle
+-rw-r--r--   0 fusionbot   (505) staff       (20)      770 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/styles/DIII-D_beamer_multifig.mplstyle
+-rw-r--r--   0 fusionbot   (505) staff       (20)      859 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/extras/styles/DIII-D_paper_one_of_two_columns.mplstyle
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/framework_guis/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3423 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/developerModeGUI.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    44586 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/efitviewer_gui.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6805 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/efitviewer_settings.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)    18806 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/efitviewer_support_gui.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3147 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/imasActorGUI.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3703 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/imasGUI.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2121 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/latexGUI.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    10662 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/machine_mappings.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3399 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/moduleSetupGUI.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2316 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/namelistGUI.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     9715 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/preferencesGUI.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6189 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/framework_guis/spruceUpFigures.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     7823 2024-03-08 20:50:52.000000 omfit_classes-3.2024.9.2/framework_guis/styleGUI.py
+-rwxr-xr-x   0 fusionbot   (505) staff       (20)     4448 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/
+-rw-r--r--   0 fusionbot   (505) staff       (20)   304834 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/OMFITx.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/__init__.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    76415 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/adaptors.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    42383 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/atomic_elements.json
+-rw-r--r--   0 fusionbot   (505) staff       (20)     9475 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/brainfuse.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     9710 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/brainfusetf.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2368 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/exceptions_omfit.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   144808 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/fluxSurface.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    12090 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/gapy.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     9302 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/harvest_lib.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    64521 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/namelist.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     4953 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_accome.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3673 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_ascii.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     4580 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_asciitable.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2346 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_aurora.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   212488 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_base.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    10776 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_bibtex.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    24974 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_boundary.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     5916 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_bout.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    12867 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_brainfuse.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6416 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_cdb.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    33174 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_chease.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2867 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_chombo.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6732 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_clusters.json
+-rw-r--r--   0 fusionbot   (505) staff       (20)    10357 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_clusters.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    25698 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_coils.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6311 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_cotsim.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     7018 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_csv.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   140223 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_ctrl_analysis.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    31373 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_data.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     5059 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_dir.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    11301 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_dmp.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6926 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_efit.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    97543 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_efitviewer.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    73309 2024-03-08 20:50:52.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_efund.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    14430 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_elite.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   181065 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_elm.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1594 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_environment.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6068 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_eped.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   348799 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_eqdsk.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1759 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_error.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2435 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_execution_diagram.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1273 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_fastran.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    16304 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_focus.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     4212 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_formatter.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    54185 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gacode.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1428 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gaprofiles.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   133115 2024-03-08 20:50:52.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gapy.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    18819 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gato.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    12142 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_genray.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1728 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gingred.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    46693 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_github.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     4243 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gks.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2592 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gnuplot.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    57394 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_google_sheet.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    51592 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gpec.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1616 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_gptools.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    17339 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_harvest.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     8303 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_hdf5.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    48570 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_helena.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1507 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_idl.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     5034 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_idlSav.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     5022 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_ini.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    13082 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_interface.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     5481 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_ionorb.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     5154 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_jscope.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1774 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_jsolver.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     7459 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_json.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2877 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_kepler.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    29701 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_latex.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    92530 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_mars.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2352 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_matlab.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     6709 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_matrix.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    85242 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_mds.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1724 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_mmm.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3425 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_namelist.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    21157 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_nc.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    33491 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_nimrod.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    56023 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_oedge.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    19310 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_omas.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    53177 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_d3d.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    11705 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_east.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    12148 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_kstar.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   157087 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_utils.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   114847 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_onetwo.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    49418 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_osborne.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    51257 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_patch.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)      784 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_path.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3078 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_pdb.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   116962 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_profiles.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    85704 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_python.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    33627 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_rabbit.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    39649 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_rdb.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2366 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_reviewplus.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   114264 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_solps.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3423 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_spider.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    98670 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_testing.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   107516 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_tglf.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   115550 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_thomson.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     7856 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_timcon.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    21853 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_toksearch.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     7617 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_toq.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    71812 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_transp.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    48768 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_trip3d.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    13791 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_tsc.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2695 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_uda.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    11728 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_uedge.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    18800 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_ufile.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2146 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_weblink.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3451 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_xml.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2822 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/omfit_yaml.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/GUIS/
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/GUIS/__init__.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/INPUTS/
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/INPUTS/__init__.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/LIB/
+-rw-r--r--   0 fusionbot   (505) staff       (20)       15 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/LIB/OMFITlib_startup.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     2627 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/OMFITsave.txt
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/OUTPUTS/
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/OUTPUTS/__init__.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/PLOTS/
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/PLOTS/__init__.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/SCRIPTS/
+-rw-r--r--   0 fusionbot   (505) staff       (20)        0 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/SCRIPTS/__init__.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)      478 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/SettingsNamelist.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1589 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/help.rst
+-rw-r--r--   0 fusionbot   (505) staff       (20)    41260 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettings.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)     7677 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettingsNamelist.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)       92 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettingsNamelistOSX.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)      141 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettingsNamelistUNIX.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)       89 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettingsOSX.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)       90 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettingsUNIX.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)    57188 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/sortedDict.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1032 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/startup_choice.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    12200 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/startup_classes.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    55483 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/startup_framework.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   734548 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/uedge_common_map.json
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes/unix_os/
+-rw-r--r--   0 fusionbot   (505) staff       (20)      139 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/unix_os/__init__.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)      325 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/unix_os/path.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)      761 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/unix_os/setup.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)        3 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/unix_os/version
+-rw-r--r--   0 fusionbot   (505) staff       (20)   158516 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/utils_base.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   128683 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/utils_fit.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   147207 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/utils_fusion.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   236581 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/utils_math.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)   166642 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/utils_plot.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)       10 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/version
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3549 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_classes/zdata.py
+drwxr-xr-x   0 fusionbot   (505) staff       (20)        0 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/omfit_classes.egg-info/
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1178 2024-03-08 20:50:54.000000 omfit_classes-3.2024.9.2/omfit_classes.egg-info/PKG-INFO
+-rw-r--r--   0 fusionbot   (505) staff       (20)    32245 2024-03-08 20:50:56.000000 omfit_classes-3.2024.9.2/omfit_classes.egg-info/SOURCES.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)        1 2024-03-08 20:50:54.000000 omfit_classes-3.2024.9.2/omfit_classes.egg-info/dependency_links.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)       14 2024-03-08 20:50:54.000000 omfit_classes-3.2024.9.2/omfit_classes.egg-info/top_level.txt
+-rw-r--r--   0 fusionbot   (505) staff       (20)   370599 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_gui.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     3236 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_halt.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)     4949 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_parse_args.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    83252 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_plot.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    12707 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_setup.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    83673 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/omfit_tree.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)       38 2024-03-08 20:50:57.000000 omfit_classes-3.2024.9.2/setup.cfg
+-rw-r--r--   0 fusionbot   (505) staff       (20)     1314 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/setup.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    26589 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/utils.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    62680 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/utils_tk.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)    32777 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/utils_widgets.py
+-rw-r--r--   0 fusionbot   (505) staff       (20)       10 2024-03-08 19:19:04.000000 omfit_classes-3.2024.9.2/version
```

### Comparing `omfit_classes-3.2024.13.2/LICENSE.txt` & `omfit_classes-3.2024.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/PKG-INFO` & `omfit_classes-3.2024.9.2/omfit_classes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: omfit_classes
-Version: 3.2024.13.2
+Name: omfit-classes
+Version: 3.2024.9.2
 Summary: Classes of OMFIT (One Modeling Framework For Integrated Tasks)
 Home-page: https://omfit.io
 Author: OMFIT developers
 Author-email: meneghini@fusion.gat.com
 License: MIT
 Keywords: integrated modeling plasma framework
 Platform: UNKNOWN
```

### Comparing `omfit_classes-3.2024.13.2/README.rst` & `omfit_classes-3.2024.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/externalImports.py` & `omfit_classes-3.2024.9.2/externalImports.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/LOM.png` & `omfit_classes-3.2024.9.2/extras/graphics/LOM.png`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_font.bf` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_font.bf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_font.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_font.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo.gif` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo.pdf` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo.pdf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_color.gif` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_color.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_color.pdf` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_color.pdf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_olympics.gif` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_olympics.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/OMFIT_logo_olympics.pdf` & `omfit_classes-3.2024.9.2/extras/graphics/OMFIT_logo_olympics.pdf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/bookmark.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/bookmark.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/colors.py` & `omfit_classes-3.2024.9.2/extras/graphics/colors.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/copy.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/copy.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/crosshair.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/crosshair.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/error.gif` & `omfit_classes-3.2024.9.2/extras/graphics/error.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Humor-Sans.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Bold.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Bold.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-BoldItalic.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-ExtraLight.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-ExtraLightItalic.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Italic.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Italic.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Light.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Light.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-LightItalic.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-Semi-BoldItalic.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-Semi-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli-SemiBold.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts/Muli.ttf` & `omfit_classes-3.2024.9.2/extras/graphics/fonts/Muli.ttf`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/fonts.py` & `omfit_classes-3.2024.9.2/extras/graphics/fonts.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/help.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/help.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/info.gif` & `omfit_classes-3.2024.9.2/extras/graphics/info.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/legend.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/legend.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/linked.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/linked.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/mail.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/mail.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/matplotlib_backends.py` & `omfit_classes-3.2024.9.2/extras/graphics/matplotlib_backends.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/paste.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/paste.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/pdf.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/pdf.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/pin.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/pin.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/question.gif` & `omfit_classes-3.2024.9.2/extras/graphics/question.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/select.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/select.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/settings.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/settings.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/storage.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/storage.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/text.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/text.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/CreateImageLib.def` & `omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/CreateImageLib.def`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/ImageLib.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/ImageLib.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/LICENSE` & `omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/LICENSE`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/aquativo.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/aquativo.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/aquativo/images.tgz` & `omfit_classes-3.2024.9.2/extras/graphics/themes/aquativo/images.tgz`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/black/LICENSE` & `omfit_classes-3.2024.9.2/extras/graphics/themes/black/LICENSE`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/black/black.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/black/black.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/blue/LICENSE` & `omfit_classes-3.2024.9.2/extras/graphics/themes/blue/LICENSE`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/button-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/button-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/button-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/button-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/button-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/button-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/radio-hc.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/radio-hc.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue/radio-hu.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue/radio-hu.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/blue/blue.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/blue/blue.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/LICENSE` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/LICENSE`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-a.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-a.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-d.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-d.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/button-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/button-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-ra.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-ra.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-rd.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-rd.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-rf.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-rf.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/combo-rn.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/combo-rn.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/scale-va.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/scale-va.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tab-a.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tab-a.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tab-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tab-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-a.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-a.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/toolbutton-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tree-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tree-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks/tree-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks/tree-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/clearlooks/clearlooks.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/clearlooks/clearlooks.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/LICENSE` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/LICENSE`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-active-disabled.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-active-disabled.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-active-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-active-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-active.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-active.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-default.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-default.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/button-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/button-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/list-header-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/list-header-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/list-header.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/list-header.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/progressbar-horiz.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/progressbar-horiz.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/progressbar-vert.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/progressbar-vert.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-horiz-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-horiz-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-horiz.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-horiz.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-vert-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-vert-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/slider-vert.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/slider-vert.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-down-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-down-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-down.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-down.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-left-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-left-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-left.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-left.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-right-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-right-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-right.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-right.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-up-prelight.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-up-prelight.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/stepper-up.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/stepper-up.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/tab-top-active.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/tab-top-active.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/tab-top.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/tab-top.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-progressbar-horiz.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-progressbar-horiz.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-progressbar-vert.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-progressbar-vert.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-horiz.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-horiz.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-vert.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance/trough-scrollbar-vert.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/elegance/elegance.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/elegance/elegance.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/radio-checked-insensitive.png` & `omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/radio-checked-insensitive.png`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/radio-checked.png` & `omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/radio-checked.png`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux/radio-unchecked.png` & `omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux/radio-unchecked.png`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/equilux/equilux.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/equilux/equilux.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/LICENSE` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/LICENSE`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-d.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-d.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/button-s.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/button-s.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/cbox-a.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/cbox-a.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/cbox-d.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/cbox-d.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/cbox-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/cbox-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hslider-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hslider-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/hslider-t.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/hslider-t.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/mbut-a.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/mbut-a.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/mbut-d.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/mbut-d.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/mbut-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/mbut-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/progress-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/progress-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/progress-v.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/progress-v.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/radio-c.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/radio-c.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/radio-u.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/radio-u.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tab-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tab-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tab-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tab-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tbar-a.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tbar-a.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tbar-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tbar-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/tree-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/tree-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vslider-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vslider-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik/vslider-t.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik/vslider-t.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/keramik/keramik.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/keramik/keramik.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/pkgIndex.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/pkgIndex.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/LICENSE` & `omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/LICENSE`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/button-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/button-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/button-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/button-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-r.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-r.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/combo-ra.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/combo-ra.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik/tbutton-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik/tbutton-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/plastik/plastik.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/plastik/plastik.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/LICENSE.ORIG` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/LICENSE.ORIG`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/arrowleft-d.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/arrowleft-d.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-a.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-a.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-d.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-d.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-s.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-s.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/button-sa.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/button-sa.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/check-dc.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/check-dc.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/check-nc.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/check-nc.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-rf.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-rf.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/combo-rp.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/combo-rp.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/progress-h.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/progress-h.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/progress-v.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/progress-v.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/radio-dc.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/radio-dc.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/radio-nc.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/radio-nc.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/radio-nu.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/radio-nu.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-d.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-d.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-n.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-n.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-p.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-p.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance/toolbutton-pa.gif` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance/toolbutton-pa.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/themes/radiance/radiance.tcl` & `omfit_classes-3.2024.9.2/extras/graphics/themes/radiance/radiance.tcl`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/trash.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/trash.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/unlinked.ppm` & `omfit_classes-3.2024.9.2/extras/graphics/unlinked.ppm`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/graphics/warning.gif` & `omfit_classes-3.2024.9.2/extras/graphics/warning.gif`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/styles/DIII-D_beamer.mplstyle` & `omfit_classes-3.2024.9.2/extras/styles/DIII-D_beamer.mplstyle`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/styles/DIII-D_beamer_half.mplstyle` & `omfit_classes-3.2024.9.2/extras/styles/DIII-D_beamer_half.mplstyle`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/styles/DIII-D_beamer_multifig.mplstyle` & `omfit_classes-3.2024.9.2/extras/styles/DIII-D_beamer_multifig.mplstyle`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/extras/styles/DIII-D_paper_one_of_two_columns.mplstyle` & `omfit_classes-3.2024.9.2/extras/styles/DIII-D_paper_one_of_two_columns.mplstyle`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/developerModeGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/developerModeGUI.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/efitviewer_gui.py` & `omfit_classes-3.2024.9.2/framework_guis/efitviewer_gui.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/efitviewer_settings.txt` & `omfit_classes-3.2024.9.2/framework_guis/efitviewer_settings.txt`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/efitviewer_support_gui.py` & `omfit_classes-3.2024.9.2/framework_guis/efitviewer_support_gui.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/imasActorGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/imasActorGUI.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/imasGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/imasGUI.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/latexGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/latexGUI.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/machine_mappings.py` & `omfit_classes-3.2024.9.2/framework_guis/machine_mappings.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/moduleSetupGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/moduleSetupGUI.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/namelistGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/namelistGUI.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/preferencesGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/preferencesGUI.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/spruceUpFigures.py` & `omfit_classes-3.2024.9.2/framework_guis/spruceUpFigures.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/framework_guis/styleGUI.py` & `omfit_classes-3.2024.9.2/framework_guis/styleGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,16 +173,16 @@
 options.insert(0, '', '')
 
 
 def iter_style_files(style_dir):
     """Yield file path and name of styles in the given directory."""
     for path in os.listdir(style_dir):
         filename = os.path.basename(path)
-        match = matplotlib.style.core.STYLE_FILE_PATTERN.match(filename)
-        if match is not None:
+        if is_style_file(filename):
+            match = STYLE_FILE_PATTERN.match(filename)
             path = os.path.abspath(os.path.join(style_dir, path))
             yield path, match.group(1)
 
 
 for filename, stl in iter_style_files(os.sep.join([matplotlib.get_configdir(), 'stylelib'])):
     options[stl] = filename
 OMFITx.ComboBox(
```

### Comparing `omfit_classes-3.2024.13.2/omfit.py` & `omfit_classes-3.2024.9.2/omfit.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/OMFITx.py` & `omfit_classes-3.2024.9.2/omfit_classes/OMFITx.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/adaptors.py` & `omfit_classes-3.2024.9.2/omfit_classes/adaptors.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/atomic_elements.json` & `omfit_classes-3.2024.9.2/omfit_classes/atomic_elements.json`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/brainfuse.py` & `omfit_classes-3.2024.9.2/omfit_classes/brainfuse.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/brainfusetf.py` & `omfit_classes-3.2024.9.2/omfit_classes/brainfusetf.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/exceptions_omfit.py` & `omfit_classes-3.2024.9.2/omfit_classes/exceptions_omfit.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/fluxSurface.py` & `omfit_classes-3.2024.9.2/omfit_classes/fluxSurface.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/gapy.py` & `omfit_classes-3.2024.9.2/omfit_classes/gapy.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/harvest_lib.py` & `omfit_classes-3.2024.9.2/omfit_classes/harvest_lib.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/namelist.py` & `omfit_classes-3.2024.9.2/omfit_classes/namelist.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_accome.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_accome.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_ascii.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_ascii.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_asciitable.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_asciitable.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_aurora.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_aurora.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_base.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_base.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_bibtex.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_bibtex.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_boundary.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_boundary.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_bout.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_bout.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_brainfuse.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_brainfuse.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_cdb.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_cdb.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_chease.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_chease.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_chombo.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_chombo.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_clusters.json` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_clusters.json`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_clusters.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_clusters.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_coils.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_coils.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_cotsim.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_cotsim.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_csv.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_csv.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_ctrl_analysis.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_ctrl_analysis.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_data.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_data.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_dir.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_dir.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_dmp.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_dmp.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_efit.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_efit.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_efitviewer.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_efitviewer.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_efund.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_efund.py`

 * *Files 2% similar despite different names*

```diff
@@ -787,15 +787,15 @@
          :param outline: ods outline entry
 
          :return: outline
         """
 
         a1 = coil_data[4] * np.pi / 180.0
         a2 = coil_data[5] * np.pi / 180.0
-        if abs(a1) < 1e-8 and abs(a2) > 1e-8:
+        if a1 < 1e-8 and a2 > 1e-8:
             side = coil_data[3] / np.tan(a2)
             hw1 = (coil_data[2] + side) / 2.0
             hw2 = (coil_data[2] - side) / 2.0
             hh = coil_data[3] / 2.0
             outline['r'] = [
                 coil_data[0] - hw1,
                 coil_data[0] - hw2,
@@ -1009,15 +1009,14 @@
         self['IN3']['ZVS'] = []
         self['IN3']['WVS'] = []
         self['IN3']['HVS'] = []
         self['IN3']['AVS'] = []
         self['IN3']['AVS2'] = []
         self['IN3']['RSISVS'] = []
         self['IN3']['VSID'] = []
-        self['IN3']['VSNAME'] = []
 
         self['IN3']['RACOIL'] = []
         self['IN3']['ZACOIL'] = []
         self['IN3']['WACOIL'] = []
         self['IN3']['HACOIl'] = []
 
         self['IN3']['RSI'] = []
@@ -1039,116 +1038,93 @@
         self['IN5']['IECOIL'] = 0
         self['IN5']['IVESEL'] = 0
         self['IN5']['IACOIL'] = 0
         self['IN5']['mgaus1'] = 8
         self['IN5']['mgaus2'] = 12
         return self
 
-    def from_omas(self, ods, passive_map='VS'):
+    def from_omas(self, ods, passive_map='F'):
 
         if 'dataset_description.data_entry.machine' in ods:
             device = ods['dataset_description.data_entry.machine']
         else:
             device = 'my_device'
 
         self = self.init_mhdin(device)
 
         ncoil = {'F': 0, 'E': 0, 'ACOIL': 0, 'VS': 0}
         nsum = {'F': 0, 'E': 0, 'ACOIL': 0, 'VS': 0}
         # DIII-D
         coil_map = {'OH': 'E', 'PF': 'F', 'DIV': 'ACOIL'}
         # ITER
         coil_map['CS'] = 'E'  # Central solenoid
-        coil_map['VS'] = 'F'  # Vertical Stabilzation (in-vessel coils)
+        coil_map['VS'] = passive_map  # Vertical Stabilzation (in-vessel coils)
         coil_map['TF'] = 'ACOIL'  # TF coil busbars
         coil_map['VC'] = 'S'  # Virtual coils (skip)
 
         for coil_type in ['pf_active.coil', 'pf_passive.loop']:
 
-            if not coil_type in ods:
-                continue
-
             for isum in ods[coil_type]:
 
                 coil = ods[coil_type][isum]
-                efund_name = 'S'
-                if coil_type == 'pf_passive.loop':
-                    efund_name = passive_map
-                else:
-                    for i in coil_map.keys():
-                        if i in coil['name']:
-                            efund_name = coil_map[i]
+                for i in coil_map.keys():
+                    if i in coil['name']:
+                        efund_name = coil_map[i]
 
                 if efund_name == 'S':
                     continue
 
                 nsum[efund_name] += 1
-                if 'CS1L' in coil['name']:  # ITER
-                    nsum[efund_name] -= 1
-                elif efund_name == 'F':
-                    if 'nstx' in device or 'mast' in device:
-                        self['IN3']['TURNFC'].append(1.0)
-                    else:
-                        self['IN3']['TURNFC'].append(coil['element'][0]['turns_with_sign'])
-
                 for ielement in coil['element']:
                     ncoil[efund_name] += 1
                     element = coil['element'][ielement]
                     if 'rectangle' in element['geometry']:
                         [r, z, w, h, a1, a2] = self.rectangle_to_efund(element['geometry.rectangle'])
                     elif 'annulus' in element['geometry']:
                         [r, z, w, h, a1, a2] = self.annulus_to_efund(element['geometry.annulus'])
                     elif 'outline' in element['geometry']:
                         [r, z, w, h, a1, a2] = self.outline_to_efund(element['geometry.outline'])
-                    elif 'thick_line' in element['geometry']:
-                        [r, z, w, h, a1, a2] = self.thick_line_to_efund(element['geometry.thick_line'])
                     else:
-                        raise ValueError(f'No conversion defined for geometry of {coil_type}.{isum}')
+                        raise ValueError(f'No conversion defined for geometry of coil {isum}')
 
                     self['IN3'][f'R{efund_name}'].append(r)
                     self['IN3'][f'Z{efund_name}'].append(z)
                     self['IN3'][f'W{efund_name}'].append(w)
                     self['IN3'][f'H{efund_name}'].append(h)
 
                     if efund_name == 'F' or efund_name == 'VS':
                         self['IN3'][f'A{efund_name}'].append(a1)
                         self['IN3'][f'A{efund_name}2'].append(a2)
 
-                    if efund_name == 'VS':
+                    if efund_name == 'F':
+                        self['IN3'][f'TURN{efund_name}C'].append(1.0)
+                    elif efund_name == 'VS':
                         self['IN3'][f'VSID'].append(nsum[efund_name])
                         self['IN5'][f'IVESEL'] = 1
                         if 'resistance' in coil:
                             self['IN3']['RSISVS'].append(coil['resistance'])
                         else:
                             self['IN3']['RSISVS'].append(coil['resistivity'] / 2 / np.pi / r)
-                        self['IN3']['VSNAME'].append(coil['name'])
-                    elif efund_name == 'F':
-                        self['IN3']['FCID'].append(nsum[efund_name])
-                        if 'nstx' in device or 'mast' in device:
-                            self['IN3']['FCTURN'].append(coil['element'][0]['turns_with_sign'])
-                        else:
-                            self['IN3']['FCTURN'].append(1.0)
-                        self['IN5']['IFCOIL'] = 1
                     elif efund_name != 'ACOIL':
                         self['IN3'][f'{efund_name}CID'].append(nsum[efund_name])
+
                         self['IN3'][f'{efund_name}CTURN'].append(coil['element'][0]['turns_with_sign'])
                         self['IN5'][f'I{efund_name}COIL'] = 1
                     else:
                         self['IN5'][f'I{efund_name}'] = 1
 
         self['MACHINEIN']['nfsum'] = nsum['F']
         self['machinein']['nfcoil'] = ncoil['F']
         self['MACHINEIN']['nesum'] = nsum['E']
         self['machinein']['necoil'] = ncoil['E']
         self['MACHINEIN']['nvsum'] = nsum['VS']
         self['machinein']['nvesel'] = ncoil['VS']
 
         self['MACHINEIN']['nacoil'] = ncoil['ACOIL']
 
-        self['MACHINEIN']['magpri'] = 0
         if 'magnetics' in ods:
             if 'b_field_pol_probe' in ods['magnetics']:
                 self['MACHINEIN']['magpri'] = nmp2 = len(list(filter(None, ods['magnetics.b_field_pol_probe.:.length'])))
                 self['IN3']['XMP2'] = xmp2 = np.zeros(nmp2)
                 self['IN3']['YMP2'] = ymp2 = np.zeros(nmp2)
                 self['IN3']['SMP2'] = smp2 = np.zeros(nmp2)
                 self['IN3']['AMP2'] = amp2 = np.zeros(nmp2)
@@ -1160,32 +1136,39 @@
                         xmp2[n] = probe['position.r']
                         ymp2[n] = probe['position.z']
                         smp2[n] = probe['length']
                         amp2[n] = -180 / np.pi * probe['poloidal_angle']
                         mpnam2[n] = probe['name']
                         n += 1
 
-            self['MACHINEIN']['nsilop'] = 0
             if 'flux_loop' in ods['magnetics']:
-                self['MACHINEIN']['nsilop'] = nsilop = len(
-                    np.where(np.array(list(filter(None, ods['magnetics.flux_loop.:.type.index']))) == 1)[0]
-                )
+                self['MACHINEIN']['nsilop'] = nsilop = len(ods['magnetics.flux_loop'])
                 self['IN3']['RSI'] = rsi = np.zeros(nsilop)
                 self['IN3']['ZSI'] = zsi = np.zeros(nsilop)
                 self['IN3']['LPNAME'] = lpname = np.chararray(nsilop, itemsize=10, unicode=True)
                 for i in ods['magnetics.flux_loop']:
                     loop = ods['magnetics.flux_loop'][i]
-                    if 'type' in loop and 'index' in loop['type'] and loop['type.index'] == 1:
-                        rsi[i] = loop['position.0.r']
-                        zsi[i] = loop['position.0.z']
-                        lpname[i] = loop['name']
-
-        # only use vessel described in wall if pf_passive hasn't been already
-        # (these should be equivalent, but the annular wall type is harder to represent)
-        if 'wall.description_2d[0].vessel.unit' in ods and not 'pf_passive.loop' in ods:
+                    # this assumes simple loops and
+                    # mean(psi(r1,z1), psi(r2,z2)) = psi(mean(r1, r2), mean(z1, z2))
+                    r = loop['position.0.r']
+                    z = loop['position.0.z']
+                    n = 1
+                    # last position in loop may be repeated
+                    for j in loop['position']:
+                        if loop['position'][j] == loop['position'][0]:
+                            continue
+                        r += loop['position'][j]['r']
+                        z += loop['position'][j]['z']
+                        n += 1
+                    rsi[i] = r / n
+                    zsi[i] = z / n
+                    lpname[i] = loop['name']
+
+        # NOTE: the vacuum vessel could also be described in 'pf_passive' (not yet included)
+        if 'wall.description_2d[0].vessel.unit' in ods:
             self['IN5']['IVESEL'] = 1
 
             nvesel = 0
             for i in ods['wall.description_2d.0.vessel.unit']:
                 unit = ods['wall.description_2d.0.vessel.unit'][i]
                 if 'element' in unit:
                     nvesel += 1
@@ -1204,29 +1187,29 @@
             self['IN3']['VSID'] = vsid = np.zeros(nvesel, dtype=int)
             self['IN3']['VSNAME'] = vsname = np.chararray(nvesel, itemsize=10, unicode=True)
             n = 0
             for i in ods['wall.description_2d.0.vessel.unit']:
                 unit = ods['wall.description_2d.0.vessel.unit'][i]
                 if 'element' in unit:
                     rvs[n], zvs[n], wvs[n], hvs[n], avs[n], avs2[n] = self.outline_to_efund(unit['element.0.outline'])
-                    if 'resistance' in unit['annular.0']:
+                    if 'resistance' in unit['element.0']:
                         rsisvs[n] = unit['element.0.resistance']
                     else:
                         rsisvs[n] = unit['element.0.resistivity'] / 2 / np.pi / rvs[n]
                     vsid[n] = n + 1
                     vsname[n] = unit['name']
                     n += 1
                 elif 'annular' in unit:
                     nl = n + len(unit['annular.centreline.r']) - 1 + unit['annular.centreline.closed']
                     rvs[n:nl], zvs[n:nl], wvs[n:nl], hvs[n:nl], avs[n:nl], avs2[n:nl] = self.annular_to_efund(unit['annular'])
                     # IMAS data schema is missing annular resistance...
-                    # if 'resistance' in unit['annular']:
-                    #    rsisvs[n:nl] = unit['annular.resistance']
+                    # if 'resistance' in unit['element.0']:
+                    #    rsisvs[n:nl] = unit['element.0.resistance']
                     # else:
-                    rsisvs[n:nl] = unit['annular.resistivity'] / 2 / np.pi / rvs[n:nl]
+                    rsisvs[n:nl] = unit['element.0.resistivity'] / 2 / np.pi / rvs[n:nl]
                     vsid[n:nl] = np.arange(n + 1, nl + 1)
                     vsname[n:nl] = unit['name']
                     n = nl
 
         # currently unused (not part of mhdin.dat, but could be used to make lim.dat files)
         # if 'wall.description_2d[0].limiter.unit[0].outline' in ods:
         #    rwall = ods['wall.description_2d[0].limiter.unit[0].outline.r']
@@ -1261,15 +1244,15 @@
         # pf_active
         if 'pf_active' in update and 'RE' in self['IN3']:
             r = self['IN3']['RE']
             z = self['IN3']['ZE']
             width = self['IN3']['WE']
             height = self['IN3']['HE']
             turns = self['IN3']['ECTURN']
-            elements_id = (np.array(self['IN3']['ECID']) - 1).astype(int)
+            elements_id = (self['IN3']['ECID'] - 1).astype(int)
             rect_code = geo_type_lookup('rectangle', 'pf_active', ods.imas_version, reverse=True)
             with omas_environment(ods, dynamic_path_creation='dynamic_array_structures'):
                 for i in range(len(r)):
                     c = elements_id[i]
                     e = sum(elements_id[:i] == elements_id[i])
                     ods['pf_active.coil'][c]['name'] = f'OH{c}'
                     ods['pf_active.coil'][c]['identifier'] = f'OH{c}'
@@ -1291,15 +1274,15 @@
             angle1 = self['IN3']['AF']
             angle2 = self['IN3']['AF2']
             turns = self['IN3']['FCTURN']
             if 'TURNFC' in self['IN3']:
                 turnfc = self['IN3']['TURNFC']
             else:
                 turnfc = np.ones(int(max(self['IN3']['FCID'])))
-            elements_id = (np.array(self['IN3']['FCID']) - 1).astype(int)
+            elements_id = (self['IN3']['FCID'] - 1).astype(int)
             rect_code = geo_type_lookup('rectangle', 'pf_active', ods.imas_version, reverse=True)
             outline_code = geo_type_lookup('outline', 'pf_active', ods.imas_version, reverse=True)
             offset = len(ods['pf_active.coil'])
             for i in range(len(r)):
                 c = elements_id[i] + offset
                 e = sum(elements_id[:i] == elements_id[i])
                 ods['pf_active.coil'][c]['name'] = f'PF{c}'
@@ -1357,16 +1340,16 @@
             r = self['IN3']['RVS']
             z = self['IN3']['ZVS']
             width = self['IN3']['WVS']
             height = self['IN3']['HVS']
             angle1 = self['IN3']['AVS']
             angle2 = self['IN3']['AVS2']
             resistance = self['IN3']['RSISVS']
-            resistivity = np.array(self['IN3']['RSISVS']) * 2 * np.pi * np.array(r)
-            elements_id = (np.array(self['IN3']['VSID']) - 1).astype(int)
+            resistivity = self['IN3']['RSISVS'] * 2 * np.pi * r
+            elements_id = (self['IN3']['VSID'] - 1).astype(int)
 
             for i in range(len(r)):
                 c = elements_id[i]
                 e = sum(elements_id[:i] == elements_id[i])
                 ods['pf_passive.loop'][c]['name'] = f'VS{c}'
                 # ods['pf_passive.loop'][c]['identifier'] = f'PF{c}'
                 ods['pf_passive.loop'][c]['element'][e]['name'] = f'VS{c}_{e}'
@@ -1729,45 +1712,27 @@
             printw('could not read array sizes from mhdin.dat')
         except Exception:
             printw('could not read array sizes from mhdin.dat or dprobe.dat')
 
     if ods is None:
         ods = ODS()
 
+    ods['em_coupling.code.name'] = 'EFUND'
+    ods['em_coupling.poloidal_probes'] = mhdin['in3']['mpnam2']
+    ods['em_coupling.flux_loops'] = mhdin['in3']['lpname']
+
     green = {}
     green['nesum'] = nesum
     green['nsilop'] = nsilop
     green['magpri'] = magpri
     green['nfsum'] = nfsum
     green['nvsum'] = nvsum
     green['nw'] = nw
     green['nh'] = nh
 
-    ods['em_coupling.code.name'] = 'EFUND'
-    ods['em_coupling.ids_properties.homogeneous_time'] = 2
-
-    # Missing/TODO: These should be setup as URIs now but not sure how to do that... using names or meaningless strings for now
-    if magpri > 0:
-        ods['em_coupling.b_field_pol_probes'] = mhdin['in3']['mpnam2']
-    else:
-        ods['em_coupling.b_field_pol_probes'] = np.empty(0)
-    if nsilop > 0:
-        ods['em_coupling.flux_loops'] = mhdin['in3']['lpname']
-    else:
-        ods['em_coupling.flux_loops'] = np.empty(0)
-    if nesum > 0 or nfsum > 0:
-        ods['em_coupling.active_coils'] = np.chararray(nesum + nfsum, itemsize=1, unicode=True)
-    else:
-        ods['em_coupling.active_coils'] = np.empty(0)
-    if nvsum > 0:
-        ods['em_coupling.passive_loops'] = mhdin['in3']['vsname']
-    else:
-        ods['em_coupling.passive_loops'] = np.empty(0)
-    ods['em_coupling.plasma_elements'] = np.chararray(nw * nh, itemsize=1, unicode=True)
-
     endian = '>'
     # Response of poloidal field (F) coils on grid, and grid on itself.
     filename = f'ec{nw}{nh}.ddd'
     file = filedir + filename
     f = scipy.io.FortranFile(file, 'r', f'{endian}i4')
     [mw, mh] = f.read_ints(f'{endian}i4')
     grid = f.read_reals(f'{endian}f8')
@@ -1777,50 +1742,50 @@
     try:
         ods['equilibrium.time_slice.0.profiles_2d.0.grid.dim1'] = green['rgrid']
         ods['equilibrium.time_slice.0.profiles_2d.0.grid.dim2'] = green['zgrid']
     except Exception:
         printw('could not write grid sizes to equilibium')
 
     ggridfc = f.read_reals(f'{endian}f8').reshape([nfsum, mw * mh]).T
-    ods['em_coupling.mutual_plasma_plasma'] = f.read_reals(f'{endian}f8').reshape(mw, mh * mw).T
+    ods['em_coupling.mutual_grid_grid'] = f.read_reals(f'{endian}f8').reshape(mw, mh * mw).T
 
     # Response of poloidal field coil on flux loops, magnetic probes, and grid
     filename = f'rfcoil.ddd'
     file = filedir + filename
     f = scipy.io.FortranFile(file, 'r', f'{endian}i4')
     rsilfc = f.read_reals(f'{endian}f8').reshape([nfsum, nsilop]).T
     rmp2fc = f.read_reals(f'{endian}f8').reshape([nfsum, magpri]).T
 
-    # Response of Ohmic heating coil on flux loops, magnetic probes, and plasma
+    # Response of Ohmic heating coil on flux loops, magnetic probes, and grid
     try:
         filename = f're{nw}{nh}.ddd'
         file = filedir + filename
         f = scipy.io.FortranFile(file, 'r', f'{endian}i4')
         rsilec = f.read_reals(f'{endian}f8').reshape([nesum, nsilop]).T
         rmp2ec = f.read_reals(f'{endian}f8').reshape([nesum, magpri]).T
         gridec = f.read_reals(f'{endian}f8').reshape([nesum, mw * mh]).T
         ods['em_coupling.mutual_loops_active'] = np.append(rsilec, rsilfc, axis=1)
-        ods['em_coupling.b_field_pol_probes_active'] = np.append(rmp2ec, rmp2fc, axis=1)
-        ods['em_coupling.mutual_plasma_active'] = np.append(gridec, ggridfc, axis=1)
+        ods['em_coupling.field_probes_active'] = np.append(rmp2ec, rmp2fc, axis=1)
+        ods['em_coupling.mutual_grid_active'] = np.append(gridec, ggridfc, axis=1)
         no_ecoil = False
     except Exception:
         ods['em_coupling.mutual_loops_active'] = rsilfc
-        ods['em_coupling.b_field_pol_probes_active'] = rmp2fc
-        ods['em_coupling.mutual_plasma_active'] = ggridfc
+        ods['em_coupling.field_probes_active'] = rmp2fc
+        ods['em_coupling.mutual_grid_active'] = ggridfc
         no_ecoil = True
         printw('Ohmic heating coil tables not available')
 
-    # Response of vessel on flux loops, probes, and plasma
+    # Response of vessel on flux loops, probes, and grid
     try:
         filename = f'rv{nw}{nh}.ddd'
         file = filedir + filename
         f = scipy.io.FortranFile(file, 'r', f'{endian}i4')
         ods['em_coupling.mutual_loops_passive'] = f.read_reals(f'{endian}f8').reshape([nvsum, nsilop]).T
-        ods['em_coupling.b_field_pol_probes_passive'] = f.read_reals(f'{endian}f8').reshape([nvsum, magpri]).T
-        ods['em_coupling.mutual_plasma_passive'] = f.read_reals(f'{endian}f8').reshape([nvsum, mw * mh]).T
+        ods['em_coupling.field_probes_passive'] = f.read_reals(f'{endian}f8').reshape([nvsum, magpri]).T
+        ods['em_coupling.mutual_grid_passive'] = f.read_reals(f'{endian}f8').reshape([nvsum, mw * mh]).T
 
     except Exception:
         printw('Vessel not available')
 
     # Response of coils on vessel
     try:
         gfcvs = f.read_reals(f'{endian}f8').reshape([nvsum, nfsum])
@@ -1832,20 +1797,20 @@
             ods['em_coupling.mutual_passive_active'] = gfcvs
 
         ods['em_coupling.mutual_passive_passive'] = f.read_reals(f'{endian}f8').reshape([nvsum, nvsum])
 
     except Exception:
         printw('Vessel-coil mutual inductances not available')
 
-    # Response of magnetics flux loops and probes on plasma
+    # Response of magnetics flux loops and probes on grid
     filename = f'ep{nw}{nh}.ddd'
     file = filedir + filename
     f = scipy.io.FortranFile(file, 'r', f'{endian}i4')
-    ods['em_coupling.mutual_loops_plasma'] = f.read_reals(f'{endian}f8').reshape([mw * mh, nsilop]).T
-    ods['em_coupling.b_field_pol_probes_plasma'] = f.read_reals(f'{endian}f8').reshape([mw * mh, magpri]).T
+    ods['em_coupling.mutual_loops_grid'] = f.read_reals(f'{endian}f8').reshape([mw * mh, nsilop]).T
+    ods['em_coupling.field_probes_grid'] = f.read_reals(f'{endian}f8').reshape([mw * mh, magpri]).T
     ods['em_coupling.ids_properties.homogeneous_time'] = 2
     ods['em_coupling.code.parameters'] = green
     return ods
 
 
 ############################################
 if '__main__' == __name__:
```

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_elite.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_elite.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_elm.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_elm.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_environment.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_environment.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_eped.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_eped.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_eqdsk.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_eqdsk.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_error.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_error.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_execution_diagram.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_execution_diagram.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_fastran.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_fastran.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_focus.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_focus.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_formatter.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_formatter.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gacode.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gacode.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gaprofiles.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gaprofiles.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gapy.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gapy.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,22 +779,18 @@
             for k, item in enumerate(what):
                 if len(inputaxs):
                     if item in inputaxs:
                         ax = inputaxs[item]
                     else:
                         continue
                 else:
-                    # cplot is used in other calculations so use another variable to cast to int.
-                    # one for rplot is done for consistency
-                    plot_cols = int(cplot)
-                    plot_rows = int(rplot)
                     if k == 0:
-                        ax1 = ax = pyplot.subplot(plot_rows, plot_cols, k + 1)
+                        ax1 = ax = pyplot.subplot(rplot, cplot, k + 1)
                     else:
-                        ax = pyplot.subplot(plot_rows, plot_cols, k + 1, sharex=ax1)
+                        ax = pyplot.subplot(rplot, cplot, k + 1, sharex=ax1)
                 axs[item] = ax
                 r = np.floor(k * 1.0 / cplot)
                 c = k - r * cplot
                 ax.ticklabel_format(style='sci', scilimits=(-3, 3))
                 if 'rho' in self:
                     x = self['rho']
                     ax.set_xlabel('$\\rho$')
@@ -2951,15 +2947,15 @@
         input_tglf['BETAE'] = 8.0 * np.pi * ne * k * Te / bunit**2
         loglam = 24.0 - np.log(np.sqrt(ne) / (Te))
         input_tglf['XNUE'] = a / c_s * np.sqrt(self['IONS'][1][2]) * e**4 * np.pi * ne * loglam / (np.sqrt(me) * (k * Te) ** 1.5)
         input_tglf['ZEFF'] = zeff = self['z_eff']
         rho_s = c_s / (e * np.abs(bunit) / (mi * c))
         input_tglf['DEBYE'] = 7.43e2 * np.sqrt(Te / (ne)) / rho_s
 
-        input_tglf['VEXB_SHEAR'] = self['gamma_e'] * (a / c_s)
+        input_tglf['VEXB_SHEAR'] = -1 * self['gamma_e'] * (a / c_s)
 
         input_tglf['RMIN_LOC'] = self['rmin'] * m_to_cm / a
         input_tglf['RMAJ_LOC'] = self['rmaj'] * m_to_cm / a
         input_tglf['ZMAJ_LOC'] = self['zmag'] * m_to_cm / a
         input_tglf['DRMINDX_LOC'] = 1.0 * one
         input_tglf['DRMAJDX_LOC'] = self['drmaj']
         input_tglf['DZMAJDX_LOC'] = self['dzmag']
```

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gato.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gato.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_genray.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_genray.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gingred.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gingred.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_github.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_github.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gks.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gks.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gnuplot.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gnuplot.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_google_sheet.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_google_sheet.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gpec.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gpec.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_gptools.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_gptools.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_harvest.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_harvest.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_hdf5.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_hdf5.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_helena.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_helena.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_idl.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_idl.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_idlSav.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_idlSav.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_ini.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_ini.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_interface.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_interface.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_ionorb.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_ionorb.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_jscope.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_jscope.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_jsolver.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_jsolver.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_json.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_json.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_kepler.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_kepler.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_latex.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_latex.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_mars.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_mars.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_matlab.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_matlab.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_matrix.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_matrix.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_mds.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_mds.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_mmm.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_mmm.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_namelist.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_namelist.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_nc.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_nc.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_nimrod.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_nimrod.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_oedge.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_oedge.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_omas.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_omas.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_d3d.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_d3d.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_east.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_east.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_kstar.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_kstar.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_omas_utils.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_omas_utils.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_onetwo.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_onetwo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1855,18 +1855,14 @@
                 ods.set_time_array('core_profiles.time', time_index, int(self['time']['data'] * 1000))
                 prof1d = ods['core_profiles.profiles_1d'][time_index]
                 prof1d['grid.psi'] = self['psir_grid']['data']
 
                 prof1d['electrons.density_thermal'] = self['ene']['data']
                 prof1d['electrons.temperature'] = self['Te']['data'] * 1e3
 
-                prof1d['q'] = self['q_value']['data']
-
-                rhon = self['rho_grid']['data'] / max(self['rho_grid']['data'])
-
                 if 'ion' in prof1d:
                     del prof1d['ion']
                 ks_ions = {}  # ks is the ion index used in OMAS
                 kt_ions = {'ip': 0, 'b': 0, 'a': 0}  # kt is the ion index used in the statefile
                 for i in ['p', 'i', 'b', 'a']:
                     for k, ion_name in enumerate(map(lambda x: str(x).strip(), self.get('name' + i, {'data': ['He']})['data'])):
                         ion_name = ion_name[0].upper() + ion_name.lower()[1:]
@@ -1955,15 +1951,14 @@
 
         # ------------------
         # Core sources
         # ------------------
         if 'core_sources' in update:
             ods.set_time_array('core_sources.time', time_index, int(self['time']['data'] * 1000))
             source = ods['core_sources.source']
-            eq = ods['equilibrium.time_slice'][time_index]
             if clear_sources:
                 ods['core_sources.source'].clear()
             volume = self.volume_integral(1)
             ks_source = {}
 
             def add_source(location, identifier, sign, id_index):
                 if identifier in self:  # some terms may not be written by ONETWO in the statefile if the array is all zeros
@@ -1997,49 +1992,52 @@
 
             # momentum kg.m^-1.s^-2
             for identifier, (sign, id_index) in self.volumetric_momentum_terms.items():
                 add_source('momentum_tor', identifier, sign, id_index)
 
             # eq = ods['equilibrium.time_slice'][time_index]
             rho_tor_norm = self['rho_grid']['data'] / max(self['rho_grid']['data'])
-            if 'curbeam' not in ks_source:
-                ks_source['curbeam'] = len(ks_source)
-            ks = ks_source['curbeam']
-            coordsio = {f'core_sources.source.{ks}.profiles_1d.{time_index}.grid.rho_tor_norm': rho_tor_norm}
+            coordsio = {'core_profiles.profiles_1d.%d.grid.rho_tor_norm' % time_index: rho_tor_norm}
             with omas_environment(ods, cocosio=cocosio, coordsio=coordsio):
-                ods['core_sources.vacuum_toroidal_field.r0'] = R0 = ods['equilibrium.vacuum_toroidal_field.r0']
-                ods.set_time_array(
-                    'core_sources.vacuum_toroidal_field.b0', time_index, ods['equilibrium.vacuum_toroidal_field.b0'][time_index]
-                )
-                B0 = ods['core_sources.vacuum_toroidal_field.b0'][time_index]
-
-                rhon = self['rho_grid']['data'] / max(self['rho_grid']['data'])
+                R0 = ods['equilibrium.vacuum_toroidal_field.r0']
+                # ods.set_time_array(
+                #    'core_profiles.vacuum_toroidal_field.b0', time_index, ods['equilibrium.vacuum_toroidal_field.b0'][time_index]
+                # )
+                B0 = ods['equilibrium.vacuum_toroidal_field.b0'][time_index]
+
+                # prof1d['q'] = self['q_value']['data']
+
+            rhon = self['rho_grid']['data'] / max(self['rho_grid']['data'])
+
+            if clear_sources and time_index == 0:
+                # we just append
+                isource = len(ods['core_sources.source'])
+                iisource = isource + 1
+            else:
+                # need to find the actual source index
+                for i in ods['core_sources.source']:
+                    j = int(i)  # make sure we have ints
+                    source_name = ods[f'core_sources.source.{i}.identifier.name']
+                    if source_name == 'curbeam':
+                        isource = j
+                    elif source_name == 'currf':
+                        iisource = j
 
+            for item, value, ii in zip(['curbeam', 'currf'], [2, 3], [isource, iisource]):
                 j_actuator = (1.0 / B0) * transform_current(
-                    rhon, JtoR=self['curbeam']['data'] / R0, equilibrium=eq, includes_bootstrap=False
+                    rhon, JtoR=self[item]['data'] / R0, equilibrium=ods['equilibrium.time_slice'][time_index], includes_bootstrap=False
                 )
-                ods[f'core_sources.source.{ks}.identifier.description'] = 'curbeam'
-                ods[f'core_sources.source.{ks}.identifier.name'] = 'curbeam'
-                ods[f'core_sources.source.{ks}.identifier.index'] = 2
-                ods[f'core_sources.source.{ks}.profiles_1d.{time_index}.grid.volume'] = volume
-                ods[f'core_sources.source.{ks}.profiles_1d.{time_index}.grid.rho_tor_norm'] = rho_tor_norm
-                ods[f'core_sources.source.{ks}.profiles_1d.{time_index}.j_parallel'] = j_actuator
-
-            if 'currf' not in ks_source:
-                ks_source['currf'] = len(ks_source)
-            ks = ks_source['currf']
-            coordsio = {f'core_sources.source.{ks}.profiles_1d.{time_index}.grid.rho_tor_norm': rho_tor_norm}
-            with omas_environment(ods, cocosio=cocosio, coordsio=coordsio):
-                j_actuator = (1.0 / B0) * transform_current(rhon, JtoR=self['currf']['data'] / R0, equilibrium=eq, includes_bootstrap=False)
-                ods[f'core_sources.source.{ks}.profiles_1d.{time_index}.j_parallel'] = j_actuator
-                ods[f'core_sources.source.{ks}.identifier.description'] = 'currf'
-                ods[f'core_sources.source.{ks}.identifier.name'] = 'currf'
-                ods[f'core_sources.source.{ks}.identifier.index'] = 3
-                ods[f'core_sources.source.{ks}.profiles_1d.{time_index}.grid.volume'] = volume
-                ods[f'core_sources.source.{ks}.profiles_1d.{time_index}.grid.rho_tor_norm'] = rho_tor_norm
+                ods[f'core_sources.source.{ii}.profiles_1d.{time_index}.j_parallel'] = j_actuator
+                ods[f'core_sources.source.{ii}.identifier.description'] = item
+                ods[f'core_sources.source.{ii}.identifier.name'] = item
+                ods[f'core_sources.source.{ii}.identifier.index'] = value
+                ods[f'core_sources.source.{ii}.profiles_1d.{time_index}.grid.volume'] = volume
+                ods[f'core_sources.source.{ii}.profiles_1d.{time_index}.grid.rho_tor_norm'] = rho_tor_norm
+
+                isource += 1
 
         # ------------------
         # Plasma currents
         # ------------------
         if 'core_profiles' in update and 'equilibrium' in ods:
             eq = ods['equilibrium.time_slice'][time_index]
             rho_tor_norm = self['rho_grid']['data'] / max(self['rho_grid']['data'])
```

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_osborne.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_osborne.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_patch.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_patch.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_path.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_path.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_pdb.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_pdb.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_profiles.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_profiles.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_python.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_python.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_rabbit.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_rabbit.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_rdb.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_rdb.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_reviewplus.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_reviewplus.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_solps.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_solps.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_spider.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_spider.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_testing.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_testing.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_tglf.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_tglf.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_thomson.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_thomson.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_timcon.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_timcon.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_toksearch.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_toksearch.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_toq.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_toq.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_transp.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_transp.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_trip3d.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_trip3d.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_tsc.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_tsc.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_uda.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_uda.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_uedge.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_uedge.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_ufile.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_ufile.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_weblink.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_weblink.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_xml.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_xml.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/omfit_yaml.py` & `omfit_classes-3.2024.9.2/omfit_classes/omfit_yaml.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/OMFITsave.txt` & `omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/OMFITsave.txt`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/skeleton/NEW_MODULE/help.rst` & `omfit_classes-3.2024.9.2/omfit_classes/skeleton/NEW_MODULE/help.rst`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettings.txt` & `omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettings.txt`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/skeleton/skeletonMainSettingsNamelist.txt` & `omfit_classes-3.2024.9.2/omfit_classes/skeleton/skeletonMainSettingsNamelist.txt`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/sortedDict.py` & `omfit_classes-3.2024.9.2/omfit_classes/sortedDict.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/startup_choice.py` & `omfit_classes-3.2024.9.2/omfit_classes/startup_choice.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/startup_classes.py` & `omfit_classes-3.2024.9.2/omfit_classes/startup_classes.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/startup_framework.py` & `omfit_classes-3.2024.9.2/omfit_classes/startup_framework.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/uedge_common_map.json` & `omfit_classes-3.2024.9.2/omfit_classes/uedge_common_map.json`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/unix_os/setup.py` & `omfit_classes-3.2024.9.2/omfit_classes/unix_os/setup.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/utils_base.py` & `omfit_classes-3.2024.9.2/omfit_classes/utils_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,16 +249,14 @@
             print(f"$OMAS_ROOT: {os.environ['OMAS_ROOT']} does not exist: {msg_submodule}")
     else:
         print(f"$OMAS_ROOT: {os.environ['OMAS_ROOT']}")
         if os.environ['OMAS_ROOT'] in sys.path:
             sys.path.remove(os.environ['OMAS_ROOT'])
         sys.path.insert(0, os.environ['OMAS_ROOT'])
 
-    local_nimpy = os.path.abspath(OMFITsrc + os.sep + '..' + os.sep + "nimpy")
-
 # Keep track of original environment versions before they get modified within OMFIT
 for k in ['PATH', 'LD_LIBRARY_PATH', 'DYLD_LIBRARY_PATH']:
     if f'ORIGINAL_{k}' not in os.environ and k in os.environ:
         os.environ[f'ORIGINAL_{k}'] = os.environ[k]
 # Add directory of python executable to PATH
 if os.path.split(sys.executable)[0] not in os.environ['PATH']:
     os.environ['PATH'] = os.path.split(sys.executable)[0] + os.path.pathsep + os.environ['PATH']
```

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/utils_fit.py` & `omfit_classes-3.2024.9.2/omfit_classes/utils_fit.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/utils_fusion.py` & `omfit_classes-3.2024.9.2/omfit_classes/utils_fusion.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/utils_math.py` & `omfit_classes-3.2024.9.2/omfit_classes/utils_math.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/utils_plot.py` & `omfit_classes-3.2024.9.2/omfit_classes/utils_plot.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes/zdata.py` & `omfit_classes-3.2024.9.2/omfit_classes/zdata.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_classes.egg-info/PKG-INFO` & `omfit_classes-3.2024.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: omfit-classes
-Version: 3.2024.13.2
+Name: omfit_classes
+Version: 3.2024.9.2
 Summary: Classes of OMFIT (One Modeling Framework For Integrated Tasks)
 Home-page: https://omfit.io
 Author: OMFIT developers
 Author-email: meneghini@fusion.gat.com
 License: MIT
 Keywords: integrated modeling plasma framework
 Platform: UNKNOWN
```

### Comparing `omfit_classes-3.2024.13.2/omfit_classes.egg-info/SOURCES.txt` & `omfit_classes-3.2024.9.2/omfit_classes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_gui.py` & `omfit_classes-3.2024.9.2/omfit_gui.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_halt.py` & `omfit_classes-3.2024.9.2/omfit_halt.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_parse_args.py` & `omfit_classes-3.2024.9.2/omfit_parse_args.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_plot.py` & `omfit_classes-3.2024.9.2/omfit_plot.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_setup.py` & `omfit_classes-3.2024.9.2/omfit_setup.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/omfit_tree.py` & `omfit_classes-3.2024.9.2/omfit_tree.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/setup.py` & `omfit_classes-3.2024.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/utils.py` & `omfit_classes-3.2024.9.2/utils.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/utils_tk.py` & `omfit_classes-3.2024.9.2/utils_tk.py`

 * *Files identical despite different names*

### Comparing `omfit_classes-3.2024.13.2/utils_widgets.py` & `omfit_classes-3.2024.9.2/utils_widgets.py`

 * *Files identical despite different names*

