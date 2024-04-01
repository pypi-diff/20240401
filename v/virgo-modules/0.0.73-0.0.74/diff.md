# Comparing `tmp/virgo_modules-0.0.73.tar.gz` & `tmp/virgo_modules-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.73.tar", last modified: Fri Mar 29 14:10:53 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.74.tar", last modified: Mon Apr  1 09:24:46 2024, max compression
```

## Comparing `virgo_modules-0.0.73.tar` & `virgo_modules-0.0.74.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 14:10:53.748313 virgo_modules-0.0.73/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.73/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-03-29 14:10:53.743311 virgo_modules-0.0.73/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.73/README.md
--rw-rw-rw-   0        0        0       42 2024-03-29 14:10:53.749315 virgo_modules-0.0.73/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-03-29 14:01:19.000000 virgo_modules-0.0.73/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 14:10:53.615312 virgo_modules-0.0.73/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-03-29 14:10:53.653310 virgo_modules-0.0.73/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.73/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 14:10:53.738312 virgo_modules-0.0.73/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.73/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     1383 2024-03-05 19:39:06.000000 virgo_modules-0.0.73/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0     7691 2024-03-03 08:13:30.000000 virgo_modules-0.0.73/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.73/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    53096 2024-03-29 14:10:19.000000 virgo_modules-0.0.73/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   104837 2024-03-28 18:45:37.000000 virgo_modules-0.0.73/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-03-29 14:10:53.706312 virgo_modules-0.0.73/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-03-29 14:10:53.000000 virgo_modules-0.0.73/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-03-29 14:10:53.000000 virgo_modules-0.0.73/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 14:10:53.000000 virgo_modules-0.0.73/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-03-29 14:10:53.000000 virgo_modules-0.0.73/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-29 14:10:53.000000 virgo_modules-0.0.73/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:24:46.157435 virgo_modules-0.0.74/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.74/LICENSE
+-rw-rw-rw-   0        0        0      859 2024-04-01 09:24:46.156431 virgo_modules-0.0.74/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.74/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 09:24:46.157435 virgo_modules-0.0.74/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-01 08:57:47.000000 virgo_modules-0.0.74/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:24:46.104180 virgo_modules-0.0.74/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-01 09:24:46.113267 virgo_modules-0.0.74/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.74/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:24:46.152433 virgo_modules-0.0.74/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.74/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     1383 2024-03-05 19:39:06.000000 virgo_modules-0.0.74/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0     7691 2024-03-03 08:13:30.000000 virgo_modules-0.0.74/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.74/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    53096 2024-03-29 14:10:19.000000 virgo_modules-0.0.74/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   105165 2024-04-01 09:14:49.000000 virgo_modules-0.0.74/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:24:46.130253 virgo_modules-0.0.74/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0      859 2024-04-01 09:24:45.000000 virgo_modules-0.0.74/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-01 09:24:45.000000 virgo_modules-0.0.74/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 09:24:45.000000 virgo_modules-0.0.74/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-01 09:24:45.000000 virgo_modules-0.0.74/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-01 09:24:45.000000 virgo_modules-0.0.74/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.73/LICENSE` & `virgo_modules-0.0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.73/setup.py` & `virgo_modules-0.0.74/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.73",
+    version="0.0.74",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.73/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.74/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.73/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.74/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.73/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.74/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.73/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.74/virgo_app/virgo_modules/src/re_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.73/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.74/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -870,15 +870,15 @@
 
             fig.show()
     #######################
     
     def rsi_feature_improved(self, window, threshold, plot = False, save_features = False):
         feature_name = 'RSI'
         rsi = RSIIndicator(close = self.df['Close'], window = window).rsi()
-        self.df[feature_name] = rsi 
+        self.df[feature_name] = rsi.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_rsi_feature_v2 = {'window':window, 'threshold':threshold}
 
         if plot:
@@ -1046,63 +1046,63 @@
             axs[1].set_title(f'z_{feature_name}')
 
             plt.show()
 
     def roc_feature(self, window, threshold, plot = False, save_features = False):
         feature_name = 'ROC'
         roc = ROCIndicator(close = self.df['Close'], window = window).roc()
-        self.df[feature_name] = roc 
+        self.df[feature_name] = roc.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_roc_feature = {'window':window, 'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
     
     def stoch_feature(self, window, smooth1, smooth2, threshold, plot = False, save_features = False):
         feature_name = 'STOCH'
         stoch = StochRSIIndicator(close = self.df['Close'], window = window, smooth1=smooth1, smooth2=smooth2).stochrsi()
-        self.df[feature_name] = stoch
+        self.df[feature_name] = stoch.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_stoch_feature = {'window':window, 'smooth1':smooth1, 'smooth2':smooth2, 'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
     def stochastic_feature(self, window, smooth, threshold, plot = False, save_features = False):
         feature_name = 'STOCHOSC'
         stochast = StochasticOscillator(close = self.df['Close'], high = self.df['High'], low = self.df['Low'], window = window,smooth_window=smooth).stoch()
-        self.df[feature_name] = stochast
+        self.df[feature_name] = stochast.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_stochastic_feature = {'window':window, 'smooth':smooth,'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
     def william_feature(self, lbp, threshold, plot = False, save_features = False):
         feature_name = 'WILL'
         will = WilliamsRIndicator(close = self.df['Close'], high = self.df['High'], low = self.df['Low'], lbp = lbp).williams_r() 
-        self.df[feature_name] = will
+        self.df[feature_name] = will.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_william_feature = {'lbp':lbp,'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
     def vortex_feature(self, window, threshold, plot = False, save_features = False):
         feature_name = 'VORTEX'
         vortex = VortexIndicator(close = self.df['Close'], high = self.df['High'], low = self.df['Low'], window = window).vortex_indicator_diff()
-        self.df[feature_name] = vortex
+        self.df[feature_name] = vortex.replace([np.inf, -np.inf], 0).fillna(method = 'ffill')
         self.compute_clip_bands(feature_name,threshold)
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_vortex_feature = {'window':window, 'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
```

### Comparing `virgo_modules-0.0.73/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.74/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

