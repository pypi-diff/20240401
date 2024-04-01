# Comparing `tmp/cleosim-0.8.0.tar.gz` & `tmp/cleosim-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleosim-0.8.0.tar", max compression
+gzip compressed data, was "cleosim-0.9.0.tar", max compression
```

## Comparing `cleosim-0.8.0.tar` & `cleosim-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,83 @@
--rw-r--r--   0        0        0     5950 2022-08-31 16:18:03.755471 cleosim-0.8.0/README.md
--rw-r--r--   0        0        0      294 2022-08-31 00:05:35.579596 cleosim-0.8.0/cleo/__init__.py
--rw-r--r--   0        0        0    15556 2022-08-30 23:58:27.589596 cleosim-0.8.0/cleo/base.py
--rw-r--r--   0        0        0     6635 2022-08-30 23:48:38.239596 cleosim-0.8.0/cleo/coords.py
--rw-r--r--   0        0        0      386 2022-08-31 00:01:07.839596 cleosim-0.8.0/cleo/ephys/__init__.py
--rw-r--r--   0        0        0     7785 2022-08-31 00:01:07.939596 cleosim-0.8.0/cleo/ephys/lfp.py
--rw-r--r--   0        0        0    15869 2022-08-30 23:49:12.389596 cleosim-0.8.0/cleo/ephys/probes.py
--rw-r--r--   0        0        0    12034 2022-08-31 00:01:07.979596 cleosim-0.8.0/cleo/ephys/spiking.py
--rw-r--r--   0        0        0      365 2022-08-31 00:05:35.699596 cleosim-0.8.0/cleo/ioproc/__init__.py
--rw-r--r--   0        0        0     9126 2022-08-31 00:05:35.699596 cleosim-0.8.0/cleo/ioproc/base.py
--rw-r--r--   0        0        0     2138 2022-08-31 00:05:35.699596 cleosim-0.8.0/cleo/ioproc/controllers.py
--rw-r--r--   0        0        0     1312 2022-08-31 00:05:39.229596 cleosim-0.8.0/cleo/ioproc/delays.py
--rw-r--r--   0        0        0     1868 2022-08-31 00:05:35.699596 cleosim-0.8.0/cleo/ioproc/observers.py
--rw-r--r--   0        0        0    21992 2022-08-30 23:48:41.059596 cleosim-0.8.0/cleo/opto.py
--rw-r--r--   0        0        0     3496 2022-08-30 23:48:44.089596 cleosim-0.8.0/cleo/recorders.py
--rw-r--r--   0        0        0     1392 2022-08-30 23:48:53.489596 cleosim-0.8.0/cleo/stimulators.py
--rw-r--r--   0        0        0     7162 2022-08-30 22:14:15.619596 cleosim-0.8.0/cleo/utilities.py
--rw-r--r--   0        0        0    10691 2022-08-31 00:15:49.439596 cleosim-0.8.0/cleo/viz.py
--rw-r--r--   0        0        0     1606 2022-08-31 15:23:45.755471 cleosim-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6887 2022-08-31 18:13:15.328650 cleosim-0.8.0/setup.py
--rw-r--r--   0        0        0     6958 2022-08-31 18:13:15.329038 cleosim-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     5950 2023-03-20 16:12:02.069689 cleosim-0.9.0/README.md
+-rw-r--r--   0        0        0      330 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/__init__.py
+-rw-r--r--   0        0        0    15365 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/base.py
+-rw-r--r--   0        0        0     7273 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/coords.py
+-rw-r--r--   0        0        0      386 2023-03-20 16:12:02.069689 cleosim-0.9.0/cleo/ephys/__init__.py
+-rw-r--r--   0        0        0      630 2023-03-20 18:28:18.519689 cleosim-0.9.0/cleo/ephys/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      324 2022-01-25 16:21:37.065253 cleosim-0.9.0/cleo/ephys/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      628 2023-03-20 16:35:42.179689 cleosim-0.9.0/cleo/ephys/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      614 2022-08-31 00:30:31.679596 cleosim-0.9.0/cleo/ephys/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4726 2022-01-18 17:16:53.574859 cleosim-0.9.0/cleo/ephys/__pycache__/electrodes.cpython-38.pyc
+-rw-r--r--   0        0        0     6931 2023-08-25 15:56:50.911622 cleosim-0.9.0/cleo/ephys/__pycache__/lfp.cpython-310.pyc
+-rw-r--r--   0        0        0     4697 2022-01-25 18:51:50.635253 cleosim-0.9.0/cleo/ephys/__pycache__/lfp.cpython-37.pyc
+-rw-r--r--   0        0        0     6831 2023-07-18 18:40:32.806375 cleosim-0.9.0/cleo/ephys/__pycache__/lfp.cpython-38.pyc
+-rw-r--r--   0        0        0     6468 2022-08-31 00:30:31.679596 cleosim-0.9.0/cleo/ephys/__pycache__/lfp.cpython-39.pyc
+-rw-r--r--   0        0        0    15205 2023-08-25 15:56:51.001622 cleosim-0.9.0/cleo/ephys/__pycache__/probes.cpython-310.pyc
+-rw-r--r--   0        0        0     6764 2022-01-25 18:51:50.725253 cleosim-0.9.0/cleo/ephys/__pycache__/probes.cpython-37.pyc
+-rw-r--r--   0        0        0    15031 2023-07-18 18:40:32.836375 cleosim-0.9.0/cleo/ephys/__pycache__/probes.cpython-38.pyc
+-rw-r--r--   0        0        0    15102 2022-08-31 00:30:33.749596 cleosim-0.9.0/cleo/ephys/__pycache__/probes.cpython-39.pyc
+-rw-r--r--   0        0        0    10513 2023-08-25 15:56:51.011622 cleosim-0.9.0/cleo/ephys/__pycache__/spiking.cpython-310.pyc
+-rw-r--r--   0        0        0     6777 2022-01-25 18:51:50.735253 cleosim-0.9.0/cleo/ephys/__pycache__/spiking.cpython-37.pyc
+-rw-r--r--   0        0        0    10362 2023-07-18 18:40:32.846375 cleosim-0.9.0/cleo/ephys/__pycache__/spiking.cpython-38.pyc
+-rw-r--r--   0        0        0     9728 2022-08-31 00:30:33.759596 cleosim-0.9.0/cleo/ephys/__pycache__/spiking.cpython-39.pyc
+-rw-r--r--   0        0        0     8364 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/ephys/lfp.py
+-rw-r--r--   0        0        0    15749 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/ephys/probes.py
+-rw-r--r--   0        0        0    12264 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/ephys/spiking.py
+-rw-r--r--   0        0        0      602 2023-08-02 19:27:41.167912 cleosim-0.9.0/cleo/imaging/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      315 2023-07-20 19:06:13.651614 cleosim-0.9.0/cleo/imaging/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1577 2023-07-25 14:13:10.665552 cleosim-0.9.0/cleo/imaging/__pycache__/indicators.cpython-310.pyc
+-rw-r--r--   0        0        0     1267 2023-07-20 19:06:13.651614 cleosim-0.9.0/cleo/imaging/__pycache__/indicators.cpython-38.pyc
+-rw-r--r--   0        0        0      156 2023-07-20 17:10:13.561614 cleosim-0.9.0/cleo/imaging/__pycache__/noise.cpython-310.pyc
+-rw-r--r--   0        0        0     5936 2023-08-02 15:29:57.117912 cleosim-0.9.0/cleo/imaging/__pycache__/scope.cpython-310.pyc
+-rw-r--r--   0        0        0     3909 2023-07-20 19:38:07.111614 cleosim-0.9.0/cleo/imaging/__pycache__/scope.cpython-38.pyc
+-rw-r--r--   0        0        0     5803 2023-08-02 19:51:22.197912 cleosim-0.9.0/cleo/imaging/__pycache__/sensors.cpython-310.pyc
+-rw-r--r--   0        0        0      365 2023-03-20 16:12:02.069689 cleosim-0.9.0/cleo/ioproc/__init__.py
+-rw-r--r--   0        0        0      596 2023-03-20 18:28:18.879689 cleosim-0.9.0/cleo/ioproc/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6710 2022-01-25 18:51:50.755253 cleosim-0.9.0/cleo/ioproc/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      594 2023-03-20 16:35:42.339689 cleosim-0.9.0/cleo/ioproc/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      580 2022-08-31 00:30:33.779596 cleosim-0.9.0/cleo/ioproc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8638 2023-03-20 18:28:18.879689 cleosim-0.9.0/cleo/ioproc/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     8539 2023-03-20 16:35:42.339689 cleosim-0.9.0/cleo/ioproc/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     8533 2022-08-31 00:30:33.779596 cleosim-0.9.0/cleo/ioproc/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     2350 2023-03-20 18:28:18.889689 cleosim-0.9.0/cleo/ioproc/__pycache__/controllers.cpython-310.pyc
+-rw-r--r--   0        0        0     1575 2022-01-25 18:51:50.755253 cleosim-0.9.0/cleo/ioproc/__pycache__/controllers.cpython-37.pyc
+-rw-r--r--   0        0        0     2282 2023-03-20 16:35:42.339689 cleosim-0.9.0/cleo/ioproc/__pycache__/controllers.cpython-38.pyc
+-rw-r--r--   0        0        0     2272 2022-08-31 00:30:33.779596 cleosim-0.9.0/cleo/ioproc/__pycache__/controllers.cpython-39.pyc
+-rw-r--r--   0        0        0     2160 2023-03-20 18:28:18.889689 cleosim-0.9.0/cleo/ioproc/__pycache__/delays.cpython-310.pyc
+-rw-r--r--   0        0        0     1658 2022-01-25 16:21:37.155253 cleosim-0.9.0/cleo/ioproc/__pycache__/delays.cpython-37.pyc
+-rw-r--r--   0        0        0     2149 2023-03-20 16:35:42.339689 cleosim-0.9.0/cleo/ioproc/__pycache__/delays.cpython-38.pyc
+-rw-r--r--   0        0        0     2135 2022-08-31 00:30:33.779596 cleosim-0.9.0/cleo/ioproc/__pycache__/delays.cpython-39.pyc
+-rw-r--r--   0        0        0     2072 2023-03-20 18:28:18.889689 cleosim-0.9.0/cleo/ioproc/__pycache__/observers.cpython-310.pyc
+-rw-r--r--   0        0        0     1576 2022-01-25 18:51:50.755253 cleosim-0.9.0/cleo/ioproc/__pycache__/observers.cpython-37.pyc
+-rw-r--r--   0        0        0     2055 2023-03-20 16:35:42.339689 cleosim-0.9.0/cleo/ioproc/__pycache__/observers.cpython-38.pyc
+-rw-r--r--   0        0        0     2045 2022-08-31 00:30:33.779596 cleosim-0.9.0/cleo/ioproc/__pycache__/observers.cpython-39.pyc
+-rw-r--r--   0        0        0     9126 2023-03-20 16:12:02.069689 cleosim-0.9.0/cleo/ioproc/base.py
+-rw-r--r--   0        0        0     2138 2023-03-20 16:12:02.069689 cleosim-0.9.0/cleo/ioproc/controllers.py
+-rw-r--r--   0        0        0     1312 2023-03-20 16:12:02.069689 cleosim-0.9.0/cleo/ioproc/delays.py
+-rw-r--r--   0        0        0     1868 2023-03-20 16:12:02.069689 cleosim-0.9.0/cleo/ioproc/observers.py
+-rw-r--r--   0        0        0      402 2023-08-02 15:40:12.467912 cleosim-0.9.0/cleo/light/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    13681 2023-08-02 15:25:58.337912 cleosim-0.9.0/cleo/light/__pycache__/light.cpython-310.pyc
+-rw-r--r--   0        0        0     4673 2023-08-02 15:59:00.117912 cleosim-0.9.0/cleo/light/__pycache__/light_dependence.cpython-310.pyc
+-rw-r--r--   0        0        0      571 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/opto/__init__.py
+-rw-r--r--   0        0        0      787 2023-08-25 15:56:51.031622 cleosim-0.9.0/cleo/opto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      785 2023-07-20 19:06:13.621614 cleosim-0.9.0/cleo/opto/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    13687 2023-08-25 15:56:51.071622 cleosim-0.9.0/cleo/opto/__pycache__/light.cpython-310.pyc
+-rw-r--r--   0        0        0    13479 2023-07-18 18:40:32.866375 cleosim-0.9.0/cleo/opto/__pycache__/light.cpython-38.pyc
+-rw-r--r--   0        0        0     5980 2023-08-25 15:56:51.061622 cleosim-0.9.0/cleo/opto/__pycache__/opsin_library.cpython-310.pyc
+-rw-r--r--   0        0        0     5616 2023-07-12 18:20:45.792395 cleosim-0.9.0/cleo/opto/__pycache__/opsin_library.cpython-38.pyc
+-rw-r--r--   0        0        0    18067 2023-08-25 15:56:51.061622 cleosim-0.9.0/cleo/opto/__pycache__/opsins.cpython-310.pyc
+-rw-r--r--   0        0        0    16050 2023-07-18 18:40:32.856375 cleosim-0.9.0/cleo/opto/__pycache__/opsins.cpython-38.pyc
+-rw-r--r--   0        0        0     4966 2023-08-25 15:56:51.031622 cleosim-0.9.0/cleo/opto/__pycache__/registry.cpython-310.pyc
+-rw-r--r--   0        0        0     4912 2023-07-12 18:20:45.782395 cleosim-0.9.0/cleo/opto/__pycache__/registry.cpython-38.pyc
+-rw-r--r--   0        0        0      634 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/opto/holo_stim.py
+-rw-r--r--   0        0        0    17363 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/opto/light.py
+-rw-r--r--   0        0        0     6342 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/opto/opsin_library.py
+-rw-r--r--   0        0        0    19918 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/opto/opsins.py
+-rw-r--r--   0        0        0     5744 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/opto/registry.py
+-rw-r--r--   0        0        0     3184 2023-07-07 21:23:36.687036 cleosim-0.9.0/cleo/recorders.py
+-rw-r--r--   0        0        0     1128 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/stimulators.py
+-rw-r--r--   0        0        0     9333 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/utilities.py
+-rw-r--r--   0        0        0    11238 2023-08-25 15:55:55.891622 cleosim-0.9.0/cleo/viz.py
+-rw-r--r--   0        0        0     1650 2023-08-25 15:56:33.121622 cleosim-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6947 2023-08-25 16:05:17.311341 cleosim-0.9.0/setup.py
+-rw-r--r--   0        0        0     7034 2023-08-25 16:05:17.311745 cleosim-0.9.0/PKG-INFO
```

### Comparing `cleosim-0.8.0/README.md` & `cleosim-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cleosim-0.8.0/cleo/base.py` & `cleosim-0.9.0/cleo/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,68 @@
 """Contains definitions for essential, base classes."""
 
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, Tuple, Iterable
+import datetime
 
+from attrs import define, field
 from brian2 import (
     NeuronGroup,
     Subgroup,
     Network,
     NetworkOperation,
     defaultclock,
     ms,
     Unit,
     Quantity,
 )
 from matplotlib import pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D
 from matplotlib.artist import Artist
+import neo
 
+import cleo.utilities
 
+
+class NeoExportable(ABC):
+    """Mixin class for classes that can be exported to Neo objects"""
+
+    @abstractmethod
+    def to_neo(self) -> neo.core.BaseNeo:
+        """Return a neo.core.AnalogSignal object with the device's data
+
+        Returns
+        -------
+        neo.core.BaseNeo
+            Neo object representing exported data
+        """
+        pass
+
+
+@define(eq=False)
 class InterfaceDevice(ABC):
     """Base class for devices to be injected into the network"""
 
-    name: str
-    """Unique identifier for device.
-    Used as a key in output/input dicts
-    """
-    brian_objects: set
+    brian_objects: set = field(factory=set, init=False)
     """All the Brian objects added to the network by this device.
     Must be kept up-to-date in :meth:`connect_to_neuron_group` and
     other functions so that those objects can be automatically added
     to the network when the device is injected.
     """
-    sim: CLSimulator
-    """The simulator the device is injected into
-    """
+    sim: CLSimulator = field(init=False, default=None)
+    """The simulator the device is injected into """
 
-    def __init__(self, name: str) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            Unique identifier for the device.
-        """
-        self.name = name
-        self.brian_objects = set()
-        self.sim = None
+    name: str = field(kw_only=True)
+    """Unique identifier for device, used in sampling, plotting, etc.
+    Name of the class by default."""
+
+    @name.default
+    def _default_name(self) -> str:
+        return self.__class__.__name__
 
     def init_for_simulator(self, simulator: CLSimulator) -> None:
         """Initialize device for simulator on initial injection
 
         This function is called only the first time a device is
         injected into a simulator and performs any operations
         that are independent of the individual neuron groups it
@@ -58,27 +71,31 @@
         Parameters
         ----------
         simulator : CLSimulator
             simulator being injected into
         """
         pass
 
+    def reset(self, **kwargs) -> None:
+        """Reset the device to a neutral state"""
+        pass
+
     @abstractmethod
     def connect_to_neuron_group(self, neuron_group: NeuronGroup, **kwparams) -> None:
         """Connect device to given `neuron_group`.
 
         If your device introduces any objects which Brian must
         keep track of, such as a NeuronGroup, Synapses, or Monitor,
         make sure to add these to `self.brian_objects`.
 
         Parameters
         ----------
         neuron_group : NeuronGroup
-        **kwparams : optional, passed from `inject_recorder` or
-            `inject_stimulator`
+        **kwparams : optional, passed from `inject` or
+            `inject`
         """
         pass
 
     def add_self_to_plot(
         self, ax: Axes3D, axis_scale_unit: Unit, **kwargs
     ) -> list[Artist]:
         """Add device to an existing plot
@@ -97,15 +114,15 @@
         -------
         list[Artist]
             A list of artists used to render the device. Needed for use
             in conjunction with :class:`~cleo.viz.VideoVisualizer`.
         """
         return []
 
-    def update_artists(artists: list[Artist], *args, **kwargs) -> list[Artist]:
+    def update_artists(self, artists: list[Artist], *args, **kwargs) -> list[Artist]:
         """Update the artists used to render the device
 
         Used to set the artists' state at every frame of a video visualization.
         The current state would be passed in `*args` or `**kwargs`
 
         Parameters
         ----------
@@ -179,64 +196,47 @@
         """
         pass
 
     def reset(self, **kwargs) -> None:
         pass
 
 
+@define(eq=False)
 class Recorder(InterfaceDevice):
     """Device for taking measurements of the network."""
 
     @abstractmethod
     def get_state(self) -> Any:
         """Return current measurement."""
         pass
 
-    def reset(self, **kwargs) -> None:
-        """Reset the recording device to a neutral state"""
-        pass
-
 
-class Stimulator(InterfaceDevice):
+@define(eq=False)
+class Stimulator(InterfaceDevice, NeoExportable):
     """Device for manipulating the network"""
 
-    value: Any
+    value: Any = field(init=False, default=None)
     """The current value of the stimulator device"""
-    default_value: Any
+    default_value: Any = 0
     """The default value of the device---used on initialization and on :meth:`~reset`"""
-    t_ms: list[float]
+    t_ms: list[float] = field(factory=list, init=False, repr=False)
     """Times stimulator was updated, stored if :attr:`save_history`"""
-    values: list[Any]
+    values: list[Any] = field(factory=list, init=False, repr=False)
     """Values taken by the stimulator at each :meth:`~update` call, 
     stored if :attr:`save_history`"""
-    save_history: bool
+    save_history: bool = True
     """Determines whether :attr:`t_ms` and :attr:`values` are recorded"""
 
-    def __init__(self, name: str, default_value, save_history: bool = False) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            Unique device name used in :meth:`CLSimulator.update_stimulators`
-        default_value : any
-            The stimulator's default value
-        """
-        super().__init__(name)
-        self.value = default_value
-        self.default_value = default_value
-        self.save_history = save_history
-
-    def init_for_simulator(self, simulator: CLSimulator) -> None:
-        super().init_for_simulator(simulator)
-        self._init_saved_vars()
+    def __attrs_post_init__(self):
+        self.value = self.default_value
 
     def _init_saved_vars(self):
         if self.save_history:
-            self.t_ms = [self.sim.network.t / ms]
-            self.values = [self.default_value]
+            self.t_ms = []
+            self.values = []
 
     def update(self, ctrl_signal) -> None:
         """Set the stimulator value.
 
         By default this simply sets `value` to `ctrl_signal`.
         You will want to implement this method if your
         stimulator requires additional logic. Use super.update(self, value)
@@ -250,55 +250,56 @@
         self.value = ctrl_signal
         if self.save_history:
             self.t_ms.append(self.sim.network.t / ms)
             self.values.append(self.value)
 
     def reset(self, **kwargs) -> None:
         """Reset the stimulator device to a neutral state"""
+        self.value = self.default_value
         self._init_saved_vars()
 
+    def to_neo(self):
+        signal = cleo.utilities.analog_signal(self.t_ms, self.values, "dimensionless")
+        signal.name = self.name
+        signal.description = "Exported from Cleo stimulator device"
+        signal.annotate(export_datetime=datetime.datetime.now())
+        return signal
 
-class CLSimulator:
-    """The centerpiece of cleo. Integrates simulation components and runs."""
 
-    io_processor: IOProcessor
-    network: Network
-    recorders = "set[Recorder]"
-    stimulators = "set[Stimulator]"
-    _processing_net_op: NetworkOperation
-    _net_store_name: str = "cleo default"
+@define(eq=False)
+class CLSimulator(NeoExportable):
+    """The centerpiece of cleo. Integrates simulation components and runs."""
 
-    def __init__(self, brian_network: Network) -> None:
-        """
-        Parameters
-        ----------
-        brian_network : Network
-            The Brian network forming the core model
-        """
-        self.network = brian_network
-        self.stimulators = {}
-        self.recorders = {}
-        self.io_processor = None
-        self._processing_net_op = None
+    network: Network = field(repr=False)
+    """The Brian network forming the core model"""
+    io_processor: IOProcessor = field(default=None, init=False)
+    recorders: dict[str, Recorder] = field(factory=dict, init=False, repr=False)
+    stimulators: dict[str, Stimulator] = field(factory=dict, init=False, repr=False)
+    devices: set[InterfaceDevice] = field(factory=set, init=False)
+    _processing_net_op: NetworkOperation = field(default=None, init=False, repr=False)
+    _net_store_name: str = field(default="cleo default", init=False, repr=False)
 
-    def inject_device(
+    def inject(
         self, device: InterfaceDevice, *neuron_groups: NeuronGroup, **kwparams: Any
-    ) -> None:
+    ) -> CLSimulator:
         """Inject InterfaceDevice into the network, connecting to specified neurons.
 
         Calls :meth:`~InterfaceDevice.connect_to_neuron_group` for each group with
         kwparams and adds the device's :attr:`~InterfaceDevice.brian_objects`
         to the simulator's :attr:`network`.
 
-        Automatically called by :meth:`inject_recorder` and :meth:`inject_stimulator`.
-
         Parameters
         ----------
         device : InterfaceDevice
             Device to inject
+
+        Returns
+        -------
+        CLSimulator
+            self
         """
         if len(neuron_groups) == 0:
             raise Exception("Injecting stimulator for no neuron groups is meaningless.")
         for ng in neuron_groups:
             if type(ng) == NeuronGroup:
                 if ng not in self.network.objects:
                     raise Exception(
@@ -319,58 +320,23 @@
                     "Each device can only be injected into one CLSimulator."
                 )
             if device.sim is None:
                 device.sim = self
                 device.init_for_simulator(self)
             device.connect_to_neuron_group(ng, **kwparams)
         for brian_object in device.brian_objects:
-            self.network.add(brian_object)
+            if brian_object not in self.network.objects:
+                self.network.add(brian_object)
         self.network.store(self._net_store_name)
-
-    def inject_stimulator(
-        self, stimulator: Stimulator, *neuron_groups: NeuronGroup, **kwparams
-    ) -> None:
-        """Inject stimulator into given neuron groups.
-
-        :meth:`Stimulator.connect_to_neuron_group` is called for each `group`.
-
-        Parameters
-        ----------
-        stimulator : Stimulator
-            The stimulator to inject
-        *neuron_groups : NeuronGroup
-            The groups to inject the stimulator into
-        **kwparams : any
-            Passed on to :meth:`Stimulator.connect_to_neuron_group` function.
-            Necessary for parameters that can vary by neuron group, such
-            as opsin expression levels.
-        """
-        self.inject_device(stimulator, *neuron_groups, **kwparams)
-        self.stimulators[stimulator.name] = stimulator
-
-    def inject_recorder(
-        self, recorder: Recorder, *neuron_groups: NeuronGroup, **kwparams
-    ) -> None:
-        """Inject recorder into given neuron groups.
-
-        :meth:`Recorder.connect_to_neuron_group` is called for each `group`.
-
-        Parameters
-        ----------
-        recorder : Recorder
-            The recorder to inject into the simulation
-        *neuron_groups : NeuronGroup
-            The groups to inject the recorder into
-        **kwparams : any
-            Passed on to :meth:`Recorder.connect_to_neuron_group` function.
-            Necessary for parameters that can vary by neuron group, such
-            as inhibitory/excitatory cell type
-        """
-        self.inject_device(recorder, *neuron_groups, **kwparams)
-        self.recorders[recorder.name] = recorder
+        if isinstance(device, Recorder):
+            self.recorders[device.name] = device
+        if isinstance(device, Stimulator):
+            self.stimulators[device.name] = device
+        self.devices.add(device)
+        return self
 
     def get_state(self) -> dict:
         """Return current recorder measurements.
 
         Returns
         -------
         dict
@@ -392,24 +358,29 @@
             to update each stimulator.
         """
         if ctrl_signals is None:
             return
         for name, signal in ctrl_signals.items():
             self.stimulators[name].update(signal)
 
-    def set_io_processor(self, io_processor, communication_period=None) -> None:
+    def set_io_processor(self, io_processor, communication_period=None) -> CLSimulator:
         """Set simulator IO processor
 
         Will replace any previous IOProcessor so there is only one at a time.
         A Brian NetworkOperation is created to govern communication between
         the Network and the IOProcessor.
 
         Parameters
         ----------
         io_processor : IOProcessor
+
+        Returns
+        -------
+        CLSimulator
+            self
         """
         self.io_processor = io_processor
         # remove previous NetworkOperation
         if self._processing_net_op is not None:
             self.network.remove(self._processing_net_op)
             self._processing_net_op = None
 
@@ -427,14 +398,15 @@
         if communication_period is None:
             communication_period = defaultclock.dt
         self._processing_net_op = NetworkOperation(
             communicate_with_io_proc, dt=communication_period
         )
         self.network.add(self._processing_net_op)
         self.network.store(self._net_store_name)
+        return self
 
     def run(self, duration: Quantity, **kwparams) -> None:
         """Run simulation.
 
         Parameters
         ----------
         duration : brian2 temporal Quantity
@@ -447,17 +419,34 @@
         self.network.run(duration, **kwparams)
 
     def reset(self, **kwargs):
         """Reset the simulator to a neutral state
 
         Restores the Brian Network to where it was when the
         CLSimulator was last modified (last injection, IOProcessor change).
-        Calls reset() on stimulators, recorders, and IOProcessor.
+        Calls reset() on devices and IOProcessor.
         """
         # kwargs passed to stimulators, recorders, and io_processor reset
         self.network.restore(self._net_store_name)
-        for stim in self.stimulators.values():
-            stim.reset(**kwargs)
-        for rec in self.recorders.values():
-            rec.reset(**kwargs)
+        for device in self.devices:
+            device.reset(**kwargs)
         if self.io_processor is not None:
             self.io_processor.reset(**kwargs)
+
+    def to_neo(self) -> neo.core.Block:
+        block = neo.Block(
+            description="Exported from Cleo simulation",
+        )
+        block.annotate(export_datetime=datetime.datetime.now())
+        seg = neo.Segment()
+        block.segments.append(seg)
+        for device in self.devices:
+            if not isinstance(device, NeoExportable):
+                continue
+            dev_neo = device.to_neo()
+            if isinstance(dev_neo, neo.core.Group):
+                data_objects = dev_neo.data_children_recur
+                block.groups.append(dev_neo)
+            elif isinstance(dev_neo, neo.core.dataobject.DataObject):
+                data_objects = [dev_neo]
+            cleo.utilities.add_to_neo_segment(seg, *data_objects)
+        return block
```

### Comparing `cleosim-0.8.0/cleo/coords.py` & `cleosim-0.9.0/cleo/coords.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from brian2 import mm, meter, Unit
 from brian2.groups.group import Group
 from brian2.groups.neurongroup import NeuronGroup
 from brian2.units.fundamentalunits import get_dimensions
 import numpy as np
 
 from cleo.utilities import (
-    get_orth_vectors_for_v,
+    get_orth_vectors_for_V,
     modify_model_with_eqs,
     uniform_cylinder_rθz,
     xyz_from_rθz,
 )
 
 
 def assign_coords_grid_rect_prism(
@@ -54,15 +54,15 @@
             f"does not match the number of neurons in the group ({len(neuron_group)})."
         )
 
     x = np.linspace(xlim[0], xlim[1], shape[0])
     y = np.linspace(ylim[0], ylim[1], shape[1])
     z = np.linspace(zlim[0], zlim[1], shape[2])
 
-    x, y, z = np.meshgrid(x, y, z)
+    x, y, z = np.meshgrid(x, y, z, indexing="ij")
     assign_coords(neuron_group, x, y, z)
 
 
 def assign_coords_rand_rect_prism(
     neuron_group: NeuronGroup,
     xlim: Tuple[float, float],
     ylim: Tuple[float, float],
@@ -181,14 +181,36 @@
     """
     _init_variables(neuron_group)
     neuron_group.x = np.reshape(x, (-1,)) * unit
     neuron_group.y = np.reshape(y, (-1,)) * unit
     neuron_group.z = np.reshape(z, (-1,)) * unit
 
 
+def coords_from_xyz(x: Quantity, y: Quantity, z: Quantity) -> Quantity:
+    """Get ...x3 coordinate array from x, y, z arrays (with units)."""
+    # have to add unit back on since it's stripped by vstack
+    n = x.shape[-1]
+    return (
+        np.concatenate(
+            [
+                np.reshape(x, (-1, n, 1)),
+                np.reshape(y, (-1, n, 1)),
+                np.reshape(z, (-1, n, 1)),
+            ],
+            axis=-1,
+        )
+        * meter
+    )
+
+
+def coords_from_ng(ng: NeuronGroup) -> Quantity:
+    """Get nx3 coordinate array from NeuronGroup."""
+    return coords_from_xyz(ng.x, ng.y, ng.z)
+
+
 def _init_variables(group: Group):
     for dim_name in ["x", "y", "z"]:
         if hasattr(group, dim_name):
             setattr(group, dim_name, 0 * mm)
         else:
             if type(group) == NeuronGroup:
                 modify_model_with_eqs(group, f"{dim_name}: meter")
```

### Comparing `cleosim-0.8.0/cleo/ephys/lfp.py` & `cleosim-0.9.0/cleo/ephys/lfp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,64 @@
 """Contains LFP signals"""
 from __future__ import annotations
 from typing import Any
+from datetime import datetime
 
+from attrs import define, field
 from brian2 import NeuronGroup, mm, ms
 from brian2.monitors.spikemonitor import SpikeMonitor
 import numpy as np
 from nptyping import NDArray
 from tklfp import TKLFP
+import quantities as pq
 
+from cleo.base import NeoExportable
 from cleo.ephys.probes import Signal, Probe
+import cleo.utilities
 
 
-class TKLFPSignal(Signal):
+@define(eq=False)
+class TKLFPSignal(Signal, NeoExportable):
     """Records the Teleńczuk kernel LFP approximation.
 
     Requires ``tklfp_type='exc'|'inh'`` to specify cell type
     on injection.
 
     An ``orientation`` keyword argument can also be specified on
     injection, which should be an array of shape ``(n_neurons, 3)``
     representing which way is "up," that is, towards the surface of
     the cortex, for each neuron. If a single vector is given, it is
     taken to be the orientation for all neurons in the group. [0, 0, -1]
     is the default, meaning the negative z axis is "up." As stated
     elsewhere, Cleo's convention is that z=0 corresponds to the
     cortical surface and increasing z values represent increasing depth.
 
-    TKLFP is computed from spikes using the tklfp package."""
+    TKLFP is computed from spikes using the `tklfp package <https://github.com/kjohnsen/tklfp/>`_.
+    """
 
-    uLFP_threshold_uV: float
-    """Threshold, in microvolts, above which the uLFP for a single
-    spike is guaranteed to be considered. This determines the buffer
-    length of past spikes, since the uLFP from a long-past spike
-    becomes negligible and is ignored."""
-    save_history: bool
+    uLFP_threshold_uV: float = 1e-3
+    """Threshold, in microvolts, above which the uLFP for a single spike is guaranteed
+    to be considered, by default 1e-3.
+    This determines the buffer length of past spikes, since the uLFP from a long-past
+    spike becomes negligible and is ignored."""
+    save_history: bool = True
     """Whether to record output from every timestep in :attr:`lfp_uV`.
     Output is stored every time :meth:`get_state` is called."""
-    t_ms: NDArray[(Any,), float]
+    t_ms: NDArray[(Any,), float] = field(init=False, repr=False)
     """Times at which LFP is recorded, in ms, stored if :attr:`save_history`"""
-    lfp_uV: NDArray[(Any, Any), float]
+    lfp_uV: NDArray[(Any, Any), float] = field(init=False, repr=False)
     """Approximated LFP from every call to :meth:`get_state`, recorded
     if :attr:`save_history`. Shape is (n_samples, n_channels)."""
-    _elec_coords_mm: np.ndarray
-    _tklfps: list[TKLFP]
-    _monitors: list[SpikeMonitor]
-    _mon_spikes_already_seen: list[int]
-    _i_buffers: list[list[np.ndarray]]
-    _t_ms_buffers: list[list[np.ndarray]]
-
-    def __init__(
-        self, name: str, uLFP_threshold_uV: float = 1e-3, save_history: bool = False
-    ) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            Unique identifier for signal, used to identify signal output in :meth:`Probe.get_state`
-        uLFP_threshold_uV : float, optional
-            Sets :attr:`uLFP_threshold_uV`, by default 1e-3
-        save_history : bool, optional
-            Sets :attr:`save_history` to determine whether output is recorded, by default False
-        """
-        super().__init__(name)
-        self.uLFP_threshold_uV = uLFP_threshold_uV
-        self.save_history = save_history
-        self._tklfps = []
-        self._monitors = []
-        self._mon_spikes_already_seen = []
-        self._i_buffers = []
-        self._t_ms_buffers = []
-        self._buffer_positions = []
+    _elec_coords_mm: np.ndarray = field(init=False, repr=False)
+    _tklfps: list[TKLFP] = field(init=False, factory=list, repr=False)
+    _monitors: list[SpikeMonitor] = field(init=False, factory=list, repr=False)
+    _mon_spikes_already_seen: list[int] = field(init=False, factory=list, repr=False)
+    _i_buffers: list[list[np.ndarray]] = field(init=False, factory=list, repr=False)
+    _t_ms_buffers: list[list[np.ndarray]] = field(init=False, factory=list, repr=False)
+    _buffer_positions: list[int] = field(init=False, factory=list, repr=False)
 
     def init_for_probe(self, probe: Probe):
         # inherit docstring
         super().init_for_probe(probe)
         self._elec_coords_mm = probe.coords / mm
         # need to invert z coords since cleo uses an inverted z axis and
         # tklfp does not
@@ -93,15 +78,15 @@
     def connect_to_neuron_group(self, neuron_group: NeuronGroup, **kwparams):
         # inherit docstring
         # prep tklfp object
         tklfp_type = kwparams.pop("tklfp_type", "not given")
         if tklfp_type not in ["exc", "inh"]:
             raise Exception(
                 "tklfp_type ('exc' or 'inh') must be passed as a keyword argument to "
-                "inject_recorder() when injecting an electrode with a TKLFPSignal."
+                "inject() when injecting an electrode with a TKLFPSignal."
             )
         orientation = kwparams.pop("orientation", np.array([[0, 0, -1]])).copy()
         orientation[:, 2] *= -1
 
         tklfp = TKLFP(
             neuron_group.x / mm,
             neuron_group.y / mm,
@@ -178,13 +163,35 @@
         if sample_period_ms is None:
             try:
                 sample_period_ms = self.probe.sim.io_processor.sample_period_ms
             except AttributeError:  # probably means sim doesn't have io_processor
                 raise Exception(
                     "TKLFP needs to know the sampling period. Either set the simulator's "
                     f"IO processor before injecting {self.probe.name} or "
-                    f"specify it on injection: .inject_recorder({self.probe.name} "
+                    f"specify it on injection: .inject({self.probe.name} "
                     ", tklfp_type=..., sample_period_ms=...)"
                 )
         return np.ceil(
             tklfp.compute_min_window_ms(self.uLFP_threshold_uV) / sample_period_ms
         ).astype(int)
+
+    def to_neo(self) -> neo.AnalogSignal:
+        # inherit docstring
+        try:
+            signal = cleo.utilities.analog_signal(
+                self.t_ms,
+                self.lfp_uV,
+                "uV",
+            )
+        except AttributeError:
+            return
+        signal.name = self.probe.name + "." + self.name
+        signal.description = f"Exported from Cleo {self.__class__.__name__} object"
+        signal.annotate(export_datetime=datetime.now())
+        # broadcast in case of uniform direction
+        signal.array_annotate(
+            x=self.probe.coords[..., 0] / mm * pq.mm,
+            y=self.probe.coords[..., 1] / mm * pq.mm,
+            z=self.probe.coords[..., 2] / mm * pq.mm,
+            i_channel=np.arange(self.probe.n),
+        )
+        return signal
```

### Comparing `cleosim-0.8.0/cleo/ephys/probes.py` & `cleosim-0.9.0/cleo/ephys/probes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 """Contains Probe and Signal classes and electrode coordinate functions"""
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from operator import concat
 from typing import Any, Tuple
 
+from attrs import field, define
 from mpl_toolkits.mplot3d.axes3d import Axes3D
 from matplotlib.artist import Artist
 from brian2 import NeuronGroup, mm, Unit, Quantity, umeter, np
+import neo
 
-from cleo.base import Recorder
-from cleo.utilities import get_orth_vectors_for_v
+from cleo.base import Recorder, NeoExportable
+from cleo.utilities import get_orth_vectors_for_V
 
 
+@define(eq=False)
 class Signal(ABC):
     """Base class representing something an electrode can record"""
 
-    name: str
-    """Unique identifier used to organize probe output"""
-    brian_objects: set
+    name: str = field(kw_only=True)
+    """Unique identifier used to organize probe output.
+    Name of the class by default."""
+
+    @name.default
+    def _default_name(self) -> str:
+        return self.__class__.__name__
+
+    brian_objects: set = field(init=False, factory=set)
     """All Brian objects created by the signal.
     Must be kept up-to-date for automatic injection into the network"""
-    probe: Probe
+    probe: Probe = field(init=False, default=None)
     """The probe the signal is configured to record for."""
 
-    def __init__(self, name: str) -> None:
-        """
-        Constructor must be called at beginning of children constructors.
-
-        Parameters
-        ----------
-        name : str
-            Unique identifier used when reading the state from the network
-        """
-        self.name = name
-        self.brian_objects = set()
-        self.probe = None
-
     def init_for_probe(self, probe: Probe) -> None:
         """Called when attached to a probe.
 
         Ensures signal can access probe and is only attached
         to one
 
         Parameters
@@ -78,64 +74,52 @@
         pass
 
     def reset(self, **kwargs) -> None:
         """Reset signal to a neutral state"""
         pass
 
 
-class Probe(Recorder):
+@define(eq=False)
+class Probe(Recorder, NeoExportable):
     """Picks up specified signals across an array of electrodes.
 
     Visualization kwargs
     --------------------
     marker : str, optional
         The marker used to represent each contact. "x" by default.
     size : float, optional
         The size of each contact marker. 40 by default.
     color : Any, optional
         The color of contact markers. "xkcd:dark gray" by default.
     """
 
-    coords: Quantity
-    """n x 3 array (with Brian length unit) specifying contact locations"""
-    signals: list[Signal]
-    """Signals recorded by the probe"""
-    n: int
-    """Number of electrode contacts in the probe"""
+    coords: Quantity = field(repr=False)
+    """Coordinates of n electrodes. Must be an n x 3 array (with unit)
+    where columns represent x, y, and z"""
+
+    signals: list[Signal] = field(factory=list)
+    """Signals recorded by the probe.
+    Can be added to post-init with :meth:`add_signals`."""
 
-    def __init__(
-        self, name: str, coords: Quantity, signals: Iterable[Signal] = []
-    ) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            Unique identifier for device
-        coords : Quantity
-            Coordinates of n electrodes. Must be an n x 3 array (with unit)
-            where columns represent x, y, and z
-        signals : Iterable[Signal], optional
-            Signals to record with probe, by default [].
-            Can be specified later with :meth:`add_signals`.
+    probe: Probe = field(init=False)
 
-        Raises
-        ------
-        ValueError
-            When coords aren't n x 3
-        """
-        super().__init__(name)
-        self.coords = np.reshape(coords, (-1, 3))
+    def __attrs_post_init__(self):
+        self.coords = self.coords.reshape((-1, 3))
         if len(self.coords.shape) != 2 or self.coords.shape[1] != 3:
             raise ValueError(
                 "coords must be an n by 3 array (with unit) with x, y, and z"
                 "coordinates for n contact locations."
             )
-        self.n = len(self.coords)
-        self.signals = []
-        self.add_signals(*signals)
+        for signal in self.signals:
+            signal.init_for_probe(self)
+
+    @property
+    def n(self):
+        """Number of electrode contacts in the probe"""
+        return len(self.coords)
 
     def add_signals(self, *signals: Signal) -> None:
         """Add signals to the probe for recording
 
         Parameters
         ----------
         *signals : Signal
@@ -239,14 +223,24 @@
         """Reset the probe to a neutral state
 
         Calls reset() on each signal
         """
         for signal in self.signals:
             signal.reset()
 
+    def to_neo(self) -> neo.core.Group:
+        group = neo.core.Group(
+            name=self.name, description="Exported from Cleo Probe device"
+        )
+        for sig in self.signals:
+            if not isinstance(sig, NeoExportable):
+                continue
+            group.add(sig.to_neo())
+        return group
+
 
 def concat_coords(*coords: Quantity) -> Quantity:
     """Combine multiple coordinate Quantity arrays into one
 
     Parameters
     ----------
     *coords : Quantity
@@ -335,15 +329,15 @@
     center_locs = np.linspace(start_location, end_location, tetrode_count)
     # need to add coords around the center locations
     # tetrode_width is the length of one side of the square, so the diagonals
     # are measured in width/sqrt(2)
     #    x      -dir*width/sqrt(2)
     # x  .  x   +/- orth*width/sqrt(2)
     #    x      +dir*width/sqrt(2)
-    orth_uvec, _ = get_orth_vectors_for_v(dir_uvec)
+    orth_uvec, _ = get_orth_vectors_for_V(dir_uvec)
     return np.repeat(center_locs, 4, axis=0) + tetrode_width / np.sqrt(2) * np.tile(
         np.vstack([-dir_uvec, -orth_uvec, orth_uvec, dir_uvec]), (tetrode_count, 1)
     )
 
 
 def poly2_shank_coords(
     array_length: Quantity,
@@ -378,15 +372,15 @@
     Quantity
         channel_count x 3 array of coordinates, where the 3 columns
         represent x, y, and z
     """
     dir_uvec = direction / np.linalg.norm(direction)
     end_location = start_location + array_length * dir_uvec
     out = np.linspace(start_location, end_location, channel_count)
-    orth_uvec, _ = get_orth_vectors_for_v(dir_uvec)
+    orth_uvec, _ = get_orth_vectors_for_V(dir_uvec)
     # place contacts on alternating sides of the central axis
     even_channels = np.arange(channel_count) % 2 == 0
     out[even_channels] += intercol_space / 2 * orth_uvec
     out[~even_channels] -= intercol_space / 2 * orth_uvec
     return out
 
 
@@ -435,15 +429,15 @@
     n_middle = channel_count // 3 + channel_count % 3
     n_side = int((channel_count - n_middle) / 2)
 
     middle = np.linspace(start_location, end_location, n_middle)
 
     spacing = array_length / n_middle
     side_length = n_side * spacing
-    orth_uvec, _ = get_orth_vectors_for_v(dir_uvec)
+    orth_uvec, _ = get_orth_vectors_for_V(dir_uvec)
     side = np.linspace(
         center_loc - dir_uvec * side_length / 2,
         center_loc + dir_uvec * side_length / 2,
         n_side,
     )
     side1 = side + orth_uvec * intercol_space
     side2 = side - orth_uvec * intercol_space
```

### Comparing `cleosim-0.8.0/cleo/ephys/spiking.py` & `cleosim-0.9.0/cleo/ephys/spiking.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,68 @@
 """Contains multi-unit and sorted spiking signals"""
 from __future__ import annotations
 from abc import abstractmethod
 from typing import Any, Tuple
+from datetime import datetime
 
+from attrs import define, field, fields
 from bidict import bidict
-from brian2 import NeuronGroup, Quantity, SpikeMonitor, meter, ms
+from brian2 import NeuronGroup, Quantity, SpikeMonitor, meter, ms, mm
 import numpy as np
-
-# import numpy.typing as npt
+import neo
+import quantities as pq
 from nptyping import NDArray
 
+from cleo.base import NeoExportable
 from cleo.ephys.probes import Signal
 
 
-class Spiking(Signal):
+@define(eq=False)
+class Spiking(Signal, NeoExportable):
     """Base class for probabilistically detecting spikes"""
 
-    perfect_detection_radius: Quantity
+    r_perfect_detection: Quantity
     """Radius (with Brian unit) within which all spikes
     are detected"""
-    half_detection_radius: Quantity
+    r_half_detection: Quantity
     """Radius (with Brian unit) within which half of all spikes
     are detected"""
-    cutoff_probability: float
+    cutoff_probability: float = 0.01
     """Spike detection probability below which neurons will not be
     considered. For computational efficiency."""
-    save_history: bool
+    save_history: bool = True
     """Determines whether :attr:`t_ms`, :attr:`i`, and :attr:`t_samp_ms` are recorded"""
-    t_ms: NDArray[(Any,), float]
+    t_ms: NDArray[(Any,), float] = field(
+        init=False, factory=lambda: np.array([], dtype=float), repr=False
+    )
     """Spike times in ms, stored if :attr:`save_history`"""
-    i: NDArray[(Any,), np.uint]
+    i: NDArray[(Any,), np.uint] = field(
+        init=False, factory=lambda: np.array([], dtype=np.uint), repr=False
+    )
     """Channel (for multi-unit) or neuron (for sorted) indices
     of spikes, stored if :attr:`save_history`"""
-    t_samp_ms: NDArray[(Any,), float]
+    t_samp_ms: NDArray[(Any,), float] = field(
+        init=False, factory=lambda: np.array([], dtype=float), repr=False
+    )
     """Sample times in ms when each spike was recorded, stored 
     if :attr:`save_history`"""
-    i_probe_by_i_ng: bidict
+    i_probe_by_i_ng: bidict = field(init=False, factory=bidict, repr=False)
     """(neuron_group, i_ng) keys,  i_probe values. bidict for converting between
     neuron group indices and the indices the probe uses"""
-    _monitors: list[SpikeMonitor]
-    _mon_spikes_already_seen: list[int]
-    _dtct_prob_array: NDArray[(Any, Any), float]
-
-    def __init__(
-        self,
-        name: str,
-        perfect_detection_radius: Quantity,
-        half_detection_radius: Quantity = None,
-        cutoff_probability: float = 0.01,
-        save_history: bool = False,
-    ) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            Unique identifier for signal
-        perfect_detection_radius : Quantity
-            Radius (with Brian unit) within which all spikes
-            are detected
-        half_detection_radius : Quantity, optional
-            Radius (with Brian unit) within which half of all spikes
-            are detected
-        cutoff_probability : float, optional
-            Spike detection probability below which neurons will not be
-            considered, by default 0.01. For computational efficiency.
-        save_history : bool, optional
-            If True, will save t_ms (spike times), i (neuron or
-            channel index), and t_samp_ms (sample times) as attributes.
-            By default False
-        """
-        super().__init__(name)
-        self.perfect_detection_radius = perfect_detection_radius
-        self.half_detection_radius = half_detection_radius
-        self.cutoff_probability = cutoff_probability
-        self.save_history = save_history
-        self._init_saved_vars()
-        self._monitors = []
-        self._mon_spikes_already_seen = []
-        self._dtct_prob_array = None
-        self.i_probe_by_i_ng = bidict()
+    _monitors: list[SpikeMonitor] = field(init=False, factory=list, repr=False)
+    _mon_spikes_already_seen: list[int] = field(init=False, factory=list, repr=False)
+    _dtct_prob_array: NDArray[(Any, Any), float] = field(
+        init=False, default=None, repr=False
+    )
 
     def _init_saved_vars(self):
         if self.save_history:
-            self.t_ms = np.array([], dtype=float)
-            self.i = np.array([], dtype=np.uint)
-            self.t_samp_ms = np.array([], dtype=float)
+            self.t_ms = fields(type(self)).t_ms.default.factory()
+            self.i = fields(type(self)).i.default.factory()
+            self.t_samp_ms = fields(type(self)).t_samp_ms.default.factory()
 
     def _update_saved_vars(self, t_ms, i, t_samp_ms):
         if self.save_history:
             self.i = np.concatenate([self.i, i])
             self.t_ms = np.concatenate([self.t_ms, t_ms])
             self.t_samp_ms = np.concatenate([self.t_samp_ms, [t_samp_ms]])
 
@@ -160,16 +134,16 @@
             theoretic uses---i.e., a 0 for every channel/neuron that hasn't spiked and a 1
             for a single spike.
         """
         pass
 
     def _detection_prob_for_distance(self, r: Quantity) -> float:
         # p(d) = h/(r-c)
-        a = self.perfect_detection_radius
-        b = self.half_detection_radius
+        a = self.r_perfect_detection
+        b = self.r_half_detection
         # solving for p(a) = 1 and p(b) = .5 yields:
         c = 2 * a - b
         h = b - a
         with np.errstate(divide="ignore"):
             decaying_p = h / (r - c)
         decaying_p[decaying_p == np.inf] = 1  # to fix NaNs caused by /0
         p = 1 * (r <= a) + decaying_p * (r > a)
@@ -198,15 +172,31 @@
     def reset(self, **kwargs) -> None:
         # crucial that this be called after network restore
         # since that would reset monitors
         for j, mon in enumerate(self._monitors):
             self._mon_spikes_already_seen[j] = mon.num_spikes
         self._init_saved_vars()
 
+    def to_neo(self) -> neo.Group:
+        group = neo.Group(allowed_types=[neo.SpikeTrain])
+        for i in set(self.i):
+            st = neo.SpikeTrain(
+                times=self.t_ms[self.i == i] * pq.ms,
+                t_stop=self.probe.sim.network.t / ms * pq.ms,
+            )
+            st.annotate(i=int(i))
+            group.add(st)
+
+        group.annotate(export_datetime=datetime.now())
+        group.name = f"{self.probe.name}.{self.name}"
+        group.description = f"Exported from Cleo {self.__class__.__name__} object"
+        return group
 
+
+@define(eq=False)
 class MultiUnitSpiking(Spiking):
     """Detects spikes per channel, that is, unsorted."""
 
     def connect_to_neuron_group(self, neuron_group: NeuronGroup, **kwparams) -> None:
         """Configure signal to record from specified neuron group
 
         Parameters
@@ -241,15 +231,28 @@
         detected_spikes = np.random.random(probs_for_spikes.shape) < probs_for_spikes
         y = np.sum(detected_spikes, axis=0)
         # ⬇ nonzero gives row, column indices of each nonzero element
         i_spike_detected, i_c_detected = detected_spikes.nonzero()
         t_detected = t[i_spike_detected]
         return i_c_detected, t_detected, y
 
+    def to_neo(self) -> neo.Group:
+        group = super().to_neo()
+        for st in group.spiketrains:
+            i = int(st.annotations["i"])
+            st.annotate(
+                i_channel=i,
+                x_contact=self.probe.coords[i, 0] / mm * pq.mm,
+                y_contact=self.probe.coords[i, 1] / mm * pq.mm,
+                z_contact=self.probe.coords[i, 2] / mm * pq.mm,
+            )
+        return group
+
 
+@define(eq=False)
 class SortedSpiking(Spiking):
     """Detect spikes identified by neuron indices.
 
     The indices used by the probe do not correspond to those
     coming from neuron groups, since the probe must consider
     multiple potential groups and within a group ignores those
     neurons that are too far away to be easily detected."""
```

### Comparing `cleosim-0.8.0/cleo/ioproc/base.py` & `cleosim-0.9.0/cleo/ioproc/base.py`

 * *Files identical despite different names*

### Comparing `cleosim-0.8.0/cleo/ioproc/controllers.py` & `cleosim-0.9.0/cleo/ioproc/controllers.py`

 * *Files identical despite different names*

### Comparing `cleosim-0.8.0/cleo/ioproc/delays.py` & `cleosim-0.9.0/cleo/ioproc/delays.py`

 * *Files identical despite different names*

### Comparing `cleosim-0.8.0/cleo/ioproc/observers.py` & `cleosim-0.9.0/cleo/ioproc/observers.py`

 * *Files identical despite different names*

### Comparing `cleosim-0.8.0/cleo/opto.py` & `cleosim-0.9.0/cleo/opto/opsins.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,199 @@
-"""Contains opsin models, parameters, and OptogeneticIntervention device"""
+"""Contains opsin models and default parameters"""
 from __future__ import annotations
-from abc import ABC, abstractmethod
-from typing import Tuple, Any
+from typing import Callable, Tuple
 import warnings
 
+from attrs import define, field, asdict, fields_dict
 from brian2 import (
     Synapses,
+    Function,
     NeuronGroup,
     Unit,
     BrianObjectException,
     get_unit,
     Equations,
+    implementation,
+    check_units,
 )
+from nptyping import NDArray
 from brian2.units import (
     mm,
     mm2,
     nmeter,
-    meter,
-    kgram,
     Quantity,
     second,
     ms,
     second,
     psiemens,
+    nsiemens,
     mV,
     volt,
     amp,
-    mwatt,
+    mM,
 )
-from brian2.units.allunits import meter2, radian
-import brian2.units.unitsafefunctions as usf
+from brian2.units.allunits import radian
 import numpy as np
-import matplotlib
-from matplotlib import colors
-from matplotlib.artist import Artist
-from matplotlib.collections import PathCollection
-
-from cleo.utilities import uniform_cylinder_rθz, wavelength_to_rgb, xyz_from_rθz
-from cleo.stimulators import Stimulator
-
-
-ChR2_four_state = {
-    "g0": 114000 * psiemens,
-    "gamma": 0.00742,
-    "phim": 2.33e17 / mm2 / second,  # *photon, not in Brian2
-    "k1": 4.15 / ms,
-    "k2": 0.868 / ms,
-    "p": 0.833,
-    "Gf0": 0.0373 / ms,
-    "kf": 0.0581 / ms,
-    "Gb0": 0.0161 / ms,
-    "kb": 0.063 / ms,
-    "q": 1.94,
-    "Gd1": 0.105 / ms,
-    "Gd2": 0.0138 / ms,
-    "Gr0": 0.00033 / ms,
-    "E": 0 * mV,
-    "v0": 43 * mV,
-    "v1": 17.1 * mV,
-}
-"""Parameters for the 4-state ChR2 model.
+from scipy.interpolate import CubicSpline
 
-Taken from try.projectpyrho.org's default 4-state params.
-"""
+from cleo.base import InterfaceDevice
+from cleo.coords import assign_coords
+from cleo.opto.registry import lor_for_sim
+from cleo.utilities import wavelength_to_rgb
 
 
-class OpsinModel(ABC):
-    """Base class for opsin model"""
+def linear_interpolator(lambdas_nm, epsilons, lambda_new_nm):
+    return np.interp(lambda_new_nm, lambdas_nm, epsilons)
 
-    model: str
+
+def cubic_interpolator(lambdas_nm, epsilons, lambda_new_nm):
+    return CubicSpline(lambdas_nm, epsilons)(lambda_new_nm)
+
+
+@define(eq=False)
+class Opsin(InterfaceDevice):
+    """Base class for opsin model.
+
+    We approximate dynamics under multiple wavelengths using a weighted sum
+    of photon fluxes, where the :math:`\\varepsilon` factor indicates the activation
+    relative to the peak-sensitivy wavelength for an equivalent number of photons
+    (see Mager et al, 2018). This weighted sum is an approximation of a nonlinear
+    peak-non-peak wavelength relation; see notebooks/multi_wavelength_model.ipynb
+    for details."""
+
+    model: str = field(init=False)
     """Basic Brian model equations string.
     
     Should contain a `rho_rel` term reflecting relative expression 
     levels. Will likely also contain special NeuronGroup-dependent
     symbols such as V_VAR_NAME to be replaced on injection in 
     :meth:`~OpsinModel.modify_model_and_params_for_ng`."""
 
-    params: dict
-    """Parameter values for model, passed in as a namespace dict"""
+    per_ng_unit_replacements: list[Tuple[str, str]] = field(
+        factory=list, init=False, repr=False
+    )
+    """List of (UNIT_NAME, neuron_group_specific_unit_name) tuples to be substituted
+    in the model string on injection and before checking required variables."""
 
-    required_vars: list[Tuple[str, Unit]]
+    required_vars: list[Tuple[str, Unit]] = field(factory=list, init=False, repr=False)
     """Default names of state variables required in the neuron group,
     along with units, e.g., [('Iopto', amp)].
     
     It is assumed that non-default values can be passed in on injection
     as a keyword argument ``[default_name]_var_name=[non_default_name]``
     and that these are found in the model string as 
     ``[DEFAULT_NAME]_VAR_NAME`` before replacement."""
 
+    light_agg_ngs: dict[str, NeuronGroup] = field(factory=dict, init=False, repr=False)
+    """{target_ng.name: light_agg_ng} dict of light aggregator neuron groups."""
+
+    opto_syns: dict[NeuronGroup, Synapses] = field(factory=dict, init=False, repr=False)
+    """Stores the synapse objects implementing the opsin model,
+    with NeuronGroup keys and Synapse values."""
+
+    action_spectrum: list[tuple[float, float]] = field(
+        factory=lambda: [(-1e10, 1), (1e10, 1)]
+    )
+    """List of (wavelength, epsilon) tuples representing the action spectrum."""
+
+    action_spectrum_interpolator: Callable = field(
+        default=cubic_interpolator, repr=False
+    )
+    """Function of signature (lambdas_nm, epsilons, lambda_new_nm) that interpolates
+    the action spectrum data and returns :math:`\\varepsilon \\in [0,1]` for the new
+    wavelength."""
+
+    extra_namespace: dict = field(factory=dict, repr=False)
+    """Additional items (beyond parameters) to be added to the opto synapse namespace"""
+
+    def connect_to_neuron_group(self, neuron_group: NeuronGroup, **kwparams) -> None:
+        """Transfect neuron group with opsin.
+
+        Parameters
+        ----------
+        neuron_group : NeuronGroup
+            The neuron group to stimulate with the given opsin and light source
+
+        Keyword args
+        ------------
+        p_expression : float
+            Probability (0 <= p <= 1) that a given neuron in the group
+            will express the opsin. 1 by default.
+        rho_rel : float
+            The expression level, relative to the standard model fit,
+            of the opsin. 1 by default. For heterogeneous expression,
+            this would have to be modified in the opsin synapse post-injection,
+            e.g., ``opto.opto_syns["neuron_group_name"].rho_rel = ...``
+        Iopto_var_name : str
+            The name of the variable in the neuron group model representing
+            current from the opsin
+        v_var_name : str
+            The name of the variable in the neuron group model representing
+            membrane potential
+        """
+        if neuron_group.name in self.light_agg_ngs:
+            assert neuron_group.name in self.opto_syns
+            raise ValueError(
+                f"Opsin {self.name} already connected to neuron group {neuron_group.name}"
+            )
+
+        # get modified opsin model string (i.e., with names/units specified)
+        mod_opsin_model, mod_opsin_params = self.modify_model_and_params_for_ng(
+            neuron_group, kwparams
+        )
+
+        # handle p_expression
+        p_expression = kwparams.get("p_expression", 1)
+        i_expression_bool = np.random.rand(neuron_group.N) < p_expression
+        i_expression = np.where(i_expression_bool)[0]
+        if len(i_expression) == 0:
+            return
+
+        # create light aggregator neurons
+        light_agg_ng = NeuronGroup(
+            len(i_expression),
+            model="""
+            phi : 1/second/meter**2
+            Irr : watt/meter**2
+            """,
+            name=f"light_agg_{self.name}_{neuron_group.name}",
+        )
+        assign_coords(
+            light_agg_ng,
+            neuron_group.x[i_expression] / mm,
+            neuron_group.y[i_expression] / mm,
+            neuron_group.z[i_expression] / mm,
+            unit=mm,
+        )
+
+        # create opsin synapses
+        opto_syn = Synapses(
+            light_agg_ng,
+            neuron_group,
+            model=mod_opsin_model,
+            namespace=mod_opsin_params,
+            name=f"opto_syn_{self.name}_{neuron_group.name}",
+        )
+        opto_syn.namespace.update(self.extra_namespace)
+        opto_syn.connect(i=range(len(i_expression)), j=i_expression)
+        self.init_opto_syn_vars(opto_syn)
+        # relative channel density
+        opto_syn.rho_rel = kwparams.get("rho_rel", 1)
+
+        # store at the end, after all checks have passed
+        self.light_agg_ngs[neuron_group.name] = light_agg_ng
+        self.brian_objects.add(light_agg_ng)
+        self.opto_syns[neuron_group.name] = opto_syn
+        self.brian_objects.add(opto_syn)
+
+        lor = lor_for_sim(self.sim)
+        lor.register_opsin(self, neuron_group)
+
     def modify_model_and_params_for_ng(
-        self, neuron_group: NeuronGroup, injct_params: dict, model="class-defined"
+        self, neuron_group: NeuronGroup, injct_params: dict
     ) -> Tuple[Equations, dict]:
         """Adapt model for given neuron group on injection
 
         This enables the specification of variable names
         differently for each neuron group, allowing for custom names
         and avoiding conflicts.
 
@@ -116,40 +216,57 @@
         -------
         Equations, dict
             A tuple containing an Equations object
             and a parameter dictionary, constructed from :attr:`~model`
             and :attr:`~params`, respectively, with modified names for use
             in :attr:`~cleo.opto.OptogeneticIntervention.opto_syns`
         """
-        if model == "class-defined":
-            model = self.model
+        model = self.model
 
+        # perform unit substitutions
+        for unit_name, neuron_group_unit_name in self.per_ng_unit_replacements:
+            model = model.replace(unit_name, neuron_group_unit_name)
+
+        # check required variables/units and replace placeholder names
         for default_name, unit in self.required_vars:
             var_name = injct_params.get(f"{default_name}_var_name", default_name)
             if var_name not in neuron_group.variables or not neuron_group.variables[
                 var_name
             ].unit.has_same_dimensions(unit):
                 raise BrianObjectException(
                     (
                         f"{var_name} : {unit.name} needed in the model of NeuronGroup "
-                        f"{neuron_group.name} to connect OptogeneticIntervention."
+                        f"{neuron_group.name} to connect Opsin {self.name}."
                     ),
                     neuron_group,
                 )
             # opsin synapse model needs modified names
             to_replace = f"{default_name}_var_name".upper()
             model = model.replace(to_replace, var_name)
 
         # Synapse variable and parameter names cannot be the same as any
         # neuron group variable name
         return self._fix_name_conflicts(model, neuron_group)
 
+    @property
+    def params(self) -> dict:
+        """Returns a dictionary of parameters for the model"""
+        params = asdict(self, recurse=False)
+        # remove generic fields that are not parameters
+        for field in fields_dict(Opsin):
+            params.pop(field)
+        # remove private attributes
+        for key in list(params.keys()):
+            if key.startswith("_"):
+                params.pop(key)
+        return params
+
     def _fix_name_conflicts(
         self, modified_model: str, neuron_group: NeuronGroup
-    ) -> Tuple[str, dict]:
+    ) -> Tuple[Equations, dict]:
         modified_params = self.params.copy()
         rename = lambda x: f"{x}_syn"
 
         # get variables to rename
         opsin_eqs = Equations(modified_model)
         substitutions = {}
         for var in opsin_eqs.names:
@@ -162,455 +279,294 @@
                 substitutions[param] = rename(param)
                 modified_params[rename(param)] = modified_params[param]
                 del modified_params[param]
 
         mod_opsin_eqs = opsin_eqs.substitute(**substitutions)
         return mod_opsin_eqs, modified_params
 
+    def reset(self, **kwargs):
+        for opto_syn in self.opto_syns.values():
+            self.init_opto_syn_vars(opto_syn)
+
     def init_opto_syn_vars(self, opto_syn: Synapses) -> None:
         """Initializes appropriate variables in Synapses implementing the model
 
         Can also be used to reset the variables.
 
         Parameters
         ----------
         opto_syn : Synapses
             The synapses object implementing this model
         """
         pass
 
+    def epsilon(self, lambda_new) -> float:
+        """Returns the epsilon value for a given lambda (in nm)
+        representing the relative sensitivity of the opsin to that wavelength."""
+        action_spectrum = np.array(self.action_spectrum)
+        lambdas = action_spectrum[:, 0]
+        epsilons = action_spectrum[:, 1]
+        if lambda_new < min(lambdas) or lambda_new > max(lambdas):
+            warnings.warn(
+                f"λ = {lambda_new} nm is outside the range of the action spectrum data"
+                f" for {self.name}. Assuming ε = 0."
+            )
+            return 0
+        return self.action_spectrum_interpolator(lambdas, epsilons, lambda_new)
+
+
+def plot_action_spectra(*opsins: Opsin):
+    import matplotlib.pyplot as plt
 
-class MarkovModel(OpsinModel):
+    fig, ax = plt.subplots()
+    for opsin in opsins:
+        action_spectrum = np.array(opsin.action_spectrum)
+        lambdas = action_spectrum[:, 0]
+        epsilons = action_spectrum[:, 1]
+        lambdas_new = np.linspace(min(lambdas), max(lambdas), 100)
+        epsilons_new = opsin.action_spectrum_interpolator(
+            lambdas, epsilons, lambdas_new
+        )
+        c_points = [wavelength_to_rgb(l) for l in lambdas]
+        c_line = wavelength_to_rgb(lambdas_new[np.argmax(epsilons_new)])
+        ax.plot(lambdas_new, epsilons_new, c=c_line, label=opsin.name)
+        ax.scatter(lambdas, epsilons, marker="o", s=50, color=c_points)
+    title = "Action spectra" if len(opsins) > 1 else f"Action spectrum"
+    ax.set(xlabel="λ (nm)", ylabel="ε", title=title)
+    fig.legend()
+    return fig, ax
+
+
+@define(eq=False)
+class MarkovOpsin(Opsin):
     """Base class for Markov state models à la Evans et al., 2016"""
 
-    required_vars: list[Tuple[str, Unit]] = [("Iopto", amp), ("v", volt)]
+    required_vars: list[Tuple[str, Unit]] = field(
+        factory=lambda: [("Iopto", amp), ("v", volt)],
+        init=False,
+    )
 
-    def __init__(self, params: dict) -> None:
-        """
-        Parameters
-        ----------
-        params : dict
-            dict defining params in the :attr:`model`
-        """
-        super().__init__()
-        self.params = params
+
+@implementation(
+    "cython",
+    """
+    cdef double f_unless_x0(double f, double x, double f_when_x0):
+        if x == 0:
+            return f_when_x0
+        else:
+            return f
+    """,
+)
+@check_units(f=1, x=volt, f_when_0=1, result=1)
+def f_unless_x0(f, x, f_when_x0):
+    f[x == 0] = f_when_x0
+    return f
 
 
-class FourStateModel(MarkovModel):
+@define(eq=False)
+class FourStateOpsin(MarkovOpsin):
     """4-state model from PyRhO (Evans et al. 2016).
 
     rho_rel is channel density relative to standard model fit;
     modifying it post-injection allows for heterogeneous opsin expression.
 
     IOPTO_VAR_NAME and V_VAR_NAME are substituted on injection.
+
+    Defaults are for ChR2.
     """
 
-    model: str = """
+    g0: Quantity = 114000 * psiemens
+    gamma: Quantity = 0.00742
+    phim: Quantity = 2.33e17 / mm2 / second  # *photon, not in Brian2
+    k1: Quantity = 4.15 / ms
+    k2: Quantity = 0.868 / ms
+    p: Quantity = 0.833
+    Gf0: Quantity = 0.0373 / ms
+    kf: Quantity = 0.0581 / ms
+    Gb0: Quantity = 0.0161 / ms
+    kb: Quantity = 0.063 / ms
+    q: Quantity = 1.94
+    Gd1: Quantity = 0.105 / ms
+    Gd2: Quantity = 0.0138 / ms
+    Gr0: Quantity = 0.00033 / ms
+    E: Quantity = 0 * mV
+    v0: Quantity = 43 * mV
+    v1: Quantity = 17.1 * mV
+    model: str = field(
+        init=False,
+        default="""
         dC1/dt = Gd1*O1 + Gr0*C2 - Ga1*C1 : 1 (clock-driven)
         dO1/dt = Ga1*C1 + Gb*O2 - (Gd1+Gf)*O1 : 1 (clock-driven)
         dO2/dt = Ga2*C2 + Gf*O1 - (Gd2+Gb)*O2 : 1 (clock-driven)
         C2 = 1 - C1 - O1 - O2 : 1
-        # dC2/dt = Gd2*O2 - (Gr0+Ga2)*C2 : 1 (clock-driven)
 
-        Theta = int(phi > 0*phi) : 1
-        Hp = Theta * phi**p/(phi**p + phim**p) : 1
+        Theta = int(phi_pre > 0*phi_pre) : 1
+        Hp = Theta * phi_pre**p/(phi_pre**p + phim**p) : 1
         Ga1 = k1*Hp : hertz
         Ga2 = k2*Hp : hertz
-        Hq = Theta * phi**q/(phi**q + phim**q) : 1
+        Hq = Theta * phi_pre**q/(phi_pre**q + phim**q) : 1
         Gf = kf*Hq + Gf0 : hertz
         Gb = kb*Hq + Gb0 : hertz
 
         fphi = O1 + gamma*O2 : 1
-        fv = (1 - exp(-(V_VAR_NAME_post-E)/v0)) / -2 : 1
+        # TODO: get this voltage dependence right 
+        # v1/v0 when v-E == 0 via l'Hopital's rule
+        # fv = (1 - exp(-(V_VAR_NAME_post-E)/v0)) / -2 : 1
+        fv = f_unless_x0(
+            (1 - exp(-(V_VAR_NAME_post-E)/v0)) / ((V_VAR_NAME_post-E)/v1),
+            V_VAR_NAME_post - E,
+            v1/v0
+        ) : 1
 
         IOPTO_VAR_NAME_post = -g0*fphi*fv*(V_VAR_NAME_post-E)*rho_rel : ampere (summed)
-        rho_rel : 1
-    """
+        rho_rel : 1""",
+    )
+
+    extra_namespace: dict[str, Any] = field(
+        init=False, factory=lambda: {"f_unless_x0": f_unless_x0}
+    )
 
     def init_opto_syn_vars(self, opto_syn: Synapses) -> None:
-        for varname, value in {"Irr0": 0, "C1": 1, "O1": 0, "O2": 0}.items():
+        for varname, value in {"C1": 1, "O1": 0, "O2": 0}.items():
             setattr(opto_syn, varname, value)
 
 
-class ProportionalCurrentModel(OpsinModel):
-    """A simple model delivering current proportional to light intensity"""
-
-    # would be IOPTO_UNIT but that throws off Equation parsing
-    model: str = """
-        IOPTO_VAR_NAME_post = gain * Irr * rho_rel : IOPTO_UNIT (summed)
-        rho_rel : 1
-    """
+@define(eq=False)
+class BansalFourStateOpsin(MarkovOpsin):
+    """4-state model from Bansal et al. 2020.
 
-    def __init__(self, Iopto_per_mW_per_mm2: Quantity) -> None:
-        """
-        Parameters
-        ----------
-        Iopto_per_mW_per_mm2 : Quantity
-            How much current (in amps or unitless, depending on neuron model) to
-            deliver per mW/mm2
-        """
-        self.params = {"gain": Iopto_per_mW_per_mm2 / (mwatt / mm2)}
-        if isinstance(Iopto_per_mW_per_mm2, Quantity):
-            self._Iopto_unit = get_unit(Iopto_per_mW_per_mm2.dim)
-        else:
-            self._Iopto_unit = radian
-        self.required_vars = [("Iopto", self._Iopto_unit)]
-
-    def modify_model_and_params_for_ng(
-        self, neuron_group: NeuronGroup, injct_params: dict
-    ) -> Tuple[Equations, dict]:
-        mod_model = self.model.replace("IOPTO_UNIT", self._Iopto_unit.name)
-        return super().modify_model_and_params_for_ng(
-            neuron_group, injct_params, model=mod_model
-        )
+    The difference from the PyRhO model is that there is no voltage dependence.
 
+    rho_rel is channel density relative to standard model fit;
+    modifying it post-injection allows for heterogeneous opsin expression.
 
-default_blue = {
-    "R0": 0.1 * mm,  # optical fiber radius
-    "NAfib": 0.37,  # optical fiber numerical aperture
-    "wavelength": 473 * nmeter,
-    # NOTE: the following depend on wavelength and tissue properties and thus would be different for another wavelength
-    "K": 0.125 / mm,  # absorbance coefficient
-    "S": 7.37 / mm,  # scattering coefficient
-    "ntis": 1.36,  # tissue index of refraction
-}
-"""Light parameters for 473 nm wavelength delivered via an optic fiber.
-
-From Foutz et al., 2012"""
-
-
-class OptogeneticIntervention(Stimulator):
-    """Enables optogenetic stimulation of the network.
-
-    Essentially "transfects" neurons and provides a light source.
-    Under the hood, it delivers current via a Brian :class:`~brian2.synapses.synapses.Synapses`
-    object.
-
-    Requires neurons to have 3D spatial coordinates already assigned.
-    Also requires that the neuron model has a current term
-    (by default Iopto) which is assumed to be positive (unlike the
-    convention in many opsin modeling papers, where the current is
-    described as negative).
-
-    See :meth:`connect_to_neuron_group` for optional keyword parameters
-    that can be specified when calling
-    :meth:`cleo.CLSimulator.inject_stimulator`.
-
-    Visualization kwargs
-    --------------------
-    n_points : int, optional
-        The number of points used to represent light intensity in space.
-        By default 1e4.
-    T_threshold : float, optional
-        The transmittance below which no points are plotted. By default
-        1e-3.
-    intensity : float, optional
-        How bright the light appears, should be between 0 and 1. By default 0.5.
-    rasterized : bool, optional
-        Whether to render as rasterized in vector output, True by default.
-        Useful since so many points makes later rendering and editing slow.
+    IOPTO_VAR_NAME and V_VAR_NAME are substituted on injection.
     """
 
-    opto_syns: dict[str, Synapses]
-    """Stores the synapse objects implementing the opsin model,
-    with NeuronGroup name keys and Synapse values."""
-
-    max_Irr0_mW_per_mm2: float
-    """The maximum irradiance the light source can emit.
-    
-    Usually determined by hardware in a real experiment."""
-
-    max_Irr0_mW_per_mm2_viz: float
-    """Maximum irradiance for visualization purposes. 
-    
-    i.e., the level at or above which the light appears maximally bright.
-    Only relevant in video visualization.
-    """
+    Gd1: Quantity = 0.066 / ms
+    Gd2: Quantity = 0.01 / ms
+    Gr0: Quantity = 3.33e-4 / ms
+    g0: Quantity = 3.2 * nsiemens
+    phim: Quantity = 1e16 / mm2 / second  # *photon, not in Brian2
+    k1: Quantity = 0.4 / ms
+    k2: Quantity = 0.12 / ms
+    Gf0: Quantity = 0.018 / ms
+    Gb0: Quantity = 0.008 / ms
+    kf: Quantity = 0.01 / ms
+    kb: Quantity = 0.008 / ms
+    gamma: Quantity = 0.05
+    p: Quantity = 1
+    q: Quantity = 1
+    E: Quantity = 0 * mV
+
+    model: str = field(
+        init=False,
+        default="""
+        dC1/dt = Gd1*O1 + Gr0*C2 - Ga1*C1 : 1 (clock-driven)
+        dO1/dt = Ga1*C1 + Gb*O2 - (Gd1+Gf)*O1 : 1 (clock-driven)
+        dO2/dt = Ga2*C2 + Gf*O1 - (Gd2+Gb)*O2 : 1 (clock-driven)
+        C2 = 1 - C1 - O1 - O2 : 1
 
-    def __init__(
-        self,
-        name: str,
-        opsin_model: OpsinModel,
-        light_model_params: dict,
-        location: Quantity = (0, 0, 0) * mm,
-        direction: Tuple[float, float, float] = (0, 0, 1),
-        max_Irr0_mW_per_mm2: float = None,
-        save_history: bool = False,
-    ):
-        """
-        Parameters
-        ----------
-        name : str
-            Unique identifier for stimulator
-        opsin_model : OpsinModel
-            OpsinModel object defining how light affects target
-            neurons. See :class:`FourStateModel` and :class:`ProportionalCurrentModel`
-            for examples.
-        light_model_params : dict
-            Parameters for the light propagation model in Foutz et al., 2012.
-            See :attr:`default_blue` for an example.
-        location : Quantity, optional
-            (x, y, z) coords with Brian unit specifying where to place
-            the base of the light source, by default (0, 0, 0)*mm
-        direction : Tuple[float, float, float], optional
-            (x, y, z) vector specifying direction in which light
-            source is pointing, by default (0, 0, 1)
-        max_Irr0_mW_per_mm2 : float, optional
-            Set :attr:`max_Irr0_mW_per_mm2`.
-        save_history : bool, optional
-            Determines whether :attr:`~values` and :attr:`~t_ms` are saved.
-        """
-        super().__init__(name, 0, save_history)
-        self.opsin_model = opsin_model
-        self.light_model_params = light_model_params
-        self.location = location
-        # direction unit vector
-        self.dir_uvec = direction / np.linalg.norm(direction)
-        self.opto_syns = {}
-        self.max_Irr0_mW_per_mm2 = max_Irr0_mW_per_mm2
-        self.max_Irr0_mW_per_mm2_viz = None
-
-    def _Foutz12_transmittance(self, r, z, scatter=True, spread=True, gaussian=True):
-        """Foutz et al. 2012 transmittance model: Gaussian cone with Kubelka-Munk propagation"""
-
-        if spread:
-            # divergence half-angle of cone
-            theta_div = np.arcsin(
-                self.light_model_params["NAfib"] / self.light_model_params["ntis"]
-            )
-            Rz = self.light_model_params["R0"] + z * np.tan(
-                theta_div
-            )  # radius as light spreads ("apparent radius" from original code)
-            C = (self.light_model_params["R0"] / Rz) ** 2
-        else:
-            Rz = self.light_model_params["R0"]  # "apparent radius"
-            C = 1
+        Theta = int(phi_pre > 0*phi_pre) : 1
+        Hp = Theta * phi_pre**p/(phi_pre**p + phim**p) : 1
+        Ga1 = k1*Hp : hertz
+        Ga2 = k2*Hp : hertz
+        Hq = Theta * phi_pre**q/(phi_pre**q + phim**q) : 1
+        Gf = kf*Hq + Gf0 : hertz
+        Gb = kb*Hq + Gb0 : hertz
 
-        if gaussian:
-            G = 1 / np.sqrt(2 * np.pi) * np.exp(-2 * (r / Rz) ** 2)
-        else:
-            G = 1
+        fphi = O1 + gamma*O2 : 1
 
-        if scatter:
-            S = self.light_model_params["S"]
-            a = 1 + self.light_model_params["K"] / S
-            b = np.sqrt(a**2 - 1)
-            dist = np.sqrt(r**2 + z**2)
-            M = b / (a * np.sinh(b * S * dist) + b * np.cosh(b * S * dist))
-        else:
-            M = 1
+        IOPTO_VAR_NAME_post = -g0*fphi*(V_VAR_NAME_post-E)*rho_rel : ampere (summed)
+        rho_rel : 1""",
+    )
 
-        T = G * C * M
-        T[z < 0] = 0
-        return T
-
-    def _get_rz_for_xyz(self, x, y, z):
-        """Assumes x, y, z already have units"""
-
-        # have to add unit back on since it's stripped by vstack
-        coords = np.column_stack([x, y, z]) * meter
-        rel_coords = coords - self.location  # relative to fiber location
-        # must use brian2's dot function for matrix multiply to preserve
-        # units correctly.
-        zc = usf.dot(rel_coords, self.dir_uvec)  # distance along cylinder axis
-        # just need length (norm) of radius vectors
-        # not using np.linalg.norm because it strips units
-        r = np.sqrt(
-            np.sum((rel_coords - zc[..., np.newaxis] * self.dir_uvec.T) ** 2, axis=1)
-        )
-        return r, zc
+    def init_opto_syn_vars(self, opto_syn: Synapses) -> None:
+        for varname, value in {"C1": 1, "O1": 0, "O2": 0}.items():
+            setattr(opto_syn, varname, value)
 
-    def connect_to_neuron_group(
-        self, neuron_group: NeuronGroup, **kwparams: Any
-    ) -> None:
-        """Configure opsin and light source to stimulate given neuron group.
 
-        Parameters
-        ----------
-        neuron_group : NeuronGroup
-            The neuron group to stimulate with the given opsin and light source
+@define(eq=False)
+class BansalThreeStatePump(MarkovOpsin):
+    """3-state model from `Bansal et al. 2020 <10.1016/j.neuroscience.2020.09.022>`_.
 
-        Keyword args
-        ------------
-        p_expression : float
-            Probability (0 <= p <= 1) that a given neuron in the group
-            will express the opsin. 1 by default.
-        rho_rel : float
-            The expression level, relative to the standard model fit,
-            of the opsin. 1 by default. For heterogeneous expression,
-            this would have to be modified in the opsin synapse post-injection,
-            e.g., ``opto.opto_syns["neuron_group_name"].rho_rel = ...``
-        Iopto_var_name : str
-            The name of the variable in the neuron group model representing
-            current from the opsin
-        v_var_name : str
-            The name of the variable in the neuron group model representing
-            membrane potential
-        """
-        # get modified opsin model string (i.e., with names/units specified)
-        (
-            mod_opsin_model,
-            mod_opsin_params,
-        ) = self.opsin_model.modify_model_and_params_for_ng(neuron_group, kwparams)
-
-        # fmt: off
-        # Ephoton = h*c/lambda
-        E_photon = (
-            6.63e-34 * meter2 * kgram / second
-            * 2.998e8 * meter / second
-            / self.light_model_params["wavelength"]
-        )
-        # fmt: on
-
-        light_model = Equations(
-            """
-            Irr = Irr0*T : watt/meter**2
-            Irr0 : watt/meter**2 
-            T : 1
-            phi = Irr / Ephoton : 1/second/meter**2
-            """
-        )
-
-        opto_syn = Synapses(
-            neuron_group,
-            model=mod_opsin_model + light_model,
-            namespace=mod_opsin_params,
-            name=f"synapses_{self.name}_{neuron_group.name}",
-            method="rk2",
-        )
-        opto_syn.namespace["Ephoton"] = E_photon
+    rho_rel is channel density relative to standard model fit;
+    modifying it post-injection allows for heterogeneous opsin expression.
 
-        p_expression = kwparams.get("p_expression", 1)
-        if p_expression == 1:
-            opto_syn.connect(j="i")
-        else:
-            opto_syn.connect(condition="i==j", p=p_expression)
+    IOPTO_VAR_NAME and V_VAR_NAME are substituted on injection.
+    """
 
-        self.opsin_model.init_opto_syn_vars(opto_syn)
+    Gd: Quantity = 0
+    Gr: Quantity = 0
+    ka: Quantity = 0
+    p: Quantity = 0
+    q: Quantity = 0
+    phim: Quantity = 0
+    E: Quantity = 0
+    a: Quantity = 0
+    b: Quantity = 0
+    vartheta_max = 5 * mM
+    kd = 16 * mM
+    model: str = field(
+        init=False,
+        default="""
+        dP0/dt = Gr*P6 - Ga*P0 : 1 (clock-driven)
+        dP4/dt = Ga*P0 - Gd*P4 : 1 (clock-driven)
+        P6 = 1 - P0 - P4 : 1
+
+        Theta = int(phi_pre > 0*phi_pre) : 1
+        Hp = Theta * phi_pre**p/(phi_pre**p + phim**p) : 1
+        Ga = ka*Hp : hertz
+
+        fphi = P4 : 1
+        dCl_in/dt = a*(I_i + b*I_Cl_leak) : molar
+        Cl_out : molar
+        E_Cl = -26.67*mV * log(Cl_out/Cl_in) : volt
+        I_Cl_leak = g_Cl * (E_Cl0 - E_Cl)
+
+        Psi = vartheta_max*Cl_out / (kd + Cl_out) / 4.43 : 1
+        I_i = fphi*(V_VAR_NAME_post-E)*Psi*rho_rel
+
+        IOPTO_VAR_NAME_post = -(I_i + I_Cl_leak) : ampere (summed)
+        rho_rel : 1""",
+    )
+
+    extra_namespace: dict[str, Any] = field(
+        init=False, factory=lambda: {"E_Cl0": -70 * mV, "g_Cl": 2.3 * msiemens / cm2}
+    )
 
-        # relative channel density
-        opto_syn.rho_rel = kwparams.get("rho_rel", 1)
-        # calculate transmittance coefficient for each point
-        r, z = self._get_rz_for_xyz(neuron_group.x, neuron_group.y, neuron_group.z)
-        T = self._Foutz12_transmittance(r, z).flatten()
-        assert len(T) == len(neuron_group)
-        # reduce to subset expressing opsin before assigning
-        T = T[opto_syn.i]
+    def init_opto_syn_vars(self, opto_syn: Synapses) -> None:
+        raise NotImplementedError("Still need to figure out [Cl-_out]")
+        opto_syn.P0 = 1
+        opto_syn.P4 = 0
+        opto_syn.P6 = 0
+        opto_syn.Cl_out = 124 * mM
+        opto_syn.Cl_in = np.exp(np.log(124) - 70 / 26.67) * mM
 
-        opto_syn.T = T
 
-        self.opto_syns[neuron_group.name] = opto_syn
-        self.brian_objects.add(opto_syn)
+@define(eq=False)
+class ProportionalCurrentOpsin(Opsin):
+    """A simple model delivering current proportional to light intensity"""
 
-    def add_self_to_plot(self, ax, axis_scale_unit, **kwargs) -> PathCollection:
-        # show light with point field, assigning r and z coordinates
-        # to all points
-        # filter out points with <0.001 transmittance to make plotting faster
-
-        T_threshold = kwargs.get("T_threshold", 0.001)
-        n_points = kwargs.get("n_points", 1e4)
-        intensity = kwargs.get("intensity", 0.5)
-        r_thresh, zc_thresh = self._find_rz_thresholds(T_threshold)
-        r, theta, zc = uniform_cylinder_rθz(n_points, r_thresh, zc_thresh)
-
-        T = self._Foutz12_transmittance(r, zc)
-
-        end = self.location + zc_thresh * self.dir_uvec
-        x, y, z = xyz_from_rθz(r, theta, zc, self.location, end)
-
-        idx_to_plot = T >= T_threshold
-        x = x[idx_to_plot]
-        y = y[idx_to_plot]
-        z = z[idx_to_plot]
-        T = T[idx_to_plot]
-        point_cloud = ax.scatter(
-            x / axis_scale_unit,
-            y / axis_scale_unit,
-            z / axis_scale_unit,
-            c=T,
-            cmap=self._alpha_cmap_for_wavelength(intensity),
-            marker="o",
-            edgecolors="none",
-            label=self.name,
-        )
-        with warnings.catch_warnings():
-            warnings.filterwarnings(
-                "ignore", message=".*Rasterization.*will be ignored.*"
-            )
-            # to make manageable in SVGs
-            point_cloud.set_rasterized(kwargs.get("rasterized", True))
-        handles = ax.get_legend().legendHandles
-        c = wavelength_to_rgb(self.light_model_params["wavelength"] / nmeter)
-        opto_patch = matplotlib.patches.Patch(color=c, label=self.name)
-        handles.append(opto_patch)
-        ax.legend(handles=handles)
-        return [point_cloud]
-
-    def _find_rz_thresholds(self, thresh):
-        """find r and z thresholds for visualization purposes"""
-        res_mm = 0.01
-        zc = np.arange(20, 0, -res_mm) * mm  # ascending T
-        T = self._Foutz12_transmittance(0 * mm, zc)
-        zc_thresh = zc[np.searchsorted(T, thresh)]
-        # look at half the z threshold for the r threshold
-        r = np.arange(20, 0, -res_mm) * mm
-        T = self._Foutz12_transmittance(r, zc_thresh / 2)
-        r_thresh = r[np.searchsorted(T, thresh)]
-        # multiply by 1.2 just in case
-        return r_thresh * 1.2, zc_thresh
-
-    def update_artists(
-        self, artists: list[Artist], value, *args, **kwargs
-    ) -> list[Artist]:
-        self._prev_value = getattr(self, "_prev_value", None)
-        if value == self._prev_value:
-            return []
-
-        assert len(artists) == 1
-        point_cloud = artists[0]
-
-        if self.max_Irr0_mW_per_mm2_viz is not None:
-            max_Irr0 = self.max_Irr0_mW_per_mm2_viz
-        elif self.max_Irr0_mW_per_mm2 is not None:
-            max_Irr0 = self.max_Irr0_mW_per_mm2
+    I_per_Irr: Quantity = field(kw_only=True)
+    """ How much current (in amps or unitless, depending on neuron model)
+    to deliver per mW/mm2.
+    """
+    # would be IOPTO_UNIT but that throws off Equation parsing
+    model: str = field(
+        init=False,
+        default="""
+            IOPTO_VAR_NAME_post = I_per_Irr / (mwatt / mm2) 
+                * Irr_pre * rho_rel : IOPTO_UNIT (summed)
+            rho_rel : 1
+        """,
+    )
+
+    required_vars: list[Tuple[str, Unit]] = field(factory=list, init=False)
+
+    def __attrs_post_init__(self):
+        if isinstance(self.I_per_Irr, Quantity):
+            Iopto_unit = get_unit(self.I_per_Irr.dim)
         else:
-            raise Exception(
-                f"OptogeneticIntervention '{self.name}' needs max_Irr0_mW_per_mm2_viz "
-                "or max_Irr0_mW_per_mm2 "
-                "set to visualize light intensity."
-            )
-
-        intensity = value / max_Irr0 if value <= max_Irr0 else max_Irr0
-        point_cloud.set_cmap(self._alpha_cmap_for_wavelength(intensity))
-        return [point_cloud]
-
-    def update(self, Irr0_mW_per_mm2: float):
-        """Set the light intensity, in mW/mm2 (without unit)
-
-        Parameters
-        ----------
-        Irr0_mW_per_mm2 : float
-            Desired light intensity for light source
-        """
-        if Irr0_mW_per_mm2 < 0:
-            warnings.warn(f"{self.name}: negative light intensity Irr0 clipped to 0")
-            Irr0_mW_per_mm2 = 0
-        if (
-            self.max_Irr0_mW_per_mm2 is not None
-            and Irr0_mW_per_mm2 > self.max_Irr0_mW_per_mm2
-        ):
-            Irr0_mW_per_mm2 = self.max_Irr0_mW_per_mm2
-        super().update(Irr0_mW_per_mm2)
-        for opto_syn in self.opto_syns.values():
-            opto_syn.Irr0 = Irr0_mW_per_mm2 * mwatt / mm2
-
-    def reset(self, **kwargs):
-        for opto_syn in self.opto_syns.values():
-            self.opsin_model.init_opto_syn_vars(opto_syn)
-
-    def _alpha_cmap_for_wavelength(self, intensity=0.5):
-        c = wavelength_to_rgb(self.light_model_params["wavelength"] / nmeter)
-        c_clear = (*c, 0)
-        c_opaque = (*c, 0.6 * intensity)
-        return colors.LinearSegmentedColormap.from_list(
-            "incr_alpha", [(0, c_clear), (1, c_opaque)]
-        )
+            Iopto_unit = radian
+        self.per_ng_unit_replacements = [("IOPTO_UNIT", Iopto_unit.name)]
+        self.required_vars = [("Iopto", Iopto_unit)]
```

### Comparing `cleosim-0.8.0/cleo/recorders.py` & `cleosim-0.9.0/cleo/recorders.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 """Contains basic recorders."""
 from typing import Any
-from brian2 import PopulationRateMonitor, StateMonitor, SpikeMonitor, Quantity
+from attrs import define, field
+from brian2 import (
+    PopulationRateMonitor,
+    StateMonitor,
+    SpikeMonitor,
+    Quantity,
+    NeuronGroup,
+)
 import numpy as np
 from nptyping import NDArray
 
 from cleo.base import Recorder
 
 
+@define(eq=False)
 class RateRecorder(Recorder):
     """Records firing rate from a single neuron.
 
-    Firing rate comes from Brian's :class:`~brian2.monitors.ratemonitor.PopulationRateMonitor`"""
+    Firing rate comes from Brian's :class:`~brian2.monitors.ratemonitor.PopulationRateMonitor`
+    """
 
-    def __init__(self, name: str, index: int):
-        """
-        Parameters
-        ----------
-        name : str
-            Unique device name
-        index : int
-            index of neuron to record
-        """
-        super().__init__(name)
-        self.i = index
-        self.mon = None
+    i: int
+    """index of neuron to record"""
+
+    mon: PopulationRateMonitor = field(init=False)
 
     def connect_to_neuron_group(self, neuron_group):
         self.mon = PopulationRateMonitor(neuron_group[self.i])
         self.brian_objects.add(self.mon)
 
     def get_state(self):
         try:
             return self.mon.rate[-1]
         except IndexError:
             return 0
 
 
+@define(eq=False)
 class VoltageRecorder(Recorder):
     """Records the voltage of a single neuron group."""
 
-    def __init__(self, name: str, voltage_var_name: str = "v"):
-        """
-        Parameters
-        ----------
-        name : str
-            Unique device name
-        voltage_var_name : str, optional
-            Name of variable representing membrane voltage, by default "v"
-        """
-        super().__init__(name)
-        self.voltage_var_name = voltage_var_name
-        self.mon = None
+    voltage_var_name: str = "v"
+    """Name of variable representing membrane voltage"""
+
+    mon: StateMonitor = field(init=False, default=None)
 
     def connect_to_neuron_group(self, neuron_group):
         if self.mon is not None:
             raise UserWarning(
                 "Recorder was already connected to a neuron group. "
                 "Can only record from one at a time."
             )
@@ -70,46 +64,46 @@
         """
         try:
             return self.mon.v[:, -1]
         except IndexError:
             return None
 
 
+@define(eq=False)
 class GroundTruthSpikeRecorder(Recorder):
     """Reports the number of spikes seen since last queried for each neuron.
 
     This amounts effectively to the number of spikes per control period.
     Note: this will only work for one neuron group at the moment.
     """
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.mon = None
-        self.num_spikes_seen = 0
+    _mon: SpikeMonitor = field(init=False, default=None)
+
+    _num_spikes_seen: int = field(init=False, default=0)
+
+    neuron_group: NeuronGroup = field(init=False, default=None)
 
     def connect_to_neuron_group(self, neuron_group):
-        if self.mon is not None:
+        if self._mon is not None:
             raise UserWarning(
                 "Recorder was already connected to a neuron group. "
                 "Can only record from one at a time."
             )
-        self.mon = SpikeMonitor(neuron_group)
-        self.brian_objects.add(self.mon)
-        self.out_template = np.zeros(len(neuron_group))
+        self._mon = SpikeMonitor(neuron_group)
+        self.brian_objects.add(self._mon)
+        self.neuron_group = neuron_group
 
     def get_state(self) -> NDArray[(Any,), np.uint]:
         """
         Returns
         -------
         NDArray[(n_neurons,), np.uint]
             n_neurons-length array with spike counts over the latest
             control period.
         """
-        num_new_spikes = len(self.mon.t) - self.num_spikes_seen
-        self.num_spikes_seen += num_new_spikes
-        if len(self.out_template) == 1:
-            out = np.array([num_new_spikes])
-        else:
-            out = self.out_template.copy()
-            for spike_i in self.mon.i[-num_new_spikes:]:
+        num_new_spikes = len(self._mon.t) - self._num_spikes_seen
+        self._num_spikes_seen += num_new_spikes
+        out = np.zeros(len(self.neuron_group), dtype=np.uint)
+        if num_new_spikes > 0:
+            for spike_i in self._mon.i[-num_new_spikes:]:
                 out[spike_i] += 1
         return out
```

### Comparing `cleosim-0.8.0/cleo/utilities.py` & `cleosim-0.9.0/cleo/utilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,114 @@
 """Assorted utilities for developers."""
 from collections.abc import MutableMapping
 from math import ceil, floor
 
-from scipy import linalg
+# from scipy import linalg
 import numpy as np
 from matplotlib import pyplot as plt
 
-from brian2 import second
+from brian2 import second, meter, NeuronGroup, Quantity
 from brian2.groups.group import get_dtype
 from brian2.equations.equations import (
     Equations,
     DIFFERENTIAL_EQUATION,
     SUBEXPRESSION,
     PARAMETER,
 )
+import neo
+import quantities as pq
 
 
-def get_orth_vectors_for_v(v):
-    """Returns w1, w2 as 1x3 row vectors"""
-    q, r = linalg.qr(
-        np.column_stack([v, v, v])
-    )  # get two vectors orthogonal to v from QR decomp
-    return q[:, 1], q[:, 2]
+def times_are_regular(times):
+    if len(times) < 2:
+        return False
+    return np.allclose(np.diff(times), times[1] - times[0])
+
+
+def analog_signal(t_ms, values_no_unit, units) -> neo.core.basesignal.BaseSignal:
+    if times_are_regular(t_ms):
+        return neo.AnalogSignal(
+            values_no_unit,
+            t_start=t_ms[0] * pq.ms,
+            units=units,
+            sampling_period=(t_ms[1] - t_ms[0]) * pq.ms,
+        )
+    else:
+        return neo.IrregularlySampledSignal(
+            t_ms * pq.ms,
+            values_no_unit,
+            units=units,
+        )
+
+
+def add_to_neo_segment(
+    segment: neo.core.Segment, *objects: neo.core.dataobject.DataObject
+):
+    """Taken from neo.core.group.Group."""
+    container_lookup = {
+        cls_name: getattr(segment, container_name)
+        for cls_name, container_name in zip(
+            segment._child_objects, segment._child_containers
+        )
+    }
+
+    for obj in objects:
+        cls = obj.__class__
+        if hasattr(cls, "proxy_for"):
+            cls = cls.proxy_for
+        container = container_lookup[cls.__name__]
+        container.append(obj)
+
+
+def normalize_coords(coords: Quantity) -> Quantity:
+    """Normalize coordinates to unit vectors."""
+    return coords / np.linalg.norm(coords, axis=-1, keepdims=True)
+
+
+def get_orth_vectors_for_V(V):
+    """For nx3 block of row vectors V, return nx3 W1, W2 orthogonal
+    vector blocks"""
+    V = V.reshape((-1, 3, 1))
+    n = V.shape[0]
+    V = np.repeat(V, 3, axis=-1)
+    assert V.shape == (n, 3, 3)
+    q, r = np.linalg.qr(V)
+    # get two vectors orthogonal to v from QR decomp
+    W1, W2 = q[..., 1], q[..., 2]
+    assert W1.shape == W2.shape == (n, 3)
+    return W1.squeeze(), W2.squeeze()
 
 
 def xyz_from_rθz(rs, thetas, zs, xyz_start, xyz_end):
     """Convert from cylindrical to Cartesian coordinates."""
     # not using np.linalg.norm because it strips units
     cyl_length = np.sqrt(np.sum(np.subtract(xyz_end, xyz_start) ** 2))
     c = (xyz_end - xyz_start) / cyl_length  # unit vector in direction of cylinder
+    m = xyz_start.reshape((-1, 3)).shape[0]
+    n = len(rs)
 
-    r1, r2 = get_orth_vectors_for_v(c)
+    r1, r2 = get_orth_vectors_for_V(c)
 
     def r_unit_vecs(thetas):
         cosines = np.reshape(np.cos(thetas), (len(thetas), 1))
         sines = np.reshape(np.sin(thetas), (len(thetas), 1))
         # add axis for broadcasting so result is nx3
         cosines = np.cos(thetas)[..., np.newaxis]
         sines = np.sin(thetas)[..., np.newaxis]
-        return r1 * cosines + r2 * sines
+        return r1.reshape((m, 1, 3)) * cosines + r2.reshape((m, 1, 3)) * sines
 
     coords = (
-        xyz_start + c * zs[..., np.newaxis] + rs[..., np.newaxis] * r_unit_vecs(thetas)
+        xyz_start.reshape((m, 1, 3))
+        + c.reshape((m, 1, 3)) * zs.reshape((1, n, 1))
+        + rs.reshape((1, n, 1)) * r_unit_vecs(thetas)
     )
-    return coords[:, 0], coords[:, 1], coords[:, 2]
+    assert coords.shape == (m, n, 3)
+    return coords[..., 0], coords[..., 1], coords[..., 2]
+    # coords = coords.reshape((m * n), 3)
+    # return coords[:, 0], coords[:, 1], coords[:, 2]
 
 
 def uniform_cylinder_rθz(n, rmax, zmax):
     # generate Fibonacci spiral cylinder by rotating around axis
     # and up and down cylinder simultaneously, using different angles
     indices = np.arange(0, n) + 0.5
     rs = rmax * np.sqrt(indices / n)
@@ -114,18 +175,24 @@
         for eq in neuron_group.equations.values():
             if eq.type == DIFFERENTIAL_EQUATION and "unless refractory" in eq.flags:
                 not_refractory_var = neuron_group.variables["not_refractory"]
                 var = neuron_group.variables[eq.varname]
                 var.set_conditional_write(not_refractory_var)
 
     # Stochastic variables
-    for xi in neuron_group.equations.stochastic_variables:
-        neuron_group.variables.add_auxiliary_variable(
-            xi, dimensions=(second**-0.5).dim
-        )
+    for xi in eqs_to_add.stochastic_variables:
+        try:
+            neuron_group.variables.add_auxiliary_variable(
+                xi, dimensions=(second**-0.5).dim
+            )
+        except KeyError as ex:
+            warnings.warn(
+                "Adding a stochastic variable to a neuron group that already"
+                " has a variable with the same name."
+            )
 
     # Check scalar subexpressions
     for eq in neuron_group.equations.values():
         if eq.type == SUBEXPRESSION and "shared" in eq.flags:
             var = neuron_group.variables[eq.varname]
             for identifier in var.identifiers:
                 if identifier in neuron_group.variables:
@@ -183,18 +250,21 @@
     else:
         R = 0.0
         G = 0.0
         B = 0.0
     return (R, G, B)
 
 
-def style_plots_for_docs():
+def style_plots_for_docs(dark=True):
     # some hacky workaround for params not being updated until after first plot
     f = plt.figure()
     plt.plot()
     plt.close(f)
 
-    plt.style.use("dark_background")
+    if dark:
+        plt.style.use("dark_background")
+        for obj in ["figure", "axes", "savefig"]:
+            plt.rc(obj, facecolor="131416")  # color of Furo dark background
+    else:
+        plt.style.use("default")
     plt.rc("savefig", transparent=False)
-    for obj in ["figure", "axes", "savefig"]:
-        plt.rc(obj, facecolor="131416")  # color of Furo dark background
     plt.rc("axes.spines", top=False, right=False)
```

### Comparing `cleosim-0.8.0/cleo/viz.py` & `cleosim-0.9.0/cleo/viz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 """Tools for visualizing models and simulations"""
 from __future__ import annotations
 from typing import Tuple, Any, Union
 from collections.abc import Iterable
-from matplotlib.artist import Artist
 
+from attrs import define, field
+from matplotlib.artist import Artist
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.animation as anim
 from mpl_toolkits.mplot3d import Axes3D
 from brian2 import mm, Unit, NeuronGroup, ms, NetworkOperation, Quantity, SpikeMonitor
 
 from cleo.base import CLSimulator, InterfaceDevice
 
 _neuron_alpha = 0.2
 
 
+@define(eq=False)
 class VideoVisualizer(InterfaceDevice):
     """Device for visualizing a simulation.
 
     Must be injected after all other devices and before the simulation
     is run."""
 
-    def __init__(
-        self,
-        devices: Iterable[Union[InterfaceDevice, Tuple[InterfaceDevice, dict]]] = "all",
-        dt: Quantity = 1 * ms,
-    ) -> None:
-        """
-        Parameters
-        ----------
-        devices : Iterable[Union[InterfaceDevice, Tuple[InterfaceDevice, dict]]], optional
-            list of devices or (device, vis_kwargs) tuples to include in the plot,
-            just as in the :func:`plot` function, by default "all", which will
-            include all recorders and stimulators currently injected when this
-            visualizer is injected into the simulator.
-        dt : Brian 2 temporal Quantity, optional
-            length of each frame---that is, every `dt` the visualizer takes a
-            snapshot of the network, by default 1*ms
-        """
-        super().__init__("video_visualizer")
-        self.neuron_groups = []
-        self._spike_mons = []
-        self._num_old_spikes = []
-        self.devices = devices
-        self.dt = dt
-        # store data to generate video
-        self._value_per_device_per_frame = []
-        self._i_spikes_per_ng_per_frame: list[list[np.ndarray]] = []
+    devices: Iterable[Union[InterfaceDevice, Tuple[InterfaceDevice, dict]]] = field(
+        factory=list
+    )
+    """list of devices or (device, vis_kwargs) tuples to include in the plot,
+    just as in the :func:`plot` function, by default "all", which will
+    include all recorders and stimulators currently injected when this
+    visualizer is injected into the simulator.
+    """
+
+    dt: Quantity = 1 * ms
+    """length of each frame---that is, every ``dt`` the visualizer takes a
+    snapshot of the network, by default 1*ms
+    """
+
+    fig: plt.Figure = field(init=False, default=None)
+
+    ax: plt.Axes = field(init=False, default=None)
+
+    neuron_groups: list[NeuronGroup] = field(init=False, factory=list)
+
+    _spike_mons: list[SpikeMonitor] = field(init=False, factory=list)
+
+    _num_old_spikes: list[int] = field(init=False, factory=list)
+
+    _value_per_device_per_frame: list[list[Any]] = field(init=False, factory=list)
+
+    _i_spikes_per_ng_per_frame: list[list[np.ndarray]] = field(init=False, factory=list)
 
     def init_for_simulator(self, simulator: CLSimulator):
         if self.devices == "all":
             self.devices = list(self.sim.recorders.values())
             self.devices.extend(list(self.sim.stimulators.values()))
+
         # network op
         def snapshot(t):
             i_spikes_per_ng = [
                 self._new_spikes_for_ng(i_ng) for i_ng in range(len(self.neuron_groups))
             ]
             self._i_spikes_per_ng_per_frame.append(i_spikes_per_ng)
             device_values = []
@@ -107,19 +111,22 @@
             self.ax,
             self.neuron_groups,
             devices=self.devices,
             **plotargs,
         )
 
         def update(i):
+            prev_device_values = self._value_per_device_per_frame[i - 1]
             device_values = self._value_per_device_per_frame[i]
             updated_artists = []
-            for device, artists, value in zip(
-                self.devices, device_artists, device_values
+            for device, artists, value, prev_value in zip(
+                self.devices, device_artists, device_values, prev_device_values
             ):
+                if np.allclose(value, prev_value):
+                    continue
                 updated_artists_for_device = device.update_artists(artists, value)
                 updated_artists.extend(updated_artists_for_device)
             self._update_neuron_artists_for_frame(neuron_artists, i)
             return updated_artists + neuron_artists
 
         return anim.FuncAnimation(
             self.fig,
@@ -227,14 +234,15 @@
     ylim: Tuple[float, float] = None,
     zlim: Tuple[float, float] = None,
     colors: Iterable = None,
     axis_scale_unit: Unit = mm,
     devices: Iterable[Union[InterfaceDevice, Tuple[InterfaceDevice, dict]]] = [],
     invert_z: bool = True,
     scatterargs: dict = {},
+    sim: CLSimulator = None,
     **figargs: Any,
 ) -> None:
     """Visualize neurons and interface devices
 
     Parameters
     ----------
     xlim : Tuple[float, float], optional
@@ -252,24 +260,35 @@
         :meth:`~cleo.InterfaceDevice.add_self_to_plot` is called
         for each, using the kwargs dict if given. By default []
     invert_z : bool, optional
         whether to invert z-axis, by default True to reflect the convention
         that +z represents depth from cortex surface
     scatterargs : dict, optional
         arguments passed to plt.scatter() for each neuron group, such as marker
+    sim: CLSimulator, optional
+        Optional shortcut to include all neuron groups and devices
     **figargs : Any, optional
         keyword arguments passed to plt.figure(), such as figsize
 
     Raises
     ------
     ValueError
         When neuron group doesn't have x, y, and z already defined
     """
     fig = plt.figure(**figargs)
     ax = fig.add_subplot(111, projection="3d")
+    if sim is not None:
+        if len(neuron_groups) == 0:
+            for obj in sim.network.objects:
+                neuron_groups = []
+                if type(obj) == NeuronGroup:
+                    neuron_groups.append(obj)
+        if len(devices) == 0:
+            devices = sim.devices
+
     _plot(
         ax,
         neuron_groups,
         xlim,
         ylim,
         zlim,
         colors,
```

### Comparing `cleosim-0.8.0/pyproject.toml` & `cleosim-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 [tool.poetry]
 name = "cleosim"
-version = "0.8.0"
+version = "0.9.0"
 description = "Cleo: the Closed-Loop, Electrophysiology, and Optogenetics experiment simulation testbed"
 authors = [
     "Kyle Johnsen <kyle@kjohnsen.org>",
     "Nathan Cruzado <ncruzado3@gatech.edu>",
 ]
 license = "MIT"
 homepage = "https://cleosim.readthedocs.io"
 repository = "https://github.com/Sensory-Information-Processing-Lab/Cleo"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
 ]
-packages = [
-    { include = "cleo" },
-]
+packages = [{ include = "cleo" }]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.10"
+python = ">=3.8,<=3.11"
 brian2 = "^2.4, !=2.5.0.2"
 matplotlib = "^3.4"
 numpy = "^1.16"
 scipy = "^1.7.2"
 tklfp = "^0.2"
 bidict = "*"
 nptyping = "^1.4.4"
+attrs = "^21.0"
+neo = "^0.12.0"
 
 [tool.poetry.dev-dependencies]
-black = "^21.12b0"
+black = "^23.0"
 flake8 = "^4.0.1"
-pytest = "^6.2.5"
+pytest = "^7.0.0"
 pytest-flake8 = "^1.0.7"
 pep8-naming = "^0.12.1"
 flake8-docstrings = "^1.6.0"
 flake8-pytest-style = "^1.6.0"
 nbmake = "^1.2"
 Sphinx = "^4.0"
 sphinx-copybutton = "^0.4.0"
 myst-nb = "^0.13.1"
 sphinx-favicon = "^0.2"
 furo = "^2022.6.21"
+nbdev = "^2.3.12"
+elephant = "^0.13.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
     # "--doctest-modules",
     "--nbmake",
     # "--flake8",
     # will want to call this on CI where ldsctrlest is not installed
     # "--ignore=examples/adaptive_ctrl_ldsctrlest.ipynb"
     # "--ignore=docs/tutorials/video_visualization.ipynb"
 ]
-markers = [
-    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
-]
-testpaths = [
-    "tests",
-    "docs/tutorials",
-]
+markers = ["slow: marks tests as slow (deselect with '-m \"not slow\"')"]
+testpaths = ["tests", "docs/tutorials"]
```

### Comparing `cleosim-0.8.0/setup.py` & `cleosim-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['cleo', 'cleo.ephys', 'cleo.ioproc']
+['cleo', 'cleo.ephys', 'cleo.ioproc', 'cleo.opto']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bidict',
+['attrs>=21.0,<22.0',
+ 'bidict',
  'brian2>=2.4,<3.0,!=2.5.0.2',
  'matplotlib>=3.4,<4.0',
+ 'neo>=0.12.0,<0.13.0',
  'nptyping>=1.4.4,<2.0.0',
  'numpy>=1.16,<2.0',
  'scipy>=1.7.2,<2.0.0',
  'tklfp>=0.2,<0.3']
 
 setup_kwargs = {
     'name': 'cleosim',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Cleo: the Closed-Loop, Electrophysiology, and Optogenetics experiment simulation testbed',
     'long_description': '###### Cleo: the Closed-Loop, Electrophysiology, and Optogenetics experiment simulation testbed\n[![Test and lint](https://github.com/kjohnsen/cleosim/actions/workflows/test.yml/badge.svg)](https://github.com/kjohnsen/cleosim/actions/workflows/test.yml)\n[![Documentation Status](https://readthedocs.org/projects/cleosim/badge/?version=latest)](https://cleosim.readthedocs.io/en/latest/?badge=latest)\n\n\n<h1>\n<p align="center">\n  <img \n      style="display: block; \n             width: 50%;"\n      src="https://user-images.githubusercontent.com/19983357/187561700-100b853a-d226-4039-a580-1d798b00f9e4.png" \n      alt="Cleo: the Closed-Loop, Electrophysiology, and Optogenetics experiment simulation testbed">\n  </img>\n</p>\n</h1>\n\n\nHello there! Cleo has the goal of bridging theory and experiment for mesoscale neuroscience, facilitating electrode recording, optogenetic stimulation, and closed-loop experiments (e.g., real-time input and output processing) with the [Brian 2](https://brian2.readthedocs.io/en/stable/) spiking neural network simulator. We hope users will find these components useful for prototyping experiments, innovating methods, and testing observations about a hypotheses *in silico*, incorporating into spiking neural network models laboratory techniques ranging from passive observation to complex model-based feedback control. Cleo also serves as an extensible, modular base for developing additional recording and stimulation modules for Brian simulations.\n\nThis package was developed by [Kyle Johnsen](https://kjohnsen.org) and Nathan Cruzado under the direction of [Chris Rozell](https://siplab.gatech.edu) at Georgia Institute of Technology.\n\n<p align="center">\n  <img \n      style="display: block; \n             width: 90%;"\n      src="https://user-images.githubusercontent.com/19983357/187724696-b880a884-1c32-4bad-8b2c-acdd4add44d0.png" \n      alt="logo">\n  </img>\n</p>\n\n## <img align="bottom" src="https://user-images.githubusercontent.com/19983357/167456512-fb10619b-255e-4a53-8ed9-79ae954d3ff4.png" alt="CL icon" > Closed Loop processing\nCleo allows for flexible I/O processing in real time, enabling the simulation of closed-loop experiments such as event-triggered or feedback control. The user can also add latency to closed-loop stimulation to study the effects of computation delays.\n\n\n## <img align="bottom" src="https://user-images.githubusercontent.com/19983357/167461111-b0a3746c-03fa-47b7-a9a9-7b651157044f.png" alt="CL icon" > Electrode recording\nCleo provides functions for configuring electrode arrays and placing them in arbitrary locations in the simulation. The user can then specify parameters for probabilistic spike detection or a spike-based LFP approximation developed by [Teleńczuk et al., 2020](https://www.sciencedirect.com/science/article/pii/S0165027020302946).\n\n## <img align="bottom" src="https://user-images.githubusercontent.com/19983357/187728089-62fae854-1d69-4e8f-a597-a25934ca3eaa.png" alt="CL icon" > Optogenetic stimulation\nBy providing an optic fiber-light propagation model, Cleo enables users to flexibly add photostimulation to their model. Both a four-state Markov state model of opsin dynamics is available, as well as a minimal proportional current option for compatibility with simple neuron models. Parameters are provided for the common blue light/ChR2 setup.\n\n## Getting started\nJust use pip to install&mdash;the name on PyPI is `cleosim`:\n```\npip install cleosim\n```\n\nThen head to the [overview section of the documentation](https://cleosim.readthedocs.io/en/latest/overview.html) for a more detailed discussion of motivation, structure, and basic usage.\n\n## Related resources\nThose using Cleo to simulate closed-loop control experiments may be interested in software developed for the execution of real-time, *in-vivo* experiments. Developed by members of [Chris Rozell](https://siplab.gatech.edu)\'s and [Garrett Stanley](https://stanley.gatech.edu/)\'s labs at Georgia Tech, the [CLOCTools repository](https://cloctools.github.io) can serve these users in two ways:\n\n1. By providing utilities and interfaces with experimental platforms for moving from simulation to reality.\n2. By providing performant control and estimation algorithms for feedback control. Although Cleo enables closed-loop manipulation of network simulations, it does not include any advanced control algorithms itself. The `ldsCtrlEst` library implements adaptive linear dynamical system-based control while the `hmm` library can generate and decode systems with discrete latent states and observations.\n\n<p align="center">\n  <img \n      style="display: block; \n             width: 100%;"\n      src="https://user-images.githubusercontent.com/19983357/187723498-f0f03da8-096a-46eb-90df-28da55dce7a0.png" \n      alt="CLOCTools and Cleo">\n  </img>\n</p>\n\n### Publications\n[**CLOC Tools: A Library of Tools for Closed-Loop Neuroscience**](https://github.com/cloctools/tools-for-neuro-control-manuscript)<br>\nA.A. Willats, M.F. Bolus, K.A. Johnsen, G.B. Stanley, and C.J. Rozell. *In prep*, 2022.\n\n[**State-Aware Control of Switching Neural Dynamics**](https://github.com/awillats/state-aware-control)<br>\nA.A. Willats, M.F. Bolus, C.J. Whitmire, G.B. Stanley, and C.J. Rozell. *In prep*, 2022.\n\n[**Closed-Loop Identifiability in Neural Circuits**](https://github.com/awillats/clinc)<br>\nA. Willats, M. O\'Shaughnessy, and C. Rozell. *In prep*, 2022.\n\n[**State-space optimal feedback control of optogenetically driven neural activity**](https://www.biorxiv.org/content/10.1101/2020.06.25.171785v2)<br>\nM.F. Bolus, A.A. Willats, C.J. Rozell and G.B. Stanley. *Journal of Neural Engineering*, 18(3), pp. 036006, March 2021.\n\n[**Design strategies for dynamic closed-loop optogenetic neurocontrol in vivo**](https://iopscience.iop.org/article/10.1088/1741-2552/aaa506)<br>\nM.F. Bolus, A.A. Willats, C.J. Whitmire, C.J. Rozell and G.B. Stanley. *Journal of Neural Engineering*, 15(2), pp. 026011, January 2018.\n',
     'author': 'Kyle Johnsen',
     'author_email': 'kyle@kjohnsen.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://cleosim.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.10',
+    'python_requires': '>=3.8,<=3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `cleosim-0.8.0/PKG-INFO` & `cleosim-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: cleosim
-Version: 0.8.0
+Version: 0.9.0
 Summary: Cleo: the Closed-Loop, Electrophysiology, and Optogenetics experiment simulation testbed
 Home-page: https://cleosim.readthedocs.io
 License: MIT
 Author: Kyle Johnsen
 Author-email: kyle@kjohnsen.org
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.8,<=3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: attrs (>=21.0,<22.0)
 Requires-Dist: bidict
 Requires-Dist: brian2 (>=2.4,<3.0,!=2.5.0.2)
 Requires-Dist: matplotlib (>=3.4,<4.0)
+Requires-Dist: neo (>=0.12.0,<0.13.0)
 Requires-Dist: nptyping (>=1.4.4,<2.0.0)
 Requires-Dist: numpy (>=1.16,<2.0)
 Requires-Dist: scipy (>=1.7.2,<2.0.0)
 Requires-Dist: tklfp (>=0.2,<0.3)
 Project-URL: Repository, https://github.com/Sensory-Information-Processing-Lab/Cleo
 Description-Content-Type: text/markdown
```

