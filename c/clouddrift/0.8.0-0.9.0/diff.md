# Comparing `tmp/clouddrift-0.8.0.tar.gz` & `tmp/clouddrift-0.9.0.tar.gz`

## Comparing `clouddrift-0.8.0.tar` & `clouddrift-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 clouddrift-0.8.0/.codecov.yml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 clouddrift-0.8.0/environment.yml
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 clouddrift-0.8.0/.github/workflows/black.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 clouddrift-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 clouddrift-0.8.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 clouddrift-0.8.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/_version.py
--rw-r--r--   0        0        0    13978 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/analysis.py
--rw-r--r--   0        0        0    15218 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/dataformat.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/haversine.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/select.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/sphere.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/adapters/__init__.py
--rw-r--r--   0        0        0    24510 2020-02-02 00:00:00.000000 clouddrift-0.8.0/clouddrift/adapters/gdp.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/Makefile
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/api.rst
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/conf.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/contributing.rst
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/favicon.ico
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/index.rst
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/install.rst
--rw-r--r--   0        0        0   605248 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/logo.png
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/make.bat
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/paper.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/requirements.txt
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 clouddrift-0.8.0/docs/usage.rst
--rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 clouddrift-0.8.0/tests/analysis_tests.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 clouddrift-0.8.0/tests/dataformat_tests.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 clouddrift-0.8.0/tests/haversine_tests.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 clouddrift-0.8.0/tests/select_tests.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 clouddrift-0.8.0/tests/sphere_tests.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 clouddrift-0.8.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 clouddrift-0.8.0/LICENSE
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 clouddrift-0.8.0/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 clouddrift-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 clouddrift-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 clouddrift-0.9.0/.codecov.yml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 clouddrift-0.9.0/environment.yml
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 clouddrift-0.9.0/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 clouddrift-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 clouddrift-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 clouddrift-0.9.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/_version.py
+-rw-r--r--   0        0        0    14817 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/analysis.py
+-rw-r--r--   0        0        0    16508 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/dataformat.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/haversine.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/select.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/sphere.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/adapters/__init__.py
+-rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 clouddrift-0.9.0/clouddrift/adapters/gdp.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/api.rst
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/contributing.rst
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/favicon.ico
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/install.rst
+-rw-r--r--   0        0        0   605248 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/logo.png
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/paper.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 clouddrift-0.9.0/docs/usage.rst
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 clouddrift-0.9.0/tests/analysis_tests.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 clouddrift-0.9.0/tests/dataformat_tests.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 clouddrift-0.9.0/tests/haversine_tests.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 clouddrift-0.9.0/tests/select_tests.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 clouddrift-0.9.0/tests/sphere_tests.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 clouddrift-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 clouddrift-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 clouddrift-0.9.0/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 clouddrift-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 clouddrift-0.9.0/PKG-INFO
```

### Comparing `clouddrift-0.8.0/.github/workflows/ci.yml` & `clouddrift-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/.github/workflows/docs.yml` & `clouddrift-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/.github/workflows/pypi.yml` & `clouddrift-0.9.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/clouddrift/analysis.py` & `clouddrift-0.9.0/clouddrift/analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 from typing import Optional, Tuple, Union
 import xarray as xr
+import pandas as pd
 from concurrent import futures
+from datetime import timedelta
 from clouddrift.haversine import distance, bearing
 from clouddrift.dataformat import unpack_ragged
 
 
 def apply_ragged(
     func: callable,
     arrays: list[np.ndarray],
@@ -87,23 +89,25 @@
             outputs.append(np.concatenate([r[i] for r in res]))
         return tuple(outputs)
     else:
         return np.concatenate(res)
 
 
 def segment(
-    x: np.ndarray, tolerance: float, rowsize: np.ndarray[int] = None
+    x: np.ndarray,
+    tolerance: Union[float, np.timedelta64, timedelta, pd.Timedelta],
+    rowsize: np.ndarray[int] = None,
 ) -> np.ndarray[int]:
     """Segment an array into contiguous segments.
 
     Parameters
     ----------
     x : list, np.ndarray, or xr.DataArray
         An array to segment.
-    tolerance : float
+    tolerance : float, np.timedelta64, timedelta, pd.Timedelta
         The maximum signed difference between consecutive points in a segment.
     rowsize : np.ndarray[int], optional
         The size of rows if x is a ragged array. If present, x will be
         segmented both by gaps that exceed the tolerance, and by rows
         of the ragged array.
 
     Returns
@@ -117,14 +121,23 @@
     The simplest use of ``segment`` is to provide a tolerance value that is
     used to segment an array into contiguous segments.
 
     >>> x = [0, 1, 1, 1, 2, 2, 3, 3, 3, 3, 4]
     >>> segment(x, 0.5)
     array([1, 3, 2, 4, 1])
 
+    If the array represents time and the tolerance is a timedelta,
+    the same logic applies.
+
+    >>> x = np.array([np.datetime64("2023-01-01"), np.datetime64("2023-01-02"),
+                      np.datetime64("2023-01-03"), np.datetime64("2023-02-01"),
+                      np.datetime64("2023-02-02")])
+    >>> segment(x, np.timedelta64(1, "D"))
+    np.array([3, 2])
+
     If the array is already previously segmented (e.g. multiple trajectories
     as a ragged array), then the ``rowsize`` argument can be used to preserve
     the input segments.
 
     >>> rowsize = [3, 2, 6]
     >>> segment(x, 0.5, rowsize)
     array([1, 2, 1, 1, 1, 4, 1])
@@ -143,16 +156,25 @@
     to the first ``segment`` invocation.
 
     >>> x = [1, 1, 2, 2, 1, 1, 2, 2]
     >>> segment(x, 0.5, rowsize=segment(x, -0.5))
     array([2, 2, 2, 2])
     """
 
+    # for compatibility with datetime list or np.timedelta64 arrays
+    if type(tolerance) in [np.timedelta64, timedelta]:
+        tolerance = pd.Timedelta(tolerance)
+
+    if type(tolerance) == pd.Timedelta:
+        positive_tol = tolerance >= pd.Timedelta("0 seconds")
+    else:
+        positive_tol = tolerance >= 0
+
     if rowsize is None:
-        if tolerance >= 0:
+        if positive_tol:
             exceeds_tolerance = np.diff(x) > tolerance
         else:
             exceeds_tolerance = np.diff(x) < tolerance
         segment_sizes = np.diff(np.insert(np.where(exceeds_tolerance)[0] + 1, 0, 0))
         segment_sizes = np.append(segment_sizes, len(x) - np.sum(segment_sizes))
         return segment_sizes
     else:
```

### Comparing `clouddrift-0.8.0/clouddrift/dataformat.py` & `clouddrift-0.9.0/clouddrift/dataformat.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,38 +64,53 @@
         cls,
         indices: list,
         preprocess_func: Callable[[int], xr.Dataset],
         name_coords: list,
         name_meta: Optional[list] = [],
         name_data: Optional[list] = [],
         rowsize_func: Optional[Callable[[int], int]] = None,
+        filename_pattern: Optional[str] = "drifter_{id}.nc",
     ):
         """Generate ragged arrays archive from a list of trajectory files
 
         Args:
             indices (list): identification numbers list to iterate
             preprocess_func (Callable[[int], xr.Dataset]): returns a processed xarray Dataset from an identification number
             name_coords (list): Name of the coordinate variables to include in the archive
             name_meta (list, optional): Name of metadata variables to include in the archive (Defaults to [])
             name_data (list, optional): Name of the data variables to include in the archive (Defaults to [])
             rowsize_func (Optional[Callable[[int], int]], optional): returns the number of observations from an identification number (to speed up processing) (Defaults to None)
+            filename_pattern (Optional[str]): filename pattern as function of id, e.g. 'drifter_{id}.nc' (default), to use as the second argument to preprocess_func and rowsize_func
 
         Returns:
             obj: ragged array class object
         """
         # if no method is supplied, get the dimension from the preprocessing function
         rowsize_func = (
-            rowsize_func if rowsize_func else lambda i: preprocess_func(i).dims["obs"]
+            rowsize_func
+            if rowsize_func
+            else lambda i, filename_pattern: preprocess_func(i, filename_pattern).dims[
+                "obs"
+            ]
         )
-        rowsize = cls.number_of_observations(rowsize_func, indices)
+        rowsize = cls.number_of_observations(rowsize_func, indices, filename_pattern)
         coords, metadata, data = cls.allocate(
-            preprocess_func, indices, rowsize, name_coords, name_meta, name_data
+            preprocess_func,
+            indices,
+            filename_pattern,
+            rowsize,
+            name_coords,
+            name_meta,
+            name_data,
         )
         attrs_global, attrs_variables = cls.attributes(
-            preprocess_func(indices[0]), name_coords, name_meta, name_data
+            preprocess_func(indices[0], filename_pattern),
+            name_coords,
+            name_meta,
+            name_data,
         )
 
         return cls(coords, metadata, data, attrs_global, attrs_variables)
 
     @classmethod
     def from_netcdf(cls, filename: str):
         """Read a ragged arrays archive from a NetCDF file.
@@ -164,34 +179,35 @@
                 )
             attrs_variables[var] = ds[var].attrs
 
         return cls(coords, metadata, data, attrs_global, attrs_variables)
 
     @staticmethod
     def number_of_observations(
-        rowsize_func: Callable[[int], int], indices: list
+        rowsize_func: Callable[[int], int], indices: list, filename_pattern: str
     ) -> np.array:
         """Iterate through the files and evaluate the number of observations.
 
         Args:
             rowsize_func (Callable[[int], int]): returns number observations of a trajectory from its identification number
             indices (list): identification numbers list to iterate
+            filename_pattern (str): filename pattern as function of id, e.g. 'drifter_{id}.nc'
 
         Returns:
             np.array: number of observations of each trajectory
         """
         rowsize = np.zeros(len(indices), dtype="int")
 
         for i, index in tqdm(
             enumerate(indices),
             total=len(indices),
             desc="Retrieving the number of obs",
             ncols=80,
         ):
-            rowsize[i] = rowsize_func(index)
+            rowsize[i] = rowsize_func(index, filename_pattern)
         return rowsize
 
     @staticmethod
     def attributes(
         ds: xr.Dataset, name_coords: list, name_meta: list, name_data: list
     ) -> Tuple[dict, dict]:
         """Returns the global attributes and the attributes of all variables (name_coords, name_meta, and name_data) from a xr.Dataset
@@ -206,43 +222,48 @@
             Tuple[dict, dict]: the global and variables attributes
         """
         attrs_global = ds.attrs
 
         # coordinates, metadata, and data
         attrs_variables = {}
         for var in name_coords + name_meta + name_data:
-            attrs_variables[var] = ds[var].attrs
+            if var in ds.keys():
+                attrs_variables[var] = ds[var].attrs
+            else:
+                warnings.warn(f"Variable {var} requested but not found; skipping.")
 
         return attrs_global, attrs_variables
 
     @staticmethod
     def allocate(
         preprocess_func: Callable[[int], xr.Dataset],
         indices: list,
+        filename_pattern: str,
         rowsize: list,
         name_coords: list,
         name_meta: list,
         name_data: list,
     ) -> Tuple[dict, dict, dict]:
         """Iterate through the files and fill for the ragged array associated with coordinates, and selected metadata and data variables.
 
         Args:
             preprocess_func (Callable[[int], xr.Dataset]): returns a processed xarray Dataset from an identification number
             indices (list): list of indices separating trajectory in the ragged arrays
+            filename_pattern (str): filename pattern as function of id, e.g. 'drifter_{id}.nc'
             rowsize (list): list of the number of observations per trajectory
             name_coords (list): Name of the coordinate variables to include in the archive
             name_meta (list, optional): Name of metadata variables to include in the archive (Defaults to [])
             name_data (list, optional): Name of the data variables to include in the archive (Defaults to [])
 
         Returns:
             Tuple[dict, dict, dict]: dictionaries containing numerical data and attributes of coordinates, metadata and data variables.
         """
 
         # open one file to get dtype of variables
-        ds = preprocess_func(indices[0])
+        ds = preprocess_func(indices[0], filename_pattern)
         nb_traj = len(rowsize)
         nb_obs = np.sum(rowsize).astype("int")
         index_traj = np.insert(np.cumsum(rowsize), 0, 0)
 
         # allocate memory
         coords = {}
         for var in name_coords:
@@ -250,36 +271,44 @@
 
         metadata = {}
         for var in name_meta:
             metadata[var] = np.zeros(nb_traj, dtype=ds[var].dtype)
 
         data = {}
         for var in name_data:
-            data[var] = np.zeros(nb_obs, dtype=ds[var].dtype)
+            if var in ds.keys():
+                data[var] = np.zeros(nb_obs, dtype=ds[var].dtype)
+            else:
+                warnings.warn(f"Variable {var} requested but not found; skipping.")
         ds.close()
 
         # loop and fill the ragged array
         for i, index in tqdm(
             enumerate(indices),
             total=len(indices),
             desc="Filling the Ragged Array",
             ncols=80,
         ):
-            with preprocess_func(index) as ds:
+            with preprocess_func(index, filename_pattern) as ds:
                 size = rowsize[i]
                 oid = index_traj[i]
 
                 for var in name_coords:
                     coords[var][oid : oid + size] = ds[var].data
 
                 for var in name_meta:
                     metadata[var][i] = ds[var][0].data
 
                 for var in name_data:
-                    data[var][oid : oid + size] = ds[var].data
+                    if var in ds.keys():
+                        data[var][oid : oid + size] = ds[var].data
+                    else:
+                        warnings.warn(
+                            f"Variable {var} requested but not found; skipping."
+                        )
 
         return coords, metadata, data
 
     def validate_attributes(self):
         """Validate that each variable has an assigned attribute tag."""
         for key in (
             list(self.coords.keys())
```

### Comparing `clouddrift-0.8.0/clouddrift/haversine.py` & `clouddrift-0.9.0/clouddrift/haversine.py`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/clouddrift/select.py` & `clouddrift-0.9.0/clouddrift/select.py`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/clouddrift/sphere.py` & `clouddrift-0.9.0/clouddrift/sphere.py`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/clouddrift/adapters/gdp.py` & `clouddrift-0.9.0/clouddrift/adapters/gdp.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from tqdm import tqdm
 from typing import Optional
 import os
 import warnings
 
 GDP_VERSION = "2.00"
 GDP_DATA_URL = "https://www.aoml.noaa.gov/ftp/pub/phod/lumpkin/hourly/v2.00/netcdf/"
-GDP_FILENAME_PATTERN = "drifter_{id}.nc"
+GDP_DATA_URL_EXPERIMENTAL = (
+    "https://www.aoml.noaa.gov/ftp/pub/phod/lumpkin/hourly/experimental/"
+)
 GDP_TMP_PATH = os.path.join(tempfile.gettempdir(), "clouddrift", "gdp")
 
 GDP_COORDS = [
     "ids",
     "time",
 ]
 GDP_METADATA = [
@@ -86,25 +88,26 @@
     "flg_sst1",
     "flg_sst2",
     "drogue_status",
 ]
 
 
 def parse_directory_file(filename: str) -> pd.DataFrame:
-    """Read a directory file which contains metadata of drifters' releases.
+    """Read a GDP directory file that contains metadata of drifter releases.
 
-    Due to naming of these files, a manual update of the last file name after an
-    update of the dataset is needed.
-
-    Args:
-        filename (str): Name of the directory file
-    Returns:
-        pd.DataFrame: Sorted list of drifters
+    Parameters
+    ----------
+    filename : str
+        Name of the directory file to parse.
+
+    Returns
+    -------
+    df : pd.DataFrame
+        List of drifters from a single directory file as a pandas DataFrame.
     """
-
     GDP_DIRECTORY_FILE_URL = "https://www.aoml.noaa.gov/ftp/pub/phod/buoydata/"
     df = pd.read_csv(
         os.path.join(GDP_DIRECTORY_FILE_URL, filename), delimiter="\s+", header=None
     )
 
     # Combine the date and time columns to easily parse dates below.
     df[4] += " " + df[5]
@@ -128,62 +131,107 @@
     for t in ["Deployment_date", "End_date", "Drogue_off_date"]:
         df[t] = pd.to_datetime(df[t], format="%Y/%m/%d %H:%M", errors="coerce")
 
     return df
 
 
 def get_gdp_metadata() -> pd.DataFrame:
-    """Download and parse GDP metadata and return it as a Pandas DataFrame."""
+    """Download and parse GDP metadata and return it as a Pandas DataFrame.
 
-    directory_file_names = [
-        "dirfl_1_5000.dat",
-        "dirfl_5001_10000.dat",
-        "dirfl_10001_15000.dat",
-        "dirfl_15001_jul22.dat",
-    ]
-    df = pd.concat([parse_directory_file(f) for f in directory_file_names])
+    Returns
+    -------
+    df : pd.DataFrame
+        Sorted list of drifters as a pandas DataFrame.
+    """
+    directory_file_pattern = "dirfl_{low}_{high}.dat"
+
+    dfs = []
+    start = 1
+    while True:
+        name = directory_file_pattern.format(low=start, high=start + 4999)
+        try:
+            dfs.append(parse_directory_file(name))
+            start += 5000
+        except:
+            break
+
+    name = directory_file_pattern.format(low=start, high="current")
+    dfs.append(parse_directory_file(name))
+
+    df = pd.concat(dfs)
     df.sort_values(["Deployment_date"], inplace=True, ignore_index=True)
     return df
 
 
 def order_by_date(df: pd.DataFrame, idx: list[int]) -> np.ndarray[int]:
     """From the previously sorted directory files DataFrame, return the drifter
-    indices sorted by their end date.
+    indices sorted by their deployment date.
 
-    Args:
-        idx [list]: List of drifters to include in the ragged array
-    Returns:
-        idx [list]: Sorted list of drifters
+    Parameters
+    ----------
+    idx : list
+        List of drifters to include in the ragged array
+
+    Returns
+    -------
+    idx : list
+        List of drifters sorted by their end date.
     """
     return df.ID[np.where(np.in1d(df.ID, idx))[0]].values
 
 
 def fetch_netcdf(url: str, file: str):
-    """Download and save the file from the given url, if not already downloaded."""
+    """Download and save the file from the given url, if not already downloaded.
+
+    Parameters
+    ----------
+    url : str
+        URL from which to download the file.
+    file : str
+        Name of the file to save.
+    """
     if not os.path.isfile(file):
-        req = urllib.request.urlretrieve(url, file)
+        urllib.request.urlretrieve(url, file)
 
 
-def download(drifter_ids: list = None, n_random_id: int = None):
+def download(
+    drifter_ids: list = None, n_random_id: int = None, url: str = GDP_DATA_URL
+):
     """Download individual NetCDF files from the AOML server.
 
-    :param drifter_ids [list]: list of drifter to retrieve (Default: all)
-    :param n_random_id [int]: randomly select n drifter NetCDF files
-    :return drifters_ids [list]: list of retrived drifter
+    Parameters
+    ----------
+    drifter_ids : list
+        List of drifter to retrieve (Default: all)
+    n_random_id : int
+        Randomly select n_random_id drifter IDs to download (Default: None)
+    url : str
+        URL from which to download the data (Default: GDP_DATA_URL). Alternatively, it can be GDP_DATA_URL_EXPERIMENTAL.
+
+    Returns
+    -------
+    out : list
+        List of retrived drifters
     """
 
     # Create a temporary directory if doesn't already exists.
     os.makedirs(GDP_TMP_PATH, exist_ok=True)
 
+    if url == GDP_DATA_URL:
+        pattern = "drifter_[0-9]*.nc"
+        filename_pattern = "drifter_{id}.nc"
+    elif url == GDP_DATA_URL_EXPERIMENTAL:
+        pattern = "drifter_hourly_[0-9]*.nc"
+        filename_pattern = "drifter_hourly_{id}.nc"
+
     # retrieve all drifter ID numbers
     if drifter_ids is None:
-        urlpath = urllib.request.urlopen(GDP_DATA_URL)
+        urlpath = urllib.request.urlopen(url)
         string = urlpath.read().decode("utf-8")
-        pattern = re.compile("drifter_[0-9]*.nc")
-        filelist = pattern.findall(string)
+        filelist = re.compile(pattern).findall(string)
         drifter_ids = np.unique([int(f.split("_")[-1][:-3]) for f in filelist])
 
     # retrieve only a subset of n_random_id trajectories
     if n_random_id:
         if n_random_id > len(drifter_ids):
             warnings.warn(
                 f"Retrieving all listed trajectories because {n_random_id} is larger than the {len(drifter_ids)} listed trajectories."
@@ -193,16 +241,16 @@
             drifter_ids = sorted(rng.choice(drifter_ids, n_random_id, replace=False))
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         # create list of urls and paths
         urls = []
         files = []
         for i in drifter_ids:
-            file = GDP_FILENAME_PATTERN.format(id=i)
-            urls.append(os.path.join(GDP_DATA_URL, file))
+            file = filename_pattern.format(id=i)
+            urls.append(os.path.join(url, file))
             files.append(os.path.join(GDP_TMP_PATH, file))
 
         # parallel retrieving of individual netCDF files
         list(
             tqdm(
                 executor.map(fetch_netcdf, urls, files),
                 total=len(files),
@@ -214,126 +262,176 @@
     # Download the metadata so we can order the drifter IDs by end date.
     gdp_metadata = get_gdp_metadata()
 
     return order_by_date(gdp_metadata, drifter_ids)
 
 
 def decode_date(t):
-    """The date format is specified in 'seconds since 1970-01-01 00:00:00' but
+    """The date format is specified as 'seconds since 1970-01-01 00:00:00' but
     the missing values are stored as -1e+34 which is not supported by the
     default parsing mechanism in xarray.
 
     This function returns replaced the missing value by NaN and returns a
     datetime instance.
-    :param t: date
-    :return: datetime
+
+    Parameters
+    ----------
+    t : array
+        Array of time values
+
+    Returns
+    -------
+    out : datetime
+        Datetime instance with the missing value replaced by NaN
     """
     nat_index = np.logical_or(np.isclose(t, -1e34), np.isnan(t))
     t[nat_index] = np.nan
     return t
 
 
 def fill_values(var, default=np.nan):
     """Change fill values (-1e+34, inf, -inf) in var array to the value
     specified by default.
+
+    Parameters
+    ----------
+    var : array
+        Array to fill
+    default : float
+        Default value to use for fill values
     """
     missing_value = np.logical_or(np.isclose(var, -1e34), ~np.isfinite(var))
     if np.any(missing_value):
         var[missing_value] = default
     return var
 
 
-def str_to_float(value: str, default=np.nan) -> float:
+def str_to_float(value: str, default: float = np.nan) -> float:
     """Convert a string to float, while returning the value of default if the
     string is not convertible to a float, or if it's a NaN.
 
-    :param value: str
-    :return: bool
+    Parameters
+    ----------
+    value : str
+        String to convert to float
+    default : float
+        Default value to return if the string is not convertible to float
+
+    Returns
+    -------
+    out : float
+        Float value of the string, or default if the string is not convertible to float.
     """
     try:
         fvalue = float(value)
         if np.isnan(fvalue):
             return default
         else:
             return fvalue
     except ValueError:
         return default
 
 
 def cut_str(value: str, max_length: int) -> np.chararray:
     """Cut a string to a specific length and return it as a numpy chararray.
 
-    Args:
-        value (str): String to cut
-        max_length (int): Length of the output
-    Returns:
-        out (np.chararray): String with max_length characters
+    Parameters
+    ----------
+    value : str
+        String to cut
+    max_length : int
+        Length of the output
+
+    Returns
+    -------
+    out : np.chararray
+        String with max_length characters
     """
     charar = np.chararray(1, max_length)
     charar[:max_length] = value
     return charar
 
 
-def drogue_presence(lost_time, time):
+def drogue_presence(lost_time, time) -> bool:
     """Create drogue status from the drogue lost time and the trajectory time.
 
-    Args:
-        lost_time: Timestamp of the drogue loss (or NaT)
-        time: Observation time
-    Returns:
-        out (bool): True if drogues and False otherwise
+    Parameters
+    ----------
+    lost_time
+        Timestamp of the drogue loss (or NaT)
+    time
+        Observation time
+
+    Returns
+    -------
+    out : bool
+        True if drogues and False otherwise
     """
     if pd.isnull(lost_time) or lost_time >= time[-1]:
         return np.ones_like(time, dtype="bool")
     else:
         return time < lost_time
 
 
-def rowsize(index: int) -> int:
+def rowsize(index: int, filename_pattern: str) -> int:
     return xr.open_dataset(
-        os.path.join(GDP_TMP_PATH, GDP_FILENAME_PATTERN.format(id=index)),
+        os.path.join(GDP_TMP_PATH, filename_pattern.format(id=index)),
         decode_cf=False,
         decode_times=False,
         concat_characters=False,
         decode_coords=False,
     ).dims["obs"]
 
 
-def preprocess(index: int) -> xr.Dataset:
-    """Extract and preprocess the Lagrangian data and attributes. This function
-    takes an identification number that can be used to: create a file or url
-    pattern or select data from a Dataframe. It then preprocess the data and
-    returns a clean xarray Dataset.
+def preprocess(index: int, filename_pattern: str) -> xr.Dataset:
+    """Extract and preprocess the Lagrangian data and attributes.
 
-    :param index: drifter's identification number
-    :return: xr.Dataset containing the data and attributes
+    This function takes an identification number that can be used to create a
+    file or url pattern or select data from a Dataframe. It then preprocesses
+    the data and returns a clean Xarray Dataset.
+
+    Parameters
+    ----------
+    index : int
+        Drifter's identification number
+
+    Returns
+    -------
+    ds : xr.Dataset
+        Xarray Dataset containing the data and attributes
     """
     ds = xr.load_dataset(
-        os.path.join(GDP_TMP_PATH, GDP_FILENAME_PATTERN.format(id=index)),
+        os.path.join(GDP_TMP_PATH, filename_pattern.format(id=index)),
         decode_times=False,
         decode_coords=False,
     )
 
     # parse the date with custom function
     ds["deploy_date"].data = decode_date(np.array([ds.deploy_date.data[0]]))
     ds["end_date"].data = decode_date(np.array([ds.end_date.data[0]]))
     ds["drogue_lost_date"].data = decode_date(np.array([ds.drogue_lost_date.data[0]]))
     ds["time"].data = decode_date(np.array([ds.time.data[0]]))
 
     # convert fill values to nan
-    ds["err_lon"].data = fill_values(ds["err_lon"].data)
-    ds["err_lat"].data = fill_values(ds["err_lat"].data)
-    ds["err_ve"].data = fill_values(ds["err_ve"].data)
-    ds["err_vn"].data = fill_values(ds["err_vn"].data)
-    ds["sst"].data = fill_values(ds["sst"].data)
-    ds["sst1"].data = fill_values(ds["sst1"].data)
-    ds["sst2"].data = fill_values(ds["sst2"].data)
-    ds["err_sst"].data = fill_values(ds["err_sst"].data)
-    ds["err_sst1"].data = fill_values(ds["err_sst1"].data)
-    ds["err_sst2"].data = fill_values(ds["err_sst2"].data)
+    for var in [
+        "err_lon",
+        "err_lat",
+        "err_ve",
+        "err_vn",
+        "sst",
+        "sst1",
+        "sst2",
+        "err_sst",
+        "err_sst1",
+        "err_sst2",
+    ]:
+        try:
+            ds[var].data = fill_values(ds[var].data)
+        except KeyError:
+            warnings.warn(f"Variable {var} not found; skipping.")
 
     # fix missing values stored as str
     for var in [
         "longitude",
         "latitude",
         "err_lat",
         "err_lon",
@@ -341,24 +439,35 @@
         "vn",
         "err_ve",
         "err_vn",
         "sst",
         "sst1",
         "sst2",
     ]:
-        ds[var].encoding["missing value"] = -1e-34
+        try:
+            ds[var].encoding["missing value"] = -1e-34
+        except KeyError:
+            warnings.warn(f"Variable {var} not found in upstream data; skipping.")
 
     # convert type of some variable
-    ds["ID"].data = ds["ID"].data.astype("int64")
-    ds["WMO"].data = ds["WMO"].data.astype("int32")
-    ds["expno"].data = ds["expno"].data.astype("int32")
-    ds["typedeath"].data = ds["typedeath"].data.astype("int8")
-    ds["flg_sst"].data = ds["flg_sst"].data.astype("int8")
-    ds["flg_sst1"].data = ds["flg_sst1"].data.astype("int8")
-    ds["flg_sst2"].data = ds["flg_sst2"].data.astype("int8")
+    target_dtype = {
+        "ID": "int64",
+        "WMO": "int32",
+        "expno": "int32",
+        "typedeath": "int8",
+        "flg_sst": "int8",
+        "flg_sst1": "int8",
+        "flg_sst2": "int8",
+    }
+
+    for var in target_dtype.keys():
+        if var in ds.keys():
+            ds[var].data = ds[var].data.astype(target_dtype[var])
+        else:
+            warnings.warn(f"Variable {var} not found in upstream data; skipping.")
 
     # new variables
     ds["ids"] = (["traj", "obs"], [np.repeat(ds.ID.values, ds.dims["obs"])])
     ds["drogue_status"] = (
         ["traj", "obs"],
         [drogue_presence(ds.drogue_lost_date.data, ds.time.data[0])],
     )
@@ -612,39 +721,57 @@
         "acknowledgement": "Elipot, Shane; Sykulski, Adam; Lumpkin, Rick; Centurioni, Luca; Pazos, Mayra (2022). Hourly location, current velocity, and temperature collected from Global Drifter Program drifters world-wide. [indicate subset used]. NOAA National Centers for Environmental Information. Dataset. https://doi.org/10.25921/x46c-3620. Accessed [date]. Elipot et al. (2022): A Dataset of Hourly Sea Surface Temperature From Drifting Buoys, Scientific Data, 9, 567, https://dx.doi.org/10.1038/s41597-022-01670-2. Elipot et al. (2016): A global surface drifter dataset at hourly resolution, J. Geophys. Res.-Oceans, 121, https://dx.doi.org/10.1002/2016JC011716.",
         "summary": "Global Drifter Program hourly data",
         "doi": "10.25921/x46c-3620",
     }
 
     # set attributes
     for var in vars_attrs.keys():
-        ds[var].attrs = vars_attrs[var]
+        if var in ds.keys():
+            ds[var].attrs = vars_attrs[var]
+        else:
+            warnings.warn(f"Variable {var} not found in upstream data; skipping.")
     ds.attrs = attrs
 
     # rename variables
     ds = ds.rename_vars({"longitude": "lon", "latitude": "lat"})
 
     return ds
 
 
 def to_raggedarray(
-    drifter_ids: Optional[list[int]] = None, n_random_id: Optional[int] = None
+    drifter_ids: Optional[list[int]] = None,
+    n_random_id: Optional[int] = None,
+    url: Optional[str] = GDP_DATA_URL,
 ) -> RaggedArray:
-    """Download and process individual GDP hourly files and return a
-    RaggedArray instance with the data.
+    """Download and process individual GDP hourly files and return a RaggedArray
+    instance with the data.
 
-    Args:
-        drifter_ids [list]: list of drifters to retrieve (Default: all)
-        n_random_id [int]: randomly select n drifter NetCDF files
-    Returns:
-        out [RaggedArray]: A RaggedArray instance of the requested dataset
+    Parameters
+    ----------
+    drifter_ids : list[int], optional
+        List of drifters to retrieve (Default: all)
+    n_random_id : list[int], optional
+        Randomly select n_random_id drifter NetCDF files
+
+    Returns
+    -------
+    out : RaggedArray
+        A RaggedArray instance of the requested dataset
     """
+    ids = download(drifter_ids, n_random_id, url)
 
-    ids = download(drifter_ids, n_random_id)
+    if url == GDP_DATA_URL:
+        filename_pattern = "drifter_{id}.nc"
+    elif url == GDP_DATA_URL_EXPERIMENTAL:
+        filename_pattern = "drifter_hourly_{id}.nc"
+    else:
+        raise ValueError(f"url must be {GDP_DATA_URL} or {GDP_DATA_URL_EXPERIMENTAL}.")
 
     return RaggedArray.from_files(
         indices=ids,
         preprocess_func=preprocess,
         name_coords=GDP_COORDS,
         name_meta=GDP_METADATA,
         name_data=GDP_DATA,
         rowsize_func=rowsize,
+        filename_pattern=filename_pattern,
     )
```

### Comparing `clouddrift-0.8.0/docs/Makefile` & `clouddrift-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/api.rst` & `clouddrift-0.9.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/conf.py` & `clouddrift-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/contributing.rst` & `clouddrift-0.9.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/favicon.ico` & `clouddrift-0.9.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/index.rst` & `clouddrift-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/install.rst` & `clouddrift-0.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/logo.png` & `clouddrift-0.9.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/make.bat` & `clouddrift-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/paper.md` & `clouddrift-0.9.0/docs/paper.md`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/docs/usage.rst` & `clouddrift-0.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/tests/analysis_tests.py` & `clouddrift-0.9.0/tests/analysis_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from clouddrift.analysis import segment, velocity_from_position, apply_ragged
 from clouddrift.haversine import EARTH_RADIUS_METERS
 import unittest
 import numpy as np
 import xarray as xr
+import pandas as pd
+from datetime import datetime, timedelta
 
 
 if __name__ == "__main__":
     unittest.main()
 
 
 class segment_tests(unittest.TestCase):
@@ -16,14 +18,21 @@
         self.assertTrue(type(segment(x, tol)) is np.ndarray)
         self.assertTrue(np.all(segment(x, tol) == np.array([1, 3, 2, 4, 1])))
         self.assertTrue(np.all(segment(np.array(x), tol) == np.array([1, 3, 2, 4, 1])))
         self.assertTrue(
             np.all(segment(xr.DataArray(data=x), tol) == np.array([1, 3, 2, 4, 1]))
         )
 
+    def test_segment_zero_tolerance(self):
+        x = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4]
+        tol = 0
+        self.assertIsNone(
+            np.testing.assert_equal(segment(x, tol), np.array([1, 2, 3, 4]))
+        )
+
     def test_segment_negative_tolerance(self):
         x = [0, 1, 1, 1, 2, 0, 3, 3, 3, 4]
         tol = -1
         self.assertTrue(np.all(segment(x, tol) == np.array([5, 5])))
 
     def test_segment_rowsize(self):
         x = [0, 1, 1, 1, 2, 2, 3, 3, 3, 3, 4]
@@ -41,14 +50,49 @@
     def test_segment_rowsize_raises(self):
         x = [0, 1, 2, 3]
         tol = 0.5
         rowsize = [1, 2]  # rowsize is too short
         with self.assertRaises(ValueError):
             segment(x, tol, rowsize)
 
+    def test_segments_datetime(self):
+        x = [
+            datetime(2023, 1, 1),
+            datetime(2023, 1, 2),
+            datetime(2023, 1, 3),
+            datetime(2023, 2, 1),
+            datetime(2023, 2, 2),
+        ]
+        for tol in [pd.Timedelta("1 day"), timedelta(days=1), np.timedelta64(1, "D")]:
+            self.assertIsNone(
+                np.testing.assert_equal(segment(x, tol), np.array([3, 2]))
+            )
+
+    def test_segments_numpy(self):
+        x = np.array(
+            [
+                np.datetime64("2023-01-01"),
+                np.datetime64("2023-01-02"),
+                np.datetime64("2023-01-03"),
+                np.datetime64("2023-02-01"),
+                np.datetime64("2023-02-02"),
+            ]
+        )
+        for tol in [pd.Timedelta("1 day"), timedelta(days=1), np.timedelta64(1, "D")]:
+            self.assertIsNone(
+                np.testing.assert_equal(segment(x, tol), np.array([3, 2]))
+            )
+
+    def test_segments_pandas(self):
+        x = pd.to_datetime(["1/1/2023", "1/2/2023", "1/3/2023", "2/1/2023", "2/2/2023"])
+        for tol in [pd.Timedelta("1 day"), timedelta(days=1), np.timedelta64(1, "D")]:
+            self.assertIsNone(
+                np.testing.assert_equal(segment(x, tol), np.array([3, 2]))
+            )
+
 
 class velocity_from_position_tests(unittest.TestCase):
     def setUp(self):
         self.INPUT_SIZE = 100
         self.lon = np.rad2deg(np.linspace(-np.pi, np.pi, self.INPUT_SIZE))
         self.lat = np.zeros(self.lon.shape)
         self.time = np.linspace(0, 1e7, self.INPUT_SIZE)
```

### Comparing `clouddrift-0.8.0/tests/dataformat_tests.py` & `clouddrift-0.9.0/tests/dataformat_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             list_ds.append(
                 xr.Dataset(coords=xr_coords, data_vars=xr_data, attrs=self.attrs_global)
             )
 
         # create test ragged array
         self.ra = RaggedArray.from_files(
             [0, 1, 2],
-            lambda i: list_ds[i],
+            lambda i, _: list_ds[i],
             self.variables_coords,
             ["ID", "rowsize"],
             ["temp"],
         )
 
         # output archive
         self.ra.to_netcdf(NETCDF_ARCHIVE)
```

### Comparing `clouddrift-0.8.0/tests/haversine_tests.py` & `clouddrift-0.9.0/tests/haversine_tests.py`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/tests/select_tests.py` & `clouddrift-0.9.0/tests/select_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             list_ds.append(
                 xr.Dataset(coords=xr_coords, data_vars=xr_data, attrs=attrs_global)
             )
 
         # create test ragged array
         ra = RaggedArray.from_files(
             [0, 1, 2],
-            lambda i: list_ds[i],
+            lambda i, _: list_ds[i],
             variables_coords,
             ["ID", "rowsize"],
             ["test"],
         )
 
         self.ds = ra.to_awkward()
```

### Comparing `clouddrift-0.8.0/tests/sphere_tests.py` & `clouddrift-0.9.0/tests/sphere_tests.py`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/.gitignore` & `clouddrift-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/LICENSE` & `clouddrift-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/README.md` & `clouddrift-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `clouddrift-0.8.0/pyproject.toml` & `clouddrift-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "clouddrift"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="Shane Elipot", email="selipot@miami.edu" },
   { name="Philippe Miron", email="philippemiron@gmail.com" },
   { name="Milan Curcic", email="mcurcic@miami.edu" }
 ]
 description = "Accelerating the use of Lagrangian data for atmospheric, oceanic, and climate sciences"
 readme = "README.md"
```

### Comparing `clouddrift-0.8.0/PKG-INFO` & `clouddrift-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clouddrift
-Version: 0.8.0
+Version: 0.9.0
 Summary: Accelerating the use of Lagrangian data for atmospheric, oceanic, and climate sciences
 Project-URL: Homepage, https://github.com/Cloud-Drift/clouddrift
 Project-URL: Documentation, https://cloud-drift.github.io/clouddrift
 Author-email: Shane Elipot <selipot@miami.edu>, Philippe Miron <philippemiron@gmail.com>, Milan Curcic <mcurcic@miami.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

