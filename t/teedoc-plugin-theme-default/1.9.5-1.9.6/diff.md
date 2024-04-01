# Comparing `tmp/teedoc-plugin-theme-default-1.9.5.tar.gz` & `tmp/teedoc-plugin-theme-default-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/teedoc-plugin-theme-default-1.9.5.tar", last modified: Wed Aug 18 02:28:57 2021, max compression
+gzip compressed data, was "dist/teedoc-plugin-theme-default-1.9.6.tar", last modified: Thu Aug 19 02:55:52 2021, max compression
```

## Comparing `teedoc-plugin-theme-default-1.9.5.tar` & `teedoc-plugin-theme-default-1.9.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      643 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/PKG-INFO
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      104 2021-01-23 03:07:39.000000 teedoc-plugin-theme-default-1.9.5/README.md
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)       38 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/setup.cfg
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3103 2021-08-18 02:28:45.000000 teedoc-plugin-theme-default-1.9.5/setup.py
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     8950 2021-08-13 06:21:37.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/__init__.py
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2027 2021-06-01 03:06:27.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/dark.css
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2317 2021-01-27 08:26:37.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/dark_mode.svg
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      780 2021-01-23 08:45:18.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/indicator.svg
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)    89476 2021-01-23 08:56:16.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/jquery.min.js
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)    21662 2021-08-05 08:33:17.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/light.css
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1587 2021-01-27 08:12:53.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/light_mode.svg
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     7537 2021-08-17 12:08:08.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/main.js
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      609 2021-01-26 09:51:53.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/menu.svg
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1423 2021-01-30 01:33:52.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/pre_main.js
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     5139 2021-03-01 08:29:58.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/prism.min.css
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)    94443 2021-03-01 08:30:02.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/prism.min.js
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     6658 2021-05-28 09:40:28.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/split.js
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      836 2021-01-27 07:13:26.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/to-top.svg
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)    11511 2021-08-18 02:24:47.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/tocbot.min.js
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     8168 2021-07-22 02:10:22.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/viewer.min.css
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)    36574 2021-07-22 02:10:22.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/viewer.min.js
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/templates/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     4700 2021-08-16 03:30:38.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/templates/article.html
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1960 2021-08-09 09:03:52.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/templates/page.html
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default.egg-info/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      643 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default.egg-info/PKG-INFO
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1116 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default.egg-info/SOURCES.txt
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)        1 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default.egg-info/dependency_links.txt
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)       28 2021-08-18 02:28:57.000000 teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default.egg-info/top_level.txt
+drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-19 02:55:52.000000 teedoc-plugin-theme-default-1.9.6/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      643 2021-08-19 02:55:52.000000 teedoc-plugin-theme-default-1.9.6/PKG-INFO
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      104 2021-01-23 03:07:39.000000 teedoc-plugin-theme-default-1.9.6/README.md
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)       38 2021-08-19 02:55:52.000000 teedoc-plugin-theme-default-1.9.6/setup.cfg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3103 2021-08-19 02:54:52.000000 teedoc-plugin-theme-default-1.9.6/setup.py
+drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-19 02:55:52.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     8950 2021-08-13 06:21:37.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/__init__.py
+drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-19 02:55:52.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2027 2021-06-01 03:06:27.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/dark.css
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2317 2021-01-27 08:26:37.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/dark_mode.svg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      780 2021-01-23 08:45:18.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/indicator.svg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    89476 2021-01-23 08:56:16.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/jquery.min.js
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    21973 2021-08-19 02:28:51.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/light.css
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1587 2021-01-27 08:12:53.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/light_mode.svg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     7698 2021-08-19 02:43:14.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/main.js
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      609 2021-01-26 09:51:53.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/menu.svg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1423 2021-01-30 01:33:52.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/pre_main.js
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     5139 2021-03-01 08:29:58.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/prism.min.css
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    94443 2021-03-01 08:30:02.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/prism.min.js
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     6658 2021-05-28 09:40:28.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/split.js
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      836 2021-01-27 07:13:26.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/to-top.svg
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    11511 2021-08-18 02:24:47.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/tocbot.min.js
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     8168 2021-07-22 02:10:22.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/viewer.min.css
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)    36574 2021-07-22 02:10:22.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/viewer.min.js
+drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-19 02:55:52.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/templates/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     4641 2021-08-19 02:29:04.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/templates/article.html
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1960 2021-08-09 09:03:52.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/templates/page.html
+drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-08-19 02:55:52.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default.egg-info/
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)      643 2021-08-19 02:55:51.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default.egg-info/PKG-INFO
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1116 2021-08-19 02:55:51.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default.egg-info/SOURCES.txt
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)        1 2021-08-19 02:55:51.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default.egg-info/dependency_links.txt
+-rw-r--r--   0 neucrack  (1000) neucrack  (1000)       28 2021-08-19 02:55:51.000000 teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default.egg-info/top_level.txt
```

### Comparing `teedoc-plugin-theme-default-1.9.5/PKG-INFO` & `teedoc-plugin-theme-default-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teedoc-plugin-theme-default
-Version: 1.9.5
+Version: 1.9.6
 Summary: default theme for teedoc
 Home-page: https://github.com/Neutree/teedoc
 Author: Neucrack
 Author-email: CZD666666@gmail.com
 License: MIT
 Description: teedoc-plugin-theme-default
         ===========
```

### Comparing `teedoc-plugin-theme-default-1.9.5/setup.py` & `teedoc-plugin-theme-default-1.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requires = []
 packages = find_packages()
 print("packages:", packages)
 
 setup(
     name='teedoc-plugin-theme-default',
-    version="1.9.5",
+    version="1.9.6",
     author='Neucrack',
     author_email='CZD666666@gmail.com',
 
     description='default theme for teedoc',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Neutree/teedoc',
```

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/__init__.py` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/__init__.py`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/dark.css` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/dark.css`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/dark_mode.svg` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/dark_mode.svg`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/indicator.svg` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/indicator.svg`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/jquery.min.js` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/jquery.min.js`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/light.css` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/light.css`

 * *Files 0% similar despite different names*

```diff
@@ -221,21 +221,30 @@
 
 
 /* sidebar */
 #sidebar_wrapper {
     width: 300px;
 }
 /* sidebar splitter */
+.gutter_icon {
+    background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAeCAYAAADkftS9AAAAIklEQVQoU2M4c+bMfxAGAgYYmwGrIIiDjrELjpo5aiZeMwF+yNnOs5KSvgAAAABJRU5ErkJggg==);
+    width: 3px;
+    height: 2em;
+    background-repeat: no-repeat;
+    position: fixed;
+    top: 50%;
+}
 .gutter {
     background-color: #eee;
     background-repeat: no-repeat;
     background-position: 50%;
     transition: 0.2s;
     border-radius: 5px;
     display: block;
+    z-index: 99;
 }
 
 .gutter.gutter-horizontal {
     /* background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAeCAYAAADkftS9AAAAIklEQVQoU2M4c+bMfxAGAgYYmwGrIIiDjrELjpo5aiZeMwF+yNnOs5KSvgAAAABJRU5ErkJggg=='); */
     cursor: col-resize;
 }
```

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/light_mode.svg` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/light_mode.svg`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/main.js` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/main.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -165,15 +165,15 @@
     localStorage.setItem("splitter_w", JSON.stringify(sizes));
 }
 
 var hasSplitter = false;
 
 function createSplitter() {
     var split = Split(["#sidebar_wrapper", "#article"], {
-        gutterSize: 10,
+        gutterSize: 3,
         gutterAlign: 'start',
         minSize: 200,
         elementStyle: function(dimension, size, gutterSize) {
             return {
                 'width': 'calc(' + size + '% - ' + gutterSize + 'px)',
             }
         },
@@ -189,18 +189,21 @@
         if (!sidebar_width_is_percent) {
             split_w = parseInt(sidebar_width / screenW * 100);
         } else {
             split_w = sidebar_width;
         }
     }
     split.setSizes([split_w, 100 - split_w]);
+    $(".gutter").append('<div class="gutter_icon"></div>');
     $(".gutter").hover(function() {
-        $(".gutter").css("width", "18px");
-    }, function() {
         $(".gutter").css("width", "10px");
+        $(".gutter_icon").css("width", "10px");
+    }, function() {
+        $(".gutter").css("width", "3px");
+        $(".gutter_icon").css("width", "3px");
     });
 }
 
 function addSplitter() {
     var screenW = $(window).width();
     if (screenW > 900) {
         createSplitter();
```

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/menu.svg` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/menu.svg`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/pre_main.js` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/pre_main.js`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/prism.min.css` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/prism.min.css`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/prism.min.js` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/prism.min.js`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/split.js` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/split.js`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/to-top.svg` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/to-top.svg`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/tocbot.min.js` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/tocbot.min.js`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/viewer.min.css` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/viewer.min.css`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/assets/viewer.min.js` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/assets/viewer.min.js`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/templates/article.html` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/templates/article.html`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,14 @@
         <div id="sidebar_wrapper">
             <div id="sidebar">
                 <div id="sidebar_title">
                     {{ sidebar_title|safe }}
                 </div>
                 {{ sidebar_items_html|safe }}
             </div>
-            <div id="sidebar_splitter">
-            </div>
         </div>
         <div id="article">
             <div id="menu_wrapper">
                 <div id="menu">
                 </div>
             </div>
             <div id="content_wrapper">
```

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default/templates/page.html` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default/templates/page.html`

 * *Files identical despite different names*

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default.egg-info/PKG-INFO` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teedoc-plugin-theme-default
-Version: 1.9.5
+Version: 1.9.6
 Summary: default theme for teedoc
 Home-page: https://github.com/Neutree/teedoc
 Author: Neucrack
 Author-email: CZD666666@gmail.com
 License: MIT
 Description: teedoc-plugin-theme-default
         ===========
```

### Comparing `teedoc-plugin-theme-default-1.9.5/teedoc_plugin_theme_default.egg-info/SOURCES.txt` & `teedoc-plugin-theme-default-1.9.6/teedoc_plugin_theme_default.egg-info/SOURCES.txt`

 * *Files identical despite different names*

