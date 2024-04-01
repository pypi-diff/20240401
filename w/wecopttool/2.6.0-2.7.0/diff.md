# Comparing `tmp/wecopttool-2.6.0.tar.gz` & `tmp/wecopttool-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wecopttool-2.6.0.tar", last modified: Thu Jul 13 20:53:49 2023, max compression
+gzip compressed data, was "wecopttool-2.7.0.tar", last modified: Mon Apr  1 15:22:19 2024, max compression
```

## Comparing `wecopttool-2.6.0.tar` & `wecopttool-2.7.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.040675 wecopttool-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 20:53:36.000000 wecopttool-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-13 20:53:36.000000 wecopttool-2.6.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-13 20:53:49.040675 wecopttool-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-13 20:53:36.000000 wecopttool-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-13 20:53:36.000000 wecopttool-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:53:49.040675 wecopttool-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.036675 wecopttool-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.040675 wecopttool-2.6.0/wecopttool/
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87143 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.040675 wecopttool-2.6.0/wecopttool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:19.926051 wecopttool-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 15:22:12.000000 wecopttool-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-01 15:22:12.000000 wecopttool-2.7.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-01 15:22:19.926051 wecopttool-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-01 15:22:12.000000 wecopttool-2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-01 15:22:12.000000 wecopttool-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:22:19.926051 wecopttool-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:19.922051 wecopttool-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    57469 2024-04-01 15:22:12.000000 wecopttool-2.7.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-01 15:22:12.000000 wecopttool-2.7.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-04-01 15:22:12.000000 wecopttool-2.7.0/tests/test_pto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17824 2024-04-01 15:22:12.000000 wecopttool-2.7.0/tests/test_waves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:19.922051 wecopttool-2.7.0/wecopttool/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-01 15:22:12.000000 wecopttool-2.7.0/wecopttool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87044 2024-04-01 15:22:12.000000 wecopttool-2.7.0/wecopttool/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-01 15:22:12.000000 wecopttool-2.7.0/wecopttool/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36432 2024-04-01 15:22:12.000000 wecopttool-2.7.0/wecopttool/pto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18959 2024-04-01 15:22:12.000000 wecopttool-2.7.0/wecopttool/waves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:19.922051 wecopttool-2.7.0/wecopttool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-01 15:22:19.000000 wecopttool-2.7.0/wecopttool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-01 15:22:19.000000 wecopttool-2.7.0/wecopttool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:22:19.000000 wecopttool-2.7.0/wecopttool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 15:22:19.000000 wecopttool-2.7.0/wecopttool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 15:22:19.000000 wecopttool-2.7.0/wecopttool.egg-info/top_level.txt
```

### Comparing `wecopttool-2.6.0/LICENSE` & `wecopttool-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.6.0/NOTICE` & `wecopttool-2.7.0/NOTICE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.6.0/PKG-INFO` & `wecopttool-2.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,43 @@
-Metadata-Version: 2.1
-Name: wecopttool
-Version: 2.6.0
-Summary: WEC Design Optimization Toolbox
-Author: Sandia National Laboratories
-License: GNU General Public License v3 (GPLv3)
-Project-URL: Documentation, https://sandialabs.github.io/WecOptTool/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: geometry
-License-File: LICENSE
-License-File: NOTICE
-
 [![Test-WecOptTool](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml/badge.svg)](https://github.com/sandialabs/WecOptTool/actions/workflows/push.yml)
 [![Coverage Status](https://coveralls.io/repos/github/sandialabs/WecOptTool/badge.svg?branch=main)](https://coveralls.io/github/sandialabs/WecOptTool?branch=main)
 
 # WecOptTool
 The Wave Energy Converter Design Optimization Toolbox (WecOptTool) allows users to perform wave energy converter (WEC) device design optimization studies with constrained optimal control.
 
 **NOTE:** If you are looking for the WecOptTool code used in previous published work (MATLAB version) please see [WecOptTool-MATLAB](https://github.com/SNL-WaterPower/WecOptTool-MATLAB).
 
 ## Project Information
 Refer to [WecOptTool documentation](https://sandialabs.github.io/WecOptTool/) for more information, including project overview, tutorials, theory, and API documentation.
 
 ## Getting started
-WecOptTool requires Python >= 3.8. Python 3.9 & 3.10 are supported.
-It is strongly recommended you create a dedicated virtual environment (e.g., using `conda`, `venv`, etc.) before installing `wecopttool`.
+**If you are brand new to Python and/or want detailed installation instructions, [click here](https://github.com/sandialabs/WecOptTool/blob/main/INSTALLATION.md).**
+
+WecOptTool requires Python >= 3.8. Python 3.10 & 3.11 are supported.
+It is strongly recommended you create a dedicated virtual environment (e.g., using [`conda`](https://www.anaconda.com/), [`mamba`](https://mamba.readthedocs.io/en/latest/), `venv`, etc.) before installing WecOptTool.
+
+From your dedicated environment, you can install WecOptTool via `conda`, `pip`, or `mamba`:
 
 **Option 1** - using `Conda`:
 
 ```bash
 conda install -c conda-forge wecopttool
 ```
 
 **Option 2** - using `pip` (requires Fortran compilers on your system):
 
 ```bash
 pip install wecopttool
 ```
 
-This approach is not recommended for Windows users since compiling `capytaine` on Windows requires [extra steps](https://github.com/capytaine/capytaine/issues/115).
+**Option 3** - using `Mamba`:
+
+```bash
+mamba install wecopttool
+```
 
 **Geometry module and tutorials**
 
 To use our geometry examples, including for running the tutorials, you will need to install some additional dependencies. 
 For the tutorials you will also need to install `jupyter`. 
 
 ```bash
```

### Comparing `wecopttool-2.6.0/pyproject.toml` & `wecopttool-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wecopttool"
-version = "2.6.0"
+version = "2.7.0"
 description = "WEC Design Optimization Toolbox"
 readme = "README.md"
 authors = [
     {name = "Sandia National Laboratories"},
 ]
 urls = {Documentation = "https://sandialabs.github.io/WecOptTool/"}
 requires-python = ">=3.8"
@@ -22,14 +22,15 @@
     "numpy>=1.20",
     "scipy",
     "xarray",
     "autograd",
     "capytaine",
     "joblib",
     "wavespectra>=3.13",
+    "netcdf4",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "sphinx",
     "sphinxcontrib-bibtex",
```

### Comparing `wecopttool-2.6.0/tests/test_core.py` & `wecopttool-2.7.0/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,56 +49,59 @@
         'omega': [2*np.pi*(ifreq+1)*f1 for ifreq in range(nfreq)],
         'influenced_dof': ['DOF_1', 'DOF_2'],
         'radiating_dof': ['DOF_1', 'DOF_2'],
         'wave_direction': [0.0, 1.5, 2.1],
     }
 
     ndof = 2; ndir = 3;
-    radiation_dims = ['radiating_dof', 'influenced_dof', 'omega']
-    excitation_dims = ['influenced_dof', 'wave_direction', 'omega']
-
-    added_mass = np.ones([ndof, ndof, nfreq])
-    radiation_damping = np.ones([ndof, ndof, nfreq])
-    diffraction_force = np.ones([ndof, ndir, nfreq], dtype=complex) + 1j
-    Froude_Krylov_force = np.ones([ndof, ndir, nfreq], dtype=complex) + 1j
-
+    radiation_dims = ['omega', 'radiating_dof', 'influenced_dof']
+    excitation_dims = ['omega', 'influenced_dof', 'wave_direction']
+    hydrostatics_dims = ['radiating_dof', 'influenced_dof']
+
+    added_mass = np.ones([nfreq, ndof, ndof])
+    radiation_damping = np.ones([nfreq, ndof, ndof])
+    diffraction_force = np.ones([nfreq, ndof, ndir], dtype=complex) + 1j
+    Froude_Krylov_force = np.ones([nfreq, ndof, ndir], dtype=complex) + 1j
+    inertia_matrix = np.ones([ndof, ndof])
+    hydrostatic_stiffness = np.ones([ndof, ndof])
+    
     data_vars = {
         'added_mass': (radiation_dims, added_mass),
         'radiation_damping': (radiation_dims, radiation_damping),
         'diffraction_force': (excitation_dims, diffraction_force),
-        'Froude_Krylov_force': (excitation_dims, Froude_Krylov_force)
+        'Froude_Krylov_force': (excitation_dims, Froude_Krylov_force),
+        'inertia_matrix': (hydrostatics_dims, inertia_matrix),
+        'hydrostatic_stiffness': (hydrostatics_dims, hydrostatic_stiffness)
     }
     return xr.Dataset(data_vars=data_vars, coords=coords)
 
 
 @pytest.fixture(scope='module')
 def hydro_data(bem_data):
     """Synthetic hydro-data containing inertia, stiffness, and friction
     in addition to the coefficients in `bem_data`."""
     ndof = len(bem_data.influenced_dof)
-    inertia_matrix = np.ones([ndof, ndof])
-    stiffness = np.ones([ndof, ndof])
     friction = np.ones([ndof, ndof])
-    data = wot.linear_hydrodynamics(
-        bem_data, inertia_matrix, stiffness, friction
+    data = wot.add_linear_friction(
+        bem_data, friction
     )
     return data
 
 
 # fixture: regular wave
 @pytest.fixture(scope="module")
 def wave_regular(f1, nfreq):
     """Wave structure consisting of a single regular wave."""
     n = np.random.randint(1, nfreq)
     freq = n*f1  # Hz
     amp = 1.1  # m
     phase = 24.5  # degrees
     wave = wot.waves.regular_wave(f1, nfreq, freq, amp, phase)
     params = {'n': n, 'amp': amp, 'phase': phase}
-    return wave, params
+    return wave.sel(realization=0), params
 
 
 @pytest.fixture(scope="module")
 def ndof_waves():
     """Number of WEC degrees of freedom to consider for the wave tests.
     """
     return 3
@@ -153,29 +156,30 @@
 @pytest.fixture(scope="module")
 def waves_multi(f1, nfreq):
     """Waves structure composed of two sinusoidal waves in different
     directions.
     """
     n = np.random.randint(1, nfreq)
     directions = [0.0, 30.0]
+    nrealizations = 1
     ndir = len(directions)
 
-    amplitudes = np.zeros([nfreq, ndir])
-    phases = np.zeros([nfreq, ndir])
+    amplitudes = np.zeros([nfreq, ndir, nrealizations])
+    phases = np.zeros([nfreq, ndir, nrealizations])
     amp0, amp1 = 1.2, 2.1
     phase0, phase1 = 26, -13
-    amplitudes[n-1, :] = [amp0, amp1]
-    phases[n-1, :] = [phase0, phase1]
+    amplitudes[n-1, :, :] = [[amp0], [amp1]]
+    phases[n-1, :, :] = [[phase0], [phase1]]
 
-    waves = wot.waves.elevation_fd(f1, nfreq, directions, amplitudes, phases)
+    waves = wot.waves.elevation_fd(f1, nfreq, directions, nrealizations, amplitudes, phases)
 
-    params = {'n': n, 'directions': directions, 'amp0': amp0, 'amp1': amp1,
-              'phase0': phase0, 'phase1': phase1}
+    params = {'n': n, 'directions': directions, 'nrealizations': nrealizations, 'amp0': amp0, 
+              'amp1': amp1, 'phase0': phase0, 'phase1': phase1}
 
-    return waves, params
+    return waves.sel(realization=0), params
 
 
 @pytest.fixture(scope="module")
 def fexc_multi(nfreq, waves_multi, exc_coeff, ndof_waves):
     """Excitation force for the multi-directional wave."""
     # wave elevation
     waves_multi, params_multi = waves_multi
@@ -206,19 +210,19 @@
     """Number of frequencies in synthetic impedance."""
     return 2
 
 
 @pytest.fixture(scope="module")
 def rao(ndof_imp, nfreq_imp):
     """Synthetic RAO transfer matrix."""
-    rao = np.empty([ndof_imp, ndof_imp, nfreq_imp], dtype=complex)
-    rao[0, 0, :] = [0+1j, 0+2j]
-    rao[1, 0, :] = [1+1j, 11+2j]
-    rao[0, 1, :] = [2+1j, 22+2j]
-    rao[1, 1, :] = [3+1j, 33+2j]
+    rao = np.empty([nfreq_imp, ndof_imp, ndof_imp], dtype=complex)
+    rao[:, 0, 0] = [0+1j, 0+2j]
+    rao[:, 1, 0] = [1+1j, 11+2j]
+    rao[:, 0, 1] = [2+1j, 22+2j]
+    rao[:, 1, 1] = [3+1j, 33+2j]
     return rao
 
 
 @pytest.fixture(scope="module")
 def mimo(nfreq_imp):
     """Correct MIMO matrix corresponding to the synthetic RAO
     transfer matrix.
@@ -569,15 +573,15 @@
         F = np.concatenate([
             [0.],
             np.reshape(
                 [[np.real(z[i]*x[i]), np.imag(z[i]*x[i])] for 
                 i in range(np.size(x)-1)], -1),
             [np.real(z[-1]) * np.real(x[-1])],
         ])
-        Z_mimo = wot.mimo_transfer_mat(np.reshape([z], [1,1,-1]), False)
+        Z_mimo = wot.mimo_transfer_mat(np.reshape([z], [-1, 1,1]), False)
         assert np.allclose(Z_mimo @ X, F)
 
 
 class TestVecToDOFMatToVec:
     """Test functions :python:`vec_to_dofmat` and
     :python:`dofmat_to_vec`.
     """
@@ -940,16 +944,14 @@
         return wot.check_linear_damping(data, tol)
 
     @pytest.fixture(scope="class")
     def data_new_nonuniform(self, data, tol):
         """Hydrodynamic data structure for which the function
         :python:`check_linear_damping` has been called.
         """
-        # TODO: clean this up when fixing the dim order discrepancy
-        data['radiation_damping'] = data['radiation_damping'].transpose('omega', ...)
         return wot.check_linear_damping(data, tol, False)
 
     def test_friction(self, data_new_uniform, tol):
         """Test that the modified friction diagonal has the expected
         value for a uniform shift.
         """
         assert np.allclose(np.diagonal(data_new_uniform.friction.values), tol)
@@ -1029,22 +1031,22 @@
         """
         return wot.check_impedance(data, tol)
 
     def test_friction(self, data_new, tol):
         """Test that the modified impedance diagonal has the expected
         value.
         """
-        assert np.allclose(np.real(np.diagonal(data_new)), tol)
+        assert np.allclose(np.real(np.diagonal(data_new, axis1=1, axis2=2)), tol)
 
     def test_only_diagonal_friction(self, data, data_new):
         """Test that only the diagonal was changed."""
         data_org = data.copy(deep=True)
 
         def offdiags(x):
-            return x.values[np.invert(np.eye(x.shape[0], dtype=bool))]
+            return x.values[:, np.invert(np.eye(x.shape[1], dtype=bool))]
         assert np.allclose(offdiags(data_new), offdiags(data_org))
 
     def test_only_friction(self, data, data_new):
         """Test that only the real part of the impedance was changed.
         """
         assert np.allclose(np.imag(data), np.imag(data_new))
 
@@ -1190,22 +1192,22 @@
         wave_phase_deg = np.rad2deg(wave_phase)
         diff = 4 + 5j
         fk_coeff = -2 + 1.2j
         # build hydrodynamic dataset
         data['inertia_matrix'][:, :] = np.eye(ndof)*mass
         data['hydrostatic_stiffness'][:, :] = np.eye(ndof)*hstiff
         data['friction'][:, :] = np.eye(ndof)*fric
-        data['radiation_damping'].values[:, :, index_freq-1] = np.eye(ndof)*rad
-        data['added_mass'].values[:, :, index_freq-1] = np.eye(ndof)*addmass
-        data['diffraction_force'].values[:, :, index_freq-1] = (
+        data['radiation_damping'].values[index_freq-1, :, :] = np.eye(ndof)*rad
+        data['added_mass'].values[index_freq-1, :, :] = np.eye(ndof)*addmass
+        data['diffraction_force'].values[index_freq-1, :, :] = (
             np.zeros([ndof, ndir], dtype=complex))
-        data['diffraction_force'].values[0, 0, index_freq-1] = diff
-        data['Froude_Krylov_force'].values[:, :, index_freq-1] = (
+        data['diffraction_force'].values[index_freq-1, 0, 0] = diff
+        data['Froude_Krylov_force'].values[index_freq-1, :, :] = (
             np.zeros([ndof, ndir], dtype=complex))
-        data['Froude_Krylov_force'].values[0, 0, index_freq-1] = fk_coeff
+        data['Froude_Krylov_force'].values[index_freq-1, 0, 0] = fk_coeff
         # standard forces
         forces = wot.standard_forces(data)
         # calculated inertia and forces
         wec = wot.WEC(
             f1, nfreq, {}, inertia_matrix=data['inertia_matrix'].values)
         waves = wot.waves.regular_wave(
             f1, nfreq, wave_freq, wave_amp, wave_phase_deg)
@@ -1213,16 +1215,16 @@
         x_wec[(index_freq*2-1)*1] = amplitude
         inertia_func = wot.inertia(
             f1, nfreq, inertia_matrix=data['inertia_matrix'].values)
         inertia = inertia_func(wec, x_wec, None, None)
         radiation = forces['radiation'](wec, x_wec, None, None)
         hydrostatics = forces['hydrostatics'](wec, x_wec, None, None)
         friction = forces['friction'](wec, x_wec, None, None)
-        fk = forces['Froude_Krylov'](wec, None, None, waves)
-        diffraction = forces['diffraction'](wec, None, None, waves)
+        fk = forces['Froude_Krylov'](wec, None, None, waves.sel(realization=0))
+        diffraction = forces['diffraction'](wec, None, None, waves.sel(realization=0))
         # true/expected inertia and forces
         inertia_truth = mass * acc
         radiation_truth = -(rad*vel + addmass*acc)
         hydrostatics_truth = -hstiff*pos
         friction_truth = -fric*vel
         diff_comp = wave_amp*np.exp(1j*wave_phase) * diff
         diffraction_truth =  (np.real(diff_comp) * np.cos(w*t) -
@@ -1256,17 +1258,19 @@
 class TestRunBEM:
     """Test function :python:`run_bem`."""
 
     def test_it_runs(self,):
         """Test that the function at least runs and returns correct
         data type.
         """
-        rect = cpy.RectangularParallelepiped(
-            size=(5.0, 5.0, 2.0), resolution=(10, 10, 10), center=(0.0, 0.0, 0.0,)
+        rect_mesh = cpy.mesh_parallelepiped(
+            size=(5.0, 5.0, 2.0), resolution=(10, 10, 10), 
+            center=(0.0, 0.0, 0.0)
         )
+        rect = cpy.FloatingBody(rect_mesh, name="rect")
         rect.add_translation_dof(name="Heave")
         bem_data = wot.run_bem(fb=rect, freq=[0.1, 0.2], wave_dirs=[0,])
         assert type(bem_data) == xr.Dataset
 
 
 class TestChangeBEMConvention:
     """Test function :python:`change_bem_convention`."""
@@ -1296,20 +1300,20 @@
 
     def test_round_trip(self, bem_data, data_back):
         """Test that a round trip returns the original dataset."""
         xr.testing.assert_allclose(data_back, bem_data)
 
 
 class TestLinearHydrodynamics:
-    """Test function :python:`linear_hydrodynamics`."""
+    """Test function :python:`add_linear_friction`."""
 
     def test_values(self, bem_data, hydro_data):
         """Test the function returns expected values."""
         mat = np.array([[1, 1], [1, 1]])
-        calculated = wot.linear_hydrodynamics(bem_data, mat, mat, mat)
+        calculated = wot.add_linear_friction(bem_data, mat)
         xr.testing.assert_allclose(calculated, hydro_data)
 
 
 class TestWaveExcitation:
     """Test function :python:`wave_excitation`."""
 
     def test_regular_value(
@@ -1335,27 +1339,27 @@
         assert calc_shape==shape and np.allclose(calculated, fexc_multi)
 
     def test_error_directions_not_subset(self, f1, nfreq, exc_coeff):
         """Test that an error is raised if the wave directions are not
         a subset of the hydrodata directions.
         """
         with pytest.raises(ValueError):
-            waves = wot.waves.elevation_fd(f1, nfreq, [0.0, 25])
+            waves = wot.waves.elevation_fd(f1, nfreq, [0.0, 25], 1)
             wot.wave_excitation(exc_coeff, waves)
 
     def test_error_different_frequencies(
             self, f1, nfreq, waves_multi, exc_coeff
         ):
         """Test that an error is raised if the wave and hydrodata do not
         have the same frequencies.
         """
         _, params_multi = waves_multi
         directions = np.deg2rad(params_multi['directions'])
         with pytest.raises(ValueError):
-            waves = wot.waves.elevation_fd(f1+0.01, nfreq, directions)
+            waves = wot.waves.elevation_fd(f1+0.01, nfreq, directions, 1)
             wot.wave_excitation(exc_coeff, waves)
 
 
 class TestAtleast2D:
     """Test function :python:`atleast_2d`."""
 
     def test_1d(self,):
```

### Comparing `wecopttool-2.6.0/tests/test_integration.py` & `wecopttool-2.7.0/tests/test_integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Integration tests spanning WecOptTool.
 """
 import pytest
 from pytest import approx
 import wecopttool as wot
 import capytaine as cpy
-import numpy as np
-import matplotlib.pyplot as plt
+import autograd.numpy as np
 from scipy.optimize import Bounds
+import xarray as xr
 
 
 kplim = -1e1
 
 
 @pytest.fixture(scope="module")
 def f1():
@@ -40,15 +40,15 @@
                       controller=wot.pto.controller_p,
                       names=["P controller PTO"])
     return pto
 
 
 @pytest.fixture(scope='module')
 def pi_controller_pto():
-    """Basic PTO: proportional-integral (PI) controller, 1 DOF, mechanical 
+    """Basic PTO: proportional-integral (PI) controller, 1 DOF, mechanical
     power."""
     ndof = 1
     pto = wot.pto.PTO(ndof=ndof, kinematics=np.eye(ndof),
                       controller=wot.pto.controller_pi,
                       names=["PI controller PTO"])
     return pto
 
@@ -100,59 +100,55 @@
     waves = wot.waves.long_crested_wave(spec)
     return waves
 
 
 @pytest.fixture(scope='module')
 def wec_from_bem(f1, nfreq, bem, fb, pto):
     """Simple WEC: 1 DOF, no constraints."""
-    mass = wot.hydrostatics.inertia_matrix(fb).values
-    hstiff = wot.hydrostatics.stiffness_matrix(fb).values
     f_add = {"PTO": pto.force_on_wec}
-    wec = wot.WEC.from_bem(bem, mass, hstiff, f_add=f_add)
+    wec = wot.WEC.from_bem(bem, f_add=f_add)
     return wec
 
 
 @pytest.fixture(scope='module')
 def wec_from_floatingbody(f1, nfreq, fb, pto):
     """Simple WEC: 1 DOF, no constraints."""
-    mass = wot.hydrostatics.inertia_matrix(fb).values
-    hstiff = wot.hydrostatics.stiffness_matrix(fb).values
     f_add = {"PTO": pto.force_on_wec}
-    wec = wot.WEC.from_floating_body(fb, f1, nfreq, mass, hstiff, f_add=f_add)
+    wec = wot.WEC.from_floating_body(fb, f1, nfreq, f_add=f_add)
     return wec
 
 
 @pytest.fixture(scope='module')
 def wec_from_impedance(bem, pto, fb):
     """Simple WEC: 1 DOF, no constraints."""
-    bemc = bem.copy().transpose(
-        "radiating_dof", "influenced_dof", "omega", "wave_direction")
+    bemc = bem.copy()
     omega = bemc['omega'].values
-    w = np.expand_dims(omega, [0, 1])
+    w = np.expand_dims(omega, [1,2])
     A = bemc['added_mass'].values
     B = bemc['radiation_damping'].values
-    mass = wot.hydrostatics.inertia_matrix(fb).values
-    hstiff = wot.hydrostatics.stiffness_matrix(fb).values
+    fb.center_of_mass = [0, 0, 0]
+    fb.rotation_center = fb.center_of_mass
+    fb = fb.copy(name=f"{fb.name}_immersed").keep_immersed_part()
+    mass = bemc['inertia_matrix'].values
+    hstiff = bemc['hydrostatic_stiffness'].values
     K = np.expand_dims(hstiff, 2)
-
+    
     freqs = omega / (2 * np.pi)
     impedance = (A + mass)*(1j*w) + B + K/(1j*w)
     exc_coeff = bem['Froude_Krylov_force'] + bem['diffraction_force']
     f_add = {"PTO": pto.force_on_wec}
 
     wec = wot.WEC.from_impedance(freqs, impedance, exc_coeff, hstiff, f_add)
     return wec
 
 
 @pytest.fixture(scope='module')
 def resonant_wave(f1, nfreq, fb, bem):
     """Regular wave at natural frequency of the WEC"""
-    mass = wot.hydrostatics.inertia_matrix(fb).values
-    hstiff = wot.hydrostatics.stiffness_matrix(fb).values
-    hd = wot.linear_hydrodynamics(bem, mass, hstiff)
+    hd = wot.add_linear_friction(bem)
     Zi = wot.hydrodynamic_impedance(hd)
     wn = Zi['omega'][np.abs(Zi).argmin(dim='omega')].item()
     waves = wot.waves.regular_wave(f1, nfreq, freq=wn/2/np.pi, amplitude=0.1)
     return waves
 
 
 def test_solve_callback(wec_from_bem, regular_wave, pto, nfreq, capfd):
@@ -177,30 +173,30 @@
     assert out.split('\n')[0] == cbstring
 
 
 @pytest.mark.parametrize("bounds_opt",
                          [Bounds(lb=kplim, ub=0), ((kplim, 0),)])
 def test_solve_bounds(bounds_opt, wec_from_bem, regular_wave,
                       p_controller_pto):
-    """Confirm that bounds are not violated and scale correctly when 
+    """Confirm that bounds are not violated and scale correctly when
     passing bounds argument as both as Bounds object and a tuple"""
 
-    # replace unstructured controller with propotional controller
+    # replace unstructured controller with proportional controller
     wec_from_bem.forces['PTO'] = p_controller_pto.force_on_wec
 
     res = wec_from_bem.solve(waves=regular_wave,
                              obj_fun=p_controller_pto.average_power,
                              nstate_opt=1,
                              x_opt_0=[kplim*0.1],
                              optim_options={'maxiter': 2e1,
                                             'ftol': 1e-8},
                              bounds_opt=bounds_opt,
                              )
 
-    assert pytest.approx(kplim, 1e-5) == res['x'][-1]
+    assert pytest.approx(kplim, 1e-5) == res[0]['x'][-1]
 
 
 def test_same_wec_init(wec_from_bem,
                        wec_from_floatingbody,
                        wec_from_impedance,
                        f1,
                        nfreq):
@@ -208,139 +204,214 @@
     """
 
     waves = wot.waves.regular_wave(f1, nfreq, 0.3, 0.0625)
     np.random.seed(0)
     x_wec_0 = np.random.randn(wec_from_bem.nstate_wec)
     np.random.seed(1)
     x_opt_0 = np.random.randn(wec_from_bem.nstate_wec)
-    bem_res = wec_from_bem._resid_fun(x_wec_0, x_opt_0, waves)
-    fb_res = wec_from_floatingbody._resid_fun(x_wec_0, x_opt_0, waves)
-    imp_res = wec_from_impedance._resid_fun(x_wec_0, x_opt_0, waves)
-
+    bem_res = wec_from_bem.residual(x_wec_0, x_opt_0, waves.sel(realization=0))
+    fb_res = wec_from_floatingbody.residual(x_wec_0, x_opt_0, waves.sel(realization=0))
+    imp_res = wec_from_impedance.residual(x_wec_0, x_opt_0, waves.sel(realization=0))
+    
     assert fb_res == approx(bem_res, rel=0.01)
     assert imp_res == approx(bem_res, rel=0.01)
 
 
 class TestTheoreticalPowerLimits:
     """Compare power from numerical solutions against known theoretical limits
     """
 
     @pytest.fixture(scope='class')
     def mass(self, fb):
         """Rigid-body mass"""
-        return wot.hydrostatics.inertia_matrix(fb).values
+        return fb.compute_rigid_body_inertia()
 
     @pytest.fixture(scope='class')
     def hstiff(self, fb):
         """Hydrostatic stiffness"""
-        return wot.hydrostatics.stiffness_matrix(fb).values
+        return fb.compute_hydrostatic_stiffness()
 
     @pytest.fixture(scope='class')
-    def hydro_impedance(self, bem, mass, hstiff):
+    def hydro_impedance(self, bem):
         """Intrinsic hydrodynamic impedance"""
-        hd = wot.linear_hydrodynamics(bem, mass, hstiff)
+        hd = wot.add_linear_friction(bem)
         hd = wot.check_linear_damping(hd)
         Zi = wot.hydrodynamic_impedance(hd)
         return Zi
 
     def test_p_controller_resonant_wave(self,
                                         bem,
                                         resonant_wave,
                                         p_controller_pto,
-                                        mass,
-                                        hstiff,
                                         hydro_impedance):
-        """Proportional controller should match optimum for natural resonant 
+        """Proportional controller should match optimum for natural resonant
         wave"""
-
+        
         f_add = {"PTO": p_controller_pto.force_on_wec}
-        wec = wot.WEC.from_bem(bem, mass, hstiff, f_add=f_add)
+        wec = wot.WEC.from_bem(bem, f_add=f_add)
 
         res = wec.solve(waves=resonant_wave,
                         obj_fun=p_controller_pto.average_power,
                         nstate_opt=1,
                         x_wec_0=1e-1*np.ones(wec.nstate_wec),
                         x_opt_0=[-1470],
                         scale_x_wec=1e2,
                         scale_x_opt=1e-3,
                         scale_obj=1e-1,
                         optim_options={'ftol': 1e-10},
                         bounds_opt=((-1*np.infty, 0),),
                         )
 
-        power_sol = -1*res['fun']
+        power_sol = -1*res[0]['fun']
 
-        res_fd, _ = wec.post_process(res, resonant_wave,nsubsteps=1)
+        res_fd, _ = wec.post_process(res[0], resonant_wave.sel(realization=0), nsubsteps=1)
         Fex = res_fd.force.sel(
             type=['Froude_Krylov', 'diffraction']).sum('type')
         power_optimal = (np.abs(Fex)**2/8 / np.real(hydro_impedance.squeeze())
                          ).squeeze().sum('omega').item()
 
-        assert power_sol == approx(power_optimal, rel=0.02)
+        assert power_sol == approx(power_optimal, rel=0.03)
 
     def test_pi_controller_regular_wave(self,
                                         bem,
                                         regular_wave,
                                         pi_controller_pto,
-                                        mass,
-                                        hstiff,
                                         hydro_impedance):
         """PI controller matches optimal for any regular wave"""
 
         f_add = {"PTO": pi_controller_pto.force_on_wec}
-        wec = wot.WEC.from_bem(bem, mass, hstiff, f_add=f_add)
+        wec = wot.WEC.from_bem(bem, f_add=f_add)
 
         res = wec.solve(waves=regular_wave,
                         obj_fun=pi_controller_pto.average_power,
                         nstate_opt=2,
                         x_wec_0=1e-1*np.ones(wec.nstate_wec),
                         x_opt_0=[-1e3, 1e4],
                         scale_x_wec=1e2,
                         scale_x_opt=1e-3,
                         scale_obj=1e-2,
                         optim_options={'maxiter': 50},
                         bounds_opt=((-1e4, 0), (0, 2e4),)
                         )
 
-        power_sol = -1*res['fun']
+        power_sol = -1*res[0]['fun']
 
-        res_fd, _ = wec.post_process(res, regular_wave, nsubsteps=1)
+        res_fd, _ = wec.post_process(res[0], regular_wave.sel(realization=0), nsubsteps=1)
         Fex = res_fd.force.sel(
             type=['Froude_Krylov', 'diffraction']).sum('type')
         power_optimal = (np.abs(Fex)**2/8 / np.real(hydro_impedance.squeeze())
                          ).squeeze().sum('omega').item()
 
         assert power_sol == approx(power_optimal, rel=1e-4)
-
     def test_unstructured_controller_irregular_wave(self,
                                                     fb,
                                                     bem,
                                                     regular_wave,
                                                     pto,
                                                     nfreq,
-                                                    mass,
-                                                    hstiff,
                                                     hydro_impedance):
-        """Unstructured (numerical optimal) controller matches optimal for any 
+        """Unstructured (numerical optimal) controller matches optimal for any
         irregular wave when unconstrained"""
 
         f_add = {"PTO": pto.force_on_wec}
-        wec = wot.WEC.from_bem(bem, mass, hstiff, f_add=f_add)
+        wec = wot.WEC.from_bem(bem, f_add=f_add)
 
         res = wec.solve(waves=regular_wave,
                         obj_fun=pto.average_power,
                         nstate_opt=2*nfreq,
                         x_wec_0=1e-1*np.ones(wec.nstate_wec),
                         scale_x_wec=1e2,
                         scale_x_opt=1e-2,
                         scale_obj=1e-2,
                         )
 
-        power_sol = -1*res['fun']
+        power_sol = -1*res[0]['fun']
 
-        res_fd, _ = wec.post_process(res, regular_wave, nsubsteps=1)
+        res_fd, _ = wec.post_process(res[0], regular_wave.sel(realization=0), nsubsteps=1)
         Fex = res_fd.force.sel(
             type=['Froude_Krylov', 'diffraction']).sum('type')
         power_optimal = (np.abs(Fex)**2/8 / np.real(hydro_impedance.squeeze())
                          ).squeeze().sum('omega').item()
 
         assert power_sol == approx(power_optimal, rel=1e-3)
+
+    def test_saturated_pi_controller(self,
+                                    bem,
+                                    regular_wave,
+                                    pto,
+                                    nfreq):
+        """Saturated PI controller matches constrained unstructured controller
+        for a regular wave
+        """
+
+        pto_tmp = pto
+        pto = {}
+        wec = {}
+        nstate_opt = {}
+        
+        # Constraint
+        f_max = 2000.0
+
+        nstate_opt['us'] = 2*nfreq
+        pto['us'] = pto_tmp
+        def const_f_pto(wec, x_wec, x_opt, waves):
+            f = pto['us'].force_on_wec(wec, x_wec, x_opt, waves, 
+                                       nsubsteps=4)
+            return f_max - np.abs(f.flatten())
+        wec['us'] = wot.WEC.from_bem(bem,
+                                     f_add={"PTO": pto['us'].force_on_wec},
+                                     constraints=[{'type': 'ineq',
+                                                   'fun': const_f_pto, }])
+        
+        
+        ndof = 1
+        nstate_opt['pi'] = 2
+        def saturated_pi(pto, wec, x_wec, x_opt, waves=None, nsubsteps=1):
+            return wot.pto.controller_pi(pto, wec, x_wec, x_opt, waves, 
+                                         nsubsteps, 
+                                         saturation=[-f_max, f_max])
+        pto['pi'] = wot.pto.PTO(ndof=ndof,
+                                kinematics=np.eye(ndof),
+                                controller=saturated_pi,)
+        wec['pi'] = wot.WEC.from_bem(bem,
+                                     f_add={"PTO": pto['pi'].force_on_wec},
+                                     constraints=[])
+        
+        x_opt_0 = {'us': np.ones(nstate_opt['us'])*0.1,
+                   'pi': [-1e3, 1e4]}
+        scale_x_wec = {'us': 1e1,
+                       'pi': 1e1}
+        scale_x_opt = {'us': 1e-3,
+                       'pi': 1e-3}
+        scale_obj = {'us': 1e-2,
+                     'pi': 1e-2}
+        bounds_opt = {'us': None,
+                      'pi': ((-1e4, 0), (0, 2e4),)}
+        
+        res = {}
+        pto_fdom = {}
+        pto_tdom = {}
+        for key in wec.keys():
+            res[key] = wec[key].solve(waves=regular_wave,
+                            obj_fun=pto[key].average_power,
+                            nstate_opt=nstate_opt[key],
+                            x_wec_0=1e-1*np.ones(wec[key].nstate_wec),
+                            x_opt_0=x_opt_0[key],
+                            scale_x_wec=scale_x_wec[key],
+                            scale_x_opt=scale_x_opt[key],
+                            scale_obj=scale_obj[key],
+                            optim_options={'maxiter': 200},
+                            bounds_opt=bounds_opt[key]
+                            )
+            
+            nsubstep_postprocess = 4
+            pto_fdom[key], pto_tdom[key] = pto[key].post_process(wec[key], 
+                                                                 res[key][0], 
+                                                                 regular_wave.sel(realization=0), 
+                                                                 nsubstep_postprocess)
+        
+        xr.testing.assert_allclose(pto_tdom['pi'].power.squeeze().mean('time'), 
+                                   pto_tdom['us'].power.squeeze().mean('time'),
+                                   rtol=1e-1)
+        
+        xr.testing.assert_allclose(pto_tdom['us'].force.max(),
+                                   pto_tdom['pi'].force.max())
```

### Comparing `wecopttool-2.6.0/tests/test_pto.py` & `wecopttool-2.7.0/tests/test_pto.py`

 * *Files 9% similar despite different names*

```diff
@@ -256,8 +256,29 @@
         vel = -1 * amp * w * np.sin(w * wec.time)
         acc = -1 * amp * w**2 * np.cos(w * wec.time)
         force = vel*pid_p + pos*pid_i + acc*pid_d
         force = force.reshape(-1, 1)
         x_wec = [0, amp, 0, 0]
         x_opt = [pid_p, pid_i, pid_d]
         calculated = pto.force(wec, x_wec, x_opt, None)
-        assert np.allclose(force, calculated)
+        assert np.allclose(force, calculated)
+
+    def test_controller_pid_saturated(
+            self, wec, ndof, kinematics, omega, pid_p, pid_i, pid_d,
+        ):
+        """Test the PID controller."""
+        saturation = np.array([[-4,5]])
+        def controller(p,w,xw,xo,wa,ns):
+            return wot.pto.controller_pid(p,w,xw,xo,wa,ns,saturation=saturation)
+        pto = wot.pto.PTO(ndof, kinematics, controller)
+        amp = 2.3
+        w = omega[-2]
+        pos = amp * np.cos(w * wec.time)
+        vel = -1 * amp * w * np.sin(w * wec.time)
+        acc = -1 * amp * w**2 * np.cos(w * wec.time)
+        force = vel*pid_p + pos*pid_i + acc*pid_d
+        force = np.clip(force, saturation[0,0], saturation[0,1])
+        force = force.reshape(-1, 1)
+        x_wec = [0, amp, 0, 0]
+        x_opt = [pid_p, pid_i, pid_d]
+        calculated = pto.force(wec, x_wec, x_opt, None)
+        assert np.allclose(force, calculated)
```

### Comparing `wecopttool-2.6.0/tests/test_waves.py` & `wecopttool-2.7.0/tests/test_waves.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Unit tests for functions in the :python:`waves.py` module.
 """
 
 import os
 
 import pytest
-import capytaine as cpy
 import numpy as np
 import wavespectra as ws
 from scipy import signal
 
 import wecopttool as wot
 from wecopttool.core import _default_parameters
 
@@ -55,21 +54,21 @@
 class TestElevationFD:
     """Test function :python:`waves.elevation_fd`."""
 
     @pytest.fixture(scope="class")
     def elevation(self, f1, nfreq, directions):
         """Complex sea state elevation amplitude [m] indexed by
         frequency and direction."""
-        return wot.waves.elevation_fd(f1, nfreq, directions)
+        return wot.waves.elevation_fd(f1, nfreq, directions, 1)
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega', 'freq']
+        coordinates = ['wave_direction', 'omega', 'freq', 'realization']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
     def test_shape(self, elevation, nfreq, ndir):
         """Test that the elevation dataArray has the correct shape."""
         assert np.squeeze(elevation.values).shape == (nfreq, ndir)
 
@@ -112,15 +111,15 @@
         frequency and direction."""
         return wot.waves.regular_wave(f1, nfreq, freq, amp, phase, dir)
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega', 'freq']
+        coordinates = ['wave_direction', 'omega', 'freq', 'realization']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
     def test_shape(self, elevation, nfreq, ndir):
         """Test that the elevation dataArray has the correct shape."""
         assert np.squeeze(elevation.values).shape == (nfreq, )
 
@@ -178,19 +177,24 @@
 
     @pytest.fixture(scope="class")
     def direction(self, ndbc_omnidirectional, ndir):
         """Wave direction."""
         return ndbc_omnidirectional.dir.values[np.random.randint(0, ndir)]
 
     @pytest.fixture(scope="class")
-    def elevation(self, ndbc_omnidirectional, direction):
+    def nrealizations(self):
+        """Number of wave realizations."""
+        return 2
+
+    @pytest.fixture(scope="class")
+    def elevation(self, ndbc_omnidirectional, direction, nrealizations):
         """Complex sea state elevation amplitude [m] indexed by
         frequency and direction."""
         elev = wot.waves.long_crested_wave(
-            ndbc_omnidirectional.efth, direction)
+            ndbc_omnidirectional.efth, nrealizations, direction)
         return elev
 
     @pytest.fixture(scope="class")
     def pm_f1(self,):
         """Fundamental frequency for the Pierson-Moskowitz spectrum."""
         return 0.05
 
@@ -219,42 +223,48 @@
         )
         return efth_xr
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega', 'freq']
+        coordinates = ['wave_direction', 'omega', 'freq', 'realization']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
-    def test_shape(self, elevation, nfreq, ndir):
+    def test_shape(self, elevation, nfreq, ndir, nrealizations):
         """Test that the elevation dataArray has the correct shape."""
-        assert np.squeeze(elevation.values).shape == (nfreq, )
+        assert np.squeeze(elevation.values).shape == (nfreq, nrealizations)
 
     def test_type(self, elevation):
         """Test that the elevation dataArray has the correct type."""
         assert np.iscomplexobj(elevation)
 
     def test_direction(self, elevation, direction):
         """Test that the wave direction is correct."""
         dir_out = elevation.wave_direction.values.item()
         assert np.isclose(dir_out, wot.degrees_to_radians(direction))
 
+    def test_realizations(self, elevation):
+        """Test that the number of realizations is correct."""
+        realization_out = elevation.realization.values
+        assert (realization_out == [0,1]).all()
+
     def test_spectrum(self, pm_spectrum, pm_hs):
         """Test that the constructed spectrum has the expected Hs."""
         efth = ws.SpecArray(pm_spectrum)
         assert np.isclose(pm_hs, efth.hs().values)
 
     def test_time_series(self, pm_spectrum, pm_f1, pm_nfreq):
         """Test that the created time series has the desired spectrum."""
         # create time-series
         direction = 0.0
-        wave = wot.waves.long_crested_wave(pm_spectrum, direction)
-        wave_ts = wot.fd_to_td(wave.values, pm_f1, pm_nfreq, False)
+        nrealizations = 1
+        wave = wot.waves.long_crested_wave(pm_spectrum, nrealizations, direction)
+        wave_ts = wot.fd_to_td(wave.sel(realization=0).values, pm_f1, pm_nfreq, False)
         # calculate the spectrum from the time-series
         t = wot.time(pm_f1, pm_nfreq)
         fs = 1/t[1]
         nnft = len(t)
         [_, S_data] = signal.welch(
             wave_ts.squeeze(), fs=fs, window='boxcar', nperseg=nnft, nfft=nnft,
             noverlap=0
@@ -275,49 +285,60 @@
         time = '2020-01-01T01:40:00.000000000'
         freq = wot.frequency(f1, nfreq, False)
         markers = ('w', 'd', 'i', 'j', 'k')
         dir = os.path.join(os.path.dirname(__file__), 'data', 'ndbc')
         files = [f'41013{i}2020.txt' for i in markers]
         spec = ws.read_ndbc_ascii([os.path.join(dir, file) for file in files])
         return spec.sel(time=time).interp(freq=freq)
+    
+    @pytest.fixture(scope="class")
+    def nrealizations(self):
+        """Number of wave realizations."""
+        return 2
 
     @pytest.fixture(scope="class")
-    def elevation(self, ndbc_spectrum):
+    def elevation(self, ndbc_spectrum, nrealizations):
         """Complex sea state elevation amplitude [m] indexed by
         frequency and direction."""
-        return wot.waves.irregular_wave(ndbc_spectrum.efth)
+        return wot.waves.irregular_wave(ndbc_spectrum.efth, nrealizations)
 
     def test_coordinates(self, elevation):
         """Test that the elevation dataArray has the correct
         coordinates.
         """
-        coordinates = ['wave_direction', 'omega', 'freq']
+        coordinates = ['wave_direction', 'omega', 'freq', 'realization']
         for icoord in coordinates:
             assert icoord in elevation.coords, f'missing coordinate: {icoord}'
 
-    def test_shape(self, ndbc_spectrum, elevation):
+    def test_shape(self, ndbc_spectrum, elevation, nrealizations):
         """Test that the elevation dataArray has the correct shape."""
         nfreq = len(ndbc_spectrum.freq)
         ndir = len(ndbc_spectrum.dir)
-        assert np.squeeze(elevation.values).shape == (nfreq, ndir)
+        assert np.squeeze(elevation.values).shape == (nfreq, ndir, nrealizations)
 
     def test_type(self, elevation):
         """Test that the elevation dataArray has the correct type."""
         assert np.iscomplexobj(elevation)
+    
+    def test_realizations(self, elevation):
+        """Test that the number of realizations is correct."""
+        realization_out = elevation.realization.values
+        assert (realization_out == [0,1]).all()
 
 
 class TestRandomPhase:
     """Test function :python:`waves.random_phase`."""
 
     @pytest.fixture(scope="class")
     def shape(self,):
         """Shape of the phase matrix, randomized each time the test is
         run.
         """
-        return (np.random.randint(10, 100), np.random.randint(10, 100))
+        return (np.random.randint(10, 100), np.random.randint(10, 100),
+                np.random.randint(10, 100))
 
     @pytest.fixture(scope="class")
     def phase_mat(self, shape):
         """Random phase matrix."""
         return wot.waves.random_phase(shape)
 
     def test_mat_shape(self, phase_mat, shape):
```

### Comparing `wecopttool-2.6.0/wecopttool/__init__.py` & `wecopttool-2.7.0/wecopttool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 from importlib.metadata import metadata as metadata
 import logging
 import warnings
 
 from wecopttool.core import *
 from wecopttool import waves
-from wecopttool import hydrostatics
 from wecopttool import pto
 
 try:
   from wecopttool import geom
 except ModuleNotFoundError:
   warnings.warn("`geom` submodule not loaded because of missing dependencies. Install these by running `pip install wecopttool[geometry]`.")
```

### Comparing `wecopttool-2.6.0/wecopttool/core.py` & `wecopttool-2.7.0/wecopttool/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,25 @@
     "force_from_rao_transfer_function",
     "force_from_impedance",
     "force_from_waves",
     "inertia",
     "standard_forces",
     "run_bem",
     "change_bem_convention",
-    "linear_hydrodynamics",
+    "add_linear_friction",
     "wave_excitation",
     "hydrodynamic_impedance",
     "atleast_2d",
     "degrees_to_radians",
     "subset_close",
     "scale_dofs",
     "decompose_state",
     "frequency_parameters",
     "time_results",
+    "set_fb_centers",
 ]
 
 
 import logging
 from typing import Iterable, Callable, Any, Optional, Mapping, TypeVar, Union
 from pathlib import Path
 import warnings
@@ -280,16 +281,14 @@
         repr_org = f"<{module}.{qualname} object at {hex(id(self))}>"
         return repr_org + " :: " + self.__str__()
 
     # other initialization methods
     @staticmethod
     def from_bem(
         bem_data: Union[Dataset, Union[str, Path]],
-        inertia_matrix: Optional[ndarray] = None,
-        hydrostatic_stiffness: Optional[ndarray] = None,
         friction: Optional[ndarray] = None,
         f_add: Optional[TIForceDict] = None,
         constraints: Optional[Iterable[Mapping]] = None,
         min_damping: Optional[float] = _default_min_damping,
         uniform_shift: Optional[bool] = True,
         dof_names: Optional[Iterable[str]] = None,
         ) -> TWEC:
@@ -308,34 +307,24 @@
         the direct results from capytaine must be modified using
         :py:func:`wecopttool.change_bem_convention` before calling
         this initialization function.
         Instead, the recommended approach is to use
         :py:func:`wecopttool.run_bem`,
         rather than running Capytaine directly, which outputs the
         results in the correct convention. The results can be saved
-        using :py:func:`wecopttool.write_netcdf`.
-
-        In addition to the Capytaine results, if the dataset contains
-        the :python:`inertia_matrix`, :python:`hydrostatic_stiffness`,
-        or :python:`friction` these do not need to be provided
-        separately.
+        using :py:func:`wecopttool.write_netcdf`. 
+        :py:func:`wecopttool.run_bem` also computes the inertia and 
+        hydrostatic stiffness which should be included in bem_data.
 
         Parameters
         ----------
         bem_data
             Linear hydrodynamic coefficients obtained using the boundary
             element method (BEM) code Capytaine, with sign convention
-            corrected.
-        inertia_matrix
-           Inertia matrix of size :python:`(ndof, ndof)`.
-           :python:`None` if included in :python:`bem_data`.
-        hydrostatic_stiffness
-            Linear hydrostatic restoring coefficient of size
-            :python:`(nodf, ndof)`.
-            :python:`None` if included in :python:`bem_data`.
+            corrected. Also includes inertia and hydrostatic stiffness.
         friction
             Linear friction, in addition to radiation damping, of size
             :python:`(nodf, ndof)`.
             :python:`None` if included in :python:`bem_data` or to set
             to zero.
         f_add
             Dictionary with entries :python:`{'force_name': fun}`, where
@@ -358,40 +347,24 @@
             See :py:func:`wecopttool.check_linear_damping` for more details.
         dof_names
             Names of the different degrees of freedom (e.g.
             :python:`'Heave'`).
             If :python:`None` the names
             :python:`['DOF_0', ..., 'DOF_N']` are used.
 
-        Raises
-        ------
-        ValueError
-            If either :python:`inertia_matrix` or
-            :python:`hydrostatic_stiffness` are :python:`None` and is
-            not included in :python:`bem_data`.
-            See :py:func:`wecopttool.linear_hydrodynamics`.
-        ValueError
-            If any of :python:`inertia_matrix`,
-            :python:`hydrostatic_stiffness`, or :python:`stiffness` are
-            both provided and included in :python:`bem_data` but have
-            different values.
-            See :py:func:`wecopttool.linear_hydrodynamics`.
-
         See Also
         --------
-        run_bem, linear_hydrodynamics, change_bem_convention,
+        run_bem, add_linear_friction, change_bem_convention,
         write_netcdf, check_linear_damping
         """
         if isinstance(bem_data, (str, Path)):
             bem_data = read_netcdf(bem_data)
-        # add inertia_matrix, hydrostatic stiffness, and friction
-        hydro_data = linear_hydrodynamics(
-            bem_data, inertia_matrix, hydrostatic_stiffness, friction)
-        if inertia_matrix is None:
-            inertia_matrix = hydro_data['inertia_matrix'].values
+        # add friction
+        hydro_data = add_linear_friction(bem_data, friction)
+        inertia_matrix = hydro_data['inertia_matrix'].values
 
         # frequency array
         f1, nfreq = frequency_parameters(
             hydro_data.omega.values/(2*np.pi), False)
 
         # check real part of damping diagonal > 0
         if min_damping is not None:
@@ -407,16 +380,14 @@
         return WEC(f1, nfreq, forces, constraints, inertia_matrix, dof_names=dof_names)
 
     @staticmethod
     def from_floating_body(
         fb: cpy.FloatingBody,
         f1: float,
         nfreq: int,
-        inertia_matrix: ndarray,
-        hydrostatic_stiffness: ndarray,
         friction: Optional[ndarray] = None,
         f_add: Optional[TIForceDict] = None,
         constraints: Optional[Iterable[Mapping]] = None,
         min_damping: Optional[float] = _default_min_damping,
         wave_directions: Optional[ArrayLike] = np.array([0.0,]),
         rho: Optional[float] = _default_parameters['rho'],
         g: Optional[float] = _default_parameters['g'],
@@ -450,19 +421,14 @@
         fb
             Capytaine FloatingBody.
         f1
             Fundamental frequency :python:`f1` [:math:`Hz`].
         nfreq
             Number of frequencies (not including zero frequency),
             i.e., :python:`freqs = [0, f1, 2*f1, ..., nfreq*f1]`.
-        inertia_matrix
-           Inertia matrix of size :python:`(ndof, ndof)`.
-        hydrostatic_stiffness
-            Linear hydrostatic restoring coefficient of size
-            :python:`(ndof, ndof)`.
         friction
             Linear friction, in addition to radiation damping, of size
             :python:`(ndof, ndof)`.
             :python:`None` to set to zero.
         f_add
             Dictionary with entries :python:`{'force_name': fun}`, where
             :python:`fun` has a  signature
@@ -500,23 +466,23 @@
         # RUN BEM
         _log.info(f"Running Capytaine (BEM): {nfreq+1} frequencies x " +
                  f"{len(wave_directions)} wave directions.")
         freq = frequency(f1, nfreq)[1:]
         bem_data = run_bem(
             fb, freq, wave_directions, rho=rho, g=g, depth=depth)
         wec = WEC.from_bem(
-            bem_data, inertia_matrix, hydrostatic_stiffness, friction, f_add,
+            bem_data, friction, f_add,
             constraints, min_damping=min_damping)
         return wec
 
     @staticmethod
     def from_impedance(
         freqs: ArrayLike,
-        impedance: ArrayLike,
-        exc_coeff: ArrayLike,
+        impedance: DataArray,
+        exc_coeff: DataArray,
         hydrostatic_stiffness: ndarray,
         f_add: Optional[TIForceDict] = None,
         constraints: Optional[Iterable[Mapping]] = None,
         min_damping: Optional[float] = _default_min_damping,
     ) -> TWEC:
         """Create a WEC object from the intrinsic impedance and
         excitation coefficients.
@@ -533,15 +499,15 @@
 
         Parameters
         ----------
         freqs
             Frequency vector [:math:`Hz`] not including the zero frequency,
             :python:`freqs = [f1, 2*f1, ..., nfreq*f1]`.
         impedance
-            Complex impedance of size :python:`(ndof, ndof, nfreq)`.
+            Complex impedance of size :python:`(nfreq, ndof, ndof)`.
         exc_coeff
             Complex excitation transfer function of size
             :python:`(ndof, nfreq)`.
         hydrostatic_stiffness
             Linear hydrostatic restoring coefficient of size
             :python:`(ndof, ndof)`.
         f_add
@@ -567,25 +533,26 @@
             :python:`(ndof, ndof, nfreq)`.
         """
         f1, nfreq = frequency_parameters(freqs, False)
 
         # impedance matrix shape
         shape = impedance.shape
         ndim = impedance.ndim
-        if (ndim!=3) or (shape[0]!=shape[1]) or (shape[2]!=nfreq):
+        if (ndim!=3) or (shape[1]!=shape[2]) or (shape[0]!=nfreq):
             raise ValueError(
-                "'impedance' must have shape '(ndof, ndof, nfreq)'.")
+                "'impedance' must have shape '(nfreq, ndof, ndof)'.")
 
         impedance = check_impedance(impedance, min_damping)
 
         # impedance force
         omega = freqs * 2*np.pi
-        transfer_func = impedance * (1j*omega)
+        omega0 = np.expand_dims(omega, [1,2])
+        transfer_func = impedance * (1j*omega0)
         transfer_func0 = np.expand_dims(hydrostatic_stiffness, 2)
-        transfer_func = np.concatenate([transfer_func0, transfer_func], 2)
+        transfer_func = np.concatenate([transfer_func0, transfer_func], axis=0)
         transfer_func = -1 * transfer_func  # RHS of equation: ma = Σf
         force_impedance = force_from_rao_transfer_function(transfer_func)
 
         # excitation force
         force_excitation = force_from_waves(exc_coeff)
 
         # all forces
@@ -594,18 +561,32 @@
             'intrinsic_impedance': force_impedance,
             'excitation': force_excitation
         }
         forces = forces | f_add
 
         # wec
         wec = WEC(f1, nfreq, forces, constraints,
-                  inertia_in_forces=True, ndof=shape[0])
+                  inertia_in_forces=True, ndof=shape[1])
         return wec
 
-    def _resid_fun(self, x_wec, x_opt, waves):
+    def residual(self, x_wec: ndarray, x_opt: ndarray, waves: Dataset,
+        ) -> float:
+        """
+        Return the residual of the dynamic equation (r = m⋅a-Σf).
+
+        Parameters
+        ----------
+        x_wec
+            WEC state vector.
+        x_opt
+            Optimization (control) state.
+        waves
+            :py:class:`xarray.Dataset` with the structure and elements
+            shown by :py:mod:`wecopttool.waves`.
+        """
         if not self.inertia_in_forces:
             ri = self.inertia(self, x_wec, x_opt, waves)
         else:
             ri = np.zeros([self.ncomponents, self.ndof])
         # forces, -Σf
         for f in self.forces.values():
             ri = ri - f(self, x_wec, x_opt, waves)
@@ -623,17 +604,17 @@
         scale_obj: Optional[float] = 1.0,
         optim_options: Optional[Mapping[str, Any]] = {},
         use_grad: Optional[bool] = True,
         maximize: Optional[bool] = False,
         bounds_wec: Optional[Bounds] = None,
         bounds_opt: Optional[Bounds] = None,
         callback: Optional[TStateFunction] = None,
-        ) -> tuple[Dataset, Dataset, OptimizeResult]:
+        ) -> list[OptimizeResult]:
         """Simulate WEC dynamics using a pseudo-spectral solution
-        method and returns the raw results dictionary produced by 
+        method and returns the raw results dictionary produced by
         :py:func:`scipy.optimize.minimize`.
 
         Parameters
         ----------
         waves
             :py:class:`xarray.Dataset` with the structure and elements
             shown by :py:mod:`wecopttool.waves`.
@@ -688,36 +669,38 @@
         ValueError
             If :python:`scale_x_opt` is a scalar and
             :python:`nstate_opt` is not provided.
         Exception
             If the optimizer fails for any reason other than maximum
             number of states, i.e. for exit modes other than 0 or 9.
             See :py:mod:`scipy.optimize` for exit mode details.
-            
+
         Examples
         --------
         The :py:meth:`wecopttool.WEC.solve` method only returns the
         raw results dictionary produced by :py:func:`scipy.optimize.minimize`.
 
         >>> res_opt = wec.solve(waves=wave,
                                 obj_fun=pto.average_power,
                                 nstate_opt=2*nfreq+1)
 
-        To get the post-processed results for the
-        :py:class:`wecopttool.pto.PTO`, you may call
-
-        >>> res_wec_fd, res_wec_td = wec.post_process(wec,res_opt)
-        >>> res_pto_fd, res_pto_td = pto.post_process(wec,res_opt)
+        To get the post-processed results for the :py:class:`wecopttool.WEC`
+        and :py:class:`wecopttool.pto.PTO` for a single realization, you
+        may call
+
+        >>> realization = 0 # realization index
+        >>> res_wec_fd, res_wec_td = wec.post_process(wec,res_opt[realization])
+        >>> res_pto_fd, res_pto_td = pto.post_process(wec,res_opt[realization])
 
         See Also
         --------
         wecopttool.waves,
         """
 
-        _log.info("Solving pseudo-spectral control problem.")
+        results = []
 
         # x_wec scaling vector
         if scale_x_wec == None:
             scale_x_wec = [1.0] * self.ndof
         elif isinstance(scale_x_wec, float) or isinstance(scale_x_wec, int):
             scale_x_wec = [scale_x_wec] * self.ndof
         scale_x_wec = scale_dofs(scale_x_wec, self.ncomponents)
@@ -727,56 +710,21 @@
             if nstate_opt is None:
                 raise ValueError("If 'scale_x_opt' is a scalar, " +
                                     "'nstate_opt' must be provided")
             scale_x_opt = scale_dofs([scale_x_opt], nstate_opt)
 
         # composite scaling vector
         scale = np.concatenate([scale_x_wec, scale_x_opt])
-
+        
         # decision variable initial guess
         if x_wec_0 is None:
             x_wec_0 = np.random.randn(self.nstate_wec)
         if x_opt_0 is None:
             x_opt_0 = np.random.randn(nstate_opt)
-        x0 = np.concatenate([x_wec_0, x_opt_0])*scale
-
-        # objective function
-        sign = -1.0 if maximize else 1.0
-
-        def obj_fun_scaled(x):
-            x_wec, x_opt = self.decompose_state(x/scale)
-            return obj_fun(self, x_wec, x_opt, waves)*scale_obj*sign
-
-        # constraints
-        constraints = self.constraints.copy()
-
-        for i, icons in enumerate(self.constraints):
-            icons_new = {"type": icons["type"]}
-
-            def make_new_fun(icons):
-                def new_fun(x):
-                    x_wec, x_opt = self.decompose_state(x/scale)
-                    return icons["fun"](self, x_wec, x_opt, waves)
-                return new_fun
-
-            icons_new["fun"] = make_new_fun(icons)
-            if use_grad:
-                icons_new['jac'] = jacobian(icons_new['fun'])
-            constraints[i] = icons_new
-
-        # system dynamics through equality constraint, ma - Σf = 0
-        def scaled_resid_fun(x):
-            x_s = x/scale
-            x_wec, x_opt = self.decompose_state(x_s)
-            return self._resid_fun(x_wec, x_opt, waves)
-
-        eq_cons = {'type': 'eq', 'fun': scaled_resid_fun}
-        if use_grad:
-            eq_cons['jac'] = jacobian(scaled_resid_fun)
-        constraints.append(eq_cons)
+        x0 = np.concatenate([x_wec_0, x_opt_0])*scale 
 
         # bounds
         if (bounds_wec is None) and (bounds_opt is None):
             bounds = None
         else:
             bounds_in = [bounds_wec, bounds_opt]
             for idx, bii in enumerate(bounds_in):
@@ -793,57 +741,101 @@
                     bo = bi
                 else:
                     bo = bd
                 bounds_list.append(bo)
             bounds = Bounds(lb=np.hstack([le.lb for le in bounds_list])*scale,
                             ub=np.hstack([le.ub for le in bounds_list])*scale)
 
-        # callback
-        if callback is None:
-            def callback_scipy(x):
-                x_wec, x_opt = self.decompose_state(x)
-                _log.info("[max(x_wec), max(x_opt), obj_fun(x)]: "
-                          + f"[{np.max(np.abs(x_wec)):.2e}, "
-                          + f"{np.max(np.abs(x_opt)):.2e}, "
-                          + f"{np.max(obj_fun_scaled(x)):.2e}]")
-        else:
-            def callback_scipy(x):
-                x_wec, x_opt = self.decompose_state(x)
-                return callback(self, x_wec, x_opt, waves)
-
-        # optimization problem
-        optim_options['disp'] = optim_options.get('disp', True)
-        problem = {'fun': obj_fun_scaled,
-                    'x0': x0,
-                    'method': 'SLSQP',
-                    'constraints': constraints,
-                    'options': optim_options,
-                    'bounds': bounds,
-                    'callback': callback_scipy,
-                    }
-        if use_grad:
-            problem['jac'] = grad(obj_fun_scaled)
-
-        # minimize
-        optim_res = minimize(**problem)
-
-        msg = f'{optim_res.message}    (Exit mode {optim_res.status})'
-        if optim_res.status == 0:
-            _log.info(msg)
-        elif optim_res.status == 9:
-            _log.warning(msg)
-        else:
-            raise Exception(msg)
+        for realization, wave in waves.groupby('realization'):
+
+            _log.info("Solving pseudo-spectral control problem "
+                      + f"for realization number {realization}.") 
+            
+            # objective function
+            sign = -1.0 if maximize else 1.0
+            
+            def obj_fun_scaled(x):
+                x_wec, x_opt = self.decompose_state(x/scale)
+                return obj_fun(self, x_wec, x_opt, wave)*scale_obj*sign
+
+            # constraints
+            constraints = self.constraints.copy()
+
+            for i, icons in enumerate(self.constraints):
+                icons_new = {"type": icons["type"]}
+
+                def make_new_fun(icons):
+                    def new_fun(x):
+                        x_wec, x_opt = self.decompose_state(x/scale)
+                        return icons["fun"](self, x_wec, x_opt, wave)
+                    return new_fun
+
+                icons_new["fun"] = make_new_fun(icons)
+                if use_grad:
+                    icons_new['jac'] = jacobian(icons_new['fun'])
+                constraints[i] = icons_new
+
+            # system dynamics through equality constraint, ma - Σf = 0
+            def scaled_resid_fun(x):
+                x_s = x/scale
+                x_wec, x_opt = self.decompose_state(x_s)
+                return self.residual(x_wec, x_opt, wave)
 
-        # unscale
-        optim_res.x = optim_res.x / scale
-        optim_res.fun = optim_res.fun / scale_obj
-        optim_res.jac = optim_res.jac / scale_obj * scale
+            eq_cons = {'type': 'eq', 'fun': scaled_resid_fun}
+            if use_grad:
+                eq_cons['jac'] = jacobian(scaled_resid_fun)
+            constraints.append(eq_cons)
+            
+            # callback
+            if callback is None:
+                def callback_scipy(x):
+                    x_wec, x_opt = self.decompose_state(x)
+                    max_x_opt = np.nan if np.size(x_opt)==0 else np.max(np.abs(x_opt))
+                    _log.info("Scaled [max(x_wec), max(x_opt), obj_fun(x)]: "
+                              + f"[{np.max(np.abs(x_wec)):.2e}, "
+                              + f"{max_x_opt:.2e}, "
+                              + f"{obj_fun_scaled(x):.2e}]")
+            else:
+                def callback_scipy(x):
+                    x_s = x/scale
+                    x_wec, x_opt = self.decompose_state(x_s)
+                    return callback(self, x_wec, x_opt, wave)
+
+            # optimization problem
+            optim_options['disp'] = optim_options.get('disp', True)
+            problem = {'fun': obj_fun_scaled,
+                        'x0': x0,
+                        'method': 'SLSQP',
+                        'constraints': constraints,
+                        'options': optim_options,
+                        'bounds': bounds,
+                        'callback': callback_scipy,
+                        }
+            if use_grad:
+                problem['jac'] = grad(obj_fun_scaled)
+
+            # minimize
+            optim_res = minimize(**problem)
 
-        return optim_res
+            msg = f'{optim_res.message}    (Exit mode {optim_res.status})'
+            if optim_res.status == 0:
+                _log.info(msg)
+            elif optim_res.status == 9:
+                _log.warning(msg)
+            else:
+                raise Exception(msg)
+
+            # unscale
+            optim_res.x = optim_res.x / scale
+            optim_res.fun = optim_res.fun / scale_obj
+            optim_res.jac = optim_res.jac / scale_obj * scale
+            
+            results.append(optim_res)
+        
+        return results
 
     def post_process(self,
         res: OptimizeResult,
         waves: Dataset,
         nsubsteps: Optional[int] = 1,
     ) -> tuple[Dataset, Dataset]:
         """Post-process the results from
@@ -863,15 +855,15 @@
 
         Returns
         -------
         results_fd
             Dynamic responses in the frequency-domain.
         results_td
             Dynamic responses in the time-domain.
-            
+
         Examples
         --------
         The :py:meth:`wecopttool.WEC.solve` method only returns the
         raw results dictionary produced by :py:func:`scipy.optimize.minimize`.
 
         >>> res_opt = wec.solve(waves=wave,
                                 obj_fun=pto.average_power,
@@ -881,28 +873,31 @@
         :py:class:`wecopttool.pto.PTO`, you may call
 
         >>> res_wec_fd, res_wec_td = wec.post_process(wec,res_opt)
         >>> res_pto_fd, res_pto_td = pto.post_process(wec,res_opt)
         """
         create_time = f"{datetime.utcnow()}"
 
+        omega_vals = np.concatenate([[0], waves.omega.values])
+        freq_vals = np.concatenate([[0], waves.freq.values])
+        period_vals = np.concatenate([[np.inf], 1/waves.freq.values])
         pos_attr = {'long_name': 'Position', 'units': 'm or rad'}
         vel_attr = {'long_name': 'Velocity', 'units': 'm/s or rad/s'}
         acc_attr = {'long_name': 'Acceleration', 'units': 'm/s^2 or rad/s^2'}
         omega_attr = {'long_name': 'Radial frequency', 'units': 'rad/s'}
         freq_attr = {'long_name': 'Frequency', 'units': 'Hz'}
         period_attr = {'long_name': 'Period', 'units': 's'}
         time_attr = {'long_name': 'Time', 'units': 's'}
         dof_attr = {'long_name': 'Degree of freedom'}
         force_attr = {'long_name': 'Force or moment', 'units': 'N or Nm'}
         wave_elev_attr = {'long_name': 'Wave elevation', 'units': 'm'}
         x_wec, x_opt = self.decompose_state(res.x)
-        omega_coord = ("omega", self.omega, omega_attr)
-        freq_coord = ("omega", self.frequency, freq_attr)
-        period_coord = ("omega", self.period, period_attr)
+        omega_coord = ("omega", omega_vals, omega_attr)
+        freq_coord = ("omega", freq_vals, freq_attr)
+        period_coord = ("omega", period_vals, period_attr)
         dof_coord = ("influenced_dof", self.dof_names, dof_attr)
 
         # frequency domain
         force_da_list = []
         for name, force in self.forces.items():
             force_td_tmp = force(self, x_wec, x_opt, waves)
             force_fd = self.td_to_fd(force_td_tmp)
@@ -1052,41 +1047,41 @@
         return self._time
 
     @property
     def time_mat(self) -> ndarray:
         """Matrix to create time-series from Fourier coefficients.
 
         For some array of Fourier coefficients :python:`x`
-        (excluding the sine component of the highest freequency), size
+        (excluding the sine component of the highest frequency), size
         :python:`(2*nfreq, ndof)`, the time series is obtained via
         :python:`time_mat @ x`, also size
         :python:`(2*nfreq, ndof)`.
         """
         return self._time_mat
 
     @property
     def derivative_mat(self) -> ndarray:
         """Matrix to create Fourier coefficients of the derivative of
         some quantity.
 
         For some array of Fourier coefficients :python:`x`
-        (excluding the sine component of the highest freequency), size
+        (excluding the sine component of the highest frequency), size
         :python:`(2*nfreq, ndof)`, the Fourier coefficients of the
         derivative of :python:`x` are obtained via
         :python:`derivative_mat @ x`.
         """
         return self._derivative_mat
 
     @property
     def derivative2_mat(self) -> ndarray:
         """Matrix to create Fourier coefficients of the second derivative of
         some quantity.
 
         For some array of Fourier coefficients :python:`x`
-        (excluding the sine component of the highest freequency), size
+        (excluding the sine component of the highest frequency), size
         :python:`(2*nfreq, ndof)`, the Fourier coefficients of the
         second derivative of :python:`x` are obtained via
         :python:`derivative2_mat @ x`.
         """
         return self._derivative2_mat
 
     @property
@@ -1480,25 +1475,25 @@
     diagonal = np.repeat(-np.ones(nfreq) * vals, 2)[:-1] # remove 2pt wave sine
     if zero_freq:
         diagonal = np.concatenate(([0.0], diagonal))
     return np.diag(diagonal)
 
 
 def mimo_transfer_mat(
-    transfer_mat: ArrayLike,
+    transfer_mat: DataArray,
     zero_freq: Optional[bool] = True,
 ) -> ndarray:
     """Create a block matrix of the MIMO transfer function.
 
     The input is a complex transfer matrix that relates the complex
     Fourier representation of two variables.
     For example, it can be an impedance matrix or an RAO transfer
     matrix.
     The input complex impedance matrix has shape
-    :python`(ndof, ndof, nfreq)`.
+    :python`(nfreq, ndof, ndof)`.
 
     Returns the 2D real matrix that transform the state representation
     of the input variable variable to the state representation of the
     output variable.
     Here, a state representation :python:`x` consists of the mean (DC)
     component followed by the real and imaginary components of the
     Fourier coefficients (excluding the imaginary component of the
@@ -1511,28 +1506,28 @@
     Parameters
     ----------
     transfer_mat
         Complex transfer matrix.
     zero_freq
         Whether the first frequency should be zero.
     """
-    ndof = transfer_mat.shape[0]
-    assert transfer_mat.shape[1] == ndof
+    ndof = transfer_mat.shape[1]
+    assert transfer_mat.shape[2] == ndof
     elem = [[None]*ndof for _ in range(ndof)]
     def block(re, im): return np.array([[re, -im], [im, re]])
     for idof in range(ndof):
         for jdof in range(ndof):
             if zero_freq:
-                Zp0 = transfer_mat[idof, jdof, 0]
+                Zp0 = transfer_mat[0, idof, jdof]
                 assert np.all(np.isreal(Zp0))
                 Zp0 = np.real(Zp0)
-                Zp = transfer_mat[idof, jdof, 1:]
+                Zp = transfer_mat[1:, idof, jdof]
             else:
                 Zp0 = [0.0]
-                Zp = transfer_mat[idof, jdof, :]
+                Zp = transfer_mat[:, idof, jdof]
             re = np.real(Zp)
             im = np.imag(Zp)
             blocks = [block(ire, iim) for (ire, iim) in zip(re[:-1], im[:-1])]
             blocks = [Zp0] + blocks + [re[-1]]
             elem[idof][jdof] = block_diag(*blocks)
     return np.block(elem)
 
@@ -1857,15 +1852,15 @@
     min_damping
         Minimum threshold for damping. Default is 1e-6.
     uniform_shift
         Boolean that determines whether the damping correction for each
         degree of freedom is frequency dependent or not. If :python:`True`,
         the damping correction is applied to :python:`friction` and shifts the
         damping for all frequencies. If :python:`False`, the damping correction
-        is applied to :python:`radiation_damping` and only shifts the 
+        is applied to :python:`radiation_damping` and only shifts the
         damping for frequencies with negative damping values. Default is
         :python:`True`.
     """
     hydro_data_new = hydro_data.copy(deep=True)
     radiation = hydro_data_new['radiation_damping']
     friction = hydro_data_new['friction']
     ndof = len(hydro_data_new.influenced_dof)
@@ -1893,15 +1888,15 @@
                     'zero terms. Shifting up damping terms to a minimum of ' +
                     f'{min_damping} N/(m/s)')
             hydro_data_new['radiation_damping'][:, idof, idof] = new_damping
     return hydro_data_new
 
 
 def check_impedance(
-    Zi: ArrayLike,
+    Zi: DataArray,
     min_damping: Optional[float] = 1e-6,
 ) -> DataArray:
     """Ensure that the real part of the impedance (resistive) is positive.
 
     Adds to real part of the impedance.
     Returns the (possibly) updated impedance with
     :math:`Re(Zi)>=` :python:`min_damping`.
@@ -1909,30 +1904,30 @@
     Parameters
     ----------
     Zi
         Linear hydrodynamic impedance.
     min_damping
         Minimum threshold for damping. Default is 1e-6.
     """
-    Zi_diag = np.diagonal(Zi,axis1=0,axis2=1)
+    Zi_diag = np.diagonal(Zi,axis1=1,axis2=2)
     Zi_shifted = Zi.copy()
     for dof in range(Zi_diag.shape[1]):
         dmin = np.min(np.real(Zi_diag[:, dof]))
         if dmin < min_damping:
             delta = min_damping - dmin
-            Zi_shifted[dof,dof,:] = Zi_diag[:, dof] \
+            Zi_shifted[:, dof, dof] = Zi_diag[:, dof] \
                 + np.abs(delta)
             _log.warning(
                 f'Real part of impedance for {dof} has negative or close to ' +
                 f'zero terms. Shifting up by {delta:.2f}')
     return Zi_shifted
 
 
 def force_from_rao_transfer_function(
-    rao_transfer_mat: ArrayLike,
+    rao_transfer_mat: DataArray,
     zero_freq: Optional[bool] = True,
 ) -> TStateFunction:
     """Create a force function from its position transfer matrix.
 
     This is the position equivalent to the velocity-based
     :py:func:`wecopttool.force_from_impedance`.
 
@@ -1956,15 +1951,15 @@
         force_fd = wec.vec_to_dofmat(np.dot(transfer_mat, x_wec))
         return np.dot(wec.time_mat, force_fd)
     return force
 
 
 def force_from_impedance(
     omega: ArrayLike,
-    impedance: ArrayLike,
+    impedance: DataArray,
 ) -> TStateFunction:
     """Create a force function from its impedance.
 
     Parameters
     ----------
     omega
         Radial frequency vector.
@@ -1974,15 +1969,15 @@
     See Also
     --------
     force_from_rao_transfer_function,
     """
     return force_from_rao_transfer_function(impedance*(1j*omega), False)
 
 
-def force_from_waves(force_coeff: ArrayLike,
+def force_from_waves(force_coeff: DataArray,
                      ) -> TStateFunction:
     """Create a force function from waves excitation coefficients.
 
     Parameters
     ----------
     force_coeff
         Complex excitation coefficients indexed by frequency and
@@ -2006,16 +2001,16 @@
     f1
         Fundamental frequency :python:`f1` [:math:`Hz`].
     nfreq
         Number of frequencies.
     inertia_matrix
         Inertia matrix.
     """
-    omega = np.reshape(frequency(f1, nfreq, False)*2*np.pi, [1,1,-1])
-    inertia_matrix = np.expand_dims(inertia_matrix, -1)
+    omega = np.expand_dims(frequency(f1, nfreq, False)*2*np.pi, [1,2])
+    inertia_matrix = np.expand_dims(inertia_matrix, 0)
     rao_transfer_function = -1*omega**2*inertia_matrix + 0j
     inertia_fun = force_from_rao_transfer_function(
         rao_transfer_function, False)
     return inertia_fun
 
 
 def standard_forces(hydro_data: Dataset) -> TForceDict:
@@ -2027,38 +2022,36 @@
     API Documentation).
 
     Parameters
     ----------
     hydro_data
         Linear hydrodynamic data.
     """
-    hydro_data = hydro_data.transpose(
-         "omega", "wave_direction", "radiating_dof", "influenced_dof")
 
     # intrinsic impedance
     w = hydro_data['omega']
     A = hydro_data['added_mass']
     B = hydro_data['radiation_damping']
     K = hydro_data['hydrostatic_stiffness']
     Bf = hydro_data['friction']
 
     rao_transfer_functions = dict()
     rao_transfer_functions['radiation'] = (1j*w*B + -1*w**2*A, False)
     rao_transfer_functions['friction'] = (1j*w*Bf, False)
 
     # include zero_freq in hydrostatics
-    hs = ((K + 0j).expand_dims({"omega": B.omega}))
+    hs = ((K + 0j).expand_dims({"omega": B.omega}, 0))
     tmp = hs.isel(omega=0).copy(deep=True)
     tmp['omega'] = tmp['omega'] * 0
     hs = xr.concat([tmp, hs], dim='omega') #, data_vars='minimal')
     rao_transfer_functions['hydrostatics'] = (hs, True)
 
     linear_force_functions = dict()
     for name, (value, zero_freq) in rao_transfer_functions.items():
-        value = value.transpose("radiating_dof", "influenced_dof", "omega")
+        value = value.transpose("omega", "radiating_dof", "influenced_dof")
         value = -1*value  # RHS of equation: ma = Σf
         linear_force_functions[name] = (
             force_from_rao_transfer_function(value, zero_freq))
 
     # wave excitation
     excitation_coefficients = {
         'Froude_Krylov': hydro_data['Froude_Krylov_force'],
@@ -2132,20 +2125,25 @@
         'radiating_dof': list(fb.dofs.keys()),
         'g': [g],
     })
     if wave_dirs is None:
         # radiation only problem, no diffraction or excitation
         test_matrix = test_matrix.drop_vars('wave_direction')
     if write_info is None:
-        write_info = {'hydrostatics': False,
+        write_info = {'hydrostatics': True,
                       'mesh': False,
                       'wavelength': False,
                       'wavenumber': False,
                      }
     wec_im = fb.copy(name=f"{fb.name}_immersed").keep_immersed_part()
+    wec_im = set_fb_centers(wec_im, rho=rho)
+    if not hasattr(wec_im, 'inertia_matrix'):
+        wec_im.inertia_matrix = wec_im.compute_rigid_body_inertia(rho=rho)
+    if not hasattr(wec_im, 'hydrostatic_stiffness'):
+        wec_im.hydrostatic_stiffness = wec_im.compute_hydrostatic_stiffness(rho=rho, g=g)
     bem_data = solver.fill_dataset(
         test_matrix, wec_im, n_jobs=njobs, **write_info)
     return change_bem_convention(bem_data)
 
 
 def change_bem_convention(bem_data: Dataset) -> Dataset:
     """Change the convention from :math:`-iωt` to :math:`+iωt`.
@@ -2164,90 +2162,57 @@
     """
     bem_data['Froude_Krylov_force'] = np.conjugate(
         bem_data['Froude_Krylov_force'])
     bem_data['diffraction_force'] = np.conjugate(bem_data['diffraction_force'])
     return bem_data
 
 
-def linear_hydrodynamics(
+def add_linear_friction(
     bem_data: Dataset,
-    inertia_matrix: Optional[ArrayLike] = None,
-    hydrostatic_stiffness: Optional[ArrayLike] = None,
     friction: Optional[ArrayLike] = None
 ) -> Dataset:
-    """Add rigid body inertia_matrix, hydrostatic stiffness, and linear
-    friction to BEM data.
+    """Add linear friction to BEM data.
 
     Returns the Dataset with the additional information added.
 
     Parameters
     ----------
     bem_data
         Linear hydrodynamic coefficients obtained using the boundary
         element method (BEM) code Capytaine, with sign convention
-        corrected.
-    inertia_matrix
-        Inertia matrix of size :python:`(ndof, ndof)`.
-        :python:`None` if included in :python:`bem_data`.
-    hydrostatic_stiffness
-        Linear hydrostatic restoring coefficient of size
-        :python:`(nodf, ndof)`.
-        :python:`None` if included in :python:`bem_data`.
+        corrected. Also includes inertia and hydrostatic stiffness.
     friction
         Linear friction, in addition to radiation damping, of size
         :python:`(nodf, ndof)`.
         :python:`None` if included in :python:`bem_data` or to set to zero.
-
-    Raises
-    ------
-    ValueError
-        If either :python:`inertia_matrix` or
-        :python:`hydrostatic_stiffness` are :python:`None` and is not
-        included in :python:`bem_data`.
-    ValueError
-        If any of :python:`inertia_matrix`,
-        :python:`hydrostatic_stiffness`, or :python:`friction` are both
-        provided and included in :python:`bem_data` but have different
-        values.
     """
-    vars = {'inertia_matrix': inertia_matrix, 'friction': friction,
-            'hydrostatic_stiffness': hydrostatic_stiffness}
-
     dims = ['radiating_dof', 'influenced_dof']
-
     hydro_data = bem_data.copy(deep=True)
-
-    for name, data in vars.items():
-        org = name in hydro_data.variables.keys()
-        new = data is not None
-        if new and org:
+    
+    if friction is not None:
+        if 'friction' in hydro_data.variables.keys():
             if not np.allclose(data, hydro_data.variables[name]):
                 raise ValueError(
-                    f'BEM data already has variable "{name}" ' +
-                    'with diferent values')
-            else :
+                        f'Variable "friction" is already in BEM data ' +
+                        f'with different values.')
+            else:
                 _log.warning(
                     f'Variable "{name}" is already in BEM data ' +
                     'with same value.')
-        elif (not new) and (not org):
-            if name=='friction':
-                ndof = len(hydro_data["influenced_dof"])
-                hydro_data[name] = (dims, np.zeros([ndof, ndof]))
-            else:
-                raise ValueError(
-                    f'Variable "{name}" is not in BEM data and ' +
-                    'was not provided.')
-        elif new:
-            data = atleast_2d(data)
-            hydro_data[name] = (dims, data)
-
+        else:
+            data = atleast_2d(friction)
+            hydro_data['friction'] = (dims, friction)
+    elif friction is None:
+        ndof = len(hydro_data["influenced_dof"])
+        hydro_data['friction'] = (dims, np.zeros([ndof, ndof]))
+            
     return hydro_data
 
 
-def wave_excitation(exc_coeff: Dataset, waves: Dataset) -> ndarray:
+def wave_excitation(exc_coeff: DataArray, waves: Dataset) -> ndarray:
     """Calculate the complex, frequency-domain, excitation force due to
     waves.
 
     The resulting force is indexed only by frequency and not direction
     angle.
     The input :python:`waves` frequencies must be same as
     :python:`exc_coeff`, but the directions can be a subset.
@@ -2269,16 +2234,15 @@
         If any of the directions in :python:`waves` is not in
         :python:`exc_coeff`.
     """
     omega_w = waves['omega'].values
     omega_e = exc_coeff['omega'].values
     dir_w = waves['wave_direction'].values
     dir_e = exc_coeff['wave_direction'].values
-    exc_coeff = exc_coeff.transpose(
-        'omega', 'wave_direction', 'influenced_dof').values
+    exc_coeff = exc_coeff.values
 
     wave_elev_fd = np.expand_dims(waves.values, -1)
 
     if not np.allclose(omega_w, omega_e):
         raise ValueError(f"Wave and excitation frequencies do not match. WW: {omega_w}, EE: {omega_e}")
 
     subset, sub_ind = subset_close(dir_w, dir_e)
@@ -2295,22 +2259,22 @@
 def hydrodynamic_impedance(hydro_data: Dataset) -> Dataset:
     """Calculate hydrodynamic intrinsic impedance.
 
     Parameters
     ----------
     hydro_data
         Dataset with linear hydrodynamic coefficients produced by
-        :py:func:`wecopttool.linear_hydrodynamics`.
+        :py:func:`wecopttool.add_linear_friction`.
     """
 
     Zi = (hydro_data['inertia_matrix'] \
         + hydro_data['added_mass'])*1j*hydro_data['omega'] \
             + hydro_data['radiation_damping'] + hydro_data['friction'] \
                 + hydro_data['hydrostatic_stiffness']/1j/hydro_data['omega']
-    return Zi
+    return Zi.transpose('omega', 'radiating_dof', 'influenced_dof')
 
 
 def atleast_2d(array: ArrayLike) -> ndarray:
     """Ensure an array is at least 2D, otherwise add trailing dimensions
     to make it 2D.
 
     This differs from :py:func:`numpy.atleast_2d` in that the additional
@@ -2341,17 +2305,15 @@
         1D array of angles in degrees.
     sort
         Whether to sort the angles from smallest to largest in
         :math:`[-π, π)`.
     """
     radians = np.asarray(np.remainder(np.deg2rad(degrees), 2*np.pi))
     radians[radians > np.pi] -= 2*np.pi
-    if radians.size == 1:
-        radians = radians.item()
-    elif sort:
+    if radians.size > 1 and sort:
         radians = np.sort(radians)
     return radians
 
 
 def subset_close(
     set_a: FloatOrArray,
     set_b: FloatOrArray,
@@ -2397,26 +2359,24 @@
 
     if len(np.unique(set_a.round(decimals = 6))) != len(set_a):
         raise ValueError("Elements in set_a not unique")
     if len(np.unique(set_b.round(decimals = 6))) != len(set_b):
         raise ValueError("Elements in set_b not unique")
 
     ind = []
-    tmp_result = [False for _ in range(len(set_a))]
-    for subset_element in set_a:
-        for set_element in set_b:
-            if np.isclose(subset_element, set_element, rtol, atol, equal_nan):
-                tmp_set_ind = np.where(
-                    np.isclose(set_element, set_b , rtol, atol, equal_nan))
-                tmp_subset_ind = np.where(
-                    np.isclose(subset_element, set_a , rtol, atol,
-                               equal_nan))
-                ind.append( int(tmp_set_ind[0]) )
-                tmp_result[ int(tmp_subset_ind[0]) ] = True
-    subset = all(tmp_result)
+    for el in set_a:
+        a_in_b = np.isclose(set_b, el,
+                            rtol=rtol, atol=atol, equal_nan=equal_nan)
+        if np.sum(a_in_b) == 1:
+            ind.append(np.flatnonzero(a_in_b)[0])
+        if np.sum(a_in_b) > 1:
+            _log.warning('Multiple matching elements in subset, ' +
+                         'selecting closest match.')
+            ind.append(np.argmin(np.abs(a_in_b - el)))
+    subset = len(set_a) == len(ind)
     ind = ind if subset else []
     return subset, ind
 
 
 def scale_dofs(scale_list: Iterable[float], ncomponents: int) -> ndarray:
     """Create a scaling vector based on a different scale for each DOF.
 
@@ -2546,7 +2506,39 @@
         Time array.
     """
     out = np.zeros((*fd.isel(omega=0).shape, len(time)))
     for w, mag in zip(fd.omega, fd):
         out = out + \
             np.real(mag)*np.cos(w*time) - np.imag(mag)*np.sin(w*time)
     return out
+
+
+def set_fb_centers(
+    fb: FloatingBody,
+    rho: float = _default_parameters["rho"],
+) -> FloatingBody:
+    """Sets default properties if not provided by the user:
+        - `center_of_mass` is set to the geometric centroid
+        - `rotation_center` is set to the center of mass
+    """
+    valid_properties = ['center_of_mass', 'rotation_center']
+    
+    for property in valid_properties:
+        if not hasattr(fb, property):
+            setattr(fb, property, None)
+        if getattr(fb, property) is None:
+            if property == 'center_of_mass':
+                def_val = fb.center_of_buoyancy
+                log_str = (
+                    "Using the geometric centroid as the center of gravity (COG).")
+            elif property == 'rotation_center':
+                def_val = fb.center_of_mass
+                log_str = (
+                    "Using the center of gravity (COG) as the rotation center " +
+                    "for hydrostatics.")
+            setattr(fb, property, def_val)
+            _log.warning(log_str)
+        elif getattr(fb, property) is not None:
+            _log.warning(
+                f'{property} already defined as {getattr(fb, property)}.')
+            
+    return fb
```

### Comparing `wecopttool-2.6.0/wecopttool/geom.py` & `wecopttool-2.7.0/wecopttool/geom.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.6.0/wecopttool/pto.py` & `wecopttool-2.7.0/wecopttool/pto.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             Number of degrees of freedom.
         kinematics
             Transforms state from WEC to PTO frame. May be a matrix
             (for linear kinematics) or function (for nonlinear
             kinematics).
         controller
             Function with signature
-            :python:`def fun(wec, x_wec, x_opt, waves, nsubsteps):`
+            :python:`def fun(pto, wec, x_wec, x_opt, waves, nsubsteps):`
             or matrix with shape (PTO DOFs, WEC DOFs) that converts
             from the WEC DOFs to the PTO DOFs.
         impedance
             Matrix representing the PTO impedance.
         loss
             Function that maps flow and effort variables to a
             non-linear power loss.
@@ -919,14 +919,15 @@
     x_wec: ndarray,
     x_opt: ndarray,
     waves: Optional[Dataset] = None,
     nsubsteps: Optional[int] = 1,
     proportional: Optional[bool] = True,
     integral: Optional[bool] = True,
     derivative: Optional[bool] = True,
+    saturation: Optional[FloatOrArray] = None,
 ) -> ndarray:
     """Proportional-integral-derivative (PID) controller that returns
     a time history of PTO forces.
 
     Parameters
     ----------
     pto
@@ -937,53 +938,81 @@
         WEC dynamic state.
     x_opt
         Optimization (control) state.
     waves
         :py:class:`xarray.Dataset` with the structure and elements shown
         by :py:mod:`wecopttool.waves`.
     nsubsteps
-            Number of steps between the default (implied) time steps.
-            A value of :python:`1` corresponds to the default step
-            length.
+        Number of steps between the default (implied) time steps.
+        A value of :python:`1` corresponds to the default step length.
     proportional
         True to include proportional gain
     integral
         True to include integral gain
     derivative
         True to include derivative gain
+    saturation
+        Maximum and minimum control value.
+        Can be symmetric ([ndof]) or asymmetric ([ndof, 2]).
     """
     ndof = pto.ndof
-    force_td = np.zeros([wec.nt*nsubsteps, ndof])
+    force_td_tmp = np.zeros([wec.nt*nsubsteps, ndof])
+
+    # PID force
     idx = 0
 
     def update_force_td(response):
-        nonlocal idx, force_td
-        gain = np.reshape(x_opt[idx*ndof:(idx+1)*ndof], [1, ndof])
-        force_td = force_td + gain*response
+        nonlocal idx, force_td_tmp
+        gain = np.diag(x_opt[idx*ndof:(idx+1)*ndof])
+        force_td_tmp = force_td_tmp + np.dot(response, gain.T)
         idx = idx + 1
+        return
 
     if proportional:
         vel_td = pto.velocity(wec, x_wec, x_opt, waves, nsubsteps)
         update_force_td(vel_td)
     if integral:
         pos_td = pto.position(wec, x_wec, x_opt, waves, nsubsteps)
         update_force_td(pos_td)
     if derivative:
         acc_td = pto.acceleration(wec, x_wec, x_opt, waves, nsubsteps)
         update_force_td(acc_td)
+
+    # Saturation
+    if saturation is not None:
+        saturation = np.atleast_2d(np.squeeze(saturation))
+        assert len(saturation)==ndof
+        if len(saturation.shape) > 2:
+            raise ValueError("`saturation` must have <= 2 dimensions.")
+        if saturation.shape[1] == 1:
+            f_min, f_max = -1*saturation, saturation
+        elif saturation.shape[1] == 2:
+            f_min, f_max = saturation[:,0], saturation[:,1]
+        else:
+            raise ValueError("`saturation` must have 1 or 2 columns.")
+
+        force_td_list = []
+        for i in range(ndof):
+            tmp = np.clip(force_td_tmp[:,i], f_min[i], f_max[i])
+            force_td_list.append(tmp)
+        force_td = np.array(force_td_list).T
+    else:
+        force_td = force_td_tmp
+
     return force_td
 
 
 def controller_pi(
     pto: TPTO,
     wec: TWEC,
     x_wec: ndarray,
     x_opt: ndarray,
     waves: Optional[Dataset] = None,
     nsubsteps: Optional[int] = 1,
+    saturation: Optional[FloatOrArray] = None,
 ) -> ndarray:
     """Proportional-integral (PI) controller that returns a time
     history of PTO forces.
 
     Parameters
     ----------
     pto
@@ -994,30 +1023,35 @@
         WEC dynamic state.
     x_opt
         Optimization (control) state.
     waves
         :py:class:`xarray.Dataset` with the structure and elements shown
         by :py:mod:`wecopttool.waves`.
     nsubsteps
-            Number of steps between the default (implied) time steps.
-            A value of :python:`1` corresponds to the default step
-            length.
+        Number of steps between the default (implied) time steps.
+        A value of :python:`1` corresponds to the default step length.
+    saturation
+        Maximum and minimum control value.
+        Can be symmetric ([ndof]) or asymmetric ([ndof, 2]).
     """
-    force_td = controller_pid(pto, wec, x_wec, x_opt, waves, nsubsteps,
-                              True, True, False)
+    force_td = controller_pid(
+        pto, wec, x_wec, x_opt, waves, nsubsteps,
+        True, True, False, saturation,
+    )
     return force_td
 
 
 def controller_p(
     pto: TPTO,
     wec: TWEC,
     x_wec: ndarray,
     x_opt: ndarray,
     waves: Optional[Dataset] = None,
     nsubsteps: Optional[int] = 1,
+    saturation: Optional[FloatOrArray] = None,
 ) -> ndarray:
     """Proportional (P) controller that returns a time history of
     PTO forces.
 
     Parameters
     ----------
     pto
@@ -1030,11 +1064,48 @@
         Optimization (control) state.
     waves
         :py:class:`xarray.Dataset` with the structure and elements shown
         by :py:mod:`wecopttool.waves`.
     nsubsteps
         Number of steps between the default (implied) time steps.
         A value of :python:`1` corresponds to the default step length.
+    saturation
+        Maximum and minimum control value. Can be symmetric ([ndof]) or
+        asymmetric ([ndof, 2]).
     """
-    force_td = controller_pid(pto, wec, x_wec, x_opt, waves, nsubsteps,
-                               True, False, False)
+    force_td = controller_pid(
+        pto, wec, x_wec, x_opt, waves, nsubsteps,
+        True, False, False, saturation,
+    )
     return force_td
+
+
+# utilities
+def nstate_unstructured(nfreq: int, ndof: int) -> int:
+    """
+    Number of states needed to represent an unstructured controller.
+
+    Parameters
+    ----------
+    nfreq
+        Number of frequencies.
+    ndof
+        Number of degrees of freedom.
+    """
+    return 2*nfreq*ndof
+
+
+def nstate_pid(
+        nterm: int,
+        ndof: int,
+) -> int:
+    """
+    Number of states needed to represent an unstructured controller.
+
+    Parameters
+    ----------
+    nterm
+        Number of terms (e.g. 1 for P, 2 for PI, 3 for PID).
+    ndof
+        Number of degrees of freedom.
+    """
+    return int(nterm*ndof)
```

### Comparing `wecopttool-2.6.0/wecopttool/waves.py` & `wecopttool-2.7.0/wecopttool/waves.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 _log = logging.getLogger(__name__)
 
 
 def elevation_fd(
     f1: float,
     nfreq: int,
     directions: Union[float, ArrayLike],
+    nrealizations: int,
     amplitudes: Optional[ArrayLike] = None,
     phases: Optional[ArrayLike] = None,
     attr: Optional[Mapping] = None,
     seed: Optional[float] = None,
 ) -> DataArray:
     """Construct the complex wave elevation
     :py:class:`xarray.DataArray`.
@@ -71,45 +72,56 @@
     f1
         Fundamental frequency :python:`f1` [Hz].
     nfreq
         Number of frequencies (not including zero frequency),
         i.e., :python:`freq = [0, f1, 2*f1, ..., nfreq*f1]`.
     directions
         Wave directions in degrees. 1D array.
+    nrealizations
+        Number of wave phase realizations.
     amplitudes:
         Wave elevation amplitude in meters.
     phases:
         Wave phases in degrees.
     attr:
         Additional attributes (metadata) to include in the
         :py:class:`xarray.DataArray`.
     seed
         Seed for random number generator. Used for reproducibility.
         Generally should not be used except for testing.
     """
     directions = np.atleast_1d(degrees_to_radians(directions, sort=False))
     ndirections = len(directions)
+    realization = range(nrealizations)
     freq = frequency(f1, nfreq, False)
     omega = freq*2*np.pi
 
-    dims = ('omega', 'wave_direction')
+    dims = ('omega', 'wave_direction', 'realization')
     omega_attr = {'long_name': 'Radial frequency', 'units': 'rad/s'}
     freq_attr = {'long_name': 'Frequency', 'units': 'Hz'}
     dir_attr = {'long_name': 'Wave direction', 'units': 'rad'}
+    real_attr = {'long_name': 'Phase realization', 'units': ''}
     coords = {'omega': (dims[0], omega, omega_attr),
               'freq': (dims[0], freq, freq_attr),
-              'wave_direction': (dims[1], directions, dir_attr)}
+              'wave_direction': (dims[1], directions, dir_attr),
+              'realization': (dims[2], realization, real_attr)}
 
     if amplitudes is None:
-        amplitudes = np.zeros([nfreq, ndirections])
+        amplitudes = np.zeros([nfreq, ndirections, nrealizations])
+    else:
+        if amplitudes.shape == (nfreq, ndirections):
+            amplitudes = np.expand_dims(amplitudes,axis=2)
+        assert amplitudes.shape == (nfreq, ndirections, 1) or \
+                amplitudes.shape == (nfreq, ndirections, nrealizations)
 
     if phases is None:
-        phases = random_phase([nfreq, ndirections],seed)
+        phases = random_phase([nfreq, ndirections, nrealizations], seed)
     else:
         phases = degrees_to_radians(phases, False)
+        assert phases.shape == (nfreq, ndirections, nrealizations)
 
     camplitude = amplitudes * np.exp(1j*phases)
 
     attr = {} if attr is None else attr
     attrs = {'units': 'm', 'long_name': 'Wave elevation'} | attr
 
     waves = DataArray(camplitude, dims=dims, coords=coords,
@@ -145,15 +157,15 @@
         Phase (in degrees) of the regular wave.
     direction
         Direction (in degrees) of the regular wave.
     """
 
     # attributes & index
     omega = freq*2*np.pi
-    tmp_waves = elevation_fd(f1, nfreq, direction)
+    tmp_waves = elevation_fd(f1, nfreq, direction, 1)
     iomega = tmp_waves.sel(omega=omega, method='nearest').omega.values
     ifreq = iomega/(2*np.pi)
 
     if not np.isclose(iomega, omega):
         _log.warning(
             f"Requested frequency {freq} Hz is not in array. " +
             f"Using nearest value of {ifreq} Hz."
@@ -171,23 +183,24 @@
     if phase is None:
         rphase = random_phase()
         phase = np.degrees(rphase)
     else:
         rphase = degrees_to_radians(phase)
 
     # wave elevation
-    tmp = np.zeros([nfreq, 1])
-    waves = elevation_fd(f1, nfreq, direction, tmp, tmp, attrs)
+    tmp = np.zeros([nfreq, 1, 1])
+    waves = elevation_fd(f1, nfreq, direction, 1, tmp, tmp, attrs)
     waves.loc[{'omega': iomega}] = amplitude  * np.exp(1j*rphase)
 
     return waves
 
 
 def long_crested_wave(
     efth: DataArray,
+    nrealizations: int,
     direction: Optional[float] = 0.0,
     seed: Optional[float] = None,
 ) -> DataArray:
     """Create a complex frequency-domain wave elevation from an
     omnidirectional spectrum.
 
     The omnidirectional spectrum is in the
@@ -199,14 +212,17 @@
               :python:`da.interp(freq=[...])`.
 
     Parameters
     ----------
     efth
         Omnidirection wave spectrum in units of m^2/Hz, in the format
         used by :py:class:`wavespectra.SpecArray`.
+    nrealizations
+        Number of wave phase realizations to be created for the 
+        long-crested wave.
     direction
         Direction (in degrees) of the long-crested wave.
     seed
         Seed for random number generator. Used for reproducibility.
         Generally should not be used except for testing.
     """
     f1, nfreq = frequency_parameters(efth.freq.values, False)
@@ -217,18 +233,19 @@
     amplitudes = np.sqrt(2 * values * df)
 
     attr = {
         'Wave type': 'Long-crested irregular',
         'Direction (degrees)': direction,
     }
 
-    return elevation_fd(f1, nfreq, direction, amplitudes, None, attr, seed)
+    return elevation_fd(f1, nfreq, direction, nrealizations, amplitudes, None, attr, seed)
 
 
 def irregular_wave(efth: DataArray,
+                   nrealizations: int,
                    seed: Optional[float] = None,) -> DataArray:
     """Create a complex frequency-domain wave elevation from a spectrum.
 
     The omnidirectional spectrum is in the
     :py:class:`wavespectra.SpecArray` format.
 
     .. note:: The frequencies must be evenly-spaced with spacing equal
@@ -239,14 +256,17 @@
     .. note:: The wave directions must also be evenly spaced.
 
     Parameters
     ----------
     efth
         Wave spectrum in units of m^2/Hz/deg, in the format used by
         :py:class:`wavespectra.SpecArray`.
+    nrealizations
+        Number of wave phase realizations to be created for the 
+        irregular wave.
     seed
         Seed for random number generator. Used for reproducibility.
         Generally should not be used except for testing.
     """
     f1, nfreq = frequency_parameters(efth.freq.values, False)
     directions = efth.dir.values
     df = f1
@@ -254,19 +274,19 @@
 
     values = efth.values
     values[values<0] = np.nan
     amplitudes = np.sqrt(2 * values * df * dd)
 
     attr = {'Wave type': 'Irregular'}
 
-    return elevation_fd(f1, nfreq, directions, amplitudes, None, attr, seed)
+    return elevation_fd(f1, nfreq, directions, nrealizations, amplitudes, None, attr, seed)
 
 
 def random_phase(
-    shape: Optional[Union[Iterable[int], int]] = None,
+    shape: Optional[Union[Iterable[int], int, int]] = None,
     seed: Optional[float] = None,
 ) -> Union[float , ndarray]:
     """Generate random phases in range [-π, π) radians.
 
     Parameters
     ----------
     shape
```

