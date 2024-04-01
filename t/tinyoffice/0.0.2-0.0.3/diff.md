# Comparing `tmp/tinyoffice-0.0.2.tar.gz` & `tmp/tinyoffice-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyoffice-0.0.2.tar", last modified: Sun Mar 31 13:51:31 2024, max compression
+gzip compressed data, was "tinyoffice-0.0.3.tar", last modified: Mon Apr  1 13:56:46 2024, max compression
```

## Comparing `tinyoffice-0.0.2.tar` & `tinyoffice-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-31 13:51:31.160726 tinyoffice-0.0.2/
--rw-r--r--   0 sam        (501) staff       (20)     1864 2024-03-31 12:26:00.000000 tinyoffice-0.0.2/.gitignore
--rw-r--r--   0 sam        (501) staff       (20)     1072 2024-03-31 12:26:00.000000 tinyoffice-0.0.2/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)     2764 2024-03-31 13:51:31.160448 tinyoffice-0.0.2/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)     2246 2024-03-31 13:50:49.000000 tinyoffice-0.0.2/README.md
--rw-r--r--   0 sam        (501) staff       (20)      640 2024-03-31 13:51:18.000000 tinyoffice-0.0.2/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)       38 2024-03-31 13:51:31.160783 tinyoffice-0.0.2/setup.cfg
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-31 13:51:31.159182 tinyoffice-0.0.2/tinyoffice/
--rw-r--r--   0 sam        (501) staff       (20)        0 2024-03-31 12:26:00.000000 tinyoffice-0.0.2/tinyoffice/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)     4955 2024-03-31 12:28:27.000000 tinyoffice-0.0.2/tinyoffice/__main__.py
--rw-r--r--   0 sam        (501) staff       (20)    21182 2024-03-31 12:26:00.000000 tinyoffice-0.0.2/tinyoffice/tinyoffice.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-31 13:51:31.160161 tinyoffice-0.0.2/tinyoffice.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)     2764 2024-03-31 13:51:31.000000 tinyoffice-0.0.2/tinyoffice.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      283 2024-03-31 13:51:31.000000 tinyoffice-0.0.2/tinyoffice.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2024-03-31 13:51:31.000000 tinyoffice-0.0.2/tinyoffice.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)        7 2024-03-31 13:51:31.000000 tinyoffice-0.0.2/tinyoffice.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)       11 2024-03-31 13:51:31.000000 tinyoffice-0.0.2/tinyoffice.egg-info/top_level.txt
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-01 13:56:46.424853 tinyoffice-0.0.3/
+-rw-r--r--   0 sam        (501) staff       (20)     1864 2024-04-01 01:59:02.000000 tinyoffice-0.0.3/.gitignore
+-rw-r--r--   0 sam        (501) staff       (20)     1072 2024-03-31 12:26:00.000000 tinyoffice-0.0.3/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)     2748 2024-04-01 13:56:46.424625 tinyoffice-0.0.3/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)     2230 2024-04-01 13:55:05.000000 tinyoffice-0.0.3/README.md
+-rw-r--r--   0 sam        (501) staff       (20)      692 2024-04-01 13:56:39.000000 tinyoffice-0.0.3/pyproject.toml
+-rw-r--r--   0 sam        (501) staff       (20)       38 2024-04-01 13:56:46.424930 tinyoffice-0.0.3/setup.cfg
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-01 13:56:46.423608 tinyoffice-0.0.3/tinyoffice/
+-rw-r--r--   0 sam        (501) staff       (20)        0 2024-03-31 12:26:00.000000 tinyoffice-0.0.3/tinyoffice/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     5694 2024-04-01 01:59:29.000000 tinyoffice-0.0.3/tinyoffice/__main__.py
+-rw-r--r--   0 sam        (501) staff       (20)    22375 2024-04-01 13:53:53.000000 tinyoffice-0.0.3/tinyoffice/tinyoffice.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-04-01 13:56:46.424382 tinyoffice-0.0.3/tinyoffice.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)     2748 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      283 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)        7 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)       21 2024-04-01 13:56:46.000000 tinyoffice-0.0.3/tinyoffice.egg-info/top_level.txt
```

### Comparing `tinyoffice-0.0.2/.gitignore` & `tinyoffice-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyoffice-0.0.2/LICENSE` & `tinyoffice-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyoffice-0.0.2/PKG-INFO` & `tinyoffice-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyoffice
-Version: 0.0.2
+Version: 0.0.3
 Summary: Make your Office files tiny!
 Author-email: Samuel Woodward <sam@woodward.fyi>
 Project-URL: Homepage, https://github.com/PyWoody/tinyoffice
 Keywords: office,compress,convert,image,Word,Excel,Powerpoint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,28 +13,26 @@
 License-File: LICENSE
 Requires-Dist: Pillow
 
 ## tinyoffice
 
 Make your Office files tiny!
 
-`tinyoffice` attemps to compresses and optionally convert your embedded image files in your Office files.
+`tinyoffice` attemps to compresses and optionally convert the embedded image files in your Office files.
 
 
 ## Installation
 
 You can install `tinyoffice` from PyPi:
 
 ```
 % pip install tinyoffice
 ```
 
-NOTE: `tinyoffice` requires `Pillow` (`PIL` Fork) [Pillow](https://pillow.readthedocs.io/en/stable/), which can have installation conflicts. If you experience any issues while installing `tinyoffice`, please follow the `Pillow` installation steps found here: https://pillow.readthed
-## tinyoffice
-ocs.io/en/stable/installation.html.
+NOTE: `tinyoffice` requires `Pillow` (`PIL` Fork) [Pillow](https://pillow.readthedocs.io/en/stable/), which can have installation conflicts. If you experience any issues while installing `tinyoffice`, please follow the `Pillow` installation steps found here: https://pillow.readthedocs.io/en/stable/installation.html.
 
 
 ## Usage
 
 ```
 usage: tinyoffice [-h] [-r] [-c] [-v]
                   [-t .docx .pptx .xlsx [.docx .pptx .xlsx ...]] [--overwrite]
```

### Comparing `tinyoffice-0.0.2/README.md` & `tinyoffice-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 ## tinyoffice
 
 Make your Office files tiny!
 
-`tinyoffice` attemps to compresses and optionally convert your embedded image files in your Office files.
+`tinyoffice` attemps to compresses and optionally convert the embedded image files in your Office files.
 
 
 ## Installation
 
 You can install `tinyoffice` from PyPi:
 
 ```
 % pip install tinyoffice
 ```
 
-NOTE: `tinyoffice` requires `Pillow` (`PIL` Fork) [Pillow](https://pillow.readthedocs.io/en/stable/), which can have installation conflicts. If you experience any issues while installing `tinyoffice`, please follow the `Pillow` installation steps found here: https://pillow.readthed
-## tinyoffice
-ocs.io/en/stable/installation.html.
+NOTE: `tinyoffice` requires `Pillow` (`PIL` Fork) [Pillow](https://pillow.readthedocs.io/en/stable/), which can have installation conflicts. If you experience any issues while installing `tinyoffice`, please follow the `Pillow` installation steps found here: https://pillow.readthedocs.io/en/stable/installation.html.
 
 
 ## Usage
 
 ```
 usage: tinyoffice [-h] [-r] [-c] [-v]
                   [-t .docx .pptx .xlsx [.docx .pptx .xlsx ...]] [--overwrite]
```

### Comparing `tinyoffice-0.0.2/pyproject.toml` & `tinyoffice-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,15 @@
 keywords = ["office", "compress", "convert", "image", "Word", "Excel", "Powerpoint"]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "0.0.2"
+version = "0.0.3"
 dependencies = ["Pillow"]
 
 [project.urls]
 Homepage = "https://github.com/PyWoody/tinyoffice"
+
+[tool.setuptools.packages.find]
+exclude = ["data"]
```

### Comparing `tinyoffice-0.0.2/tinyoffice/__main__.py` & `tinyoffice-0.0.3/tinyoffice/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -65,61 +65,88 @@
 parser.add_argument(
     '-exts',
     '--extensions',
     nargs='+',
     help='Image extensions to compress. Default will be only the extensions '
          'that are supported by Pillow on your system.\nShould be ignored.'
 )
+parser.add_argument(
+    '--jpeg-quality',
+    default=75,
+    type=int,
+    help='Default is 75',
+)
+parser.add_argument(
+    '--tiff-quality',
+    default=75,
+    type=int,
+    help='Default is 75',
+)
+parser.add_argument(
+    '--no-optimize',
+    default=False,
+    action='store_true',
+    help='Flag for disabling optimization passes on JPEGs and PNGS',
+)
 args = parser.parse_args()
 
 image_extensions = args.extensions if args.extensions else None
 types = args.types if args.types else None
 
 if args.verbose <= 0:
     verbosity = tinyoffice.Verbosity.NONE
 elif args.verbose == 1:
     verbosity = tinyoffice.Verbosity.LOW
 elif args.verbose == 2:
     verbosity = tinyoffice.Verbosity.NORMAL
-else args.verbose:
+else:
     verbosity = tinyoffice.Verbosity.HIGH
 
 path = os.path.realpath(args.path)
 output = os.path.realpath(args.output) if args.output else args.output
 
 if args.recurse:
     tinyoffice.walk(
         path,
         types=types,
         overwrite=args.overwrite,
         output=args.output,
         convert=args.convert,
         verbosity=verbosity,
         image_extensions=image_extensions,
+        jpeg_quality=args.jpeg_quality,
+        tiff_quality=args.tiff_quality,
+        optimize=not args.no_optimize,
     )
 else:
     if os.path.isdir(path):
         tinyoffice.listdir(
             path,
             types=types,
             overwrite=args.overwrite,
             output=args.output,
             convert=args.convert,
             verbosity=verbosity,
             image_extensions=image_extensions,
+            jpeg_quality=args.jpeg_quality,
+            tiff_quality=args.tiff_quality,
+            optimize=not args.no_optimize,
         )
     else:
         if output is None or not os.path.splitext(output)[1]:
             output = os.path.join(output, os.path.split(path)[1])
         if args.overwrite or not os.path.isfile(path):
             result = tinyoffice.process(
                 path,
                 output=output,
                 convert=args.convert,
                 image_extensions=image_extensions,
+                jpeg_quality=args.jpeg_quality,
+                tiff_quality=args.tiff_quality,
+                optimize=not args.no_optimize,
             )
             if verbosity is tinyoffice.Verbosity.LOW:
                 if result.num_images_compressed:
                     print(
                         f'Compressed {result.filename}. '
                         f'{len(result.errors):,} Error(s) encountered.'
                     )
```

### Comparing `tinyoffice-0.0.2/tinyoffice/tinyoffice.py` & `tinyoffice-0.0.3/tinyoffice/tinyoffice.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,17 @@
     *,
     types=None,
     overwrite=False,
     output=None,
     convert=False,
     verbosity=Verbosity.NORMAL,
     image_extensions=None,
+    jpeg_quality=75,
+    tiff_quality=75,
+    optimize=True,
 ):
     """
     Recursively iterates over the files in the directory
     and attempts to compress them if they match the listed file types
 
     Args:
         cwd: Path to directory to start from
@@ -62,14 +65,18 @@
                 the script was called
         overwrite: Overwrite if output exists. Default is False
         convert: Convert TIFFs to JPEGs. Default is False
         verbosity: Verbosity level. Default is Verbosity.NORMAL
         image_extensions: Supported image extensions. Default is None which
                           will use only the supported extensions that
                           can be OPENd and SAVEd by PIL on your machine.
+        jpeg_quality: Defaults to 75, which is PIL's default quality value
+                 Only applicable to JPEG and TIFFs
+        tiff_quality: Defaults to 75.
+        optimize: Default is True. Will be applied to JPEG and PNGs only
     """
     if types is None:
         types = {'.docx', '.pptx', '.xslx'}
     else:
         if isinstance(types, str):
             types = {types}
         else:
@@ -77,15 +84,15 @@
     if output is None:
         output = os.getcwd()
     else:
         if os.path.splitext(output)[1]:
             # A file but it may not exist so you can't .isfile it
             output = os.path.dirname(output)
         else:
-            output = output
+            output = os.path.realpath(output)
         os.makedirs(output, exist_ok=True)
 
     if verbosity is not Verbosity.NONE:
         printer_callback = partial(printer, verbosity=verbosity)
         output_record = {
             'compressed_files': [],
             'errors': [],
@@ -101,36 +108,30 @@
     if image_extensions is None:
         registered_extensions = Image.registered_extensions()
         image_extensions = {
             ext for ext, func in registered_extensions.items()
             if func in Image.SAVE
             if func in Image.OPEN
         }
-    stopped = False
     with ProcessPoolExecutor() as executor:
-        if stopped:
-            print('Shutting down executor...')
-            executor.shutdown(cancel_futures=True)
-            return
         for root, dirs, files in os.walk(cwd):
             for f in files:
-                if stopped:
-                    print('Shutting down executor...')
-                    executor.shutdown(cancel_futures=True)
-                    return
                 if os.path.splitext(f)[1].lower() in types:
                     fpath = os.path.join(root, f)
                     outpath = os.path.join(output, f)
                     if overwrite or not os.path.isfile(outpath):
                         future = executor.submit(
                             process,
                             fpath,
                             output=outpath,
                             convert=convert,
                             image_extensions=image_extensions,
+                            jpeg_quality=jpeg_quality,
+                            tiff_quality=tiff_quality,
+                            optimize=optimize,
                         )
                         if verbosity is not Verbosity.NONE:
                             future.add_done_callback(totaler_callback)
                             future.add_done_callback(printer_callback)
     if verbosity is not Verbosity.NONE:
         print_total(output_record, verbosity)
 
@@ -140,14 +141,17 @@
     *,
     types=None,
     overwrite=False,
     output=None,
     convert=False,
     verbosity=Verbosity.NORMAL,
     image_extensions=None,
+    jpeg_quality=75,
+    tiff_quality=75,
+    optimize=True,
 ):
     """
     Iterates over the files in the directory and attempts to compress
     them if they match the listed file types
 
     Args:
         cwd: Path to directory to use
@@ -158,14 +162,18 @@
                Default is None which will use .docx, .pptx, and .xlsx
         overwrite: Overwrite if output exists. Default is False
         convert: Convert TIFFs to JPEGs. Default is False
         verbosity: Verbosity level. Default is Verbosity.NORMAL
         image_extensions: Supported image extensions. Deafult is None which
                           will use only the supported extensions that
                           can be OPENd and SAVEd by PIL on your machine.
+        jpeg_quality: Defaults to 75, which is PIL's default quality value
+                 Only applicable to JPEG and TIFFs
+        tiff_quality: Defaults to 75.
+        optimize: Default is True. Will be applied to JPEG and PNGs only
     """
     if types is None:
         types = {'.docx', '.pptx', '.xslx'}
     else:
         if isinstance(types, str):
             types = {types}
         else:
@@ -173,15 +181,15 @@
     if output is None:
         output = os.getcwd()
     else:
         if os.path.splitext(output)[1]:
             # A file but it may not exist so you can't .isfile it
             output = os.path.dirname(output)
         else:
-            output = output
+            output = os.path.realpath(output)
         os.makedirs(output, exist_ok=True)
 
     if verbosity is not Verbosity.NONE:
         printer_callback = partial(printer, verbosity=verbosity)
         output_record = {
             'compressed_files': [],
             'errors': [],
@@ -197,63 +205,68 @@
     if image_extensions is None:
         registered_extensions = Image.registered_extensions()
         image_extensions = {
             ext for ext, func in registered_extensions.items()
             if func in Image.SAVE
             if func in Image.OPEN
         }
-    stopped = False
     with ProcessPoolExecutor() as executor:
-        if stopped:
-            print('Shutting down executor...')
+        try:
+            for item in os.listdir(cwd):
+                fpath = os.path.join(cwd, item)
+                if os.path.isfile(fpath):
+                    if os.path.splitext(fpath)[1].lower() in types:
+                        outpath = os.path.join(output, item)
+                        if overwrite or not os.path.isfile(outpath):
+                            future = executor.submit(
+                                process,
+                                fpath,
+                                output=outpath,
+                                convert=convert,
+                                image_extensions=image_extensions,
+                                jpeg_quality=jpeg_quality,
+                                tiff_quality=tiff_quality,
+                                optimize=optimize,
+                            )
+                            if verbosity is not Verbosity.NONE:
+                                future.add_done_callback(totaler_callback)
+                                future.add_done_callback(printer_callback)
+        except KeyboardInterrupt:
+            print('Shutting down exceutor pool...')
             executor.shutdown(cancel_futures=True)
-            return
-        for item in os.listdir(cwd):
-            if stopped:
-                print('Shutting down executor...')
-                executor.shutdown(cancel_futures=True)
-                return
-            fpath = os.path.join(cwd, item)
-            if os.path.isfile(fpath):
-                if os.path.splitext(fpath)[1].lower() in types:
-                    outpath = os.path.join(output, item)
-                    if overwrite or not os.path.isfile(outpath):
-                        future = executor.submit(
-                            process,
-                            fpath,
-                            output=outpath,
-                            convert=convert,
-                            image_extensions=image_extensions,
-                        )
-                        if verbosity is not Verbosity.NONE:
-                            future.add_done_callback(totaler_callback)
-                            future.add_done_callback(printer_callback)
     if verbosity is not Verbosity.NONE:
         print_total(output_record, verbosity)
 
 
 def process(
     fpath,
     *,
     output,
     convert=False,
     image_extensions=None,
+    jpeg_quality=75,
+    tiff_quality=75,
+    optimize=True,
 ):
     """
     Attempts to compress the images found in the Office File
 
     Args:
         fpath: File path for the Office File
 
     Kwargs:
         output: File path for the compressed output.
         convert: Convert TIFFs to JPEGs. Default is False
         image_extensions: Supported image extensions. Deafult is None which
                           will use only the supported extensions that
                           can be OPENd and SAVEd by PIL on your machine.
+        jpeg_quality: Defaults to 75, which is PIL's default quality value
+                 Only applicable to JPEG and TIFFs
+        tiff_quality: Defaults to 75.
+        optimize: Default is True. Will be applied to JPEG and PNGs only
 
     Returns:
         CompressionRecord: namedtuple of the results
     """
     if image_extensions is None:
         registered_extensions = Image.registered_extensions()
         image_extensions = {
@@ -359,59 +372,70 @@
         num_images_converted=num_images_converted,
         num_images_skipped=num_images_skipped,
         start_size=start_size,
         compressed_size=os.stat(output).st_size,
     )
 
 
-def compress_image(image_bytes, quality=75):
+def compress_image(
+    image_bytes,
+    jpeg_quality=75,
+    tiff_quality=75,
+    optimize=True,
+):
     """
     Compresses image if it is of a format of JPEG, PNG, or TIFF.
 
     Args:
         image: image to compress as bytes. Image must support `.read()`
 
     Kwargs:
-        quality: Defaults to 75, which is PIL's default quality value
-                 Only applicable to JPEG and TIFFs
+        jpeg_quality: Defaults to 75, which is PIL's
+                      default quality value for JPEGs
+        tiff_quality: Defaults to 75.
+        optimize: Default is True. Will be applied to JPEG and PNGs only
 
     Returns:
         io.BytesIO object positioned at laste write
     """
     bytes_io_image = io.BytesIO()
     pil_image = Image.open(io.BytesIO(image_bytes))
     if pil_image.format == 'JPEG':
         pil_image.save(
-            bytes_io_image, format='JPEG', quality=quality, optimize=True
+            bytes_io_image,
+            format='JPEG',
+            quality=jpeg_quality,
+            optimize=optimize,
         )
     elif pil_image.format == 'PNG':
-        pil_image.save(bytes_io_image, format='PNG', optimize=True)
+        pil_image.save(bytes_io_image, format='PNG', optimize=optimize)
     elif pil_image.format == 'TIFF':
-        pil_image.save(bytes_io_image, format='TIFF', quality=quality)
+        pil_image.save(bytes_io_image, format='TIFF', quality=tiff_quality)
     return bytes_io_image
 
 
-def convert_image(image_bytes, quality=75):
+def convert_image(image_bytes, quality=75, optimize=True):
     """
     Converts image to JPG
 
     Args:
         image: image to convert as bytes. Image must support `.read()`
 
     Kwargs:
         quality: Defaults to 75, which is PIL's default quality value
+        optimize: Defaults to True. Will attempt an optimization pass
 
     Returns:
         io.BytesIO object positioned at laste write
     """
     bytes_io_image = io.BytesIO()
     pil_image = Image.open(io.BytesIO(image_bytes))
     pil_image = pil_image.convert('RGB')
     pil_image.save(
-        bytes_io_image, 'JPEG', quality=quality, optimize=True
+        bytes_io_image, 'JPEG', quality=quality, optimize=optimize
     )
     return bytes_io_image
 
 
 def printer(future, verbosity=Verbosity.NORMAL):
     try:
         result = future.result()
@@ -480,14 +504,16 @@
             output_record['images_converted'] += result.num_images_converted
             output_record['total_bytes'] += result.start_size
             output_record['total_bytes_compressed'] += result.compressed_size
             output_record['image_errors'].extend(result.errors)
 
 
 def print_total(record, verbosity):
+    if verbosity is not Verbosity.NONE:
+        print('\n\n')
     if verbosity is Verbosity.LOW:
         print(
             f'Compressed {len(record["compressed_files"]):,} '
             f'document(s) with {len(record["image_errors"]):,} '
             'image(s) that could not be converted and '
             f'{len(record["errors"]):,} document(s) '
             'that failed.'
```

### Comparing `tinyoffice-0.0.2/tinyoffice.egg-info/PKG-INFO` & `tinyoffice-0.0.3/tinyoffice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyoffice
-Version: 0.0.2
+Version: 0.0.3
 Summary: Make your Office files tiny!
 Author-email: Samuel Woodward <sam@woodward.fyi>
 Project-URL: Homepage, https://github.com/PyWoody/tinyoffice
 Keywords: office,compress,convert,image,Word,Excel,Powerpoint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,28 +13,26 @@
 License-File: LICENSE
 Requires-Dist: Pillow
 
 ## tinyoffice
 
 Make your Office files tiny!
 
-`tinyoffice` attemps to compresses and optionally convert your embedded image files in your Office files.
+`tinyoffice` attemps to compresses and optionally convert the embedded image files in your Office files.
 
 
 ## Installation
 
 You can install `tinyoffice` from PyPi:
 
 ```
 % pip install tinyoffice
 ```
 
-NOTE: `tinyoffice` requires `Pillow` (`PIL` Fork) [Pillow](https://pillow.readthedocs.io/en/stable/), which can have installation conflicts. If you experience any issues while installing `tinyoffice`, please follow the `Pillow` installation steps found here: https://pillow.readthed
-## tinyoffice
-ocs.io/en/stable/installation.html.
+NOTE: `tinyoffice` requires `Pillow` (`PIL` Fork) [Pillow](https://pillow.readthedocs.io/en/stable/), which can have installation conflicts. If you experience any issues while installing `tinyoffice`, please follow the `Pillow` installation steps found here: https://pillow.readthedocs.io/en/stable/installation.html.
 
 
 ## Usage
 
 ```
 usage: tinyoffice [-h] [-r] [-c] [-v]
                   [-t .docx .pptx .xlsx [.docx .pptx .xlsx ...]] [--overwrite]
```

