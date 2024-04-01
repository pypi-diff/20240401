# Comparing `tmp/quantumspectra_2024-0.1.3.tar.gz` & `tmp/quantumspectra_2024-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumspectra_2024-0.1.3.tar", max compression
+gzip compressed data, was "quantumspectra_2024-0.1.4.tar", max compression
```

## Comparing `quantumspectra_2024-0.1.3.tar` & `quantumspectra_2024-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      137 2024-03-27 15:43:55.038861 quantumspectra_2024-0.1.3/README.md
--rw-r--r--   0        0        0      795 2024-03-29 14:31:00.102550 quantumspectra_2024-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 09:19:33.752822 quantumspectra_2024-0.1.3/quantumspectra_2024/__init__.py
--rw-r--r--   0        0        0      127 2024-03-28 00:01:24.766871 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/__init__.py
--rw-r--r--   0        0        0     2800 2024-03-29 14:24:44.809724 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/mlj/MLJComputation.py
--rw-r--r--   0        0        0     6102 2024-03-29 13:44:54.354185 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/mlj/MLJModel.py
--rw-r--r--   0        0        0        1 2024-03-27 20:08:21.792950 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/mlj/__init__.py
--rw-r--r--   0        0        0     6097 2024-03-29 13:43:48.279381 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/stark/StarkModel.py
--rw-r--r--   0        0        0        1 2024-03-27 20:08:18.280494 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/stark/__init__.py
--rw-r--r--   0        0        0    13105 2024-03-27 20:22:07.171765 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/two_state/TwoStateComputation.py
--rw-r--r--   0        0        0     5815 2024-03-29 13:41:33.193088 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/two_state/TwoStateModel.py
--rw-r--r--   0        0        0        1 2024-03-27 20:08:14.154954 quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/two_state/__init__.py
--rw-r--r--   0        0        0     6202 2024-03-27 20:36:20.638436 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/Config.py
--rw-r--r--   0        0        0        0 2024-03-27 13:55:54.901315 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/__init__.py
--rw-r--r--   0        0        0     2385 2024-03-29 13:45:26.874929 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/absorption/AbsorptionModel.py
--rw-r--r--   0        0        0     1342 2024-03-27 21:37:11.892183 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/absorption/AbsorptionSpectrum.py
--rw-r--r--   0        0        0       96 2024-03-22 11:34:21.656225 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/absorption/__init__.py
--rw-r--r--   0        0        0    18942 2024-03-29 14:24:34.237423 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/hamiltonian/HamiltonianComputation.py
--rw-r--r--   0        0        0     2585 2024-03-27 20:43:15.931934 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/hamiltonian/HamiltonianModel.py
--rw-r--r--   0        0        0       47 2024-03-22 11:34:21.657692 quantumspectra_2024-0.1.3/quantumspectra_2024/modules/hamiltonian/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 14:17:26.311520 quantumspectra_2024-0.1.3/quantumspectra_2024/scripts/__init__.py
--rw-r--r--   0        0        0      816 2024-03-27 20:07:05.908030 quantumspectra_2024-0.1.3/quantumspectra_2024/scripts/qs_2024.py
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 quantumspectra_2024-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      137 2024-03-27 15:43:55.038861 quantumspectra_2024-0.1.4/README.md
+-rw-r--r--   0        0        0      887 2024-04-01 11:22:06.976482 quantumspectra_2024-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-27 09:19:33.752822 quantumspectra_2024-0.1.4/quantumspectra_2024/__init__.py
+-rw-r--r--   0        0        0     6214 2024-04-01 10:31:47.640281 quantumspectra_2024-0.1.4/quantumspectra_2024/common/Config.py
+-rw-r--r--   0        0        0        0 2024-03-27 13:55:54.901315 quantumspectra_2024-0.1.4/quantumspectra_2024/common/__init__.py
+-rw-r--r--   0        0        0     2117 2024-04-01 10:31:47.597568 quantumspectra_2024-0.1.4/quantumspectra_2024/common/absorption/AbsorptionModel.py
+-rw-r--r--   0        0        0     1342 2024-03-27 21:37:11.892183 quantumspectra_2024-0.1.4/quantumspectra_2024/common/absorption/AbsorptionSpectrum.py
+-rw-r--r--   0        0        0       96 2024-03-22 11:34:21.656225 quantumspectra_2024-0.1.4/quantumspectra_2024/common/absorption/__init__.py
+-rw-r--r--   0        0        0    18600 2024-03-31 12:12:17.088504 quantumspectra_2024-0.1.4/quantumspectra_2024/common/hamiltonian/HamiltonianComputation.py
+-rw-r--r--   0        0        0     2742 2024-04-01 10:31:47.597547 quantumspectra_2024-0.1.4/quantumspectra_2024/common/hamiltonian/HamiltonianModel.py
+-rw-r--r--   0        0        0       47 2024-03-22 11:34:21.657692 quantumspectra_2024-0.1.4/quantumspectra_2024/common/hamiltonian/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-01 08:07:57.500459 quantumspectra_2024-0.1.4/quantumspectra_2024/models/__init__.py
+-rw-r--r--   0        0        0     2556 2024-03-31 12:13:34.009122 quantumspectra_2024-0.1.4/quantumspectra_2024/models/mlj/MLJComputation.py
+-rw-r--r--   0        0        0     5838 2024-04-01 10:31:47.649201 quantumspectra_2024-0.1.4/quantumspectra_2024/models/mlj/MLJModel.py
+-rw-r--r--   0        0        0        1 2024-03-27 20:08:21.792950 quantumspectra_2024-0.1.4/quantumspectra_2024/models/mlj/__init__.py
+-rw-r--r--   0        0        0     5821 2024-04-01 10:31:47.671381 quantumspectra_2024-0.1.4/quantumspectra_2024/models/stark/StarkModel.py
+-rw-r--r--   0        0        0        1 2024-03-27 20:08:18.280494 quantumspectra_2024-0.1.4/quantumspectra_2024/models/stark/__init__.py
+-rw-r--r--   0        0        0    12924 2024-03-31 12:13:17.899406 quantumspectra_2024-0.1.4/quantumspectra_2024/models/two_state/TwoStateComputation.py
+-rw-r--r--   0        0        0     5473 2024-04-01 10:31:47.676172 quantumspectra_2024-0.1.4/quantumspectra_2024/models/two_state/TwoStateModel.py
+-rw-r--r--   0        0        0        1 2024-03-27 20:08:14.154954 quantumspectra_2024-0.1.4/quantumspectra_2024/models/two_state/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 14:17:26.311520 quantumspectra_2024-0.1.4/quantumspectra_2024/scripts/__init__.py
+-rw-r--r--   0        0        0      823 2024-04-01 10:31:47.596973 quantumspectra_2024-0.1.4/quantumspectra_2024/scripts/qs_2024.py
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 quantumspectra_2024-0.1.4/PKG-INFO
```

### Comparing `quantumspectra_2024-0.1.3/pyproject.toml` & `quantumspectra_2024-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quantumspectra-2024"
-version = "0.1.3"
+version = "0.1.4"
 description = "generates absorption spectra for donor-acceptor quantum systems"
 authors = ["benkoppe <bentastic1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
@@ -13,22 +13,28 @@
 jaxtyping = "^0.2.28"
 matplotlib = "^3.8.3"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.3"
 pytest = "^8.1.1"
+
+
+[tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 sphinx-autodoc-typehints = "^2.0.0"
 esbonio = "^0.16.4"
 docutils = "^0.20.1"
 sphinx-copybutton = "^0.5.2"
 numpydoc = "^1.6.0"
 sphinx-autoapi = "^3.0.0"
+nbsphinx = "^0.9.3"
+sphinx-autobuild = "^2024.2.4"
+
 
 [tool.poetry.scripts]
 qs_2024 = "quantumspectra_2024.scripts.qs_2024:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/mlj/MLJComputation.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/models/mlj/MLJComputation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import math
 
 import numpy as np
-from jaxtyping import Float, Int, Array, Scalar
+from jaxtyping import Float, Array
 
 
 def calculate_mlj_spectrum(
-    energy_gap: Float[Scalar, ""],
-    high_freq_frequency: Float[Scalar, ""],
-    high_freq_coupling: Float[Scalar, ""],
-    low_freq_frequency: Float[Scalar, ""],
-    low_freq_coupling: Float[Scalar, ""],
-    temperature_kelvin: Float[Scalar, ""],
-    disorder_meV: Float[Scalar, ""],
-    basis_size: Int[Scalar, ""],
+    energy_gap: float,
+    high_freq_frequency: float,
+    high_freq_coupling: float,
+    low_freq_frequency: float,
+    low_freq_coupling: float,
+    temperature_kelvin: float,
+    disorder_meV: float,
+    basis_size: int,
     sample_points: Float[Array, "num_points"],
 ) -> Float[Array, "num_points"]:
     """Computes an MLJ semiclassical absorption spectrum.
 
     Notes
     -----
     TODO:
     * Add more detailed implemention description.
 
     Parameters
     ----------
-    energy_gap : Float[Scalar, ""]
+    energy_gap : float
         energy gap between states.
-    high_freq_frequency : Float[Scalar, ""]
+    high_freq_frequency : float
         frequency of high frequency mode.
-    high_freq_coupling : Float[Scalar, ""]
+    high_freq_coupling : float
         coupling of high frequency mode.
-    low_freq_frequency : Float[Scalar, ""]
+    low_freq_frequency : float
         frequency of low frequency mode.
-    low_freq_coupling : Float[Scalar, ""]
+    low_freq_coupling : float
         coupling of low frequency mode.
-    temperature_kelvin : Float[Scalar, ""]
+    temperature_kelvin : float
         temperature in Kelvin.
-    disorder_meV : Float[Scalar, ""]
+    disorder_meV : float
         disorder (sigma) in meV.
-    basis_size : Int[Scalar, ""]
+    basis_size : int
         size of basis set.
     sample_points : Float[Array, "num_points"]
         energy points to sample spectrum.
 
     Returns
     -------
     Float[Array, "num_points"]
@@ -52,17 +52,15 @@
     disorder_wavenumbers = disorder_meV * 8061 * 0.001
     low_freq_relaxation_energy = low_freq_coupling**2 * low_freq_frequency
     temperature_kbT = temperature_kelvin * 0.695028
     high_freq_huang_rhys_factor = high_freq_coupling**2
 
     factorials = [math.factorial(n) for n in range(basis_size + 1)]
 
-    def calculate_mlj_single_intensity(
-        energy: Float[Scalar, ""],
-    ) -> Float[Scalar, ""]:
+    def calculate_mlj_single_intensity(energy: float) -> float:
         abs_arr = [
             (
                 np.exp(-high_freq_huang_rhys_factor)
                 * (high_freq_huang_rhys_factor**n)
                 / factorials[n]
             )
             * np.exp(
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/mlj/MLJModel.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/models/mlj/MLJModel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 import numpy as np
 import jax.numpy as jnp
 import jax_dataclasses as jdc
-from jaxtyping import Float, Int, Array, Scalar
+from jaxtyping import Float, Array
 
-from quantumspectra_2024.modules.absorption import (
+from quantumspectra_2024.common.absorption import (
     AbsorptionModel as Model,
     AbsorptionSpectrum,
 )
-from quantumspectra_2024.absorption.mlj.MLJComputation import calculate_mlj_spectrum
+from quantumspectra_2024.models.mlj.MLJComputation import calculate_mlj_spectrum
 
 
 @jdc.pytree_dataclass(kw_only=True)
 class MLJModel(Model):
     """A two-state two-mode MLJ model for absorption spectra.
 
     Parameters
     ----------
-    start_energy : Float[Scalar, ""]
+    start_energy : float
         absorption spectrum's starting energy (wavenumbers).
-    end_energy : Float[Scalar, ""]
+    end_energy : float
         absorption spectrum's ending energy (wavenumbers).
-    num_points : Int[Scalar, ""]
+    num_points : int
         absorption spectrum's number of points (unitless).
 
-    temperature_kelvin : Float[Scalar, ""]
+    temperature_kelvin : float
         system's temperature (Kelvin).
-    energy_gap : Float[Scalar, ""]
+    energy_gap : float
         energy gap between the two states (wavenumbers).
-    disorder_meV : Float[Scalar, ""]
+    disorder_meV : float
         disorder in the system (meV).
 
-    basis_size : Int[Scalar, ""]
+    basis_size : int
         size of basis set (unitless).
 
     mode_frequencies : Float[Array, "2"]
         frequency per mode (wavenumbers).
     mode_couplings : Float[Array, "2"]
         excited state coupling per mode.
     """
 
-    #: Float[Scalar, ""]: system's temperature (Kelvin).
-    temperature_kelvin: Float[Scalar, ""]
-    #: Float[Scalar, ""]: energy gap between the two states (wavenumbers).
-    energy_gap: Float[Scalar, ""]
-    #: Float[Scalar, ""]: disorder in the system (meV).
-    disorder_meV: Float[Scalar, ""]
+    #: system's temperature (Kelvin).
+    temperature_kelvin: float
+    #: energy gap between the two states (wavenumbers).
+    energy_gap: float
+    #: disorder in the system (meV).
+    disorder_meV: float
 
-    #: Int[Scalar, ""]: size of basis set (unitless).
-    basis_size: jdc.Static[Int[Scalar, ""]] = 20
+    #: size of basis set (unitless).
+    basis_size: int = 20
 
-    #: Float[Array, "2"]: frequency per mode (wavenumbers).
+    #: frequency per mode (wavenumbers), must have exactly two.
     mode_frequencies: Float[Array, "2"]
-    #: Float[Array, "2"]: excited state coupling per mode.
+    #: excited state coupling per mode, must have exactly two.
     mode_couplings: Float[Array, "2"]
 
     def get_absorption(self) -> AbsorptionSpectrum:
         """Compute the absorption spectrum for the model.
 
         See docs in `MLJComputation` to see how this is done.
 
@@ -119,27 +119,27 @@
         higher_frequency = sorted_frequencies[-1]
         higher_coupling = sorted_couplings[-1]
 
         return lower_frequency, lower_coupling, higher_frequency, higher_coupling
 
     def apply_electric_field(
         self,
-        field_strength: Array,
-        field_delta_dipole: Array,
-        field_delta_polarizability: Array,
+        field_strength: float,
+        field_delta_dipole: float,
+        field_delta_polarizability: float,
     ) -> "MLJModel":
         """Applies an electric field to the model. Returns a new instance of the model.
 
         Parameters
         ----------
-        field_strength : Float[Scalar, ""]
+        field_strength : float
             the strength of the electric field.
-        field_delta_dipole : Float[Scalar, ""]
+        field_delta_dipole : float
             the change in dipole moment due to the electric field.
-        field_delta_polarizability : Float[Scalar, ""]
+        field_delta_polarizability : float
             the change in polarizability due to the electric field.
 
         Returns
         -------
         MLJModel
             the model with the electric field applied.
         """
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/stark/StarkModel.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/models/stark/StarkModel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 import jax.numpy as jnp
 import jax_dataclasses as jdc
-from jaxtyping import Float, Scalar
 
-from quantumspectra_2024.modules.absorption import (
+from quantumspectra_2024.common.absorption import (
     AbsorptionModel as Model,
     AbsorptionSpectrum,
 )
 
 
 @jdc.pytree_dataclass(kw_only=True)
 class StarkModel(Model):
     """A general model for Stark absorption spectrum.
 
     Parameters
     ----------
-    start_energy : Float[Scalar, ""]
+    start_energy : float
         absorption spectrum's starting energy (wavenumbers).
-    end_energy : Float[Scalar, ""]
+    end_energy : float
         absorption spectrum's ending energy (wavenumbers).
-    num_points : Int[Scalar, ""]
+    num_points : int
         absorption spectrum's number of points (unitless).
 
     neutral_submodel : Model
         parameterized neutral submodel to use in Stark effect calculation.
 
-    positive_field_strength : Float[Scalar, ""]
+    positive_field_strength : float
         positive strength of the electric field.
-    positive_field_sum_percent : Float[Scalar, ""]
+    positive_field_sum_percent : float
         fraction of positive field strength to use in spectrum (decimal).
         negative field strength is 1 - this value.
 
-    field_delta_dipole : Float[Scalar, ""]
+    field_delta_dipole : float
         change in dipole moment due to electric field.
-    field_delta_polarizability : Float[Scalar, ""]
+    field_delta_polarizability : float
         change in polarizability due to electric field.
     """
 
-    #: Model: parameterized neutral submodel to use in Stark effect calculation.
+    #: parameterized neutral submodel to use in Stark effect calculation.
     neutral_submodel: Model
 
-    #: Float[Scalar, ""]: positive strength of the electric field.
-    positive_field_strength: Float[Scalar, ""]
-    #: Float[Scalar, ""]: fraction of positive field strength to use in spectrum (decimal).
-    positive_field_sum_percent: Float[Scalar, ""] = 0.5
-
-    #: Float[Scalar, ""]: change in dipole moment due to electric field.
-    field_delta_dipole: Float[Scalar, ""]
-    #: Float[Scalar, ""]: change in polarizability due to electric field.
-    field_delta_polarizability: Float[Scalar, ""]
+    #: positive strength of the electric field.
+    positive_field_strength: float
+    #: fraction of positive field strength to use in spectrum (decimal).
+    positive_field_sum_percent: float = 0.5
+
+    #: change in dipole moment due to electric field.
+    field_delta_dipole: float
+    #: change in polarizability due to electric field.
+    field_delta_polarizability: float
 
     def get_absorption(self) -> AbsorptionSpectrum:
         """Compute the absorption spectrum for the model.
 
         First computes absorption spectrum for the neutral submodel, and then for the charged submodels.
         Two charged submodels are computed, one with positive field strength and one with negative field strength.
 
@@ -109,24 +108,24 @@
             start_energy=self.start_energy,
             end_energy=self.end_energy,
             num_points=self.num_points,
         )
 
         return neutral_submodel
 
-    def get_charged_submodel(self, field_strength_scalar: Float[Scalar, ""]) -> Model:
+    def get_charged_submodel(self, field_strength_scalar: float) -> Model:
         """Returns a charged submodel with the Stark effect applied.
 
         This method starts with the neutral submodel from `get_neutral_submodel` and applies the Stark effect.
         The Stark effect is applied through the Model's `apply_electric_field` method.
         Field strength is multiplied by `field_strength_scalar`, and all other values are inputted into the method exactly.
 
         Parameters
         ----------
-        field_strength_scalar : Float[Scalar, ""]
+        field_strength_scalar : float
             scalar to multiply the field strength by.
 
         Returns
         -------
         Model
             the charged submodel for Stark calculations.
         """
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/two_state/TwoStateComputation.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/models/two_state/TwoStateComputation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import jax
 import jax.numpy as jnp
-from jaxtyping import Float, Int, Array, Scalar
+from jaxtyping import Float, Array
 
 
 def broaden_peaks(
     sample_points: Float[Array, "num_points"],
     peak_energies: Float[Array, "num_peaks"],
     peak_intensities: Float[Array, "num_peaks"],
-    distribution_broadening: Float[Scalar, ""],
+    distribution_broadening: float,
 ) -> Float[Array, "num_points"]:
     """Broadens a set of peaks with given sample points into an absorption spectrum.
 
     This function first computes a set of Gaussian distributions centered at each peak energy, with a specified broadening.
     Then, each spectrum is scaled by the peak intensity and summed to form the final absorption spectrum.
 
     See `compute_gaussians` for more information on the Gaussian distributions.
@@ -20,15 +20,15 @@
     ----------
     sample_points : Float[Array, "num_points"]
         Sample points at which the absorption spectrum will be computed.
     peak_energies : Float[Array, "num_peaks"]
         Peak energies corresponding to the center of each Gaussian distribution.
     peak_intensities : Float[Array, "num_peaks"]
         Peak intensities to scale each Gaussian distribution.
-    distribution_broadening : Float[Scalar, ""]
+    distribution_broadening : float
         Standard deviation of the Gaussian distributions.
 
     Returns
     -------
     Float[Array, "num_points"]
         Computed absorption spectrum.
     """
@@ -40,15 +40,15 @@
     return jnp.sum(peak_intensities * gaussians, axis=1)
 
 
 @jax.jit
 def compute_gaussians(
     sample_points: Float[Array, "num_points"],
     peak_energies: Float[Array, "num_peaks"],
-    distribution_broadening: Float[Scalar, ""],
+    distribution_broadening: float,
 ) -> Float[Array, "num_points num_peaks"]:
     """Computes the Gaussian distributions for a set of sample points and peak energies.
 
     This function calculates the value of Gaussian functions for each combination of
     sample points and peak energies, considering a specified distribution broadening.
     It is `jax` JIT-compiled to improve performance.
 
@@ -56,15 +56,15 @@
     ----------
     sample_points : Float[Array, "num_points"]
         Sample points at which the Gaussian functions will be evaluated.
         Each point represents a position on the x-axis of the Gaussian distribution.
     peak_energies : Float[Array, "num_peaks"]
         Peak energies corresponding to the mean (center) of each Gaussian distribution.
         Each peak energy defines a different Gaussian function to be evaluated at the sample points.
-    distribution_broadening : Float[Scalar, ""]
+    distribution_broadening : float
         A scalar value representing the standard deviation (sigma) of the Gaussian distributions,
         which determines the broadening of the distributions.
         This value is the same for all Gaussian distributions computed by this function.
 
     Returns
     -------
     Float[Array, "num_points num_peaks"]
@@ -76,16 +76,16 @@
         )
     )
 
 
 def compute_peaks(
     eigenvalues: Float[Array, "matrix_size"],
     eigenvectors: Float[Array, "matrix_size matrix_size"],
-    transfer_integral: Float[Scalar, ""],
-    temperature_kelvin: Float[Scalar, ""],
+    transfer_integral: float,
+    temperature_kelvin: float,
 ) -> tuple[Float[Array, "num_peaks"], Float[Array, "num_peaks"]]:
     """Computes the absorption spectrum peak energies and intensities for a two-state system.
 
     Diagonalized eigenvalues and eigenvectors are first used to compute peak energies and intensities.
     See `compute_peak_energies` and `compute_peak_intensities` for more information.
 
     Intensities are scaled by probability scalars if the temperature is not 0.
@@ -97,17 +97,17 @@
 
     Parameters
     ----------
     eigenvalues : Float[Array, "matrix_size"]
         Eigenvalues of the Hamiltonian.
     eigenvectors : Float[Array, "matrix_size matrix_size"]
         Eigenvectors of the Hamiltonian.
-    transfer_integral : Float[Scalar, ""]
+    transfer_integral : float
         Transfer integral between the two states.
-    temperature_kelvin : Float[Scalar, ""]
+    temperature_kelvin : float
         System's temperature in Kelvin.
 
     Returns
     -------
     tuple[Float[Array, "num_peaks"], Float[Array, "num_peaks"]]
         Computed absorption spectrum peak energies and intensities.
     """
@@ -178,15 +178,15 @@
 
     # only the first half is necessary
     return differences_matrix[:half_size]
 
 
 def compute_peak_intensities(
     eigenvectors: Float[Array, "matrix_size matrix_size"],
-    transfer_integral: Float[Scalar, ""],
+    transfer_integral: float,
 ) -> Float[Array, "matrix_size/2 matrix_size"]:
     """Compute all raw spectrum peak intensity values.
 
     Intensity values are the dot product of two sets of sliced eigenvectors, squared.
     This function computes all squared dot products between pairs of eigenvectors and returns a matrix of intensities.
     The matrix follows the form where index i,j represents the intensity between the ith and jth eigenvectors.
 
@@ -196,15 +196,15 @@
         * if `transfer_integral` is not 0, the top half of the eigenvectors are used
         * if `transfer_integral` is 0, the bottom half of the eigenvectors are used
 
     Parameters
     ----------
     eigenvectors : Float[Array, "matrix_size matrix_size"]
         Eigenvectors of the Hamiltonian.
-    transfer_integral : Float[Scalar, ""]
+    transfer_integral : float
         Transfer integral between the two states.
 
     Returns
     -------
     Float[Array, "matrix_size/2 matrix_size"]
         intensity matrix of eigenvectors.
     """
@@ -226,15 +226,15 @@
 
     # only the first half is necessary
     return intensities_matrix[:half_size]
 
 
 def compute_peak_probability_scalars(
     eigenvalues: Float[Array, "matrix_size"],
-    temperature_wavenumbers: Float[Scalar, ""],
+    temperature_wavenumbers: float,
 ) -> Float[Array, "matrix_size/2"]:
     """Computes a probability scalars for peak intensities.
 
     Computes a normalized exponential probability distribution based on the differences
     between the first half of the eigenvalues and the first eigenvalue, scaled by a given temperature.
 
     This function first calculates the differences between the first half of eigenvalues and the first eigenvalue.
@@ -244,15 +244,15 @@
     The probability scalars are returned as a vector of the same size as the first half of the eigenvalues.
     The probability scalars are used to scale the intensities of the peaks in the absorption spectrum.
 
     Parameters
     ----------
     eigenvalues : Float[Array, "matrix_size"]
         Eigenvalues of the Hamiltonian.
-    temperature_wavenumbers : Float[Scalar, ""]
+    temperature_wavenumbers : float
         Temperature in wavenumbers.
 
     Returns
     -------
     Float[Array, "matrix_size/2"]
         probability scalars for peak intensities.
     """
@@ -267,29 +267,29 @@
     # return normalized exponential of scaled differences
     return exponentials / jnp.sum(exponentials)
 
 
 def filter_peaks(
     peak_energies: Float[Array, "matrix_size/2 matrix_size"],
     peak_intensities: Float[Array, "matrix_size/2 matrix_size"],
-    first_eigenvector_range: Int[Scalar, ""],
+    first_eigenvector_range: int,
 ) -> tuple[Float[Array, "num_peaks"], Float[Array, "num_peaks"]]:
     """Filters peak energies and intensities by selecting unique and correct pair combinations and filtering negative values.
 
     This function uses upper-triangular matrix indices to select only peaks that have been computed with
     unique pair combinations between first eigenvectors in the given `first_eigenvector_range` and all other elevated energy levels.
     It also filters out negative energy or intensity values.
 
     Parameters
     ----------
     peak_energies : Float[Array, "matrix_size/2 matrix_size"]
         peak energies computed by `compute_peak_energies`.
     peak_intensities : Float[Array, "matrix_size/2 matrix_size"]
         peak intensities computed by `compute_peak_intensities`.
-    first_eigenvector_range : Int[Scalar, ""]
+    first_eigenvector_range : int
         the range of first eigenvectors to consider for pair combinations.
 
     Returns
     -------
     tuple[Float[Array, "num_peaks"], Float[Array, "num_peaks"]]
         filtered peak energies and intensities.
     """
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/absorption/two_state/TwoStateModel.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/models/two_state/TwoStateModel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 import jax.numpy as jnp
 import jax_dataclasses as jdc
-from jaxtyping import Float, Int, Array, Scalar
+from jaxtyping import Float, Int, Array
 
-from quantumspectra_2024.modules.absorption import (
+from quantumspectra_2024.common.absorption import (
     AbsorptionModel as Model,
     AbsorptionSpectrum,
 )
-from quantumspectra_2024.modules.hamiltonian import HamiltonianModel
-from quantumspectra_2024.absorption.two_state.TwoStateComputation import (
+from quantumspectra_2024.common.hamiltonian import HamiltonianModel
+from quantumspectra_2024.models.two_state.TwoStateComputation import (
     compute_peaks,
     broaden_peaks,
 )
 
 
 @jdc.pytree_dataclass(kw_only=True)
 class TwoStateModel(Model):
     """A two-state quantum mechanical model for absorption spectra.
 
     Parameters
     ----------
-    start_energy : Float[Scalar, ""]
+    start_energy : float
         absorption spectrum's starting energy (wavenumbers).
-    end_energy : Float[Scalar, ""]
+    end_energy : float
         absorption spectrum's ending energy (wavenumbers).
-    num_points : Int[Scalar, ""]
+    num_points : int
         absorption spectrum's number of points (unitless).
 
-    broadening : Float[Scalar, ""]
+    broadening: float
         absorption spectrum broadening factor (wavenumbers).
-    temperature_kelvin : Float[Scalar, ""]
+    temperature_kelvin : float
         system's temperature (Kelvin).
 
-    transfer_integral : Float[Scalar, ""]
+    transfer_integral : float
         transfer integral between the two states.
-    energy_gap : Float[Scalar, ""]
+    energy_gap : float
         energy gap between the two states (wavenumbers).
 
-    mode_basis_sets : Int[Array, "num_modes"]
+    mode_basis_sets : Float[Array, "num_modes"]
         basis set size per mode (unitless).
     mode_frequencies : Float[Array, "num_modes"]
         frequency per mode (wavenumbers).
     mode_couplings : Float[Array, "num_modes"]
         excited state coupling per mode.
     """
 
-    #: Float[Scalar, ""]: absorption spectrum broadening factor (wavenumbers).
-    broadening: Float[Scalar, ""]
-    #: Float[Scalar, ""]: system's temperature (Kelvin).
-    temperature_kelvin: Float[Scalar, ""]
-
-    #: Float[Scalar, ""]: transfer integral between the two states.
-    transfer_integral: Float[Scalar, ""]
-    #: Float[Scalar, ""]: energy gap between the two states (wavenumbers).
-    energy_gap: Float[Scalar, ""]
-
-    #: Float[Array, "num_modes"]: basis set size per mode (unitless).
-    mode_basis_sets: jdc.Static[Int[Array, "num_modes"]]
-    #: Float[Array, "num_modes"]: frequency per mode (wavenumbers).
+    #: absorption spectrum broadening factor (wavenumbers).
+    broadening: float = 200.0
+    #: system's temperature (Kelvin).
+    temperature_kelvin: float
+
+    #: transfer integral between the two states.
+    transfer_integral: float
+    #: energy gap between the two states (wavenumbers).
+    energy_gap: float
+
+    #: basis set size per mode (unitless).
+    mode_basis_sets: Int[Array, "num_modes"]
+    #: frequency per mode (wavenumbers).
     mode_frequencies: Float[Array, "num_modes"]
-    #: Float[Array, "num_modes"]: excited state coupling per mode.
+    #: excited state coupling per mode.
     mode_couplings: Float[Array, "num_modes"]
 
     def get_absorption(self) -> AbsorptionSpectrum:
         """Compute the absorption spectrum for the model.
 
         First computes the Hamiltonian, then diagonalizes it to get eigenvalues and eigenvectors.
         Then computes the absorption spectrum peaks and broadens them into a spectrum.
@@ -124,27 +124,27 @@
             mode_state_couplings=jnp.array(
                 [[0.0, mode_coupling] for mode_coupling in self.mode_couplings]
             ),
         )
 
     def apply_electric_field(
         self,
-        field_strength: Array,
-        field_delta_dipole: Array,
-        field_delta_polarizability: Array,
+        field_strength: float,
+        field_delta_dipole: float,
+        field_delta_polarizability: float,
     ) -> "TwoStateModel":
         """Applies an electric field to the model. Returns a new instance of the model.
 
         Parameters
         ----------
-        field_strength : Float[Scalar, ""]
+        field_strength : float
             the strength of the electric field.
-        field_delta_dipole : Float[Scalar, ""]
+        field_delta_dipole : float
             the change in dipole moment due to the electric field.
-        field_delta_polarizability : Float[Scalar, ""]
+        field_delta_polarizability : float
             the change in polarizability due to the electric field.
 
         Returns
         -------
         TwoStateModel
             the model with the electric field applied.
         """
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/modules/Config.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/common/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Type, Callable
 from pathlib import Path
 from argparse import ArgumentParser
 import tomllib
 
-from quantumspectra_2024.modules.absorption import AbsorptionModel, AbsorptionSpectrum
+from quantumspectra_2024.common.absorption import (
+    AbsorptionModel,
+    AbsorptionSpectrum,
+)
 
 CONFIG_ARG_NAME = "config_path"
 CONFIG_ARG_HELP = "Path to the configuration file."
 
 OUT_CONFIG_NAME = "out"
 OUT_REQUIRED_KEYS = ["filename", "data", "plot", "overwrite"]
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/modules/absorption/AbsorptionModel.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/common/absorption/AbsorptionModel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import jax_dataclasses as jdc
-from jaxtyping import Float, Int, Scalar
 
 from abc import ABC, abstractmethod
 
-from quantumspectra_2024.modules.absorption.AbsorptionSpectrum import AbsorptionSpectrum
+from quantumspectra_2024.common.absorption.AbsorptionSpectrum import (
+    AbsorptionSpectrum,
+)
 
 
 @jdc.pytree_dataclass(kw_only=True)
 class AbsorptionModel(ABC):
     """Represents a model for generating absorption spectra.
 
     All models include a `get_absorption` method that returns an `AbsorptionSpectrum` object.
     An `apply_electric_field` method is also included to apply an electric field to base models for Stark effect.
 
     Parameters
     ----------
-    start_energy : Float[Scalar, ""]
+    start_energy : float
         absorption spectrum's starting energy (wavenumbers).
-    end_energy : Float[Scalar, ""]
+    end_energy : float
         absorption spectrum's ending energy (wavenumbers).
-    num_points : Int[Scalar, ""]
+    num_points : int
         absorption spectrum's number of points (unitless).
     """
 
-    #: Float[Scalar, ""]: absorption spectrum's starting energy (wavenumbers).
-    start_energy: jdc.Static[Float[Scalar, ""]] = 0.0
-    #: Float[Scalar, ""]: absorption spectrum's ending energy (wavenumbers).
-    end_energy: jdc.Static[Float[Scalar, ""]] = 20_000.0
-    #: Int[Scalar, ""]: absorption spectrum's number of points (unitless).
-    num_points: jdc.Static[Int[Scalar, ""]] = 2_001
+    #: absorption spectrum's starting energy (wavenumbers).
+    start_energy: float = 0.0
+    #: absorption spectrum's ending energy (wavenumbers).
+    end_energy: float = 20_000.0
+    #: absorption spectrum's number of points (unitless).
+    num_points: int = 2_001
 
     @abstractmethod
     def get_absorption(self) -> AbsorptionSpectrum:
         """Compute the absorption spectrum for the model.
 
         Returns
         -------
         AbsorptionSpectrum
             the model's parameterized absorption spectrum.
         """
         raise NotImplementedError
 
     @abstractmethod
     def apply_electric_field(
-        field_strength: Float[Scalar, ""],
-        field_delta_dipole: Float[Scalar, ""],
-        field_delta_polarizability: Float[Scalar, ""],
+        field_strength: float,
+        field_delta_dipole: float,
+        field_delta_polarizability: float,
     ) -> "AbsorptionModel":
         """Applies an electric field to the model. Returns a new instance of the model.
 
         Parameters
         ----------
-        field_strength : Float[Scalar, ""]
+        field_strength : float
             the strength of the electric field.
-        field_delta_dipole : Float[Scalar, ""]
+        field_delta_dipole : float
             the change in dipole moment due to the electric field.
-        field_delta_polarizability : Float[Scalar, ""]
+        field_delta_polarizability : float
             the change in polarizability due to the electric field.
 
         Returns
         -------
         AbsorptionModel
             the model with the electric field applied.
         """
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/modules/absorption/AbsorptionSpectrum.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/common/absorption/AbsorptionSpectrum.py`

 * *Files identical despite different names*

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/modules/hamiltonian/HamiltonianComputation.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/common/hamiltonian/HamiltonianComputation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import jax
 import jax.numpy as jnp
-from jaxtyping import Float, Int, Bool, Array, Scalar
+from jaxtyping import Float, Int, Bool, Array
 
 
 def diagonalize_matrix(matrix: Float[Array, "matrix_size matrix_size"]) -> tuple[
     Float[Array, "matrix_size"],
     Float[Array, "matrix_size matrix_size"],
 ]:
     """Diagonalizes a matrix and returns the eigenvalues and eigenvectors in a tuple.
@@ -21,15 +21,15 @@
     """
     eigenvalues, eigenvectors = jnp.linalg.eigh(matrix)
     return eigenvalues, eigenvectors
 
 
 def build_matrix(
     state_energies: Float[Array, "num_states"],
-    transfer_integral: Float[Scalar, ""],
+    transfer_integral: float,
     mode_basis_sets: Int[Array, "num_modes"],
     mode_localities: Bool[Array, "num_modes"],
     mode_frequencies: Float[Array, "num_modes"],
     mode_state_couplings: Float[Array, "num_modes num_states"],
 ) -> Float[Array, "matrix_size matrix_size"]:
     """Builds a full Hamiltonian matrix for a system of states and modes.
 
@@ -42,15 +42,15 @@
     TODO:
     * Implement multiple transfer integrals for more than two states.
 
     Parameters
     ----------
     state_energies : Float[Array, "num_states"]
         energies of all local states.
-    transfer_integral : Float[Scalar, ""]
+    transfer_integral : float
         transfer integral between states.
     mode_basis_sets : Int[Array, "num_modes"]
         basis set size per mode.
     mode_localities : Bool[Array, "num_modes"]
         locality of each mode.
     mode_frequencies : Float[Array, "num_modes"]
         frequency per mode.
@@ -95,15 +95,15 @@
         rows.append(jnp.hstack(cols))
     matrix = jnp.vstack(rows)
 
     return matrix
 
 
 def build_local_state_block(
-    state_index: Int[Scalar, ""],
+    state_index: int,
     state_energies: Float[Array, "num_states"],
     mode_basis_sets: Int[Array, "num_modes"],
     mode_localities: Bool[Array, "num_modes"],
     mode_frequencies: Float[Array, "num_modes"],
     mode_state_couplings: Float[Array, "num_modes num_states"],
 ) -> Float[Array, "block_size block_size"]:
     """Builds a local state block.
@@ -112,15 +112,15 @@
     To build a local state block, the following steps are taken.
     * Calculate the state's diagonal values with `calculate_state_local_diagonals`.
     * Calculate the state's offdiagonal values with `calculate_state_offdiagonals`.
     * Build the state block.
 
     Parameters
     ----------
-    state_index : Int[Scalar, ""]
+    state_index : int
         index of the state.
     state_energies : Float[Array, "num_states"]
         energies of all local states.
     mode_basis_sets : Int[Array, "num_modes"]
         basis set size per mode.
     mode_localities : Bool[Array, "num_modes"]
         locality of each mode.
@@ -159,16 +159,16 @@
         all_diagonal_values=all_diagonal_values,
         all_mode_offdiagonal_values=all_mode_offdiagonal_values,
         mode_basis_sets=mode_basis_sets,
     )
 
 
 def build_nonlocal_state_block(
-    state_index: Int[Scalar, ""],
-    transfer_integral: Float[Scalar, ""],
+    state_index: int,
+    transfer_integral: float,
     mode_basis_sets: Int[Array, "num_modes"],
     mode_localities: Bool[Array, "num_modes"],
     mode_frequencies: Float[Array, "num_modes"],
     mode_state_couplings: Float[Array, "num_modes num_states"],
 ):
     """Builds a nonlocal state block.
 
@@ -176,17 +176,17 @@
     To build a nonlocal state block, the following steps are taken.
     * The state's offdiagonal values are all set to the transfer integral.
     * Calculate the state's diagonal values with `calculate_state_local_diagonals`.
     * Build the state block.
 
     Parameters
     ----------
-    state_index : Int[Scalar, ""]
+    state_index : int
         index of the state.
-    transfer_integral : Float[Scalar, ""]
+    transfer_integral : float
         transfer integral between states.
     mode_basis_sets : Int[Array, "num_modes"]
         basis set size per mode.
     mode_localities : Bool[Array, "num_modes"]
         locality of each mode.
     mode_frequencies : Float[Array, "num_modes"]
         frequency per mode.
@@ -293,28 +293,28 @@
 
     # finally, fills the main diagonal of the full block
     block = block + jnp.diag(all_diagonal_values)
     return block
 
 
 def calculate_state_local_diagonals(
-    state_energy: Float[Scalar, ""],
+    state_energy: float,
     mode_frequencies: Float[Array, "num_modes"],
     mode_couplings: Float[Array, "num_modes"],
     mode_basis_sets: Int[Array, "num_modes"],
 ) -> Float[Array, "block_size"]:
     """Calculate all diagonal values for a state block in a single array. Only calculated for local blocks.
 
     Diagonal values are calculated with a sum of contributions from each mode, plus the state energy.
     Contributions for each mode are summed with all combinations of values between 1 and their basis set size - 1.
     To see how individual mode contributions are calculated, see `calculate_mode_local_diagonal_component`.
 
     Parameters
     ----------
-    state_energy : Float[Scalar, ""]
+    state_energy : float
         energy of the state.
     mode_frequencies : Float[Array, "num_modes"]
         frequencies of each mode.
     mode_couplings : Float[Array, "num_modes"]
         couplings of each mode.
     mode_basis_sets : Int[Array, "num_modes"]
         basis set size of each mode.
@@ -343,30 +343,30 @@
 
     all_diagonal_values = state_energy + sum_contribution_combinations
 
     return all_diagonal_values
 
 
 def calculate_state_offdiagonals(
-    state_locality: Bool[Scalar, ""],
+    state_locality: bool,
     mode_basis_sets: Int[Array, "num_modes"],
     mode_localities: Bool[Array, "num_modes"],
     mode_frequencies: Float[Array, "num_modes"],
     mode_couplings: Float[Array, "num_modes"],
 ) -> tuple[Float[Array, "_mode_offdiagonal_size"]]:
     """Calculate all unqiue offdiagonal values for a state block per mode. Each mode's set of offdiagonals is contained in a tuple.
 
     Offdiagonal values are an array of calculated values that range from 1 to the basis set size of the mode - 1.
     Thus, each array in the tuple will have a length of `mode_basis_set`.
     If the mode doesn't match the locality of the state, the offdiagonals are all set to zero.
     To see how individual mode offdiagonal values are calculated, see `calculate_mode_offdiagonal_component`.
 
     Parameters
     ----------
-    state_locality : Bool[Scalar, ""]
+    state_locality : bool
         the locality of the state.
     mode_basis_sets : Int[Array, "num_modes"]
         basis set size of each mode.
     mode_localities : Bool[Array, "num_modes"]
         locality of each mode.
     mode_frequencies : Float[Array, "num_modes"]
         frequencies of each mode.
@@ -396,64 +396,64 @@
         )
     )
 
     return all_mode_offdiagonal_values
 
 
 def calculate_mode_local_diagonal_component(
-    component_index: Int[Scalar, ""],
-    mode_frequency: Float[Scalar, ""],
-    mode_coupling: Float[Scalar, ""],
-) -> Float[Scalar, ""]:
+    component_index: int,
+    mode_frequency: float,
+    mode_coupling: float,
+) -> float:
     """Computes a single diagonal contribution component for a mode.
 
     Diagonal contributions are calculated as follows:
         * The mode frequency is multiplied by the component index plus one half
         * This value is then multiplied by the square of the mode coupling, divided by two.
 
     Parameters
     ----------
-    component_index : Int[Scalar, ""]
+    component_index : int
         the index of the component.
-    mode_frequency : Float[Scalar, ""]
+    mode_frequency : float
         the frequency of the mode.
-    mode_coupling : Float[Scalar, ""]
+    mode_coupling : float
         the coupling of the mode.
 
     Returns
     -------
-    Float[Scalar, ""]
+    float
         the computed diagonal contribution component.
     """
     return mode_frequency * ((component_index + (1 / 2)) + (mode_coupling**2) / 2)
 
 
 def calculate_mode_offdiagonal_component(
-    component_index: Int[Scalar, ""],
-    mode_frequency: Float[Array, ""],
-    mode_coupling: Float[Array, ""],
-) -> Float[Scalar, ""]:
+    component_index: int,
+    mode_frequency: float,
+    mode_coupling: float,
+) -> float:
     """Computes a single offdiagonal contribution component for a mode.
 
     Offdiagonal contributions are calculated as follows:
         * The mode frequency is multiplied by the square root of the component index plus one, divided by two.
         * This value is then multiplied by the mode coupling.
 
     Parameters
     ----------
-    component_index : Int[Scalar, ""]
+    component_index : int
         the index of the component.
-    mode_frequency : Float[Scalar, ""]
+    mode_frequency : float
         the frequency of the mode.
-    mode_coupling : Float[Scalar, ""]
+    mode_coupling : float
         the coupling of the mode.
 
     Returns
     -------
-    Float[Scalar, ""]
+    float
         the computed offdiagonal contribution component.
     """
     return mode_frequency * mode_coupling * jnp.sqrt((component_index + 1) / 2)
 
 
 def outer_sum(*arrays: tuple[Float[Array, "*"]]) -> Float[Array, "*"]:
     """
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/modules/hamiltonian/HamiltonianModel.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/common/hamiltonian/HamiltonianModel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 import jax_dataclasses as jdc
-from jaxtyping import Float, Int, Bool, Scalar, Array
+from jaxtyping import Float, Int, Bool, Array
 
-from quantumspectra_2024.modules.hamiltonian.HamiltonianComputation import (
+from quantumspectra_2024.common.hamiltonian.HamiltonianComputation import (
     build_matrix,
     diagonalize_matrix,
 )
 
 
 @jdc.pytree_dataclass(kw_only=True)
 class HamiltonianModel:
     """A hamiltonian model for a quantum system.
 
     Attributes
     ----------
-    transfer_integral : Float[Scalar, ""]
+    transfer_integral : float
         transfer integral between states.
     state_energies : Float[Array, "num_states"]
         energies of each state.
 
     mode_basis_sets : Int[Array, "num_modes"]
         basis set size per mode.
     mode_localities : Bool[Array, "num_modes"]
         whether each mode is local.
     mode_frequencies : Float[Array, "num_modes"]
         frequency per mode.
     mode_state_couplings : Float[Array, "num_modes num_states"]
         coupling per mode and state.
     """
 
-    transfer_integral: Float[Scalar, ""]
+    #: transfer integral between states.
+    transfer_integral: float
+    #: energies of each state.
     state_energies: Float[Array, "num_states"]
 
-    mode_basis_sets: jdc.Static[Int[Array, "num_modes"]]
+    #: basis set size per mode.
+    mode_basis_sets: Int[Array, "num_modes"]
+    #: whether each mode is local.
     mode_localities: Bool[Array, "num_modes"]
+    #: frequency per mode.
     mode_frequencies: Float[Array, "num_modes"]
+    #: coupling per mode and state.
     mode_state_couplings: Float[Array, "num_modes num_states"]
 
     def get_diagonalization(self) -> tuple[
         Float[Array, "matrix_size"],
         Float[Array, "matrix_size matrix_size"],
     ]:
         """Compute the diagonalization of the Hamiltonian.
```

### Comparing `quantumspectra_2024-0.1.3/quantumspectra_2024/scripts/qs_2024.py` & `quantumspectra_2024-0.1.4/quantumspectra_2024/scripts/qs_2024.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from quantumspectra_2024.modules.Config import (
+from quantumspectra_2024.common.Config import (
     parse_config,
     initialize_absorption_from_config,
     save_spectrum_from_config,
 )
-from quantumspectra_2024.modules.absorption import AbsorptionModel, AbsorptionSpectrum
+from quantumspectra_2024.common.absorption import (
+    AbsorptionModel,
+    AbsorptionSpectrum,
+)
 
-from quantumspectra_2024.absorption import TwoStateModel, MLJModel, StarkModel
+from quantumspectra_2024.models import TwoStateModel, MLJModel, StarkModel
 
 
 def main():
     config: dict = parse_config("Compute absorption spectrum with a given config file.")
 
     str_to_model: dict = {
         "two_state": TwoStateModel,
```

### Comparing `quantumspectra_2024-0.1.3/PKG-INFO` & `quantumspectra_2024-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumspectra-2024
-Version: 0.1.3
+Version: 0.1.4
 Summary: generates absorption spectra for donor-acceptor quantum systems
 Author: benkoppe
 Author-email: bentastic1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

