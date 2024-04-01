# Comparing `tmp/SingleOrigin-2.5.5.tar.gz` & `tmp/SingleOrigin-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SingleOrigin-2.5.5.tar", last modified: Fri Mar 29 19:58:04 2024, max compression
+gzip compressed data, was "SingleOrigin-2.5.6.tar", last modified: Mon Apr  1 17:24:55 2024, max compression
```

## Comparing `SingleOrigin-2.5.5.tar` & `SingleOrigin-2.5.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-03-29 19:58:04.851643 SingleOrigin-2.5.5/
--rw-r--r--   0 funni      (501) staff       (20)    32452 2022-01-20 18:33:29.000000 SingleOrigin-2.5.5/LICENSE.txt
--rw-r--r--   0 funni      (501) staff       (20)     3026 2024-03-29 19:58:04.851434 SingleOrigin-2.5.5/PKG-INFO
--rw-r--r--   0 funni      (501) staff       (20)     2151 2024-01-29 15:54:52.000000 SingleOrigin-2.5.5/README.md
--rw-r--r--   0 funni      (501) staff       (20)     1182 2024-03-29 19:55:52.000000 SingleOrigin-2.5.5/pyproject.toml
--rw-r--r--   0 funni      (501) staff       (20)       38 2024-03-29 19:58:04.851696 SingleOrigin-2.5.5/setup.cfg
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-03-29 19:58:04.842281 SingleOrigin-2.5.5/src/
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-03-29 19:58:04.850143 SingleOrigin-2.5.5/src/SingleOrigin/
--rw-r--r--   0 funni      (501) staff       (20)     1753 2022-02-04 19:39:13.000000 SingleOrigin-2.5.5/src/SingleOrigin/Element_table.txt
--rw-r--r--   0 funni      (501) staff       (20)     2277 2024-03-29 19:56:03.000000 SingleOrigin-2.5.5/src/SingleOrigin/__init__.py
--rw-r--r--   0 funni      (501) staff       (20)    33831 2024-01-29 18:22:49.000000 SingleOrigin-2.5.5/src/SingleOrigin/cell_transform.py
--rw-r--r--   0 funni      (501) staff       (20)   141016 2024-01-29 19:51:17.000000 SingleOrigin-2.5.5/src/SingleOrigin/find_atom_columns.py
--rw-r--r--   0 funni      (501) staff       (20)    64038 2024-03-29 19:50:32.000000 SingleOrigin-2.5.5/src/SingleOrigin/measure_lattice.py
--rw-r--r--   0 funni      (501) staff       (20)   116689 2024-03-11 19:35:52.000000 SingleOrigin-2.5.5/src/SingleOrigin/utils.py
-drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-03-29 19:58:04.851155 SingleOrigin-2.5.5/src/SingleOrigin.egg-info/
--rw-r--r--   0 funni      (501) staff       (20)     3026 2024-03-29 19:58:04.000000 SingleOrigin-2.5.5/src/SingleOrigin.egg-info/PKG-INFO
--rw-r--r--   0 funni      (501) staff       (20)      434 2024-03-29 19:58:04.000000 SingleOrigin-2.5.5/src/SingleOrigin.egg-info/SOURCES.txt
--rw-r--r--   0 funni      (501) staff       (20)        1 2024-03-29 19:58:04.000000 SingleOrigin-2.5.5/src/SingleOrigin.egg-info/dependency_links.txt
--rw-r--r--   0 funni      (501) staff       (20)      162 2024-03-29 19:58:04.000000 SingleOrigin-2.5.5/src/SingleOrigin.egg-info/requires.txt
--rw-r--r--   0 funni      (501) staff       (20)       13 2024-03-29 19:58:04.000000 SingleOrigin-2.5.5/src/SingleOrigin.egg-info/top_level.txt
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.179841 SingleOrigin-2.5.6/
+-rw-r--r--   0 funni      (501) staff       (20)    32452 2022-01-20 18:33:29.000000 SingleOrigin-2.5.6/LICENSE.txt
+-rw-r--r--   0 funni      (501) staff       (20)     3026 2024-04-01 17:24:55.179622 SingleOrigin-2.5.6/PKG-INFO
+-rw-r--r--   0 funni      (501) staff       (20)     2151 2024-01-29 15:54:52.000000 SingleOrigin-2.5.6/README.md
+-rw-r--r--   0 funni      (501) staff       (20)     1182 2024-04-01 17:24:00.000000 SingleOrigin-2.5.6/pyproject.toml
+-rw-r--r--   0 funni      (501) staff       (20)       38 2024-04-01 17:24:55.179888 SingleOrigin-2.5.6/setup.cfg
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.173117 SingleOrigin-2.5.6/src/
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.176072 SingleOrigin-2.5.6/src/SingleOrigin/
+-rw-r--r--   0 funni      (501) staff       (20)     1753 2022-02-04 19:39:13.000000 SingleOrigin-2.5.6/src/SingleOrigin/Element_table.txt
+-rw-r--r--   0 funni      (501) staff       (20)     2277 2024-04-01 17:24:32.000000 SingleOrigin-2.5.6/src/SingleOrigin/__init__.py
+-rw-r--r--   0 funni      (501) staff       (20)    33831 2024-01-29 18:22:49.000000 SingleOrigin-2.5.6/src/SingleOrigin/cell_transform.py
+-rw-r--r--   0 funni      (501) staff       (20)   141016 2024-01-29 19:51:17.000000 SingleOrigin-2.5.6/src/SingleOrigin/find_atom_columns.py
+-rw-r--r--   0 funni      (501) staff       (20)    64684 2024-03-29 21:44:25.000000 SingleOrigin-2.5.6/src/SingleOrigin/measure_lattice.py
+-rw-r--r--   0 funni      (501) staff       (20)   116689 2024-03-11 19:35:52.000000 SingleOrigin-2.5.6/src/SingleOrigin/utils.py
+drwxr-xr-x   0 funni      (501) staff       (20)        0 2024-04-01 17:24:55.179377 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/
+-rw-r--r--   0 funni      (501) staff       (20)     3026 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/PKG-INFO
+-rw-r--r--   0 funni      (501) staff       (20)      434 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/SOURCES.txt
+-rw-r--r--   0 funni      (501) staff       (20)        1 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/dependency_links.txt
+-rw-r--r--   0 funni      (501) staff       (20)      162 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/requires.txt
+-rw-r--r--   0 funni      (501) staff       (20)       13 2024-04-01 17:24:55.000000 SingleOrigin-2.5.6/src/SingleOrigin.egg-info/top_level.txt
```

### Comparing `SingleOrigin-2.5.5/LICENSE.txt` & `SingleOrigin-2.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.5/PKG-INFO` & `SingleOrigin-2.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleOrigin
-Version: 2.5.5
+Version: 2.5.6
 Summary: Crystallographic analysis for STEM data
 Author-email: Stephen Funni <sdf68@cornell.edu>
 Project-URL: homepage, https://github.com/sdfunni/SingleOrigin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `SingleOrigin-2.5.5/README.md` & `SingleOrigin-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.5/pyproject.toml` & `SingleOrigin-2.5.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SingleOrigin"
-version = "2.5.5"
+version = "2.5.6"
 authors = [{name = "Stephen Funni", email = "sdf68@cornell.edu"}]
 description = "Crystallographic analysis for STEM data"
 readme = "README.md"
 license = { file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `SingleOrigin-2.5.5/src/SingleOrigin/Element_table.txt` & `SingleOrigin-2.5.6/src/SingleOrigin/Element_table.txt`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.5/src/SingleOrigin/__init__.py` & `SingleOrigin-2.5.6/src/SingleOrigin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see https://www.gnu.org/licenses"""
 
 
-__version__ = "2.5.5"
+__version__ = "2.5.6"
 
 from SingleOrigin.utils import (
     metric_tensor,
     bond_length,
     bond_angle,
     absolute_angle_bt_vectors,
     rotation_angle_bt_vectors,
```

### Comparing `SingleOrigin-2.5.5/src/SingleOrigin/cell_transform.py` & `SingleOrigin-2.5.6/src/SingleOrigin/cell_transform.py`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.5/src/SingleOrigin/find_atom_columns.py` & `SingleOrigin-2.5.6/src/SingleOrigin/find_atom_columns.py`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.5/src/SingleOrigin/measure_lattice.py` & `SingleOrigin-2.5.6/src/SingleOrigin/measure_lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -719,27 +719,33 @@
 
         fig, axs = plt.subplots(
             2, 2,
             sharex=True,
             sharey=True,
             figsize=figsize,
             tight_layout=True,
-            # layout='constrained',
+            layout='constrained',
         )
         axs = axs.flatten()
         plots = []
 
         for i, comp in enumerate(self.lattice_maps.keys()):
             decimals = 2 if i < 2 else 1
-            vmin = np.around(np.nanmin(
-                np.where(mask, self.lattice_maps[comp], np.nan)),
-                decimals)
-            vmax = np.around(np.nanmax(
-                np.where(mask, self.lattice_maps[comp], np.nan)),
-                decimals)
+
+            masked = np.where(mask, self.lattice_maps[comp], np.nan)
+
+            vmid = np.around(np.nanmean(masked), decimals)
+            vstd = np.around(np.nanstd(masked), decimals)
+            vmin = np.around(np.nanmin(masked), decimals)
+            vmax = np.around(np.nanmax(masked), decimals)
+
+            vdiff = np.min([3*vstd, vmid-vmin, vmax-vmid])
+
+            vmin = vmid - vdiff
+            vmax = vmid + vdiff
 
             if i == 0:
                 size = np.mean(norm(self.basis_mean_real_px, axis=1))
 
                 plot_basis_vects = self.basis_mean_real_px * \
                     lattice_vect_scale * np.min([self.scan_h, self.scan_w]) \
                     / size
@@ -800,15 +806,15 @@
             )
 
             cbar.set_label(label=units[i], fontsize=20, fontweight='bold',
                            rotation='horizontal')
             axs[i].text(self.scan_w/50, self.scan_h/50,
                         labels[i], ha='left', va='top',
                         size=24, fontweight='bold',
-                        bbox=dict(facecolor='white', alpha=0.7, lw=0)
+                        bbox=dict(facecolor='white', alpha=0.8, lw=0)
                         )
 
         if return_fig:
             return fig, axs
 
     def get_strain(
         self,
@@ -1001,49 +1007,66 @@
             sharey=True,
             figsize=figsize,
             # tight_layout=True,
             layout='constrained',
         )
         axs = axs.flatten()
         plots = []
+
+        ax_scale = 0.1 * np.min([self.scan_h, self.scan_w])
+        axes_mag = (ax_scale * self.strain_basis
+                    / norm(self.strain_basis, axis=1))
+
         for i, comp in enumerate(keys):
             if (comp in ['exx', 'eyy']) & plot_strain_axes:
                 print('plotting strain axes')
                 axis_origin = [self.scan_w * strain_axes_origin[0],
                                self.scan_h * strain_axes_origin[1]]
 
-                ax_scale = 0.1 * np.min([self.scan_h, self.scan_w])
+                strain_axis = axes_mag[i]
 
-                xxwidth = 1 if comp == 'exx' else 0.3
-                yywidth = 1 if comp == 'eyy' else 0.3
-                axs[i].arrow(
-                    axis_origin[0],
-                    axis_origin[1],
-                    *(ax_scale * self.strain_basis[0]
-                      / norm(self.strain_basis[0])),
-                    fc='black',
-                    ec='black',
-                    width=xxwidth,
-                    length_includes_head=False,
-                    head_width=int(xxwidth)*3,
-                    # head_length=3,
-                    label='1',
-                )
-                axs[i].arrow(
-                    axis_origin[0],
-                    axis_origin[1],
-                    *(ax_scale * self.strain_basis[1]
-                      / norm(self.strain_basis[1])),
-                    fc='black',
-                    ec='black',
-                    width=yywidth,
-                    length_includes_head=False,
-                    head_width=int(yywidth)*3,
-                    # head_length=3,
+                # xxwidth=1 if comp == 'exx' else 0.3
+                # yywidth=1 if comp == 'eyy' else 0.3
+                # axs[i].arrow(
+                #     axis_origin[0],
+                #     axis_origin[1],
+                #     *(ax_scale * self.strain_basis[0]
+                #       / norm(self.strain_basis[0])),
+                #     fc='black',
+                #     ec='black',
+                #     width=xxwidth,
+                #     length_includes_head=False,
+                #     head_width=int(xxwidth)*3,
+                #     # head_length=3,
+                #     label='1',
+                # )
+
+                axs[i].annotate(
+                    text='',
+                    xy=axis_origin - strain_axis/2,
+                    xytext=axis_origin + strain_axis/2,
+                    arrowprops=dict(
+                        arrowstyle="<->",
+                        linewidth=3,
+                        # widthA=xxwidth,
+                    ),
                 )
+
+                # axs[i].arrow(
+                #     axis_origin[0],
+                #     axis_origin[1],
+                #     *(ax_scale * self.strain_basis[1]
+                #       / norm(self.strain_basis[1])),
+                #     fc='black',
+                #     ec='black',
+                #     width=yywidth,
+                #     length_includes_head=False,
+                #     head_width=int(yywidth)*3,
+                #     # head_length=3,
+                # )
                 # axs[i].text(axis_origin[0]+self.strain_basis[0, 0] * 1.2,
                 #             axis_origin[1]+self.strain_basis[0, 1] * 1.2,
                 #             'xx',
                 #             fontsize=20,
                 #             )
 
                 # axs[i].text(axis_origin[0]+self.strain_basis[1, 0] * 1.2,
@@ -1074,17 +1097,15 @@
 
             )
 
             cbar.ax.tick_params(labelsize=16)
             cbar.set_label(label=units, fontsize=20, fontweight='bold')
             axs[i].text(self.scan_w/50, self.scan_h/50,
                         labels[i], ha='left', va='top', size=24,
-                        # bbox={'alpha' : 0.2,
-                        #       'color' : 'white',
-                        #       'fill' : True},
+                        bbox=dict(facecolor='white', alpha=0.8, lw=0)
                         )
 
             if self.ref_region is not None:
                 dx = self.ref_region[0, 1] - self.ref_region[0, 0]
                 dy = self.ref_region[1, 0] - self.ref_region[1, 1]
                 corner = [self.ref_region[0, 0], self.ref_region[1, 1] - 1]
 
@@ -1107,15 +1128,15 @@
             alignment with higher order spots.
             Default: [1, 1]
 
         Returns
         -------
         None.
 
-        """"
+        """
 
         basis_factor = np.array(basis_factor, ndmin=2).T
 
         if dp_origin is None:
             dp_origin = np.flip(np.unravel_index(np.argmax(self.data_mean),
                                                  self.data.shape[-2:]))
 
@@ -1140,15 +1161,15 @@
             alignment with higher order spots.
             Default: [1, 1]
 
         Returns
         -------
         None.
 
-        """"
+        """
 
         fig, ax = plot_basis(
             self.ewpc_mean,
             self.basis_mean_real_px,
             self.origin,
             return_fig=True,
             vmax=self.ewpc_vmax,
```

### Comparing `SingleOrigin-2.5.5/src/SingleOrigin/utils.py` & `SingleOrigin-2.5.6/src/SingleOrigin/utils.py`

 * *Files identical despite different names*

### Comparing `SingleOrigin-2.5.5/src/SingleOrigin.egg-info/PKG-INFO` & `SingleOrigin-2.5.6/src/SingleOrigin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SingleOrigin
-Version: 2.5.5
+Version: 2.5.6
 Summary: Crystallographic analysis for STEM data
 Author-email: Stephen Funni <sdf68@cornell.edu>
 Project-URL: homepage, https://github.com/sdfunni/SingleOrigin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

