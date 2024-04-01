# Comparing `tmp/histomicsui-1.5.1.dev6.tar.gz` & `tmp/histomicsui-1.5.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicsui-1.5.1.dev6.tar", last modified: Thu Feb 22 18:40:29 2024, max compression
+gzip compressed data, was "histomicsui-1.5.1.dev8.tar", last modified: Wed Mar 27 16:29:28 2024, max compression
```

## Comparing `histomicsui-1.5.1.dev6.tar` & `histomicsui-1.5.1.dev8.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.246603 histomicsui-1.5.1.dev6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.218603 histomicsui-1.5.1.dev6/.circleci/
--rw-r--r--   0 root         (0) root         (0)     3886 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      617 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/.git-blame-ignore-revs
--rw-r--r--   0 root         (0) root         (0)      531 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2200 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    10173 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      585 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7783 2024-02-22 18:40:29.246603 histomicsui-1.5.1.dev6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6730 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/README.rst
--rw-r--r--   0 root         (0) root         (0)      460 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.218603 histomicsui-1.5.1.dev6/docs/
--rw-r--r--   0 root         (0) root         (0)     4258 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/docs/config_options.rst
--rw-r--r--   0 root         (0) root         (0)     7012 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/docs/controls.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.222603 histomicsui-1.5.1.dev6/docs/images/
--rwxr-xr-x   0 root         (0) root         (0)   133796 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/docs/images/difference.gif
--rwxr-xr-x   0 root         (0) root         (0)   133603 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/docs/images/intersect.gif
--rwxr-xr-x   0 root         (0) root         (0)   154141 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/docs/images/union.gif
--rwxr-xr-x   0 root         (0) root         (0)   168255 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/docs/images/xor.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.222603 histomicsui-1.5.1.dev6/histomicsui/
--rw-r--r--   0 root         (0) root         (0)    19497 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/constants.py
--rw-r--r--   0 root         (0) root         (0)    13678 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.222603 histomicsui-1.5.1.dev6/histomicsui/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3329 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/aperio.py
--rw-r--r--   0 root         (0) root         (0)     1927 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/case.py
--rw-r--r--   0 root         (0) root         (0)     1081 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/cohort.py
--rw-r--r--   0 root         (0) root         (0)     2923 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/image.py
--rw-r--r--   0 root         (0) root         (0)     8576 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/meta.py
--rw-r--r--   0 root         (0) root         (0)      838 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/pathology.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/models/slide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.226603 histomicsui-1.5.1.dev6/histomicsui/rest/
--rw-r--r--   0 root         (0) root         (0)      512 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3739 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/rest/aperio.py
--rw-r--r--   0 root         (0) root         (0)     9366 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/rest/hui_resource.py
--rw-r--r--   0 root         (0) root         (0)     4609 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/rest/image_browse_resource.py
--rw-r--r--   0 root         (0) root         (0)    17402 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/rest/system.py
--rw-r--r--   0 root         (0) root         (0)    29274 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/rest/tcga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.226603 histomicsui-1.5.1.dev6/histomicsui/web_client/
--rw-r--r--   0 root         (0) root         (0)     2903 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.226603 histomicsui-1.5.1.dev6/histomicsui/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)      382 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/collections/StyleCollection.js
--rw-r--r--   0 root         (0) root         (0)      405 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/collections/UserCollection.js
--rw-r--r--   0 root         (0) root         (0)      149 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/collections/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.226603 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/
--rw-r--r--   0 root         (0) root         (0)     1326 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/confirmDialog.js
--rw-r--r--   0 root         (0) root         (0)     3936 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/editElement.js
--rw-r--r--   0 root         (0) root         (0)     6663 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/editRegionOfInterest.js
--rw-r--r--   0 root         (0) root         (0)    11216 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/editStyleGroups.js
--rw-r--r--   0 root         (0) root         (0)      478 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/index.js
--rw-r--r--   0 root         (0) root         (0)     1153 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/metadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     4936 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/openAnnotatedImage.js
--rw-r--r--   0 root         (0) root         (0)     2588 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/openImage.js
--rw-r--r--   0 root         (0) root         (0)    23122 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/saveAnnotation.js
--rw-r--r--   0 root         (0) root         (0)       78 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      391 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      858 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.226603 histomicsui-1.5.1.dev6/histomicsui/web_client/models/
--rw-r--r--   0 root         (0) root         (0)      221 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/models/StyleModel.js
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     3738 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.230603 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/
--rw-r--r--   0 root         (0) root         (0)    25133 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/AnnotationSelector.js
--rw-r--r--   0 root         (0) root         (0)    43673 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/DrawWidget.js
--rw-r--r--   0 root         (0) root         (0)     1943 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/FrameSelectorWidget.js
--rw-r--r--   0 root         (0) root         (0)    14204 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/MetadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     5287 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/MetadataWidget.js
--rw-r--r--   0 root         (0) root         (0)     8115 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/OverviewWidget.js
--rw-r--r--   0 root         (0) root         (0)     1121 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/RegionSelector.js
--rw-r--r--   0 root         (0) root         (0)     9946 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/ZoomWidget.js
--rw-r--r--   0 root         (0) root         (0)      146 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/panels/index.js
--rw-r--r--   0 root         (0) root         (0)     1485 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/router.js
--rw-r--r--   0 root         (0) root         (0)      292 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.230603 histomicsui-1.5.1.dev6/histomicsui/web_client/static/
--rwxr-xr-x   0 root         (0) root         (0)     5072 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/static/favicon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.214603 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.230603 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/body/
--rw-r--r--   0 root         (0) root         (0)      504 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/body/configView.styl
--rw-r--r--   0 root         (0) root         (0)     1258 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/body/image.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.230603 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/dialogs/
--rw-r--r--   0 root         (0) root         (0)      195 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
--rw-r--r--   0 root         (0) root         (0)      237 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
--rw-r--r--   0 root         (0) root         (0)      849 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.230603 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/layout/
--rw-r--r--   0 root         (0) root         (0)      986 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/layout/header.styl
--rw-r--r--   0 root         (0) root         (0)       53 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
--rw-r--r--   0 root         (0) root         (0)      151 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/layout/headerImage.styl
--rw-r--r--   0 root         (0) root         (0)     2189 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/layout/layout.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.230603 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/
--rw-r--r--   0 root         (0) root         (0)     1671 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
--rw-r--r--   0 root         (0) root         (0)     2651 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/drawWidget.styl
--rw-r--r--   0 root         (0) root         (0)     1700 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
--rw-r--r--   0 root         (0) root         (0)      430 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
--rw-r--r--   0 root         (0) root         (0)      929 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
--rw-r--r--   0 root         (0) root         (0)       81 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/regionSelector.styl
--rw-r--r--   0 root         (0) root         (0)      878 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.234603 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/popover/
--rw-r--r--   0 root         (0) root         (0)      113 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
--rw-r--r--   0 root         (0) root         (0)     1668 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.234603 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/views/
--rw-r--r--   0 root         (0) root         (0)      222 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/views/itemList.styl
--rw-r--r--   0 root         (0) root         (0)      139 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/views/searchResultsView.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.218603 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.234603 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/body/
--rw-r--r--   0 root         (0) root         (0)     5608 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/body/configView.pug
--rw-r--r--   0 root         (0) root         (0)      783 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/body/image.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.234603 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/
--rw-r--r--   0 root         (0) root         (0)      501 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
--rw-r--r--   0 root         (0) root         (0)      428 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/confirmDialog.pug
--rw-r--r--   0 root         (0) root         (0)     2079 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/editElement.pug
--rw-r--r--   0 root         (0) root         (0)     1730 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
--rw-r--r--   0 root         (0) root         (0)     3201 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
--rw-r--r--   0 root         (0) root         (0)     1541 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      838 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
--rw-r--r--   0 root         (0) root         (0)      353 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/openImage.pug
--rw-r--r--   0 root         (0) root         (0)     5720 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.234603 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/
--rw-r--r--   0 root         (0) root         (0)      925 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/header.pug
--rw-r--r--   0 root         (0) root         (0)      865 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/headerAnalyses.pug
--rw-r--r--   0 root         (0) root         (0)     1467 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/headerImage.pug
--rw-r--r--   0 root         (0) root         (0)      641 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/headerUser.pug
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/layout.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.238603 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/
--rw-r--r--   0 root         (0) root         (0)     3947 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/annotationSelector.pug
--rw-r--r--   0 root         (0) root         (0)     5685 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/drawWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2197 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/drawWidgetElement.pug
--rw-r--r--   0 root         (0) root         (0)      116 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/frameSelectorWidget.pug
--rw-r--r--   0 root         (0) root         (0)      347 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      420 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/metadataWidgetPanel.pug
--rw-r--r--   0 root         (0) root         (0)      102 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/overviewWidget.pug
--rw-r--r--   0 root         (0) root         (0)      398 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/panel.pug
--rw-r--r--   0 root         (0) root         (0)      345 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/regionSelector.pug
--rw-r--r--   0 root         (0) root         (0)     1281 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/zoomWidget.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.238603 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/popover/
--rw-r--r--   0 root         (0) root         (0)      576 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/popover/annotationContextMenu.pug
--rw-r--r--   0 root         (0) root         (0)     1874 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/popover/annotationPopover.pug
--rw-r--r--   0 root         (0) root         (0)      427 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/popover/annotationPopoverMetadata.pug
--rw-r--r--   0 root         (0) root         (0)      204 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.238603 histomicsui-1.5.1.dev6/histomicsui/web_client/views/
--rw-r--r--   0 root         (0) root         (0)      525 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/HierarchyWidget.js
--rw-r--r--   0 root         (0) root         (0)      904 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/JobDetailsWidget.js
--rw-r--r--   0 root         (0) root         (0)     2041 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/View.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.242603 histomicsui-1.5.1.dev6/histomicsui/web_client/views/body/
--rw-r--r--   0 root         (0) root         (0)     7205 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/body/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)    71097 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/body/ImageView.js
--rw-r--r--   0 root         (0) root         (0)      119 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/body/index.js
--rw-r--r--   0 root         (0) root         (0)      190 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)     3436 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/itemList.js
--rw-r--r--   0 root         (0) root         (0)     2375 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/itemPage.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.242603 histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/
--rw-r--r--   0 root         (0) root         (0)     1658 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/HeaderAnalysesView.js
--rw-r--r--   0 root         (0) root         (0)     2861 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/HeaderImageView.js
--rw-r--r--   0 root         (0) root         (0)      421 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/HeaderUserView.js
--rw-r--r--   0 root         (0) root         (0)     1621 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/HeaderView.js
--rw-r--r--   0 root         (0) root         (0)      134 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.242603 histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/
--rw-r--r--   0 root         (0) root         (0)     4506 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/AnnotationContextMenu.js
--rw-r--r--   0 root         (0) root         (0)    11614 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/AnnotationPopover.js
--rw-r--r--   0 root         (0) root         (0)     1231 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/PixelmapContextMenu.js
--rw-r--r--   0 root         (0) root         (0)      176 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/index.js
--rw-r--r--   0 root         (0) root         (0)     1474 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/searchResultsView.js
--rw-r--r--   0 root         (0) root         (0)     2847 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/views/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.218603 histomicsui-1.5.1.dev6/histomicsui/web_client/vue/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.242603 histomicsui-1.5.1.dev6/histomicsui/web_client/vue/components/
--rw-r--r--   0 root         (0) root         (0)     2650 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/vue/components/ColorPickerInput.vue
--rw-r--r--   0 root         (0) root         (0)    12532 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
--rw-r--r--   0 root         (0) root         (0)      745 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
--rw-r--r--   0 root         (0) root         (0)      906 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/web_client/webpack.helper.js
--rw-r--r--   0 root         (0) root         (0)     1538 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/histomicsui/webroot.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.246603 histomicsui-1.5.1.dev6/histomicsui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7783 2024-02-22 18:40:29.000000 histomicsui-1.5.1.dev6/histomicsui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7621 2024-02-22 18:40:29.000000 histomicsui-1.5.1.dev6/histomicsui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 18:40:29.000000 histomicsui-1.5.1.dev6/histomicsui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-02-22 18:40:29.000000 histomicsui-1.5.1.dev6/histomicsui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 18:39:34.000000 histomicsui-1.5.1.dev6/histomicsui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      105 2024-02-22 18:40:29.000000 histomicsui-1.5.1.dev6/histomicsui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-02-22 18:40:29.000000 histomicsui-1.5.1.dev6/histomicsui.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      881 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/ruff.toml
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-22 18:40:29.246603 histomicsui-1.5.1.dev6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2219 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.242603 histomicsui-1.5.1.dev6/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1111 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     2202 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/girder_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.246603 histomicsui-1.5.1.dev6/tests/test_files/
--rw-r--r--   0 root         (0) root         (0)     1286 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_files/.histomicsui_config.yaml
--rw-r--r--   0 root         (0) root         (0)      424 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_files/sample.anot
--rw-r--r--   0 root         (0) root         (0)      101 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_files/sample.meta
--rw-r--r--   0 root         (0) root         (0)      493 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_files/sample_girder_id.anot
--rw-r--r--   0 root         (0) root         (0)     8928 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_files/test_analysis_detection.xml
--rw-r--r--   0 root         (0) root         (0)    12017 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_files/test_analysis_features.xml
--rw-r--r--   0 root         (0) root         (0)     5257 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_handlers.py
--rw-r--r--   0 root         (0) root         (0)    19460 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_hui_rest.py
--rw-r--r--   0 root         (0) root         (0)     4366 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_image_browse_endpoints.py
--rw-r--r--   0 root         (0) root         (0)      160 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)    33012 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_tcga.py
--rw-r--r--   0 root         (0) root         (0)     6003 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 18:40:29.246603 histomicsui-1.5.1.dev6/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      238 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     6643 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/analysisSpec.js
--rw-r--r--   0 root         (0) root         (0)    81971 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/annotationSpec.js
--rw-r--r--   0 root         (0) root         (0)     1985 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/girderUISpec.js
--rw-r--r--   0 root         (0) root         (0)     4036 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/huiSpec.js
--rw-r--r--   0 root         (0) root         (0)     4547 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/huiTest.js
--rw-r--r--   0 root         (0) root         (0)     4393 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/itemSpec.js
--rw-r--r--   0 root         (0) root         (0)     4436 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/metadataPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     6855 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/metadataPlotSpec.js
--rw-r--r--   0 root         (0) root         (0)     6131 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/overviewPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     2996 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/panelLayoutSpec.js
--rw-r--r--   0 root         (0) root         (0)    14056 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tests/web_client_specs/pixelmapCategorySpec.js
--rw-r--r--   0 root         (0) root         (0)     3120 2024-02-22 18:39:20.000000 histomicsui-1.5.1.dev6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.352367 histomicsui-1.5.1.dev8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.328368 histomicsui-1.5.1.dev8/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     3886 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      617 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/.git-blame-ignore-revs
+-rw-r--r--   0 root         (0) root         (0)      531 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    10173 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      585 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7783 2024-03-27 16:29:28.352367 histomicsui-1.5.1.dev8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6730 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/README.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.328368 histomicsui-1.5.1.dev8/docs/
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/docs/config_options.rst
+-rw-r--r--   0 root         (0) root         (0)     7012 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/docs/controls.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.328368 histomicsui-1.5.1.dev8/docs/images/
+-rwxr-xr-x   0 root         (0) root         (0)   133796 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/docs/images/difference.gif
+-rwxr-xr-x   0 root         (0) root         (0)   133603 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/docs/images/intersect.gif
+-rwxr-xr-x   0 root         (0) root         (0)   154141 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/docs/images/union.gif
+-rwxr-xr-x   0 root         (0) root         (0)   168255 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/docs/images/xor.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.328368 histomicsui-1.5.1.dev8/histomicsui/
+-rw-r--r--   0 root         (0) root         (0)    19497 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/constants.py
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.332368 histomicsui-1.5.1.dev8/histomicsui/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/case.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/cohort.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/image.py
+-rw-r--r--   0 root         (0) root         (0)     8576 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/meta.py
+-rw-r--r--   0 root         (0) root         (0)      838 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/pathology.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/models/slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.332368 histomicsui-1.5.1.dev8/histomicsui/rest/
+-rw-r--r--   0 root         (0) root         (0)      512 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/rest/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     9366 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/rest/hui_resource.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/rest/image_browse_resource.py
+-rw-r--r--   0 root         (0) root         (0)    17402 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/rest/system.py
+-rw-r--r--   0 root         (0) root         (0)    29274 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/rest/tcga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.332368 histomicsui-1.5.1.dev8/histomicsui/web_client/
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.332368 histomicsui-1.5.1.dev8/histomicsui/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)      382 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/collections/StyleCollection.js
+-rw-r--r--   0 root         (0) root         (0)      405 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/collections/UserCollection.js
+-rw-r--r--   0 root         (0) root         (0)      149 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/collections/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.336367 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/
+-rw-r--r--   0 root         (0) root         (0)     1326 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/confirmDialog.js
+-rw-r--r--   0 root         (0) root         (0)     3936 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/editElement.js
+-rw-r--r--   0 root         (0) root         (0)     6663 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js
+-rw-r--r--   0 root         (0) root         (0)    11216 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/editStyleGroups.js
+-rw-r--r--   0 root         (0) root         (0)      478 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/index.js
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/metadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     4936 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js
+-rw-r--r--   0 root         (0) root         (0)     2588 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/openImage.js
+-rw-r--r--   0 root         (0) root         (0)    23122 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/saveAnnotation.js
+-rw-r--r--   0 root         (0) root         (0)       78 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      391 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      858 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.336367 histomicsui-1.5.1.dev8/histomicsui/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)      221 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/models/StyleModel.js
+-rw-r--r--   0 root         (0) root         (0)       67 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     3738 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.336367 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/
+-rw-r--r--   0 root         (0) root         (0)    25133 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/AnnotationSelector.js
+-rw-r--r--   0 root         (0) root         (0)    43673 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/DrawWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1943 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/FrameSelectorWidget.js
+-rw-r--r--   0 root         (0) root         (0)    15981 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/MetadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     5287 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/MetadataWidget.js
+-rw-r--r--   0 root         (0) root         (0)     8115 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/OverviewWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/RegionSelector.js
+-rw-r--r--   0 root         (0) root         (0)     9946 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/ZoomWidget.js
+-rw-r--r--   0 root         (0) root         (0)      146 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/panels/index.js
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/router.js
+-rw-r--r--   0 root         (0) root         (0)      292 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.336367 histomicsui-1.5.1.dev8/histomicsui/web_client/static/
+-rwxr-xr-x   0 root         (0) root         (0)     5072 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/static/favicon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.324368 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.336367 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/body/
+-rw-r--r--   0 root         (0) root         (0)      504 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/body/configView.styl
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/body/image.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.336367 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      195 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
+-rw-r--r--   0 root         (0) root         (0)      237 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
+-rw-r--r--   0 root         (0) root         (0)      849 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.340368 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/layout/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/layout/header.styl
+-rw-r--r--   0 root         (0) root         (0)       53 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
+-rw-r--r--   0 root         (0) root         (0)      151 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/layout/headerImage.styl
+-rw-r--r--   0 root         (0) root         (0)     2189 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/layout/layout.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.340368 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      430 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
+-rw-r--r--   0 root         (0) root         (0)      929 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       81 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       67 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/regionSelector.styl
+-rw-r--r--   0 root         (0) root         (0)      878 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.340368 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/popover/
+-rw-r--r--   0 root         (0) root         (0)      113 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.340368 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/views/
+-rw-r--r--   0 root         (0) root         (0)      222 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/views/itemList.styl
+-rw-r--r--   0 root         (0) root         (0)      139 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/views/searchResultsView.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.324368 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.340368 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/body/
+-rw-r--r--   0 root         (0) root         (0)     5608 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/body/configView.pug
+-rw-r--r--   0 root         (0) root         (0)      783 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/body/image.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.340368 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      501 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
+-rw-r--r--   0 root         (0) root         (0)      428 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/confirmDialog.pug
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/editElement.pug
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      838 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
+-rw-r--r--   0 root         (0) root         (0)      353 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/openImage.pug
+-rw-r--r--   0 root         (0) root         (0)     5720 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.344368 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/
+-rw-r--r--   0 root         (0) root         (0)      925 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/header.pug
+-rw-r--r--   0 root         (0) root         (0)      865 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/headerImage.pug
+-rw-r--r--   0 root         (0) root         (0)      641 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/headerUser.pug
+-rw-r--r--   0 root         (0) root         (0)      157 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/layout.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.344368 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/
+-rw-r--r--   0 root         (0) root         (0)     3947 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     5685 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/drawWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2197 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug
+-rw-r--r--   0 root         (0) root         (0)      116 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/frameSelectorWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      347 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      420 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/metadataWidgetPanel.pug
+-rw-r--r--   0 root         (0) root         (0)      102 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/overviewWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      398 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      345 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/regionSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.344368 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/popover/
+-rw-r--r--   0 root         (0) root         (0)      576 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug
+-rw-r--r--   0 root         (0) root         (0)      427 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/popover/annotationPopoverMetadata.pug
+-rw-r--r--   0 root         (0) root         (0)      204 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.344368 histomicsui-1.5.1.dev8/histomicsui/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)      525 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 root         (0) root         (0)      904 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/JobDetailsWidget.js
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/View.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.348368 histomicsui-1.5.1.dev8/histomicsui/web_client/views/body/
+-rw-r--r--   0 root         (0) root         (0)     7205 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/body/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)    71097 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/body/ImageView.js
+-rw-r--r--   0 root         (0) root         (0)      119 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/body/index.js
+-rw-r--r--   0 root         (0) root         (0)      190 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/itemList.js
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/itemPage.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.348368 histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/HeaderImageView.js
+-rw-r--r--   0 root         (0) root         (0)      421 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/HeaderUserView.js
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/HeaderView.js
+-rw-r--r--   0 root         (0) root         (0)      134 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.348368 histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)    11614 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js
+-rw-r--r--   0 root         (0) root         (0)     1231 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)      176 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/index.js
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/searchResultsView.js
+-rw-r--r--   0 root         (0) root         (0)     2847 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/views/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.324368 histomicsui-1.5.1.dev8/histomicsui/web_client/vue/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.348368 histomicsui-1.5.1.dev8/histomicsui/web_client/vue/components/
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
+-rw-r--r--   0 root         (0) root         (0)      745 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
+-rw-r--r--   0 root         (0) root         (0)      906 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/web_client/webpack.helper.js
+-rw-r--r--   0 root         (0) root         (0)     1538 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/histomicsui/webroot.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.352367 histomicsui-1.5.1.dev8/histomicsui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7783 2024-03-27 16:29:28.000000 histomicsui-1.5.1.dev8/histomicsui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-03-27 16:29:28.000000 histomicsui-1.5.1.dev8/histomicsui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 16:29:28.000000 histomicsui-1.5.1.dev8/histomicsui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-03-27 16:29:28.000000 histomicsui-1.5.1.dev8/histomicsui.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 16:28:41.000000 histomicsui-1.5.1.dev8/histomicsui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      105 2024-03-27 16:29:28.000000 histomicsui-1.5.1.dev8/histomicsui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-03-27 16:29:28.000000 histomicsui-1.5.1.dev8/histomicsui.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      881 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/ruff.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2024-03-27 16:29:28.352367 histomicsui-1.5.1.dev8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.348368 histomicsui-1.5.1.dev8/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/girder_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.352367 histomicsui-1.5.1.dev8/tests/test_files/
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_files/.histomicsui_config.yaml
+-rw-r--r--   0 root         (0) root         (0)      424 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_files/sample.anot
+-rw-r--r--   0 root         (0) root         (0)      101 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_files/sample.meta
+-rw-r--r--   0 root         (0) root         (0)      493 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_files/sample_girder_id.anot
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_files/test_analysis_detection.xml
+-rw-r--r--   0 root         (0) root         (0)    12017 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_files/test_analysis_features.xml
+-rw-r--r--   0 root         (0) root         (0)     5257 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_handlers.py
+-rw-r--r--   0 root         (0) root         (0)    19460 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_hui_rest.py
+-rw-r--r--   0 root         (0) root         (0)     4366 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_image_browse_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      160 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)    33012 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_tcga.py
+-rw-r--r--   0 root         (0) root         (0)     6003 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 16:29:28.352367 histomicsui-1.5.1.dev8/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      238 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     6643 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/analysisSpec.js
+-rw-r--r--   0 root         (0) root         (0)    81971 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/annotationSpec.js
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/girderUISpec.js
+-rw-r--r--   0 root         (0) root         (0)     4036 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/huiSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4547 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/huiTest.js
+-rw-r--r--   0 root         (0) root         (0)     4393 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/itemSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4436 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/metadataPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6855 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/metadataPlotSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6131 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/overviewPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/panelLayoutSpec.js
+-rw-r--r--   0 root         (0) root         (0)    14056 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tests/web_client_specs/pixelmapCategorySpec.js
+-rw-r--r--   0 root         (0) root         (0)     3120 2024-03-27 16:28:28.000000 histomicsui-1.5.1.dev8/tox.ini
```

### Comparing `histomicsui-1.5.1.dev6/.circleci/config.yml` & `histomicsui-1.5.1.dev8/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/.git-blame-ignore-revs` & `histomicsui-1.5.1.dev8/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/.gitignore` & `histomicsui-1.5.1.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/.pre-commit-config.yaml` & `histomicsui-1.5.1.dev8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/LICENSE` & `histomicsui-1.5.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/NOTICE` & `histomicsui-1.5.1.dev8/NOTICE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/PKG-INFO` & `histomicsui-1.5.1.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.5.1.dev6
+Version: 1.5.1.dev8
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.5.1.dev6/README.rst` & `histomicsui-1.5.1.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/docs/config_options.rst` & `histomicsui-1.5.1.dev8/docs/config_options.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/docs/controls.rst` & `histomicsui-1.5.1.dev8/docs/controls.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/docs/images/difference.gif` & `histomicsui-1.5.1.dev8/docs/images/difference.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/docs/images/intersect.gif` & `histomicsui-1.5.1.dev8/docs/images/intersect.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/docs/images/union.gif` & `histomicsui-1.5.1.dev8/docs/images/union.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/docs/images/xor.gif` & `histomicsui-1.5.1.dev8/docs/images/xor.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/__init__.py` & `histomicsui-1.5.1.dev8/histomicsui/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/constants.py` & `histomicsui-1.5.1.dev8/histomicsui/constants.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/handlers.py` & `histomicsui-1.5.1.dev8/histomicsui/handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/models/aperio.py` & `histomicsui-1.5.1.dev8/histomicsui/models/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/models/case.py` & `histomicsui-1.5.1.dev8/histomicsui/models/case.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/models/cohort.py` & `histomicsui-1.5.1.dev8/histomicsui/models/cohort.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/models/image.py` & `histomicsui-1.5.1.dev8/histomicsui/models/image.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/models/meta.py` & `histomicsui-1.5.1.dev8/histomicsui/models/meta.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/models/pathology.py` & `histomicsui-1.5.1.dev8/histomicsui/models/pathology.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/models/slide.py` & `histomicsui-1.5.1.dev8/histomicsui/models/slide.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/rest/__init__.py` & `histomicsui-1.5.1.dev8/histomicsui/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/rest/aperio.py` & `histomicsui-1.5.1.dev8/histomicsui/rest/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/rest/hui_resource.py` & `histomicsui-1.5.1.dev8/histomicsui/rest/hui_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/rest/image_browse_resource.py` & `histomicsui-1.5.1.dev8/histomicsui/rest/image_browse_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/rest/system.py` & `histomicsui-1.5.1.dev8/histomicsui/rest/system.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/rest/tcga.py` & `histomicsui-1.5.1.dev8/histomicsui/rest/tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/app.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/app.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/confirmDialog.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/confirmDialog.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/editElement.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/editElement.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/editRegionOfInterest.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/editStyleGroups.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/editStyleGroups.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/metadataPlot.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/metadataPlot.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,16 @@
         ).girderModal(this);
         return this;
     },
 
     _submit(evt) {
         evt.preventDefault();
         const configOptions = {
-            folder: this.$('#h-plot-folder').is(':checked')
+            folder: this.$('#h-plot-folder').is(':checked'),
+            format: this.$('#h-plot-format').val()
         };
         ['x', 'y', 'r', 'c', 's'].forEach((series) => {
             const val = this.$('#h-plot-series-' + series).val();
             if (val !== '_none_' && val !== undefined) {
                 configOptions[series] = val;
             }
         });
```

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/openAnnotatedImage.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/openImage.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/openImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/dialogs/saveAnnotation.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/dialogs/saveAnnotation.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/main.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/main.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/package.json` & `histomicsui-1.5.1.dev8/histomicsui/web_client/package.json`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/AnnotationSelector.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/AnnotationSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/DrawWidget.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/DrawWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/FrameSelectorWidget.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/FrameSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/MetadataPlot.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/MetadataPlot.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -138,25 +138,36 @@
             sort: '_name'
         }];
         for (let midx = 0; midx < 2; midx += 1) {
             var meta = (!midx ? this.item.get('meta') : this.parentMeta) || {};
             for (const [root, entry] of Object.entries(meta)) {
                 if (_.isArray(entry) && entry.length >= 1 && _.isObject(entry[0])) {
                     for (const [key, value] of Object.entries(entry[0])) {
-                        let type;
+                        let type, distinct;
                         if (_.isFinite(value)) {
                             type = 'number';
                         } else if (_.isString(value)) {
                             type = 'string';
                         }
+                        if (Number.isInteger(value) || _.isString(value)) {
+                            distinct = {};
+                            const maxDistinct = 20;
+                            for (let eidx = 0; eidx < entry.length && Object.keys(distinct).length <= maxDistinct; eidx += 1) {
+                                distinct[entry[eidx][key]] = true;
+                            }
+                            if (Object.keys(distinct).length > maxDistinct) {
+                                distinct = null;
+                            }
+                        }
                         if (type) {
                             results.push({
                                 root,
                                 key,
                                 type,
+                                distinct,
                                 sort: `${root}.${key}`.toLowerCase()
                             });
                         }
                     }
                 }
             }
         }
@@ -176,15 +187,16 @@
         plotOptions.forEach((opt) => {
             optDict[opt.sort] = opt;
         });
         const plotData = {
             data: [],
             fieldToPlot: {},
             plotToOpt: {},
-            ranges: {}
+            ranges: {},
+            format: plotConfig.format
         };
         const usedFields = ['x', 'y', 'r', 'c', 's'].filter((series) => plotConfig[series] && optDict[plotConfig[series]]).map((series) => {
             if (!plotData.fieldToPlot[plotConfig[series]]) {
                 plotData.fieldToPlot[plotConfig[series]] = [];
             }
             plotData.fieldToPlot[plotConfig[series]].push(series);
             plotData.plotToOpt[series] = optDict[plotConfig[series]];
@@ -219,16 +231,18 @@
                         } else if (meta[opt.root] && meta[opt.root][idx]) {
                             value = meta[opt.root][idx][opt.key];
                             entry._roots[opt.root] = entry._roots[opt.root] || meta[opt.root][idx];
                         }
                         if (value === undefined || (opt.type === 'number' && !_.isFinite(value))) {
                             end = true;
                         }
-                        if (opt.type === 'string') {
+                        if (opt.type === 'string' || (['s', 'c'].includes(key) && opt.distinct)) {
                             value = '' + value;
+                        } else {
+                            value = +value;
                         }
                         entry[key] = value;
                     });
                 });
                 if (!end) {
                     plotData.data.push(entry);
                 }
@@ -236,39 +250,45 @@
         });
         plotData.data.forEach((entry, idx) => {
             Object.entries(entry).forEach(([key, value]) => {
                 if (key === '_roots') {
                     return;
                 }
                 if (!plotData.ranges[key]) {
-                    if (_.isFinite(value)) {
+                    if (!_.isString(value)) {
                         plotData.ranges[key] = {
                             min: value,
                             max: value
                         };
                     } else {
                         plotData.ranges[key] = {
                             distinct: {}
                         };
                     }
                 }
-                if (_.isFinite(value)) {
+                if (plotData.ranges[key].min !== undefined) {
                     if (value < plotData.ranges[key].min) {
                         plotData.ranges[key].min = value;
                     }
                     if (value > plotData.ranges[key].max) {
                         plotData.ranges[key].max = value;
                     }
                 } else {
                     plotData.ranges[key].distinct[value] = true;
+                }
+            });
+        });
+        if (plotData.data.length) {
+            Object.entries(plotData.data[0]).forEach(([key, value]) => {
+                if (plotData.ranges[key] && plotData.ranges[key].distinct) {
                     plotData.ranges[key].list = Object.keys(plotData.ranges[key].distinct).sort();
                     plotData.ranges[key].count = plotData.ranges[key].list.length;
                 }
             });
-        });
+        }
         return plotData;
     },
 
     onHover: function(evt) {
         // this is a stub for wrapping.
     },
 
@@ -312,14 +332,45 @@
                     ) :
                     '#000000',
                 opacity: 0.5
             },
             type: plotData.data.length > 100 ? 'scattergl' : 'scatter',
             mode: 'markers'
         };
+        if (plotData.format === 'violin') {
+            plotlyData.type = 'violin';
+            plotlyData.x = plotlyData.marker.symbol;
+            // plotlyData.points = none;
+            plotlyData.box = {
+                visible: true
+            };
+            plotlyData.meanline = {
+                visible: true
+            };
+            plotlyData.line = {
+                color: plotlyData.marker.color
+            };
+            plotlyData.yaxis = {
+                zeroline: false
+            };
+            if (plotData.ranges.c && plotData.ranges.c.distinct) {
+                plotlyData.transforms = [{
+                    type: 'groupby',
+                    groups: plotlyData.x,
+                    styles: Object.keys(plotData.ranges.c.distinct).map((k, kidx) => ({
+                        target: kidx,
+                        value: {
+                            line: {
+                                color: colorBrewerPaired12[kidx]
+                            }
+                        }
+                    }))
+                }];
+            }
+        }
         return [plotlyData];
     },
 
     render: function() {
         if (this.item && this.item.id) {
             const plotOptions = this.getPlotOptions();
             if (plotOptions.filter((v) => v.type === 'number').length < 2) {
```

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/MetadataWidget.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/OverviewWidget.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/OverviewWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/RegionSelector.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/RegionSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/panels/ZoomWidget.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/panels/ZoomWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/router.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/router.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/static/favicon.png` & `histomicsui-1.5.1.dev8/histomicsui/web_client/static/favicon.png`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/body/image.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/body/image.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/layout/header.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/layout/header.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/layout/layout.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/annotationSelector.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/drawWidget.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/frameSelectorWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/metadataWidget.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/panels/zoomWidget.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/stylesheets/popover/annotationPopover.styl` & `histomicsui-1.5.1.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/body/configView.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/body/configView.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/body/image.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/body/image.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/editElement.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/editElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/editStyleGroups.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/metadataPlot.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug`

 * *Files 21% similar despite different names*

```diff
@@ -2,29 +2,40 @@
   .modal-content
     form.modal-form(role='form')
       .modal-header
         button.close(type='button', data-dismiss='modal', aria-label='Close')
           span(aria-hidden='true') &times;
         h4.modal-title Metadata Plot
       .modal-body
+        .form-group
+          label(for='h-plot-format') Format
+          -
+            var plotFormats = [
+              {key: 'scatter', label: 'Scatter'},
+              {key: 'violin', label: 'Violin'}]
+          select#h-plot-format.form-control
+            each opt in plotFormats
+              option(value=opt.key, selected=plotConfig.format === opt.key) #{opt.label}
         -
           var seriesList = [
-            {key: 'x', label: 'x-axis', number: true},
+            {key: 'x', label: 'x-axis', number: true, comment: 'Used only for data length in violin plots'},
             {key: 'y', label: 'y-axis', number: true},
             {key: 'r', label: 'Radius'},
             {key: 'c', label: 'Color'},
-            {key: 's', label: 'Symbol', string: true}]
+            {key: 's', label: 'Symbol', string: true, comment: 'Grouping for violin plots'}]
         for series in seriesList
           .form-group
             label(for='h-plot-series-' + series.key) #{series.label}
+            if series.comment
+              p.g-hui-description #{series.comment}
             select.form-control(id='h-plot-series-' + series.key)
               if !series.number
                 option(value='_none_', selected=plotConfig[series.key] === undefined) None
               each opt in plotOptions
-                if (!series.number || opt.type === 'number') && (!series.string || opt.type === 'string')
+                if (!series.number || opt.type === 'number') && (!series.string || opt.type === 'string' || opt.distinct)
                   - var selected = plotConfig[series.key] === opt.sort
                   option(value=opt.sort, selected=selected) #{opt.root + ' - ' + opt.key}
         .form-group
           label(for='h-plot-folder')
             input#h-plot-folder(type='checkbox', checked=plotConfig.folder)
             |  Include data from other items in the same folder
       .modal-footer
```

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/dialogs/saveAnnotation.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/header.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/header.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/headerAnalyses.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/headerImage.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/headerImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/layout/headerUser.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/layout/headerUser.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/annotationSelector.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/drawWidget.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/drawWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/drawWidgetElement.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/panels/zoomWidget.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/popover/annotationContextMenu.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/templates/popover/annotationPopover.pug` & `histomicsui-1.5.1.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/HierarchyWidget.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/JobDetailsWidget.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/JobDetailsWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/View.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/View.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/body/ConfigView.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/body/ConfigView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/body/ImageView.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/body/ImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/itemList.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/itemList.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/itemPage.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/itemPage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/HeaderAnalysesView.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/HeaderImageView.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/HeaderImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/layout/HeaderView.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/AnnotationContextMenu.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/AnnotationPopover.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/popover/PixelmapContextMenu.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/searchResultsView.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/searchResultsView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/views/utils.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/vue/components/ColorPickerInput.vue` & `histomicsui-1.5.1.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue` & `histomicsui-1.5.1.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue` & `histomicsui-1.5.1.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/web_client/webpack.helper.js` & `histomicsui-1.5.1.dev8/histomicsui/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui/webroot.mako` & `histomicsui-1.5.1.dev8/histomicsui/webroot.mako`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/histomicsui.egg-info/PKG-INFO` & `histomicsui-1.5.1.dev8/histomicsui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.5.1.dev6
+Version: 1.5.1.dev8
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.5.1.dev6/histomicsui.egg-info/SOURCES.txt` & `histomicsui-1.5.1.dev8/histomicsui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/ruff.toml` & `histomicsui-1.5.1.dev8/ruff.toml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/setup.py` & `histomicsui-1.5.1.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/datastore.py` & `histomicsui-1.5.1.dev8/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/girder_utilities.py` & `histomicsui-1.5.1.dev8/tests/girder_utilities.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_files/.histomicsui_config.yaml` & `histomicsui-1.5.1.dev8/tests/test_files/.histomicsui_config.yaml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_files/test_analysis_detection.xml` & `histomicsui-1.5.1.dev8/tests/test_files/test_analysis_detection.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_files/test_analysis_features.xml` & `histomicsui-1.5.1.dev8/tests/test_files/test_analysis_features.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_handlers.py` & `histomicsui-1.5.1.dev8/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_hui_rest.py` & `histomicsui-1.5.1.dev8/tests/test_hui_rest.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_image_browse_endpoints.py` & `histomicsui-1.5.1.dev8/tests/test_image_browse_endpoints.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_tcga.py` & `histomicsui-1.5.1.dev8/tests/test_tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/test_web_client.py` & `histomicsui-1.5.1.dev8/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/analysisSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/analysisSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/annotationSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/annotationSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/girderUISpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/girderUISpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/huiSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/huiSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/huiTest.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/huiTest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/itemSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/itemSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/metadataPanelSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/metadataPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/metadataPlotSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/metadataPlotSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/overviewPanelSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/overviewPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/panelLayoutSpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/panelLayoutSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tests/web_client_specs/pixelmapCategorySpec.js` & `histomicsui-1.5.1.dev8/tests/web_client_specs/pixelmapCategorySpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.5.1.dev6/tox.ini` & `histomicsui-1.5.1.dev8/tox.ini`

 * *Files identical despite different names*

