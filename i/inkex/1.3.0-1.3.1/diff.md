# Comparing `tmp/inkex-1.3.0.tar.gz` & `tmp/inkex-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkex-1.3.0.tar", max compression
+gzip compressed data, was "inkex-1.3.1.tar", max compression
```

## Comparing `inkex-1.3.0.tar` & `inkex-1.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    18032 2023-03-15 15:46:27.013869 inkex-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0      884 2023-08-13 14:16:07.123488 inkex-1.3.0/inkex/__init__.py
--rw-r--r--   0        0        0    19663 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/base.py
--rw-r--r--   0        0        0    15498 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/bezier.py
--rw-r--r--   0        0        0    16670 2023-03-15 17:00:43.146686 inkex-1.3.0/inkex/colors.py
--rw-r--r--   0        0        0    11618 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/command.py
--rw-r--r--   0        0        0     1981 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/css.py
--rw-r--r--   0        0        0      116 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated/__init__.py
--rw-r--r--   0        0        0    10027 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated/deprecatedeffect.py
--rw-r--r--   0        0        0     4866 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated/main.py
--rw-r--r--   0        0        0     3429 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/deprecated/meta.py
--rw-r--r--   0        0        0      244 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/README.rst
--rw-r--r--   0        0        0     1924 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/bezmisc.py
--rw-r--r--   0        0        0      963 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/cspsubdiv.py
--rw-r--r--   0        0        0     1426 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/cubicsuperpath.py
--rw-r--r--   0        0        0     2609 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/ffgeom.py
--rwxr-xr-x   0        0        0     2604 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/run_command.py
--rw-r--r--   0        0        0     1656 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/simplepath.py
--rw-r--r--   0        0        0      989 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/simplestyle.py
--rw-r--r--   0        0        0     3042 2023-03-15 15:46:27.093838 inkex-1.3.0/inkex/deprecated-simple/simpletransform.py
--rw-r--r--   0        0        0     1117 2023-03-15 16:46:32.482523 inkex-1.3.0/inkex/elements/__init__.py
--rw-r--r--   0        0        0    29053 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/elements/_base.py
--rw-r--r--   0        0        0    15353 2023-03-15 16:46:32.486524 inkex-1.3.0/inkex/elements/_filters.py
--rw-r--r--   0        0        0     5193 2023-03-15 17:00:43.146686 inkex-1.3.0/inkex/elements/_groups.py
--rw-r--r--   0        0        0      974 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/elements/_image.py
--rw-r--r--   0        0        0    15551 2023-03-15 16:46:32.486524 inkex-1.3.0/inkex/elements/_meta.py
--rw-r--r--   0        0        0     4420 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/elements/_parser.py
--rw-r--r--   0        0        0    17540 2023-03-15 16:46:32.486524 inkex-1.3.0/inkex/elements/_polygons.py
--rw-r--r--   0        0        0     8028 2023-03-15 17:00:43.146686 inkex-1.3.0/inkex/elements/_selected.py
--rw-r--r--   0        0        0    15100 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/elements/_svg.py
--rw-r--r--   0        0        0     6211 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/elements/_text.py
--rw-r--r--   0        0        0     2943 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/elements/_use.py
--rw-r--r--   0        0        0     5300 2023-03-15 16:46:32.494526 inkex-1.3.0/inkex/elements/_utils.py
--rw-r--r--   0        0        0    17991 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/extensions.py
--rw-r--r--   0        0        0      980 2023-03-15 16:46:32.494526 inkex-1.3.0/inkex/gui/README.md
--rw-r--r--   0        0        0     2084 2023-03-15 16:46:32.494526 inkex-1.3.0/inkex/gui/__init__.py
--rw-r--r--   0        0        0     6348 2023-03-15 16:46:32.494526 inkex-1.3.0/inkex/gui/app.py
--rw-r--r--   0        0        0    10714 2023-03-15 17:00:43.146686 inkex-1.3.0/inkex/gui/asyncme.py
--rw-r--r--   0        0        0    18647 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/gui/listview.py
--rw-r--r--   0        0        0    11329 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/gui/pixmap.py
--rw-r--r--   0        0        0     3045 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/gui/tester.py
--rw-r--r--   0        0        0     6634 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/gui/window.py
--rw-r--r--   0        0        0     1006 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/interfaces/IElement.py
--rw-r--r--   0        0        0        0 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/interfaces/__init__.py
--rw-r--r--   0        0        0     8513 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/inx.py
--rw-r--r--   0        0        0     3537 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/localization.py
--rw-r--r--   0        0        0    64456 2023-03-15 17:00:43.146686 inkex-1.3.0/inkex/paths.py
--rw-r--r--   0        0        0     3735 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/ports.py
--rw-r--r--   0        0        0    29117 2023-03-15 16:46:32.498527 inkex-1.3.0/inkex/properties.py
--rw-r--r--   0        0        0    22410 2023-08-13 14:16:07.127490 inkex-1.3.0/inkex/styles.py
--rw-r--r--   0        0        0    17076 2023-03-15 17:00:43.150686 inkex-1.3.0/inkex/tester/__init__.py
--rw-r--r--   0        0        0      263 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/tester/decorators.py
--rw-r--r--   0        0        0     4937 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/tester/filters.py
--rw-r--r--   0        0        0    14903 2023-08-13 14:16:07.131493 inkex-1.3.0/inkex/tester/inkscape.extension.rng
--rw-r--r--   0        0        0      465 2023-03-17 09:52:59.248149 inkex-1.3.0/inkex/tester/inkscape.extension.schema
--rw-r--r--   0        0        0     5871 2023-03-17 09:54:28.772277 inkex-1.3.0/inkex/tester/inx.py
--rw-r--r--   0        0        0    18187 2023-08-13 14:16:07.131493 inkex-1.3.0/inkex/tester/mock.py
--rw-r--r--   0        0        0     1740 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/tester/svg.py
--rw-r--r--   0        0        0     1589 2023-03-17 10:05:35.670311 inkex-1.3.0/inkex/tester/test_inx_file.py
--rw-r--r--   0        0        0      789 2023-03-15 15:46:27.097836 inkex-1.3.0/inkex/tester/word.py
--rw-r--r--   0        0        0     4057 2023-03-15 15:46:27.101835 inkex-1.3.0/inkex/tester/xmldiff.py
--rw-r--r--   0        0        0    40960 2023-03-15 16:46:32.502527 inkex-1.3.0/inkex/transforms.py
--rw-r--r--   0        0        0     7504 2023-03-15 15:46:27.101835 inkex-1.3.0/inkex/turtle.py
--rw-r--r--   0        0        0    32805 2023-08-13 14:16:07.131493 inkex-1.3.0/inkex/tween.py
--rw-r--r--   0        0        0     4416 2023-03-15 15:46:27.101835 inkex-1.3.0/inkex/units.py
--rw-r--r--   0        0        0     7793 2023-03-15 15:46:27.101835 inkex-1.3.0/inkex/utils.py
--rw-r--r--   0        0        0     1363 2023-08-13 14:16:07.139498 inkex-1.3.0/package-readme.md
--rw-r--r--   0        0        0     1745 2023-08-13 14:16:07.143500 inkex-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 inkex-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    18093 2024-04-01 19:53:48.921863 inkex-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      884 2024-04-01 19:53:48.929863 inkex-1.3.1/inkex/__init__.py
+-rw-r--r--   0        0        0    19663 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/base.py
+-rw-r--r--   0        0        0    15498 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/bezier.py
+-rw-r--r--   0        0        0    16670 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/colors.py
+-rw-r--r--   0        0        0    11618 2024-03-31 19:24:55.074060 inkex-1.3.1/inkex/command.py
+-rw-r--r--   0        0        0     1981 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/css.py
+-rw-r--r--   0        0        0      116 2023-03-15 15:46:27.093838 inkex-1.3.1/inkex/deprecated/__init__.py
+-rw-r--r--   0        0        0    10027 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/deprecated/deprecatedeffect.py
+-rw-r--r--   0        0        0     4866 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/deprecated/main.py
+-rw-r--r--   0        0        0     3429 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/deprecated/meta.py
+-rw-r--r--   0        0        0      244 2023-03-15 15:46:27.093838 inkex-1.3.1/inkex/deprecated-simple/README.rst
+-rw-r--r--   0        0        0     1924 2023-03-15 15:46:27.093838 inkex-1.3.1/inkex/deprecated-simple/bezmisc.py
+-rw-r--r--   0        0        0      963 2023-03-15 15:46:27.093838 inkex-1.3.1/inkex/deprecated-simple/cspsubdiv.py
+-rw-r--r--   0        0        0     1426 2023-03-15 15:46:27.093838 inkex-1.3.1/inkex/deprecated-simple/cubicsuperpath.py
+-rw-r--r--   0        0        0     2609 2023-03-15 15:46:27.093838 inkex-1.3.1/inkex/deprecated-simple/ffgeom.py
+-rwxr-xr-x   0        0        0     2604 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/deprecated-simple/run_command.py
+-rw-r--r--   0        0        0     1656 2024-03-30 12:38:08.517431 inkex-1.3.1/inkex/deprecated-simple/simplepath.py
+-rw-r--r--   0        0        0      989 2024-03-30 12:38:08.517431 inkex-1.3.1/inkex/deprecated-simple/simplestyle.py
+-rw-r--r--   0        0        0     3042 2024-03-30 12:38:08.517431 inkex-1.3.1/inkex/deprecated-simple/simpletransform.py
+-rw-r--r--   0        0        0     1117 2023-03-15 16:46:32.482523 inkex-1.3.1/inkex/elements/__init__.py
+-rw-r--r--   0        0        0    29053 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/elements/_base.py
+-rw-r--r--   0        0        0    15353 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/elements/_filters.py
+-rw-r--r--   0        0        0     5193 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/elements/_groups.py
+-rw-r--r--   0        0        0      974 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/elements/_image.py
+-rw-r--r--   0        0        0    15551 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/elements/_meta.py
+-rw-r--r--   0        0        0     4420 2024-04-01 19:45:44.965453 inkex-1.3.1/inkex/elements/_parser.py
+-rw-r--r--   0        0        0    17540 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/elements/_polygons.py
+-rw-r--r--   0        0        0     8028 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/elements/_selected.py
+-rw-r--r--   0        0        0    15100 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/elements/_svg.py
+-rw-r--r--   0        0        0     6211 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/elements/_text.py
+-rw-r--r--   0        0        0     2943 2024-03-31 19:24:55.082056 inkex-1.3.1/inkex/elements/_use.py
+-rw-r--r--   0        0        0     5300 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/elements/_utils.py
+-rw-r--r--   0        0        0    17991 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/extensions.py
+-rw-r--r--   0        0        0      980 2023-03-15 16:46:32.494526 inkex-1.3.1/inkex/gui/README.md
+-rw-r--r--   0        0        0     2084 2023-03-15 16:46:32.494526 inkex-1.3.1/inkex/gui/__init__.py
+-rw-r--r--   0        0        0     6348 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/gui/app.py
+-rw-r--r--   0        0        0    10714 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/gui/asyncme.py
+-rw-r--r--   0        0        0    18647 2024-03-30 12:38:08.517431 inkex-1.3.1/inkex/gui/listview.py
+-rw-r--r--   0        0        0    11329 2024-03-30 12:38:08.521431 inkex-1.3.1/inkex/gui/pixmap.py
+-rw-r--r--   0        0        0     3045 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/gui/tester.py
+-rw-r--r--   0        0        0     6634 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/gui/window.py
+-rw-r--r--   0        0        0     1006 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/interfaces/IElement.py
+-rw-r--r--   0        0        0        0 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/interfaces/__init__.py
+-rw-r--r--   0        0        0     8513 2024-04-01 19:45:44.969452 inkex-1.3.1/inkex/inx.py
+-rw-r--r--   0        0        0     3537 2024-03-30 12:38:08.521431 inkex-1.3.1/inkex/localization.py
+-rw-r--r--   0        0        0    64574 2024-04-01 19:53:48.929863 inkex-1.3.1/inkex/paths.py
+-rw-r--r--   0        0        0     3735 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/ports.py
+-rw-r--r--   0        0        0    29117 2024-04-01 19:45:44.973452 inkex-1.3.1/inkex/properties.py
+-rw-r--r--   0        0        0    22410 2024-04-01 19:45:44.973452 inkex-1.3.1/inkex/styles.py
+-rw-r--r--   0        0        0    17195 2024-04-01 19:53:48.933863 inkex-1.3.1/inkex/tester/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-01 19:45:44.973452 inkex-1.3.1/inkex/tester/decorators.py
+-rw-r--r--   0        0        0     4937 2024-04-01 19:45:44.973452 inkex-1.3.1/inkex/tester/filters.py
+-rw-r--r--   0        0        0    14903 2024-03-31 19:24:55.086053 inkex-1.3.1/inkex/tester/inkscape.extension.rng
+-rw-r--r--   0        0        0      465 2024-03-31 19:24:55.086053 inkex-1.3.1/inkex/tester/inkscape.extension.schema
+-rw-r--r--   0        0        0     6193 2024-04-01 19:53:48.933863 inkex-1.3.1/inkex/tester/inx.py
+-rw-r--r--   0        0        0    18187 2024-04-01 19:45:44.973452 inkex-1.3.1/inkex/tester/mock.py
+-rw-r--r--   0        0        0     1740 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/tester/svg.py
+-rw-r--r--   0        0        0     1589 2024-04-01 19:45:44.977452 inkex-1.3.1/inkex/tester/test_inx_file.py
+-rw-r--r--   0        0        0      789 2023-03-15 15:46:27.097836 inkex-1.3.1/inkex/tester/word.py
+-rw-r--r--   0        0        0     4057 2024-04-01 19:45:44.977452 inkex-1.3.1/inkex/tester/xmldiff.py
+-rw-r--r--   0        0        0    40960 2024-04-01 19:45:44.977452 inkex-1.3.1/inkex/transforms.py
+-rw-r--r--   0        0        0     7504 2024-04-01 19:45:44.977452 inkex-1.3.1/inkex/turtle.py
+-rw-r--r--   0        0        0    32805 2024-04-01 19:45:44.977452 inkex-1.3.1/inkex/tween.py
+-rw-r--r--   0        0        0     4416 2023-03-15 15:46:27.101835 inkex-1.3.1/inkex/units.py
+-rw-r--r--   0        0        0     8040 2024-04-01 19:53:48.933863 inkex-1.3.1/inkex/utils.py
+-rw-r--r--   0        0        0     1363 2024-03-31 19:24:55.098048 inkex-1.3.1/package-readme.md
+-rw-r--r--   0        0        0     1745 2024-04-01 19:53:48.941863 inkex-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 inkex-1.3.1/PKG-INFO
```

### Comparing `inkex-1.3.0/LICENSE.txt` & `inkex-1.3.1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-            GNU GENERAL PUBLIC LICENSE
-               Version 2, June 1991
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 2, June 1991
 
- Copyright (C) 1989, 1991 Free Software Foundation, Inc.
-     59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
+ Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
+ 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
-                Preamble
+                            Preamble
 
   The licenses for most software are designed to take away your
 freedom to share and change it.  By contrast, the GNU General Public
 License is intended to guarantee your freedom to share and change free
 software--to make sure the software is free for all its users.  This
 General Public License applies to most of the Free Software
 Foundation's software and to any other program whose authors commit to
 using it.  (Some other Free Software Foundation software is covered by
-the GNU Library General Public License instead.)  You can apply it to
+the GNU Lesser General Public License instead.)  You can apply it to
 your programs, too.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 this service if you wish), that you receive source code or can get it
 if you want it, that you can change the software or use pieces of it
@@ -52,15 +52,15 @@
 program will individually obtain patent licenses, in effect making the
 program proprietary.  To prevent this, we have made it clear that any
 patent must be licensed for everyone's free use or not licensed at all.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
-            GNU GENERAL PUBLIC LICENSE
+                    GNU GENERAL PUBLIC LICENSE
    TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
 
   0. This License applies to any program or other work which contains
 a notice placed by the copyright holder saying it may be distributed
 under the terms of this General Public License.  The "Program", below,
 refers to any such program or work, and a "work based on the Program"
 means either the Program or any derivative work under copyright law:
@@ -251,15 +251,15 @@
 programs whose distribution conditions are different, write to the author
 to ask for permission.  For software which is copyrighted by the Free
 Software Foundation, write to the Free Software Foundation; we sometimes
 make exceptions for this.  Our decision will be guided by the two goals
 of preserving the free status of all derivatives of our free software and
 of promoting the sharing and reuse of software generally.
 
-                NO WARRANTY
+                            NO WARRANTY
 
   11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
 FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
 OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
 PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
 OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
 MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
@@ -273,17 +273,17 @@
 INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
 OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
 TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
 YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
 PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGES.
 
-             END OF TERMS AND CONDITIONS
+                     END OF TERMS AND CONDITIONS
 
-        How to Apply These Terms to Your New Programs
+            How to Apply These Terms to Your New Programs
 
   If you develop a new program, and you want it to be of the greatest
 possible use to the public, the best way to achieve this is to make it
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
@@ -299,25 +299,24 @@
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program; if not, write to the Free Software
-    Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
-
+    You should have received a copy of the GNU General Public License along
+    with this program; if not, write to the Free Software Foundation, Inc.,
+    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 Also add information on how to contact you by electronic and paper mail.
 
 If the program is interactive, make it output a short notice like this
 when it starts in an interactive mode:
 
-    Gnomovision version 69, Copyright (C) year  name of author
+    Gnomovision version 69, Copyright (C) year name of author
     Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, the commands you use may
 be called something other than `show w' and `show c'; they could even be
@@ -332,9 +331,10 @@
 
   <signature of Ty Coon>, 1 April 1989
   Ty Coon, President of Vice
 
 This General Public License does not permit incorporating your program into
 proprietary programs.  If your program is a subroutine library, you may
 consider it more useful to permit linking proprietary applications with the
-library.  If this is what you want to do, use the GNU Library General
+library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.
+
```

### Comparing `inkex-1.3.0/inkex/__init__.py` & `inkex-1.3.1/inkex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 from .deprecated import are_near_relative
 from .deprecated import unittouu
 
 MIN_VERSION = (3, 7)
 if sys.version_info < MIN_VERSION:
     sys.exit("Inkscape extensions require Python 3.7 or greater.")
 
-__version__ = "1.3.0"  # Version number for inkex; may differ from Inkscape version.
+__version__ = "1.3.1"  # Version number for inkex; may differ from Inkscape version.
```

### Comparing `inkex-1.3.0/inkex/base.py` & `inkex-1.3.1/inkex/base.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/bezier.py` & `inkex-1.3.1/inkex/bezier.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/colors.py` & `inkex-1.3.1/inkex/colors.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/command.py` & `inkex-1.3.1/inkex/command.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/css.py` & `inkex-1.3.1/inkex/css.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated/deprecatedeffect.py` & `inkex-1.3.1/inkex/deprecated/deprecatedeffect.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated/main.py` & `inkex-1.3.1/inkex/deprecated/main.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated/meta.py` & `inkex-1.3.1/inkex/deprecated/meta.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/bezmisc.py` & `inkex-1.3.1/inkex/deprecated-simple/bezmisc.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/cspsubdiv.py` & `inkex-1.3.1/inkex/deprecated-simple/cspsubdiv.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/cubicsuperpath.py` & `inkex-1.3.1/inkex/deprecated-simple/cubicsuperpath.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/ffgeom.py` & `inkex-1.3.1/inkex/deprecated-simple/ffgeom.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/run_command.py` & `inkex-1.3.1/inkex/deprecated-simple/run_command.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/simplepath.py` & `inkex-1.3.1/inkex/deprecated-simple/simplepath.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/simplestyle.py` & `inkex-1.3.1/inkex/deprecated-simple/simplestyle.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/deprecated-simple/simpletransform.py` & `inkex-1.3.1/inkex/deprecated-simple/simpletransform.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/__init__.py` & `inkex-1.3.1/inkex/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_base.py` & `inkex-1.3.1/inkex/elements/_base.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_filters.py` & `inkex-1.3.1/inkex/elements/_filters.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_groups.py` & `inkex-1.3.1/inkex/elements/_groups.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_image.py` & `inkex-1.3.1/inkex/elements/_image.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_meta.py` & `inkex-1.3.1/inkex/elements/_meta.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_parser.py` & `inkex-1.3.1/inkex/elements/_parser.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_polygons.py` & `inkex-1.3.1/inkex/elements/_polygons.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_selected.py` & `inkex-1.3.1/inkex/elements/_selected.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_svg.py` & `inkex-1.3.1/inkex/elements/_svg.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_text.py` & `inkex-1.3.1/inkex/elements/_text.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_use.py` & `inkex-1.3.1/inkex/elements/_use.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/elements/_utils.py` & `inkex-1.3.1/inkex/elements/_utils.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/extensions.py` & `inkex-1.3.1/inkex/extensions.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/README.md` & `inkex-1.3.1/inkex/gui/README.md`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/__init__.py` & `inkex-1.3.1/inkex/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/app.py` & `inkex-1.3.1/inkex/gui/app.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/asyncme.py` & `inkex-1.3.1/inkex/gui/asyncme.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/listview.py` & `inkex-1.3.1/inkex/gui/listview.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/pixmap.py` & `inkex-1.3.1/inkex/gui/pixmap.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/tester.py` & `inkex-1.3.1/inkex/gui/tester.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/gui/window.py` & `inkex-1.3.1/inkex/gui/window.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/interfaces/IElement.py` & `inkex-1.3.1/inkex/interfaces/IElement.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/inx.py` & `inkex-1.3.1/inkex/inx.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/localization.py` & `inkex-1.3.1/inkex/localization.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/paths.py` & `inkex-1.3.1/inkex/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1350,15 +1350,18 @@
         for item in path_d or ():
             if isinstance(item, PathCommand):
                 self.append(item)
             elif isinstance(item, (list, tuple)) and len(item) == 2:
                 if isinstance(item[1], (list, tuple)):
                     self.append(PathCommand.letter_to_class(item[0])(*item[1]))
                 else:
-                    self.append(Line(*item))
+                    if len(self) == 0:
+                        self.append(Move(*item))
+                    else:
+                        self.append(Line(*item))
             else:
                 raise TypeError(
                     f"Bad path type: {type(path_d).__name__}"
                     f"({type(item).__name__}, ...): {item}"
                 )
 
     @classmethod
```

### Comparing `inkex-1.3.0/inkex/ports.py` & `inkex-1.3.1/inkex/ports.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/properties.py` & `inkex-1.3.1/inkex/properties.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/styles.py` & `inkex-1.3.1/inkex/styles.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tester/__init__.py` & `inkex-1.3.1/inkex/tester/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,27 +374,31 @@
             with open(cmpfile, "rb") as fhl:
                 data_b = self._apply_compare_filters(fhl.read(), False)
             self._base_compare(data_a, data_b, compare_mode)
         except AssertionError:
             if write_output:
                 if isinstance(data_a, str):
                     data_a = data_a.encode("utf-8")
-                with open(write_output, "wb") as fhl:
-                    fhl.write(self._apply_compare_filters(data_a, True))
-                    print(f"Written output: {write_output}")
+                self.write_compare_data(infile, write_output, data_a)
                 # This only reruns if the original test failed.
                 # The idea here is to make sure the new output file is "stable"
                 # Because some tests can produce random changes and we don't
                 # want test authors to be too reassured by a simple write.
                 if write_output == cmpfile:
                     effect = self.assertEffect(infile, args=args)
                     self._base_compare(data_a, cmpfile, COMPARE_CHECK)
             if not write_output == cmpfile:
                 raise
 
+    def write_compare_data(self, infile, outfile, data):
+        """Write output"""
+        with open(outfile, "wb") as fhl:
+            fhl.write(self._apply_compare_filters(data, True))
+            print(f"Written output: {outfile}")
+
     def _base_compare(self, data_a, data_b, compare_mode):
         data_a = self._apply_compare_filters(data_a)
 
         if (
             isinstance(data_a, bytes)
             and isinstance(data_b, bytes)
             and data_a.startswith(b"<")
```

### Comparing `inkex-1.3.0/inkex/tester/filters.py` & `inkex-1.3.1/inkex/tester/filters.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tester/inkscape.extension.rng` & `inkex-1.3.1/inkex/tester/inkscape.extension.rng`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tester/inx.py` & `inkex-1.3.1/inkex/tester/inx.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,20 @@
                     # skip color, method types
                     continue
                 self.assertEqual(
                     argsdefault,
                     inxdefault,
                     f"Default value is not the same for {inx.filename}:param:{param}",
                 )
+            inxchoices = params[param]["choices"]
+            argschoices = args[param]["choices"]
+            if argschoices is not None and len(argschoices) > 0:
+                assert set(inxchoices).issubset(
+                    argschoices
+                ), f"params don't match: inx={inxchoices}, py={argschoices}"
 
     def introspect_arg_parser(self, arg_parser):
         """Pull apart the arg parser to find out what we have in it"""
         for (
             action
         ) in arg_parser._optionals._actions:  # pylint: disable=protected-access
             for opt in action.option_strings:
```

### Comparing `inkex-1.3.0/inkex/tester/mock.py` & `inkex-1.3.1/inkex/tester/mock.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tester/svg.py` & `inkex-1.3.1/inkex/tester/svg.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tester/test_inx_file.py` & `inkex-1.3.1/inkex/tester/test_inx_file.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tester/word.py` & `inkex-1.3.1/inkex/tester/word.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tester/xmldiff.py` & `inkex-1.3.1/inkex/tester/xmldiff.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/transforms.py` & `inkex-1.3.1/inkex/transforms.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/turtle.py` & `inkex-1.3.1/inkex/turtle.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/tween.py` & `inkex-1.3.1/inkex/tween.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/units.py` & `inkex-1.3.1/inkex/units.py`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/inkex/utils.py` & `inkex-1.3.1/inkex/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 import os
 import sys
 import random
 import re
 import math
 from argparse import ArgumentTypeError
-from itertools import tee
+from itertools import tee, cycle
 
 ABORT_STATUS = -5
 
 (X, Y) = range(2)
 PY3 = sys.version_info[0] == 3
 
 # pylint: disable=line-too-long
@@ -232,14 +232,24 @@
     first, then = tee(iterable)
     starter = [(None, next(then, None))]
     if not start:
         starter = []
     return starter + list(zip(first, then))
 
 
+def circular_pairwise(l):
+    """Iterate over a list with overlapping pairs in a periodic way, i.e.
+    [1, 2, 3] -> [(1, 2), (2, 3), (3, 1)]
+
+    ..versionadded:: 1.3.1"""
+    second = cycle(l)
+    next(second)
+    return zip(l, second)
+
+
 EVAL_GLOBALS = {}
 EVAL_GLOBALS.update(random.__dict__)
 EVAL_GLOBALS.update(math.__dict__)
 
 
 def math_eval(function, variable="x"):
     """Interpret a function string. All functions from math and random may be used.
```

### Comparing `inkex-1.3.0/package-readme.md` & `inkex-1.3.1/package-readme.md`

 * *Files identical despite different names*

### Comparing `inkex-1.3.0/pyproject.toml` & `inkex-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inkex"
-version = "1.3.0"
+version = "1.3.1"
 description = "Python extensions for Inkscape core, separated out from main repository."
 authors = ["Inkscape Authors <inkscape-devel@lists.inkscape.org>"]
 maintainers = [
     "Martin Owens <doctormo@geek-2.com>",
     "Jonathan Neuhauser <jonathan.neuhauser@outlook.com>",
 ]
 license = "GPL-2.0-or-later"
```

### Comparing `inkex-1.3.0/PKG-INFO` & `inkex-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkex
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python extensions for Inkscape core, separated out from main repository.
 Home-page: https://gitlab.com/inkscape/extensions
 License: GPL-2.0-or-later
 Keywords: extensions,graphics,inkscape,svg,vector
 Author: Inkscape Authors
 Author-email: inkscape-devel@lists.inkscape.org
 Maintainer: Martin Owens
```

