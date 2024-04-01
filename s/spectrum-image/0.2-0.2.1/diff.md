# Comparing `tmp/spectrum_image-0.2.tar.gz` & `tmp/spectrum_image-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_image-0.2.tar", last modified: Fri Mar 29 20:49:22 2024, max compression
+gzip compressed data, was "spectrum_image-0.2.1.tar", last modified: Mon Apr  1 16:55:30 2024, max compression
```

## Comparing `spectrum_image-0.2.tar` & `spectrum_image-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-03-29 20:49:22.265368 spectrum_image-0.2/
--rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2/LICENSE
--rw-r--r--   0 sung       (501) staff       (20)     1779 2024-03-29 20:49:22.265166 spectrum_image-0.2/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      977 2024-03-18 03:44:13.000000 spectrum_image-0.2/README.md
--rw-r--r--   0 sung       (501) staff       (20)      862 2024-03-29 20:49:04.000000 spectrum_image-0.2/pyproject.toml
--rw-r--r--   0 sung       (501) staff       (20)       38 2024-03-29 20:49:22.265399 spectrum_image-0.2/setup.cfg
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-03-29 20:49:22.260668 spectrum_image-0.2/src/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-03-29 20:49:22.264207 spectrum_image-0.2/src/spectrum_image/
--rw-r--r--   0 sung       (501) staff       (20)    55945 2024-03-29 20:43:01.000000 spectrum_image-0.2/src/spectrum_image/SI.py
--rw-r--r--   0 sung       (501) staff       (20)    63318 2024-03-26 23:25:55.000000 spectrum_image-0.2/src/spectrum_image/SI_bckup.py
--rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2/src/spectrum_image/SI_lineshapes.py
--rw-r--r--   0 sung       (501) staff       (20)     7848 2024-03-25 18:18:26.000000 spectrum_image-0.2/src/spectrum_image/SI_util.py
--rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2/src/spectrum_image/__init__.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-03-29 20:49:22.264951 spectrum_image-0.2/src/spectrum_image.egg-info/
--rw-r--r--   0 sung       (501) staff       (20)     1779 2024-03-29 20:49:22.000000 spectrum_image-0.2/src/spectrum_image.egg-info/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      394 2024-03-29 20:49:22.000000 spectrum_image-0.2/src/spectrum_image.egg-info/SOURCES.txt
--rw-r--r--   0 sung       (501) staff       (20)        1 2024-03-29 20:49:22.000000 spectrum_image-0.2/src/spectrum_image.egg-info/dependency_links.txt
--rw-r--r--   0 sung       (501) staff       (20)       52 2024-03-29 20:49:22.000000 spectrum_image-0.2/src/spectrum_image.egg-info/requires.txt
--rw-r--r--   0 sung       (501) staff       (20)       15 2024-03-29 20:49:22.000000 spectrum_image-0.2/src/spectrum_image.egg-info/top_level.txt
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.615615 spectrum_image-0.2.1/
+-rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.1/LICENSE
+-rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-01 16:55:30.615414 spectrum_image-0.2.1/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      977 2024-03-18 03:44:13.000000 spectrum_image-0.2.1/README.md
+-rw-r--r--   0 sung       (501) staff       (20)      864 2024-04-01 16:55:11.000000 spectrum_image-0.2.1/pyproject.toml
+-rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-01 16:55:30.615653 spectrum_image-0.2.1/setup.cfg
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.612489 spectrum_image-0.2.1/src/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.614435 spectrum_image-0.2.1/src/spectrum_image/
+-rw-r--r--   0 sung       (501) staff       (20)    34207 2024-04-01 16:51:54.000000 spectrum_image-0.2.1/src/spectrum_image/SI.py
+-rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.1/src/spectrum_image/SI_bckup.py
+-rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.1/src/spectrum_image/SI_lineshapes.py
+-rw-r--r--   0 sung       (501) staff       (20)     7848 2024-03-25 18:18:26.000000 spectrum_image-0.2.1/src/spectrum_image/SI_util.py
+-rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.1/src/spectrum_image/__init__.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.615208 spectrum_image-0.2.1/src/spectrum_image.egg-info/
+-rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      394 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/SOURCES.txt
+-rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/dependency_links.txt
+-rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/requires.txt
+-rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/top_level.txt
```

### Comparing `spectrum_image-0.2/LICENSE` & `spectrum_image-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2/PKG-INFO` & `spectrum_image-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2
+Version: 0.2.1
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
 Project-URL: Repository, https://github.com/sukhsung/spectrum_image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spectrum_image-0.2/README.md` & `spectrum_image-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2/pyproject.toml` & `spectrum_image-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spectrum_image"
-version = "0.2"
+version = "0.2.1"
 dependencies = [
   "numpy",
   "matplotlib",
   "jupyterlab",
   "ipympl",
   "scipy",
   "tqdm",
```

### Comparing `spectrum_image-0.2/src/spectrum_image/SI.py` & `spectrum_image-0.2.1/src/spectrum_image/SI_bckup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.widgets import RangeSlider, RectangleSelector, SpanSelector, CheckButtons, RadioButtons, Button
-from matplotlib.backend_bases import MouseButton
 import matplotlib.patches as patches
 from scipy.optimize import curve_fit
 from scipy.ndimage import gaussian_filter
 from tqdm import tqdm, tqdm_notebook
 import spectrum_image.SI_lineshapes as ls
-from scipy.stats import norm
 
 import numpy.linalg as LA
 
 class eels_edge:
     def __init__( self, label="", e_bsub=None, e_int=None ):
         self.label  = label
         self.e_bsub = e_bsub
@@ -38,15 +36,14 @@
     
     def __init__( self, si, energy, im_adf=None, cmap='gray', figsize=(9,4), **kwargs):
         ######### Initialize browser object ##########
         self.si = si
         self.energy = energy
         self.im_adf = im_adf
         self.im_inel =np.mean(si,axis=(-1))
-        self.edge = eels_edge( "", e_bsub=None, e_int=(energy[0], energy[-1]))
 
         self.spectrum1=np.mean(si,axis=(0,1))
         self.spectrum2=np.mean(si,axis=(0,1))
         
         ##############Initialize Display#################
         self.fig=plt.figure(figsize=figsize)
 
@@ -76,94 +73,84 @@
         ##############################################
         results_dict={}
         for key in ['spectrum','image','roi','energy_span']:
             results_dict[key]=[]
         
         ################### Selectors ###################
         self.ui = {'roi1':None, 'roi2':None, 'spec':None, 'logscale':None}
-        self.ui['roi1'] = RectangleSelector(self.ax['inel'], self.dummy, button=[1],
-                                        useblit=False ,minspanx=1, minspany=1,spancoords='pixels',
+        self.ui['roi1'] = RectangleSelector(self.ax['inel'], self.onselect_function_real_space, button=[1],
+                                        useblit=True ,minspanx=1, minspany=1,spancoords='pixels',
                                         interactive=True,props=dict(facecolor='crimson',edgecolor='crimson',alpha=0.2,fill=True),
                                         handle_props=dict(markersize=2,markerfacecolor='white'))#,ignore_event_outside=True
         
-        self.ui['roi2'] = RectangleSelector(self.ax['inel'], self.dummy, button=[3],
-                                        useblit=False ,minspanx=1, minspany=1,spancoords='pixels',
+        self.ui['roi2'] = RectangleSelector(self.ax['inel'], self.onselect_function_real_space, button=[3],
+                                        useblit=True ,minspanx=1, minspany=1,spancoords='pixels',
                                         interactive=True,props=dict(facecolor='royalblue',edgecolor='royalblue',alpha=0.2,fill=True),
                                         handle_props=dict(markersize=2,markerfacecolor='white'))#,ignore_event_outside=True)
             
-        self.ui['span_spec'] = SpanSelector(self.ax['spec'], self.dummy, button=[1],
-                                            useblit=False, minspan=1,direction="horizontal",
+        self.ui['span_spec'] = SpanSelector(self.ax['spec'], self.onselect_function_spectrum_space, button=[1],
+                                            useblit=True, minspan=1,direction="horizontal",
                                             interactive=True,props=dict(facecolor='green',edgecolor='green',alpha=0.2,fill=True),
                                             grab_range=10, drag_from_anywhere=True)
         
 
         self.ui['logscale']=CheckButtons(self.ax['bttn'],["Log Scale"],useblit=True ,)
         self.ui['logscale'].on_clicked(self.scale_button)
+        
 
-        self.fig.canvas.mpl_connect( 'motion_notify_event', 
-                                    lambda event: self.onclick_figure(event))
+        ############### Event Handlers ###################
+    def onselect_function_real_space(self, eclick, erelease):
+        
+        real_roi1 = np.array(self.ui['roi1'].extents).astype('int')
+        real_roi2 = np.array(self.ui['roi2'].extents).astype('int')
+        
+        self.spectrum1=np.mean(self.si[int(real_roi1[2]):int(real_roi1[3]),int(real_roi1[0]):int(real_roi1[1]),:],axis=(0,1))
+        self.spectrum2=np.mean(self.si[int(real_roi2[2]):int(real_roi2[3]),int(real_roi2[0]):int(real_roi2[1]),:],axis=(0,1))
 
-    ############### Event Handlers ###################
-    def onclick_figure( self, event ):
-        if event.inaxes in [self.ax['inel']]:
-            if event.button == MouseButton.LEFT:
-                # Left Click on Inelastic Image
-                real_roi1 = np.array(self.ui['roi1'].extents).astype('int')
-                self.spectrum1=np.mean(self.si[int(real_roi1[2]):int(real_roi1[3]),int(real_roi1[0]):int(real_roi1[1]),:],axis=(0,1))
-                self.update_spectrum1()
+        self.update_spectrum1()
+        self.update_spectrum2()
+
+    def onselect_function_spectrum_space(self, xmin, xmax):
+        indmin, indmax = np.searchsorted(self.energy, (xmin, xmax))
+        en_ranges=[xmin,xmax]
+        
+        self.update_image([indmin,indmax])
 
-            elif event.button == MouseButton.RIGHT:
-                # Right Click on Inelastic Image
-                real_roi2 = np.array(self.ui['roi2'].extents).astype('int')
-                self.spectrum2=np.mean(self.si[int(real_roi2[2]):int(real_roi2[3]),int(real_roi2[0]):int(real_roi2[1]),:],axis=(0,1))
-                self.update_spectrum2()
-        elif event.inaxes in [self.ax['spec']]:
-            if event.button == MouseButton.LEFT:
-                self.edge.e_int = self.ui['span_spec'].extents
-                self.update_image()
 
     ################### Update Functions ###################
     def update_spectrum1(self):
         self.h['spec1'].set_ydata(self.spectrum1)
         self.h['spec1'].set_color('maroon')
-        try:
-            self.ax['spec'].set_ylim([min(self.spectrum1.min(),self.spectrum2.min()),max(self.spectrum1.max(),self.spectrum2.max())])
-        except:
-            pass
+        self.ax['spec'].set_ylim([min(self.spectrum1.min(),self.spectrum2.min()),max(self.spectrum1.max(),self.spectrum2.max())])
         
     def update_spectrum2(self):
         self.h['spec2'].set_ydata(self.spectrum2)
         self.h['spec2'].set_alpha(1)
         self.h['spec2'].set_color('cadetblue')
-        try:
-            self.ax['spec'].set_ylim([min(self.spectrum1.min(),self.spectrum2.min()),max(self.spectrum1.max(),self.spectrum2.max())])
-        except:
-            pass
-
-    def update_image(self):
-        indmin, indmax = np.searchsorted(self.energy, self.edge.e_int)
-        self.im_inel = np.mean(self.si[:,:,indmin:indmax],axis=(-1))
-        self.h['inel'].set_data(self.im_inel)
+        self.ax['spec'].set_ylim([min(self.spectrum1.min(),self.spectrum2.min()),max(self.spectrum1.max(),self.spectrum2.max())])
+        
+    def update_image(self,  x):
+        new_im = np.mean(self.si[:,:,x[0]:x[1]],axis=(-1))
+        self.h['inel'].set_array(new_im)
         self.h['inel'].autoscale()
-
         
     def scale_button(self, event):
         if self.ax['spec'].get_yscale()=='linear':
             
             self.ax['spec'].set_yscale('log')
             self.ax['spec'].set_ylabel('Log Intensity')
             self.ax['spec'].set_yticks([])
         else:
             
             self.ax['spec'].set_yscale('linear')
             self.ax['spec'].set_ylabel('Intensity')
             self.ax['spec'].set_yticks([])
 
-    def dummy( self, *args ):
-        pass
+
+
 
 class fitbrowser:
 
     def __init__( self, si, energy, cmap='gray', figsize=(9,6), lc=False, gfwhm=10, log=True, 
                  ftol=0.0005, gtol=0.00005, xtol=None, maxfev = 50000, method='trf', edge=None):
         
         ## Initialize browser object
@@ -198,82 +185,78 @@
         for key in ['bsub_spectrum','image','bsub_SI','edge']:
             results_dict[key]=[]
 
         
         ##############Set Initial plot#################
         self.fig=plt.figure(figsize=figsize,layout='constrained')
 
-        self.ax = {'inel':None, 'spec':None, 'e_view':None, 'e_bsub':None, 'e_int':None,
-                    'btn_fit':None, 'btn_fint':None, 'btn_int':None, 'btn_save':None}
+        self.ax = {'inel':None, 'spec':None, 'slid':None, 'btn_fit':None, 'btn_fint':None, 'btn_int':None, 'btn_save':None}
         self.ax['inel']=self.fig.add_axes([0.025,0.1,0.45,0.8]) # Image
         self.ax['spec']=self.fig.add_axes([0.525,0.45,0.45,0.45]) # Spectrum
-        self.ax['e_view']=self.fig.add_axes([0.625,0.30,0.25,0.05]) # Range slider
-        self.ax['e_bsub']=self.fig.add_axes([0.625,0.25,0.25,0.05]) # Range slider
-        self.ax['e_int'] =self.fig.add_axes([0.625,0.20,0.25,0.05]) # Range slider
+        self.ax['slid']=self.fig.add_axes([0.625,0.3,0.25,0.05]) # Range slider
         self.ax['btn_fit']=self.fig.add_axes([0.520,0.1,0.125,0.1]) # Fit Buttons
         self.ax['btn_fint']=self.fig.add_axes([0.655,0.1,0.1,0.1]) # Fast Int Button
         self.ax['btn_int']=self.fig.add_axes([0.765,0.1,0.1,0.1]) # Int Button 
         self.ax['btn_save']=self.fig.add_axes([0.875,0.1,0.1,0.1]) # Save Button 
 
         ## Initialize plot handles
         self.h = {'inel':None, 'spec':None, 'bsub':None, 'fit':None}
         ################## ax['inel'] ######################
         self.h['inel'] = self.ax['inel'].imshow( self.im_inel,cmap = cmap)
         self.ax['inel'].set_axis_off()
         self.ax['inel'].set_title('Inelastic image')
 
-        ################## ax['spec'] #######################
+        ###################self.ax['spec']########################
         self.h['spec'], =self.ax['spec'].plot(energy, self.spectrum,color='k')
         self.h['bsub'], =self.ax['spec'].plot(energy, self.bsub,color='k',alpha=0)
         self.h['fit'],  =self.ax['spec'].plot(energy, self.fit,color='k',alpha=0)
         self.ax['spec'].axhline(0,color='k',linestyle='--',alpha=0.3)
         self.ax['spec'].set_ylim([self.spectrum.min(),self.spectrum.max()])
         self.ax['spec'].set_xlim([self.energy.min(),self.energy.max()])
         self.ax['spec'].set_yticks([])
         self.ax['spec'].set_xlabel('Energy (keV)')
         self.ax['spec'].set_ylabel('Intensity')
         self.ax['spec'].set_title('EELS spectrum')
 
         ## Initialize ui handles
-        self.ui = {'roi':None, 'spec1':None, 'spec2':None, 
-                   'slid_e_view':None, 'slid_e_bsub':None, 'slid_e_int':None,
-                   'rad_fit':None, 'btn_fint':None, 'btn_int':None, 'btn_save':None}
+        self.ui = {'roi':None, 'spec1':None, 'spec2':None, 'slid_e':None, 'rad_fit':None, 'btn_fint':None, 'btn_int':None, 'btn_save':None}
 
         ################### Selectors ###################
-        self.ui['roi'] = RectangleSelector(self.ax['inel'], self.dummy, button=[1],
+        self.ui['roi'] = RectangleSelector(self.ax['inel'], self.onselect_function_real_space, button=[1],
                                         useblit=True ,minspanx=1, minspany=1,spancoords='pixels',
                                         interactive=True,props=dict(facecolor='crimson',edgecolor='crimson',alpha=0.2,fill=True),
                                         handle_props=dict(markersize=2,markerfacecolor='white'))#,ignore_event_outside=True
         
             
-        self.ui['bsub'] = SpanSelector(self.ax['spec'], self.dummy, button=[1],
+        self.ui['bsub'] = SpanSelector(self.ax['spec'], self.onselect_function_spectrum_space1, button=[1],
                                             useblit=True, minspan=1,direction="horizontal",
                                             interactive=True,props=dict(facecolor='C0',edgecolor='C0',alpha=0.2,fill=True),
                                             grab_range=10, drag_from_anywhere=True)
         
-        self.ui['int'] = SpanSelector(self.ax['spec'], self.dummy, button=[3],
+        self.ui['int'] = SpanSelector(self.ax['spec'], self.onselect_function_spectrum_space2, button=[3],
                                             useblit=True, minspan=1,direction="horizontal",
                                             interactive=True,props=dict(facecolor='orange',edgecolor='orange',alpha=0.2,fill=True),
                                             grab_range=10, drag_from_anywhere=True)
         
 
-        self.ui['slid_e_view'] = RangeSlider(self.ax['e_view'],"Energy Range ",
-                                        energy[0], energy[-1], valinit=[energy[0],energy[-1]],
-                                        valstep=energy[1]-energy[0],dragging=True)
-        self.ui['slid_e_view'].on_changed( self.slider_view_action )
-        
-        self.ui['slid_e_bsub'] = RangeSlider(self.ax['e_bsub'],"Background ",
-                                            energy[0], energy[-1], valinit=[energy[0],energy[-1]],
-                                            valstep=energy[1]-energy[0],dragging=True)
-        self.ui['slid_e_bsub'].on_changed( self.slider_bsub_action )
-
-        self.ui['slid_e_int'] = RangeSlider(self.ax['e_int'],"Integration ",
-                                          energy[0],energy[-1],valinit=[energy[0],energy[-1]],
-                                          valstep=energy[1]-energy[0],dragging=True)
-        self.ui['slid_e_int'].on_changed( self.slider_int_action )
+        if edge is None:
+            self.edge = eels_edge( " ", (energy[0],energy[-1]), (energy[0],energy[-1]) )
+        else:
+            self.edge= edge
+
+            self.ui['bsub'].extents = self.edge.e_bsub
+            self.onselect_function_spectrum_space1()
+
+            self.ui['int'].extents = self.edge.e_int
+            self.onselect_function_spectrum_space2()
+        
+        
+        self.ui['slid_e'] = Eslider=RangeSlider(self.ax['slid'],"Energy Range ",energy[0],energy[-1],valinit=[energy[0],energy[-1]],
+                        valstep=energy[1]-energy[0],dragging=True)
+        self.ui['slid_e'].on_changed( self.slider_action )
 
 
         self.ax['btn_fit'].set_facecolor('0.85')
         self.ui['rad_fit'] = RadioButtons(self.ax['btn_fit'], ('Power law', 'Exponential', 'Linear'),
                             label_props={'color': ['k','k','k'], 'fontsize': [10, 10, 10]},
                             radio_props={'s': [16,16,16]})
         
@@ -282,171 +265,133 @@
         self.ui['btn_fint']=Button(self.ax['btn_fint'],"Fast Integrate",useblit=True,)
         self.ui['btn_fint'].on_clicked(self.fint_button)
 
         self.ui['btn_int']=Button(self.ax['btn_int'],"Integrate",useblit=True,)
         self.ui['btn_int'].on_clicked(self.int_button)
 
         self.ui['btn_save']=Button(self.ax['btn_save'],'Save results')
-
-
-        self.fig.canvas.mpl_connect( 'motion_notify_event', 
-                                    lambda event: self.onclick_figure(event))
         # self.ui['btn_save'].on_clicked(self.add_save_dict)
         
         # selector_collection = (spectrum_span_selector1,spectrum_span_selector2,rect_selector,ibutton,fibutton,Eslider,save_button,fitradio)
-       
-        if edge is None:
-            self.edge = eels_edge( " ", (energy[0],energy[-1]), (energy[0],energy[-1]) )
-            self.ax['e_bsub'].set_visible(False)
-            self.ax['e_int'].set_visible(False)
-        else:
-            self.edge = edge
-            if self.edge.e_bsub is None:
-                self.edge.e_bsub = (energy[0],energy[-1])
-                self.ax['e_bsub'].set_visible(False)
-            else:
-                self.fit_check = True
-                self.ui['slid_e_bsub'].set_val( self.edge.e_bsub )
-
-            if self.edge.e_int is None:
-                self.edge.e_int = (energy[0],energy[-1])
-                self.ax['e_int'].set_visible(False)
-            else:
-                self.ui['slid_e_int'].set_val( self.edge.e_int )
-
+        
         
         # return results_dict,selector_collection
 
     ################### Update Functions ###################
     def update_spectrum(self):
         self.h['spec'].set_ydata( self. spectrum)
         self.h['spec'].set_color('k')
         self.rescale_yrange()
         
-    def update_fit(self):
-        ind_min = np.searchsorted( self.energy, self.edge.e_bsub[0])
-
+    def update_fit(self,  ind):
         self.h['bsub'].set_ydata(self.bsub)
         self.h['bsub'].set_color('C1')
         self.h['bsub'].set_alpha(1)
-        self.h['fit'].set_data( self.energy[ind_min:], self.spectrum[ind_min:]-self.bsub[ind_min:])
+        self.h['fit'].set_data( self.energy[ind:], self.spectrum[ind:]-self.bsub[ind:])
         self.h['fit'].set_color('C0')
         self.h['fit'].set_alpha(1)
         self.rescale_yrange()
         
     def update_image(self):
-        self.bsub_array = bgsub_SI_fast( self.si, self.energy, self.edge, self.r, fit=self.fitfunction )
-        ind_min, ind_max = np.searchsorted(self.energy, self.edge.e_int)
-        self.im_inel = np.mean( self.bsub_array[:,:,ind_min:ind_max],axis=(-1))
+        self.bsub_array = bgsub_fast(self.si, self.energy,self.edge.e_bsub,self.r,fit = self.fitfunction)
+        indmin, indmax = np.searchsorted(self.energy, self.edge.e_int)
+        self.im_inel = np.mean( self.bsub_array[:,:,indmin:indmax],axis=(-1))
         self.h['inel'].set_array( self.im_inel)
         self.h['inel'].autoscale()
         
     def update_image_2(self):
 
         if self.lc:
-            _,self.bsub_array = bgsub_SI( self.si, self.energy, self.edge, gfwhm=self.gfwhm,fit=self.fitfunction,lc=self.lc,log=self.log,
+            _,self.bsub_array = bgsub_SI(self.si, self.energy,self.edge.e_bsub,gfwhm=self.gfwhm,fit=self.fitfunction,lc=self.lc,log=self.log,
                                     ftol=self.ftol,gtol=self.gtol,xtol=self.xtol,maxfev=self.maxfev,method=self.method)
         else:
-            self.bsub_array =   bgsub_SI( self.si, self.energy, self.edge, gfwhm=self.gfwhm,fit=self.fitfunction,lc=self.lc,log=self.log,
+            self.bsub_array =   bgsub_SI(self.si, self.energy,self.edge.e_bsub,gfwhm=self.gfwhm,fit=self.fitfunction,lc=self.lc,log=self.log,
                                     ftol=self.ftol,gtol=self.gtol,xtol=self.xtol,maxfev=self.maxfev,method=self.method)
         indmin, indmax = np.searchsorted(self.energy, self.edge.e_int)
         self.im_inel = np.mean(self.bsub_array[:,:,indmin:indmax],axis=(-1))
         self.h['inel'].set_array(self.im_inel)
         self.h['inel'].autoscale()
 
-    def slider_bsub_action(self, erange):
-        self.ui['bsub'].extents = erange
-        self.edge.e_bsub = erange
-        self.bsub, fit_param = bgsub_SI_linearized( self.spectrum, self.energy, self.edge, fit=self.fitfunction)
-        self.r = fit_param[1]
-        self.update_fit()
-
-    def slider_int_action(self, erange):
-        self.ui['int'].extents = erange
-        self.edge.e_int = erange
-
-    def slider_view_action(self, erange):
+    def slider_action(self, erange):
 
         self.slider_check=True
         slidermin, slidermax = np.searchsorted(self.energy, (erange[0],erange[1]))
         self.slider_window = [slidermin, slidermax]
         self.ax['spec'].set_xlim([erange[0],erange[1]])
 
         self.rescale_yrange()
 
     def rescale_yrange(self):
-        try:
-            if self.slider_check:
-                slidermin,slidermax = self.slider_window
-                if self.fit_check:
-                    self.ax['spec'].set_ylim([min(self.bsub[slidermin:slidermax].min(),-1*self.bsub[slidermin:slidermax].min()),self.spectrum[slidermin:slidermax].max()])
-                else:
-                    self.ax['spec'].set_ylim([self.spectrum[slidermin:slidermax].min(),self.spectrum[slidermin:slidermax].max()])
+        if self.slider_check:
+            slidermin,slidermax = self.slider_window
+            if self.fit_check:
+                self.ax['spec'].set_ylim([min(self.bsub[slidermin:slidermax].min(),-1*self.bsub[slidermin:slidermax].min()),self.spectrum[slidermin:slidermax].max()])
             else:
-                if self.fit_check:
-                    self.ax['spec'].set_ylim([min(self.bsub.min(),-1*self.bsub.min()),self.spectrum.max()])
-                else:
-                    self.ax['spec'].set_ylim([self.spectrum.min(),self.spectrum.max()])
-        except:
-            pass
+                self.ax['spec'].set_ylim([self.spectrum[slidermin:slidermax].min(),self.spectrum[slidermin:slidermax].max()])
+        else:
+            if self.fit_check:
+                self.ax['spec'].set_ylim([min(self.bsub.min(),-1*self.bsub.min()),self.spectrum.max()])
+            else:
+                self.ax['spec'].set_ylim([self.spectrum.min(),self.spectrum.max()])
 
     ############### Event Handlers ###################
-    def onclick_figure( self, event ):
-        if event.inaxes in [self.ax['inel']]:
-            if event.button == MouseButton.LEFT:
-                # Left Click on Inelastic Image
-                real_roi = np.array( self.ui['roi'].extents).astype('int')
-                self.spectrum=np.mean( self.si[int(real_roi[2]):int(real_roi[3]),int(real_roi[0]):int(real_roi[1]),:],axis=(0,1))
+    def onselect_function_real_space(self, eclick, erelease):
+        
+        real_roi = np.array( self.ui['roi'].extents).astype('int')
+        self.spectrum=np.mean( self.si[int(real_roi[2]):int(real_roi[3]),int(real_roi[0]):int(real_roi[1]),:],axis=(0,1))
 
-                self.update_spectrum()
-                
-                if self.fit_check:
-                    self.bsub, fit_param = bgsub_SI_linearized( self.spectrum, self.energy, self.edge, fit=self.fitfunction)
-                    self.r = fit_param[1]
-                    self.update_fit()
+        self.update_spectrum()
+        
+        if self.fit_check:
+            [xmin,xmax] = self.edge.e_bsub
+            indmin, indmax = np.searchsorted(self.energy, (xmin, xmax))
+            self.bsub, self.r = bgsub_1D(self.spectrum,self.energy,self.edge.e_bsub,fit =  self.fitfunction)
+            self.update_fit(indmin)
 
-        elif event.inaxes in [self.ax['spec']]:
-            if event.button == MouseButton.LEFT:
-                self.fit_check = True
-                self.ax['e_bsub'].set_visible(True)
-                self.ui['slid_e_bsub'].set_val( self.ui['bsub'].extents )
+    def onselect_function_spectrum_space1( self, e_min, e_max ):
+        
+        self.fit_check = True
+        indmin, indmax = np.searchsorted( self.energy, (e_min, e_max) ) 
+        self.edge.e_bsub = ( self.energy[indmin], self.energy[indmax] )
 
-            elif event.button == MouseButton.RIGHT:
-                self.int_check = True
-                self.ax['e_int'].set_visible(True)
-                self.ui['slid_e_int'].set_val( self.ui['int'].extents )
 
+        self.bsub, self.r = bgsub_1D(self.spectrum, self.energy, self.edge.e_bsub, fit = self.fitfunction)
+
+        self.update_fit(indmin)
+
+    def onselect_function_spectrum_space2( self, e_min, e_max ):
+
+        self.int_check = True
+        indmin, indmax = np.searchsorted(self.energy, (e_min, e_max) ) 
+        self.edge.e_int = (self.energy[indmin],self.energy[indmax])
 
     def fitcheck(self, label):
         fitdict = {'Power law': 'pl', 'Exponential': 'exp', 'Linear': 'lin'}
         self.fitfunction = fitdict[label]
         if self.fit_check:
-            self.bsub, fit_param = bgsub_SI_linearized( self.spectrum, self.energy, self.edge, fit=self.fitfunction)
-            self.r = fit_param[1]
-            self.update_fit()
+            [xmin,xmax] = self.edge.e_bsub
+            indmin, indmax = np.searchsorted(self.energy, (xmin, xmax))
+            self.bsub, self.r = bgsub_1D(self.spectrum,self.energy,self.edge.e_bsub,fit = self.fitfunction)
+            self.update_fit(indmin)
         
     def fint_button(self, event):
         if (self.int_check & self.fit_check):
             self.update_image()
 
     def int_button(self, event):
         if (self.int_check & self.fit_check):
             self.update_image_2()
 
-    def dummy(self, *args):
-        pass
-
     # def add_save_dict(event):
     #     results_dict['bsub_spectrum'] = bsub
     #     results_dict['image'] = inel_im
     #     results_dict['bsub_SI'] = bsub_array
     #     results_dict['edge'] = [fit_window[0],fit_window[1],int_window[0],int_window[1]]
 
 
- 
 
 
 class SI :
     def __init__( self, im_si, ADF=[], es=[] ):
 
         im_si[np.isnan(im_si)] = 0
         self.si = im_si
@@ -1079,194 +1024,178 @@
         """
         array = np.asarray(array)
         idx = (np.abs(array - value)).argmin()
         return array[idx]
     
         
 
-########### background subtractions ########
-def bgsub_SI_fast( si, energy, edge, rval, fit='pl'):
-    """
-    Quick background subtraction based on fixed 'r' value
-    For Y = Ax + b + error with fixed 'A':
-        Y' = b + error. MSE is minimized when b = mean(Y)
+def bgsub_1D(raw_data, energy_axis, edge, **kwargs):
     """
-    xdim, ydim, zdim = np.shape( si )
-
-    fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
-    y_win = si[:,:,fit_start_ch:fit_end_ch]
-    e_win = np.reshape( energy[fit_start_ch:fit_end_ch], (1,1,(fit_end_ch-fit_start_ch)) )
-    e_sub = np.reshape( energy[fit_start_ch:], (1,1,zdim-fit_start_ch) )
-
-    bg_SI = np.zeros_like( si )  
-
-    if fit == 'lin':
-        c_fit = np.reshape( np.mean( y_win-rval*e_win, axis=(2)), (xdim,ydim,1))
-        y_fit = c_fit + rval*e_sub
-
-    if fit == 'pl':
-        c_fit = np.reshape( np.mean( np.log(y_win)-rval*np.log(e_win), axis=(2)), (xdim,ydim,1))
-        y_fit = np.exp( c_fit + rval*np.log(e_sub) )
+    Full background subtraction function for the 1D case-
+    Optional LBA, log fitting, LCPL, and exponential fitting.
+    For more information on non-linear fitting function, see information at https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.curve_fit.html
 
-    if fit == 'exp':
-        c_fit = np.reshape( np.mean( np.log(y_win)-rval*e_win, axis=(2)), (xdim,ydim,1))
-        y_fit = np.exp( c_fit + rval*e_sub )
+    Inputs:
+    raw_data - 1D spectrum
+    energy_axis - corresponding energy axis
+    edge - edge parameters defined by KEM convention
 
-    bg_SI[:,:,fit_start_ch:] = si[:,:,fit_start_ch:] - y_fit
-    return bg_SI
+    **kawrgs:
+    fit - choose the type of background fit, default == 'pl' == Power law. Can also use 'exp'== Exponential, 'lin' == Linear, 'lcpl' == LCPL.
+    log - Boolean, if true, log transform data and fit using QR factorization, default == False.
+    nstd - Standard deviation spread of r error from non-linear power law fitting. Default == 100.
+    ftol - default to 0.0005, Relative error desired in the sum of squares.
+    gtol - default to 0.00005, Orthogonality desired between the function vector and the columns of the Jacobian.
+    xtol - default to None, Relative error desired in the approximate solution.
+    maxfev - default to 50000, Only change if you are consistenly catching runtime errors and loosening gtol/ftols are not making a good enough fit.
+    method - default is 'trf', see https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.least_squares.html#scipy.optimize.least_squares for description of methods
+    Note: may need stricter tolerances on ftol/gtol for noisier data. Anecdotally, a stricter gtol (as low as 1e-8) has a larger effect on the quality of the bgsub.
 
-def bgsub_SI_linearized( si, energy, edge, fit='pl'):
-    """
-    Quick background subtraction based on fixed 'r' value
-    For Y = Ax + b + error with fixed 'A':
-        Y' = b + error. MSE is minimized when b = mean(Y)
+    Outputs:
+    bg_1D - background spectrum
     """
+    fit_start_ch = eVtoCh(edge[0], energy_axis)
+    fit_end_ch = eVtoCh(edge[1], energy_axis)
+    zdim = len(raw_data)
+    ewin = energy_axis[fit_start_ch:fit_end_ch]
+    esub = energy_axis[fit_start_ch:]
+    bg_1D = np.zeros_like(raw_data)
+    fy = np.zeros((1,zdim))
+    fy[0,:] = raw_data
 
-    fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
-    if (fit_end_ch - fit_start_ch)<2:
-        fit_end_ch = fit_start_ch+2
-    e_win = np.atleast_2d( energy[fit_start_ch:fit_end_ch] ).T
-    e_sub = np.atleast_2d( energy[fit_start_ch:] ).T
-    zdim = len(energy)
-
-    if si.ndim == 1:
-        si = np.reshape( si, (1,1,zdim))
-    elif si.ndim == 2:
-        (nx,nz) = si.shape
-        si = np.reshape( si,(nx,1,zdim))
-
-    xdim, ydim, zdim = np.shape( si )
-    y_win = si[:,:,fit_start_ch:fit_end_ch]
-    y_win = np.reshape( y_win, (xdim*ydim, len(e_win))).T
-
-    bg_SI = np.zeros_like( si )  
-    if fit == 'lin':
-        e_win = np.insert( e_win, 0, 1, axis=1)
-        e_sub = np.insert( e_sub, 0, 1, axis=1)
-
-        b_fit = linear_regression_QR( y_win, e_win)
-        y_fit = e_sub @ b_fit
-
-    if fit == 'pl':
-        e_win = np.insert( np.log(e_win), 0, 1, axis=1)
-        e_sub = np.insert( np.log(e_sub), 0, 1, axis=1)
-
-        b_fit = linear_regression_QR( np.log(y_win), e_win )
-        y_fit = np.exp(e_sub @ b_fit )
-        
-        b_fit[0,:] = np.exp( b_fit[0,:] )
-
-    if fit == 'exp':
-        e_win = np.insert( e_win, 0, 1, axis=1)
-        e_sub = np.insert( e_sub, 0, 1, axis=1)
-
-        b_fit = linear_regression_QR( np.log(y_win), e_win )
-        y_fit = np.exp(e_sub @ b_fit )
 
-        b_fit[0,:] = np.exp( b_fit[0,:] )
-
-    b_fit = np.squeeze( np.reshape( b_fit, (2,xdim,ydim)) )
-    y_fit = np.reshape( y_fit.T, (xdim,ydim,len(e_sub)))
-    bg_SI[:,:,fit_start_ch:] = si[:,:,fit_start_ch:] - y_fit
-    bg_SI = np.squeeze( bg_SI )
-    return bg_SI, b_fit
-
-def bgsub_SI_nllsq( si, energy, edge, fit='pl',gfwhm=None, 
-                   maxfev=50000, method='trf', ftol=0.0005, gtol=0.00005, xtol=None):
     """
-    Quick background subtraction based on fixed 'r' value
-    For Y = Ax + b + error with fixed 'A':
-        Y' = b + error. MSE is minimized when b = mean(Y)
+            elif fit == 'lcpl':
+                fitfunc = lcpowerlaw
     """
+    """
+## Either fast fitting -> log fitting, Or slow fitting -> non-linear fitting
+    if 'log' in kwargs.keys():
+        log = kwargs['log']
+    else:
+        log = True
 
-    fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
-    e_win = energy[fit_start_ch:fit_end_ch]
-    e_sub = energy[fit_start_ch:]
-    zdim = len(energy)
-
-    if si.ndim == 1:
-        si = np.reshape( si, (1,1,zdim))
-    elif si.ndim == 2:
-        (nx,nz) = si.shape
-        si = np.reshape( si,(nx,1,zdim))
-
-    xdim, ydim, zdim = np.shape( si )
-    y_win = si[:,:,fit_start_ch:fit_end_ch]
-    bg_SI = np.zeros_like( si )
-
-    if fit == 'pl':
-        fitfunc = ls.powerlaw
-        fit_params = np.zeros(2,xdim,ydim)
-    elif fit == 'exp':
-        fitfunc = ls.exponential
-        fit_params = np.zeros(2,xdim,ydim)
-
-    mean_spec = np.mean( y_win, (0,1) )
-    popt_init,pcov_init = curve_fit( fitfunc, e_win, mean_spec, maxfev=maxfev,method=method,verbose=0 )
-    
-    pbar1 = tqdm(total = (xdim)*(ydim),desc = "Background subtracting")
-    for i in range(xdim):
-        for j in range(ydim):
-            popt_pl,pcov_pl=curve_fit( fitfunc, e_win, y_win[i,j,:],p0=popt_init,
-                                      maxfev=maxfev,method=method,verbose = 0,
-                                      ftol=ftol, gtol=gtol, xtol=xtol)
-            
-            bg_SI[i,j,fit_start_ch:] = si[i,j,fit_start_ch:] - fitfunc(energy[fit_start_ch:], *popt_pl)
-            fit_params[:,i,j] = popt_pl
-            pbar1.update(1)
-
-    return bg_SI, fit_params
-
-def bgsub_SI_LC(si, energy, edge, rline, fit='pl', nstd=2):
-    bg_lcpl_SI = np.zeros_like(si)
-    rmu,rstd = norm.fit(rline)
-    rmin = rmu - nstd*rstd
-    rmax = rmu + nstd*rstd
+## Fitting parameters for non-linear curve fitting if non-log based fitting
+        if 'ftol' in kwargs.keys():
+            ftol = kwargs['ftol']
+        else:
+            ftol = 1e-8
+        if 'gtol' in kwargs.keys():
+            gtol = kwargs['gtol']
+        else:
+            gtol = 1e-8
+        if 'xtol' in kwargs.keys():
+            xtol = kwargs['xtol']
+        else:
+            xtol = 1e-8
+        if 'maxfev' in kwargs.keys():
+            maxfev = kwargs['maxfev']
+        else:
+            maxfev = 50000
+        if 'method' in kwargs.keys():
+            method = kwargs['method']
+        else:
+            method = 'trf'
+    """
+## Determine if fitting is power law or exponenetial
+    if 'fit' in kwargs.keys():
+        fit = kwargs['fit']
+        if fit == 'exp':
+            fitfunc = exponential
+        elif fit == 'pl':
+            fitfunc = powerlaw
+        elif fit == 'lin':
+            fitfunc = linear
+        else:
+            print('Did not except fitting function, please use either \'pl\' for powerlaw, \'exp\' for exponential, \'lin\' for linear or \'lcpl\' for LCPL.')
+    else:
+        fitfunc = powerlaw
 
-    (xdim, ydim, zdim) = si.shape
-    fit_start_ch, fit_end_ch = np.searchsorted(energy, edge.e_bsub)
 
-    
-    if fit=='pl':
-        fitname = 'power law'
-        e_win = np.log(energy[fit_start_ch:fit_end_ch])
-        e_sub = np.log(energy[fit_start_ch:])
-    elif fit=='exp':
-        fitname = 'exponential'
-        e_win = energy[fit_start_ch:fit_end_ch]
-        e_sub = energy[fit_start_ch:]
-
-    if nstd == 2:
-        print( '5th percentile {} = {}'.format( fitname, rmin))
-        print('95th percentile {} = {}'.format( fitname, rmax))
-    elif nstd == 1:
-        print('20th percentile {} = {}'.format( fitname, rmin))
-        print('80th percentile {} = {}'.format( fitname, rmax))
-    else:
-        print('Min {} = {}'.format( fitname, rmin))
-        print('Max {} = {}'.format( fitname, rmax))
 
+## If fast fitting linear background, find fit using qr factorization
+    if fitfunc==linear:
+        Blin = fy[:,fit_start_ch:fit_end_ch]
+        Alin = np.zeros((len(ewin),2))
+        Alin[:,0] = np.ones(len(ewin))
+        Alin[:,1] = ewin
+        Xlin = qrnorm(Alin,Blin.T)
+        Elin = np.zeros((len(esub),2))
+        Elin[:,0] = np.ones(len(esub))
+        Elin[:,1] = esub
+        bgndLINline = np.dot(Xlin.T,Elin.T)
+        bg_1D[fit_start_ch:] = raw_data[fit_start_ch:] - bgndLINline
+        rval = np.squeeze(Xlin[1,:])
+
+## If fast log fitting and powerlaw, find fit using qr factorization
+    elif fitfunc==powerlaw:
+        Blog = fy[:,fit_start_ch:fit_end_ch]
+        Alog = np.zeros((len(ewin),2))
+        Alog[:,0] = np.ones(len(ewin))
+        Alog[:,1] = np.log(ewin)
+        Xlog = qrnorm(Alog,np.log(abs(Blog.T)))
+        Elog = np.zeros((len(esub),2))
+        Elog[:,0] = np.ones(len(esub))
+        Elog[:,1] = np.log(esub)
+        bgndPLline = np.exp(np.dot(Xlog.T,Elog.T))
+        bg_1D[fit_start_ch:] = raw_data[fit_start_ch:] - bgndPLline
+        rval = np.squeeze(Xlog[1,:])
+
+## If fast log fitting and exponential, find fit using qr factorization
+    elif fitfunc==exponential:
+        Bexp = fy[:,fit_start_ch:fit_end_ch]
+        Aexp = np.zeros((len(ewin),2))
+        Aexp[:,0] = np.ones(len(ewin))
+        Aexp[:,1] = ewin
+        Xexp = qrnorm(Aexp,np.log(abs(Bexp.T)))
+        Eexp = np.zeros((len(esub),2))
+        Eexp[:,0] = np.ones(len(esub))
+        Eexp[:,1] = esub
+        bgndEXPline = np.exp(np.dot(Xexp.T,Eexp.T))
+        bg_1D[fit_start_ch:] = raw_data[fit_start_ch:] - bgndEXPline
+        rval = np.squeeze(Xexp[1,:])
+    """
 
-    e_win = np.atleast_2d( energy[fit_start_ch:fit_end_ch] ).T
-    e_win = np.append( e_win**(-rmin), e_win**(-rmax), axis=1)
-    e_sub = np.atleast_2d( energy[fit_start_ch:] )
-    e_sub = np.append( e_sub**(-rmin), e_sub**(-rmax), axis=1)
-    
-    y_win = np.reshape( si[:,:,fit_start_ch:fit_end_ch], (xdim*ydim,len(e_win) ) )
-    b_fit = linear_regression_QR( y_win, e_win )
-    y_fit = e_sub @ b_fit
 
-    bgndLCPL = np.reshape( y_fit,(xdim,ydim,len(e_sub)))
-    bg_lcpl_SI[:,:,fit_start_ch:] = si[:,:,fit_start_ch:] - bgndLCPL
 
-    return 1, bg_lcpl_SI
+## Power law non-linear curve fitting using scipy.optimize.curve_fit
+    elif ~log & (fitfunc==powerlaw):
+        popt_pl,pcov_pl=curve_fit(powerlaw, ewin, raw_data[fit_start_ch:fit_end_ch],maxfev=maxfev,method=method,
+                                  verbose = 0, ftol=ftol, gtol=gtol, xtol=xtol)
+        c,r = popt_pl
+        bg_1D[fit_start_ch:] = raw_data[fit_start_ch:] - powerlaw(energy_axis[fit_start_ch:],c,r)
+
+## Exponential non-linear curve fitting using scipy.optimize.curve_fit
+    elif ~log & (fitfunc==exponential):
+        popt_exp,pcov_exp=curve_fit(exponential, ewin, raw_data[fit_start_ch:fit_end_ch],maxfev=maxfev,method=method,
+                                    verbose = 0,p0=[0,0], ftol=ftol, gtol=gtol, xtol=xtol)
+        a,b = popt_exp
+        bg_1D[fit_start_ch:] = raw_data[fit_start_ch:] - exponential(energy_axis[fit_start_ch:],a,b)
+
+## LCPL non-linear curve fitting using scipy.optimize.curve_fit
+    elif fitfunc==lcpowerlaw:
+        if 'nstd' in kwargs.keys():
+            nstd = kwargs['nstd']
+        else:
+            nstd = 100
+        popt_pl,pcov_pl=curve_fit(powerlaw, ewin, raw_data[fit_start_ch:fit_end_ch],maxfev=maxfev,method=method,
+                                  verbose = 0, ftol=ftol, gtol=gtol, xtol=xtol)
+        c,r = popt_pl
+        perr = np.sqrt(np.diag(pcov_pl))
+        rstd = perr[1]
+        popt_lcpl,pcov_lcpl=curve_fit(lcpowerlaw, ewin, raw_data[fit_start_ch:fit_end_ch],maxfev=maxfev,method=method,
+                                    verbose = 0,p0=[c/2,r-nstd*rstd,c/2,r+nstd*rstd], ftol=ftol, gtol=gtol, xtol=xtol)
+        c1,r1,c2,r2 = popt_lcpl
+        bg_1D[fit_start_ch:] = raw_data[fit_start_ch:] - lcpowerlaw(energy_axis[fit_start_ch:],c1,r1,c2,r2)
+    """
+    return bg_1D,rval
+ 
 
 
-def bgsub_SI(si, energy, edge, log=False, fit='pl', gfwhm=None, lc=False,
-             maxfev=50000, method='trf', ftol=0.0005, gtol=0.00005, xtol=None, **kwargs):
+def bgsub_SI(raw_data, energy_axis, edge, **kwargs):
     """
     Full background subtraction function-
     Optional LBA, log fitting, LCPL, and exponential fitting.
     For more information on non-linear fitting function, see information at https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.curve_fit.html
 
     Inputs:
     raw_data - SI
@@ -1290,87 +1219,461 @@
 
     Outputs:
     if lcpl == False:
         bg_pl_SI - background subtracted SI
     if lcpl == True:
         bg_pl_SI, bg_lcpl_SI - background subtracted SI, LCPL background subtracted SI
     """
+    fit_start_ch = eVtoCh(edge[0], energy_axis)
+    fit_end_ch = eVtoCh(edge[1], energy_axis)
+    raw_data = raw_data.astype('float32')
+    if len(np.shape(raw_data)) == 2:
+        tempx,tempz = np.shape(raw_data)
+        raw_data = np.reshape(raw_data,(tempx,1,tempz))
+    if len(np.shape(raw_data)) == 1:
+        tempz = len(raw_data)
+        raw_data = np.reshape(raw_data,(1,1,tempz))
+    xdim, ydim, zdim = np.shape(raw_data)
+    ewin = energy_axis[fit_start_ch:fit_end_ch]
+    esub = energy_axis[fit_start_ch:]
+    bg_pl_SI = np.zeros_like(raw_data)
 
-    fit_start_ch, fit_end_ch = np.searchsorted( energy, edge.e_bsub)
-    si = si.astype('float32')
-    if len(np.shape(si)) == 2:
-        tempx,tempz = np.shape(si)
-        si = np.reshape(si,(tempx,1,tempz))
-    if len(np.shape(si)) == 1:
-        tempz = len(si)
-        si = np.reshape(si,(1,1,tempz))
-    xdim, ydim, zdim = np.shape(si)
-
-    ## Special case: if there is vacuum in the SI and it is causing trouble with your LCPL fitting:
+## Special case: if there is vacuum in the SI and it is causing trouble with your LCPL fitting:
     if 'mask' in kwargs.keys():
-        mask = kwargs['mask']
+        threshmask = kwargs['mask']
     elif 'threshold' in kwargs.keys():
         thresh = kwargs['threshold']
-        mean_back = np.mean(si[:,:,fit_start_ch:fit_end_ch],axis=2)
-        mask = mean_back > thresh
+        mean_back = np.mean(raw_data[:,:,fit_start_ch:fit_end_ch],axis=2)
+        threshmask = mean_back > thresh
     else:
-        mask = np.ones((xdim,ydim), dtype='bool')
+        mask = np.ones((xdim,ydim))
+        threshmask = mask == 1
 
-    ## Apply Local Background Averaging
-    if gfwhm is not None:
-        fit_data = prepare_lba( si, gfwhm, fit_start_ch, fit_end_ch )
+    if 'gfwhm' in kwargs.keys():
+        gfwhm = kwargs['gfwhm']
+        lba_raw = np.copy(raw_data)
+        lba_raw_normalized = np.copy(lba_raw)
+        for energychannel in np.arange(fit_start_ch,fit_end_ch):
+            lba_raw[:,:,energychannel] = gaussian_filter(raw_data[:,:,energychannel],sigma=gfwhm/2.35)
+        pbar = tqdm(total = (xdim)*(ydim),desc = "Normalizing")
+        for i in range(xdim):
+            for j in range(ydim):
+                lba_mean = np.mean(lba_raw[i,j,fit_start_ch:fit_end_ch])
+                data_mean = np.mean(raw_data[i,j,fit_start_ch:fit_end_ch])
+                lba_raw_normalized[i,j,fit_start_ch:fit_end_ch] = lba_raw[i,j,fit_start_ch:fit_end_ch]*data_mean/lba_mean
+                pbar.update(1)
     else:
-        fit_data = si
-    
-    ## If log fitting or linear fitting, find fit using qr factorization       
-    if log | (fit=='lin'):
-        bg_pl_SI, fit_params = bgsub_SI_linearized( fit_data, energy, edge, fit=fit )
+        lba_raw_normalized = np.copy(raw_data)
+
+## Either fast fitting -> log fitting, Or slow fitting -> non-linear fitting
+    if 'log' in kwargs.keys():
+        log = kwargs['log']
+    else:
+        log = False
+
+## Fitting parameters for non-linear curve fitting if non-log based fitting
+    if 'ftol' in kwargs.keys():
+        ftol = kwargs['ftol']
+    else:
+        ftol = 0.0005
+    if 'gtol' in kwargs.keys():
+        gtol = kwargs['gtol']
+    else:
+        gtol = 0.00005
+    if 'xtol' in kwargs.keys():
+        xtol = kwargs['xtol']
+    else:
+        xtol = None
+    if 'maxfev' in kwargs.keys():
+        maxfev = kwargs['maxfev']
+    else:
+        maxfev = 50000
+    if 'method' in kwargs.keys():
+        method = kwargs['method']
+    else:
+        method = 'trf'
+
+## Determine if fitting is power law or exponenetial
+    if 'fit' in kwargs.keys():
+        fit = kwargs['fit']
+        if fit == 'exp':
+            fitfunc = exponential
+            bounds = ([0, 0], [np.inf, np.inf])
+        elif fit == 'pl':
+            fitfunc = powerlaw
+        elif fit == 'lin':
+            fitfunc = linear
+        else:
+            print('Did not except fitting function, please use either \'pl\' for powerlaw, \'exp\' for exponential or \'lin\' for linear.')
+    else:
+        fitfunc = powerlaw
 
-        maskline = np.reshape( mask,(xdim*ydim))
-        rline_long = -1*np.reshape( fit_params[1,:,:], (xdim*ydim) )
+## If fast fitting linear background, find fit using qr factorization
+    if fitfunc==linear:
+        Blin = np.reshape(lba_raw_normalized[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        Alin = np.zeros((len(ewin),2))
+        Alin[:,0] = np.ones(len(ewin))
+        Alin[:,1] = ewin
+        Xlin = qrnorm(Alin,Blin.T)
+        Elin = np.zeros((len(esub),2))
+        Elin[:,0] = np.ones(len(esub))
+        Elin[:,1] = esub
+        bgndLINline = np.dot(Xlin.T,Elin.T)
+        bgndLIN = np.reshape(bgndLINline,(xdim,ydim,len(esub)))
+        bg_pl_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndLIN
+
+## If fast log fitting and powerlaw, find fit using qr factorization
+    if log & (fitfunc==powerlaw):
+        Blog = np.reshape(lba_raw_normalized[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        Alog = np.zeros((len(ewin),2))
+        Alog[:,0] = np.ones(len(ewin))
+        Alog[:,1] = np.log(ewin)
+        Xlog = qrnorm(Alog,np.log(abs(Blog.T)))
+        Elog = np.zeros((len(esub),2))
+        Elog[:,0] = np.ones(len(esub))
+        Elog[:,1] = np.log(esub)
+        bgndPLline = np.exp(np.dot(Xlog.T,Elog.T))
+        bgndPL = np.reshape(bgndPLline,(xdim,ydim,len(esub)))
+        bg_pl_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndPL
+        maskline = np.reshape(threshmask,(xdim*ydim))
+        rline_long = -1*Xlog[1,:]
         rline = rline_long[maskline]
 
-    ## Power law non-linear curve fitting using scipy.optimize.curve_fit
-    elif (fit=='pl') | (fit=='exp') : 
-        bg_pl_SI, fit_params = bgsub_SI_nllsq( fit_data, energy, edge, fit=fit, 
-                                           maxfev=maxfev, method=method,
-                                           ftol=ftol, gtol=gtol, xtol=xtol )
-
-    ## Given r values of SI, refit background using a linear combination of power laws, 
-    ## using either 5/95 percentile or 20/80 percentile r values.
-    if lc:
-        bg_pl_SI, bg_lcpl_SI = bgsub_SI_LC(si, energy, edge, rline, fit=fit, nstd=2)
+## If fast log fitting and exponential, find fit using qr factorization
+    elif log & (fitfunc==exponential):
+        Bexp = np.reshape(lba_raw_normalized[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        Aexp = np.zeros((len(ewin),2))
+        Aexp[:,0] = np.ones(len(ewin))
+        Aexp[:,1] = ewin
+        Xexp = qrnorm(Aexp,np.log(abs(Bexp.T)))
+        Eexp = np.zeros((len(esub),2))
+        Eexp[:,0] = np.ones(len(esub))
+        Eexp[:,1] = esub
+        bgndEXPline = np.exp(np.dot(Xexp.T,Eexp.T))
+        bgndEXP = np.reshape(bgndEXPline,(xdim,ydim,len(esub)))
+        bg_pl_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndEXP
+        maskline = np.reshape(threshmask,(xdim*ydim))
+        bline_long = -1*Xexp[1,:]
+        bline = bline_long[maskline]
+
+## Power law non-linear curve fitting using scipy.optimize.curve_fit
+    elif ~log & (fitfunc==powerlaw):
+        rline = []
+        dummyspec = sum(sum(raw_data))/(xdim*ydim)
+        popt_init,pcov_init=curve_fit(powerlaw, ewin, dummyspec[fit_start_ch:fit_end_ch],maxfev=maxfev,method=method,verbose = 0)
+        pbar1 = tqdm(total = (xdim)*(ydim),desc = "Background subtracting")
+        for i in range(xdim):
+            for j in range(ydim):
+                popt_pl,pcov_pl=curve_fit(powerlaw, ewin, lba_raw_normalized[i,j,fit_start_ch:fit_end_ch],maxfev=maxfev,method=method,verbose = 0
+                                          ,p0=popt_init, ftol=ftol, gtol=gtol, xtol=xtol)
+                c,r = popt_pl
+                if threshmask[i,j]:
+                    rline = np.append(rline,r)
+                bg_pl_SI[i,j,fit_start_ch:] = raw_data[i,j,fit_start_ch:] - powerlaw(energy_axis[fit_start_ch:],c,r)
+                pbar1.update(1)
+
+## Exponential non-linear curve fitting using scipy.optimize.curve_fit
+    elif ~log & (fitfunc==exponential):
+        bline = []
+        # dummyspec = sum(sum(raw_data))/(xdim*ydim)
+        # popt_init,pcov_init=curve_fit(exponential, ewin, dummyspec[fit_start_ch:fit_end_ch],bounds=bounds,p0=[0,0],maxfev=maxfev,method=method,verbose = 0)
+        pbar1 = tqdm(total = (xdim)*(ydim),desc = "Background subtracting")
+        for i in range(xdim):
+            for j in range(ydim):
+                popt_exp,pcov_exp=curve_fit(exponential, ewin, lba_raw_normalized[i,j,fit_start_ch:fit_end_ch],maxfev=maxfev,method=method,verbose = 0
+                                          ,p0=[0,0], ftol=ftol, gtol=gtol, xtol=xtol)
+                a,b = popt_exp
+                if threshmask[i,j]:
+                    bline = np.append(bline,b)
+                bg_pl_SI[i,j,fit_start_ch:] = raw_data[i,j,fit_start_ch:] - exponential(energy_axis[fit_start_ch:],a,b)
+                pbar1.update(1)
+
+## Given r values of SI, refit background using a linear combination of power laws, using either 5/95 percentile or 20/80 percentile r values.
+    if 'lc' in kwargs.keys():
+        lc = kwargs['lc']
+    else:
+        lc = False
+
+    if lc & (fitfunc==powerlaw):
+        if 'nstd' in kwargs.keys():
+            nstd = kwargs['nstd']
+        else:
+            nstd = 2
+        bg_lcpl_SI = np.zeros_like(raw_data)
+        rmu,rstd = norm.fit(rline)
+        rmin = rmu - nstd*rstd
+        rmax = rmu + nstd*rstd
+        if nstd == 2:
+            print('5th percentile power law = {}'.format(rmin))
+            print('95th percentile power law = {}'.format(rmax))
+        elif nstd == 1:
+            print('20th percentile power law = {}'.format(rmin))
+            print('80th percentile power law = {}'.format(rmax))
+        else:
+            print('Min power law = {}'.format(rmin))
+            print('Max power law = {}'.format(rmax))
+        B = np.reshape(lba_raw_normalized[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        A = np.zeros((len(ewin),2))
+        A[:,0] = ewin**(-rmin)
+        A[:,1] = ewin**(-rmax)
+        X = qrnorm(A,B.T)
+        E = np.zeros((len(esub),2))
+        E[:,0] = esub**(-rmin)
+        E[:,1] = esub**(-rmax)
+        bgndLCPLline = np.dot(X.T,E.T)
+        bgndLCPL = np.reshape(bgndLCPLline,(xdim,ydim,len(esub)))
+        bg_lcpl_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndLCPL
         return bg_pl_SI, bg_lcpl_SI
+
+### Testing
+    elif lc & (fitfunc==exponential):
+        if 'nstd' in kwargs.keys():
+            nstd = kwargs['nstd']
+        else:
+            nstd = 2
+        bg_lcpl_SI = np.zeros_like(raw_data)
+        bmu,bstd = norm.fit(bline)
+        bmin = bmu - nstd*bstd
+        bmax = bmu + nstd*bstd
+        if nstd == 2:
+            print('5th percentile exponential = {}'.format(bmin))
+            print('95th percentile exponential = {}'.format(bmax))
+        elif nstd == 1:
+            print('20th percentile exponential = {}'.format(bmin))
+            print('80th percentile exponential = {}'.format(bmax))
+        else:
+            print('Min exponential = {}'.format(bmin))
+            print('Max exponential = {}'.format(bmax))
+        B = np.reshape(lba_raw_normalized[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        A = np.zeros((len(ewin),2))
+        A[:,0] = np.exp(-bmin*ewin)
+        A[:,1] = np.exp(-bmax*ewin)
+        X = qrnorm(A,B.T)
+        E = np.zeros((len(esub),2))
+        E[:,0] = np.exp(-bmin*esub)
+        E[:,1] = np.exp(-bmax*esub)
+        bgndLCPLline = np.dot(X.T,E.T)
+        bgndLCPL = np.reshape(bgndLCPLline,(xdim,ydim,len(esub)))
+        bg_lcpl_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndLCPL
+        return bg_pl_SI, bg_lcpl_SI
+
     else:
         return bg_pl_SI
     
-def prepare_lba( si, gfwhm, fit_start_ch, fit_end_ch ):
-    lba_raw = np.copy( si )
-    lba_normalized = np.copy( si )
-    for energychannel in np.arange(fit_start_ch,fit_end_ch):
-        lba_raw[:,:,energychannel] = gaussian_filter(si[:,:,energychannel],sigma=gfwhm/2.35)
-    
-    lba_mean = np.mean( lba_raw[:,:,fit_start_ch:fit_end_ch], 2 )
-    data_mean = np.mean(     si[:,:,fit_start_ch:fit_end_ch], 2)
 
-    for energychannel in np.arange(fit_start_ch,fit_end_ch):
-        lba_normalized[:,:,energychannel] = lba_raw[:,:,energychannel]*data_mean/lba_mean
+def bgsub_fast(raw_data, energy_axis, fit_window, rval,fit='pl'):
+
+    fit_start_ch = eVtoCh(fit_window[0], energy_axis)
+    fit_end_ch = eVtoCh(fit_window[1], energy_axis)
+    raw_data = raw_data.astype('float32')
+
+    xdim, ydim, zdim = np.shape(raw_data)
+    ewin = energy_axis[fit_start_ch:fit_end_ch]
+    esub = energy_axis[fit_start_ch:]
+    bg_SI = np.zeros_like(raw_data)  
+
+    if fit == 'lin':
+        B = np.reshape(raw_data[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        A = np.zeros((len(ewin),1))
+        A[:,0] = ewin*(rval)
+        X = qrnorm(A,B.T)
+        E = np.zeros((len(esub),1))
+        E[:,0] = esub*(rval)
+
+        bgndPLline = np.dot(X.T,E.T)
+        bgndPL = np.reshape(bgndPLline,(xdim,ydim,len(esub)))
+        bg_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndPL
+
+    if fit == 'pl':
+        B = np.reshape(raw_data[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        A = np.zeros((len(ewin),1))
+        A[:,0] = ewin**(rval)
+        X = qrnorm(A,B.T)
+        E = np.zeros((len(esub),1))
+        E[:,0] = esub**(rval)
+
+        bgndPLline = np.dot(X.T,E.T)
+        bgndPL = np.reshape(bgndPLline,(xdim,ydim,len(esub)))
+        bg_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndPL
+
+    if fit == 'exp':
+        B = np.reshape(raw_data[:,:,fit_start_ch:fit_end_ch],((xdim*ydim),len(ewin)))
+        A = np.zeros((len(ewin),1))
+        A[:,0] = np.exp(ewin*(rval))
+        X = qrnorm(A,B.T)
+        E = np.zeros((len(esub),1))
+        E[:,0] = np.exp(esub*(rval))
+
+        bgndPLline = np.dot(X.T,E.T)
+        bgndPL = np.reshape(bgndPLline,(xdim,ydim,len(esub)))
+        bg_SI[:,:,fit_start_ch:] = raw_data[:,:,fit_start_ch:] - bgndPL
+
+    return bg_SI
+
+
+def eVtoCh(energy, array):
+	return int(np.squeeze(np.argwhere(array == find_nearest(array,energy))))
+
+
+def find_nearest(array, value):
+    """
+    Inputs:
+    array - array...
+    value - value to search for in array
+
+    Outputs:
+    array[idx] - nearest value in array
+    """
+    array = np.asarray(array)
+    idx = (np.abs(array - value)).argmin()
+    return array[idx]
+
+
+def qrnorm(A,b):
+    """
+    Solve systems of linear equations Ax = b for x
+    """
+    q, r = LA.qr(A)
+    p = np.dot(q.T,b)
+    return np.dot(LA.inv(r),p)
+
+
+
+def linear(energy, a, b):
+    return a*energy + b
+
+def powerlaw(energy, c, r):
+    return c*energy**(-r)
+
+def lcpowerlaw(energy, c1, r1, c2, r2):
+    return c1*energy**(-r1) + c2*energy**(-r2)
+
+def exponential(energy,a,b):
+    return a*np.exp(-b*energy)
 
-    return lba_normalized
+
+class SIbrowser:
     
+    def __init__( self, si, energy, im_adf=None, cmap='gray', figsize=(9,4), **kwargs):
+        ######### Initialize browser object ##########
+        self.si = si
+        self.energy = energy
+        self.im_adf = im_adf
+        self.im_inel =np.mean(si,axis=(-1))
+        self.edge = eels_edge( "", e_bsub=None, e_int=(energy[0], energy[-1]))
 
-def linear_regression_QR( y, X ):
-    # Solve Linear Regression using QR Decomposition
-    # Y = Xb + error
-    # R*b = Q.T*y minimizes MSE
-    # y: (nx1) dependent variable
-    # x: (nx1) independent variable
-    # b: (2x1) [[b0],[b1]], b0: intercept, b1: slope
-    if y.ndim == 1:
-        Y = np.atleast_2d( y ).T
-    else:
-        Y = y
+        self.spectrum1=np.mean(si,axis=(0,1))
+        self.spectrum2=np.mean(si,axis=(0,1))
+        
+        ##############Initialize Display#################
+        self.fig=plt.figure(figsize=figsize)
 
-    Q, R = LA.qr(X)
-    b = LA.inv(R) @ (Q.T @ Y)
+        self.ax= {'inel':None,'spec':None,'bttn':None}
+        self.ax['inel']=self.fig.add_axes([0.05,0.3,0.425,0.6]) # Image
+        self.ax['spec']=self.fig.add_axes([0.55,0.3,0.425,0.6]) # Spectrum
+        self.ax['bttn']=self.fig.add_axes([0.88,0.012,0.1,0.2]) # Button
+        self.ax['bttn'].axis('off')
+        ##############################################
+        # Initialize plot handles
+        self.h = {'inel':None, 'spec1':None, 'spec2':None}
+
+        ## Inelastic Image
+        self.h['inel']  = self.ax['inel'].matshow(self.im_inel,cmap = cmap)
+        self.ax['inel'].set_axis_off()
+        self.ax['inel'].set_title('Inelastic image')
+        ## Spectra
+        self.h['spec1'], =self.ax['spec'].plot(self.energy,self.spectrum1,color='maroon')
+        self.h['spec2'], =self.ax['spec'].plot(self.energy,self.spectrum2,color='k',alpha=0)
 
-    return b
+        self.ax['spec'].set_ylim([self.spectrum1.min(),self.spectrum1.max()])
+        self.ax['spec'].set_xlim([self.energy.min(),self.energy.max()])
+        self.ax['spec'].set_yticks([])
+        self.ax['spec'].set_xlabel('Energy (keV)')
+        self.ax['spec'].set_ylabel('Intensity')
+        self.ax['spec'].set_title('EELS spectrum')
+        ##############################################
+        results_dict={}
+        for key in ['spectrum','image','roi','energy_span']:
+            results_dict[key]=[]
+        
+        ################### Selectors ###################
+        self.ui = {'roi1':None, 'roi2':None, 'spec':None, 'logscale':None}
+        self.ui['roi1'] = RectangleSelector(self.ax['inel'], self.dummy, button=[1],
+                                        useblit=False ,minspanx=1, minspany=1,spancoords='pixels',
+                                        interactive=True,props=dict(facecolor='crimson',edgecolor='crimson',alpha=0.2,fill=True),
+                                        handle_props=dict(markersize=2,markerfacecolor='white'))#,ignore_event_outside=True
+        
+        self.ui['roi2'] = RectangleSelector(self.ax['inel'], self.dummy, button=[3],
+                                        useblit=False ,minspanx=1, minspany=1,spancoords='pixels',
+                                        interactive=True,props=dict(facecolor='royalblue',edgecolor='royalblue',alpha=0.2,fill=True),
+                                        handle_props=dict(markersize=2,markerfacecolor='white'))#,ignore_event_outside=True)
+            
+        self.ui['span_spec'] = SpanSelector(self.ax['spec'], self.dummy, button=[1],
+                                            useblit=False, minspan=1,direction="horizontal",
+                                            interactive=True,props=dict(facecolor='green',edgecolor='green',alpha=0.2,fill=True),
+                                            grab_range=10, drag_from_anywhere=True)
+        
+
+        self.ui['logscale']=CheckButtons(self.ax['bttn'],["Log Scale"],useblit=True ,)
+        self.ui['logscale'].on_clicked(self.scale_button)
+
+        self.fig.canvas.mpl_connect( 'motion_notify_event', 
+                                    lambda event: self.onclick_figure(event))
+
+    ############### Event Handlers ###################
+    def onclick_figure( self, event ):
+        if event.inaxes in [self.ax['inel']]:
+            if event.button == MouseButton.LEFT:
+                # Left Click on Inelastic Image
+                real_roi1 = np.array(self.ui['roi1'].extents).astype('int')
+                self.spectrum1=np.mean(self.si[int(real_roi1[2]):int(real_roi1[3]),int(real_roi1[0]):int(real_roi1[1]),:],axis=(0,1))
+                self.update_spectrum1()
+
+            elif event.button == MouseButton.RIGHT:
+                # Right Click on Inelastic Image
+                real_roi2 = np.array(self.ui['roi2'].extents).astype('int')
+                self.spectrum2=np.mean(self.si[int(real_roi2[2]):int(real_roi2[3]),int(real_roi2[0]):int(real_roi2[1]),:],axis=(0,1))
+                self.update_spectrum2()
+        elif event.inaxes in [self.ax['spec']]:
+            if event.button == MouseButton.LEFT:
+                self.edge.e_int = self.ui['span_spec'].extents
+                self.update_image()
+
+    ################### Update Functions ###################
+    def update_spectrum1(self):
+        self.h['spec1'].set_ydata(self.spectrum1)
+        self.h['spec1'].set_color('maroon')
+        try:
+            self.ax['spec'].set_ylim([min(self.spectrum1.min(),self.spectrum2.min()),max(self.spectrum1.max(),self.spectrum2.max())])
+        except:
+            pass
+        
+    def update_spectrum2(self):
+        self.h['spec2'].set_ydata(self.spectrum2)
+        self.h['spec2'].set_alpha(1)
+        self.h['spec2'].set_color('cadetblue')
+        try:
+            self.ax['spec'].set_ylim([min(self.spectrum1.min(),self.spectrum2.min()),max(self.spectrum1.max(),self.spectrum2.max())])
+        except:
+            pass
+
+    def update_image(self):
+        indmin, indmax = np.searchsorted(self.energy, self.edge.e_int)
+        self.im_inel = np.mean(self.si[:,:,indmin:indmax],axis=(-1))
+        self.h['inel'].set_data(self.im_inel)
+        self.h['inel'].autoscale()
+
+        
+    def scale_button(self, event):
+        if self.ax['spec'].get_yscale()=='linear':
+            
+            self.ax['spec'].set_yscale('log')
+            self.ax['spec'].set_ylabel('Log Intensity')
+            self.ax['spec'].set_yticks([])
+        else:
+            
+            self.ax['spec'].set_yscale('linear')
+            self.ax['spec'].set_ylabel('Intensity')
+            self.ax['spec'].set_yticks([])
+
+    def dummy( self, *args ):
+        pass
```

### Comparing `spectrum_image-0.2/src/spectrum_image/SI_lineshapes.py` & `spectrum_image-0.2.1/src/spectrum_image/SI_lineshapes.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2/src/spectrum_image/SI_util.py` & `spectrum_image-0.2.1/src/spectrum_image/SI_util.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2/src/spectrum_image.egg-info/PKG-INFO` & `spectrum_image-0.2.1/src/spectrum_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2
+Version: 0.2.1
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
 Project-URL: Repository, https://github.com/sukhsung/spectrum_image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

