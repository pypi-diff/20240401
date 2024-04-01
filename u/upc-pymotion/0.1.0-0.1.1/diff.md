# Comparing `tmp/upc_pymotion-0.1.0.tar.gz` & `tmp/upc_pymotion-0.1.1.tar.gz`

## Comparing `upc_pymotion-0.1.0.tar` & `upc_pymotion-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/io/__init__.py
--rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/io/bvh.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/ops/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/ops/forward_kinematics.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/ops/forward_kinematics_torch.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/ops/skeleton.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/ops/skeleton_torch.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/ops/time.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/ops/time_torch.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/render/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/render/blender.py
--rw-r--r--   0        0        0    14468 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/render/viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/rotations/__init__.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/rotations/dual_quat.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/rotations/dual_quat_torch.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/rotations/ortho6d.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/rotations/ortho6d_torch.py
--rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/rotations/quat.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pymotion/rotations/quat_torch.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/LICENSE
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/io/__init__.py
+-rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/io/bvh.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/forward_kinematics.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/forward_kinematics_torch.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/skeleton.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/skeleton_torch.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/time.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/time_torch.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/render/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/render/blender.py
+-rw-r--r--   0        0        0    19612 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/render/viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/__init__.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/dual_quat.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/dual_quat_torch.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/ortho6d.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/ortho6d_torch.py
+-rw-r--r--   0        0        0    14636 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/quat.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/quat_torch.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/PKG-INFO
```

### Comparing `upc_pymotion-0.1.0/pymotion/io/bvh.py` & `upc_pymotion-0.1.1/pymotion/io/bvh.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/ops/forward_kinematics.py` & `upc_pymotion-0.1.1/pymotion/ops/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/ops/forward_kinematics_torch.py` & `upc_pymotion-0.1.1/pymotion/ops/forward_kinematics_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/ops/skeleton.py` & `upc_pymotion-0.1.1/pymotion/ops/skeleton.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/ops/skeleton_torch.py` & `upc_pymotion-0.1.1/pymotion/ops/skeleton_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/ops/time.py` & `upc_pymotion-0.1.1/pymotion/ops/time.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/ops/time_torch.py` & `upc_pymotion-0.1.1/pymotion/ops/time_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/render/__init__.py` & `upc_pymotion-0.1.1/pymotion/render/__init__.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/render/blender.py` & `upc_pymotion-0.1.1/pymotion/render/blender.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/render/viewer.py` & `upc_pymotion-0.1.1/pymotion/render/viewer.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,45 +3,77 @@
 from dash import Dash, html, dcc, callback, ctx, Output, Input
 import dash_bootstrap_components as dbc
 import webbrowser
 import os
 
 
 class Viewer:
-    def __init__(self, xy_size=2, z_size=2, use_reloader=False) -> None:
+    """
+    Class to represent a 3D motion visualization tool using Plotly and Dash.
+    """
+
+    def __init__(self, xy_size: float = 2, z_size: float = 2, use_reloader: bool = False) -> None:
+        """
+        Initializes the Viewer.
+
+        Args:
+            xy_size (float): Size of the viewer in the X and Y dimensions. Defaults to 2.
+            z_size (float): Size of the viewer in the Z dimension. Defaults to 2.
+            use_reloader (bool): Whether to use automatic reloading for development. Defaults to False.
+        """
         self.app = Dash(__name__, external_stylesheets=[dbc.themes.BOOTSTRAP])
         self.static_objs = []  # Array of Plotly Objects
         self.dynamic_data = {
             "skeleton": [],
             "sphere": [],
             "line": [],
         }  # Keys: Type, Value: dict with parameters + NumPy Array [frames, ...]
         self.xy_size = xy_size
         self.z_size = z_size
         self.use_reloader = use_reloader
         self._set_max_frames(0)
         self._set_up_callbacks()
 
-    def run(self):
+    def run(self) -> None:
+        """
+        Runs the Dash application to start the viewer.
+        """
+
+        # Check for debugging environment to avoid duplicated browser tabs
         if not os.environ.get("WERKZEUG_RUN_MAIN"):
             webbrowser.open_new("http://localhost:8050")
         self.app.run_server(debug=True, use_reloader=self.use_reloader)
 
     def add_skeleton(
         self,
-        data,
-        parents,
-        color="red",
-        sphere_mode="scatter",
-        scatter_size=3.0,
-        line_width=2.0,
-        radius_joints=0.025,
-        resolution=np.pi / 8,
-    ):
-        assert data.ndim == 3 or data.ndim == 2, "'data' must have shape [frames, joints, 3] or [joints, 3]"
+        data: np.ndarray,
+        parents: np.ndarray,
+        color: str = "red",
+        sphere_mode: str = "scatter",
+        scatter_size: float = 3.0,
+        line_width: float = 2.0,
+        radius_joints: float = 0.025,
+        resolution: float = np.pi / 8,
+    ) -> None:
+        """
+        Adds a skeleton to the viewer.
+
+        Args:
+            data (np.ndarray): NumPy array of shape [frames, joints, 3] or [joints, 3] containing joint positions.
+            parents (np.ndarray): NumPy array indicating the parent joint for each joint, enabling line connections.
+            color (str): Color of the skeleton elements. Defaults to "red".
+            sphere_mode (str): 'scatter' for a point cloud representation, or 'mesh' for a 3D mesh sphere. Defaults to 'scatter'.
+            scatter_size (float): Size of scatter markers if 'sphere_mode' is 'scatter'. Defaults to 3.0.
+            line_width (float): Width of the lines connecting skeleton joints. Defaults to 2.0.
+            radius_joints (float): Radius of joints if represented as spheres ('mesh' mode). Defaults to 0.025.
+            resolution (float): Angular resolution for sphere meshes (`mesh` mode). Defaults to np.pi/8.
+        """
+
+        assert data.ndim in (2, 3), "'data' must have shape [frames, joints, 3] or [joints, 3]"
+
         if data.ndim == 2 or data.shape[0] == 1:
             self.static_objs.extend(
                 _create_skeleton(
                     data if data.ndim == 2 else data[0],
                     parents,
                     color=color,
                     sphere_mode=sphere_mode,
@@ -63,18 +95,37 @@
                     "radius_joints": radius_joints,
                     "resolution": resolution,
                 }
             )
             self._set_max_frames(max(self.max_frames, data.shape[0]))
 
     def add_sphere(
-        self, center, sphere_mode="scatter", scatter_size=3.0, radius=1, color="red", resolution=np.pi / 8
-    ):
-        assert sphere_mode == "scatter" or sphere_mode == "mesh", "'sphere_mode' must be 'scatter' or 'mesh'"
-        assert center.ndim == 2 or center.ndim == 1, "'center' must have shape [frames, 3] or [3]"
+        self,
+        center: np.ndarray,
+        sphere_mode: str = "scatter",
+        scatter_size: float = 3.0,
+        radius: float = 1,
+        color: str = "red",
+        resolution: float = np.pi / 8,
+    ) -> None:
+        """
+        Adds a sphere to the viewer.
+
+        Args:
+            center (np.ndarray): NumPy array of shape [frames, 3] or [3] specifying the sphere's center coordinates.
+            sphere_mode (str): 'scatter' for a point cloud representation, or 'mesh' for a 3D mesh sphere. Defaults to 'scatter'.
+            scatter_size (float): Size of points if 'sphere_mode' is 'scatter'. Defaults to 3.0.
+            radius (float): Radius of the sphere if 'sphere_mode' is 'mesh'. Defaults to 1.
+            color (str): Color of the sphere. Defaults to 'red'.
+            resolution (float): Angular resolution for creating the sphere mesh in 'mesh' mode. Defaults to np.pi/8.
+        """
+
+        assert sphere_mode in ("scatter", "mesh"), "'sphere_mode' must be 'scatter' or 'mesh'"
+        assert center.ndim in (1, 2), "'center' must have shape [frames, 3] or [3]"
+
         if center.ndim == 1 or center.shape[0] == 1:
             if sphere_mode == "scatter":
                 self.static_objs.append(
                     go.Scatter3d(
                         x=[center[0]],
                         y=[center[1]],
                         z=[center[2]],
@@ -93,18 +144,31 @@
                     "radius": radius,
                     "color": color,
                     "resolution": resolution,
                 }
             )
             self._set_max_frames(max(self.max_frames, center.shape[0]))
 
-    def add_line(self, start, end, color="red", line_width=2.0):
-        assert start.ndim == 2 or start.ndim == 1, "'start' must have shape [frames, 3] or [3]"
-        assert end.ndim == 2 or end.ndim == 1, "'end' must have shape [frames, 3] or [3]"
+    def add_line(
+        self, start: np.ndarray, end: np.ndarray, color: str = "red", line_width: float = 2.0
+    ) -> None:
+        """
+        Adds a line to the viewer.
+
+        Args:
+            start (np.ndarray): NumPy array of shape [frames, 3] or [3] for the starting coordinates of the line.
+            end (np.ndarray): NumPy array of shape [frames, 3] or [3] for the ending coordinates of the line.
+            color (str): Color of the line. Defaults to 'red'.
+            line_width (float): Width of the line. Defaults to 2.0.
+        """
+
+        assert start.ndim in (1, 2), "'start' must have shape [frames, 3] or [3]"
+        assert end.ndim in (1, 2), "'end' must have shape [frames, 3] or [3]"
         assert start.ndim == end.ndim, "'start' and 'end' must have the same number of dimensions"
+
         if start.ndim == 1 or start.shape[0] == 1:
             self.static_objs.append(
                 go.Scatter3d(
                     x=[start[0], end[0]],
                     y=[start[1], end[1]],
                     z=[start[2], end[2]],
                     mode="lines",
@@ -118,22 +182,42 @@
                     "end": end,
                     "color": color,
                     "line_width": line_width,
                 }
             )
             self._set_max_frames(max(self.max_frames, start.shape[0]))
 
-    def add_floor(self, height=0, size=2, step=0.2, colors=["lightgrey", "darkgrey"]):
+    def add_floor(
+        self, height: float = 0, size: float = 2, step: float = 0.2, colors: list = ["lightgrey", "darkgrey"]
+    ) -> None:
+        """
+        Adds a checkered floor plane to the viewer.
+
+        Args:
+            height (float): Height (z-coordinate) of the floor plane. Defaults to 0.
+            size (float): Size of the floor in the x and y directions. Defaults to 2.
+            step (float): Size of each checkerboard square. Defaults to 0.2.
+            colors (list): A list of two colors for the checkerboard pattern. Defaults to ["lightgrey", "darkgrey"].
+        """
         self.static_objs.append(_create_floor(height=height, size=size, step=step, colors=colors))
 
-    def _set_max_frames(self, value):
+    def _set_max_frames(self, value: int) -> None:
+        """
+        Updates the 'max_frames' attribute, which is used to track the maximum number of frames across all dynamic data.
+
+        Args:
+            value (int): The new value to set for 'max_frames'.
+        """
         self.max_frames = value
         self._update_layout()
 
-    def _update_layout(self):
+    def _update_layout(self) -> None:
+        """
+        Updates the layout of the Dash application. This includes setting the plot size and the slider range.
+        """
         self.app.layout = html.Div(
             [
                 html.H1(children="PyMotion Viewer", style={"textAlign": "center"}),
                 dcc.Graph(
                     id="graph-content",
                     style={"height": "80vh", "margin": "auto"},
                     responsive=True,
@@ -163,28 +247,42 @@
                         ),
                     ],
                     justify="center",
                 ),
             ]
         )
 
-    def _set_up_callbacks(self):
+    def _set_up_callbacks(self) -> None:
+        """
+        Sets up the Dash callbacks to enable interactivity (updating frame based on input or slider interaction).
+        """
+
         @callback(
             Output("graph-content", "figure"),
             Output("frame-input", "value"),
             Output("frames-slider", "value"),
             Input("frame-input", "value"),
             Input("frames-slider", "value"),
         )
         def update_frame(input_value, slider_value):
+            """Handles changes to the frame input or slider."""
             id = ctx.triggered_id
             new_value = input_value if id == "frame-input" else slider_value
             return self._create_figure(new_value), new_value, new_value
 
-    def _create_figure(self, frame=0):
+    def _create_figure(self, frame: int = 0) -> go.Figure:
+        """
+        Creates the Plotly figure for a given frame of the visualization.
+
+        Args:
+            frame (int): The frame number to display. Defaults to 0.
+
+        Returns:
+            go.Figure: The Plotly Figure object representing the scene at the specified frame.
+        """
         data = []
         for key, value in self.dynamic_data.items():
             if key == "skeleton":
                 for skeleton in value:
                     if frame < len(skeleton["data"]):
                         data.extend(
                             _create_skeleton(
@@ -243,28 +341,32 @@
             scene_aspectratio=dict(x=1, y=1, z=self.z_size / self.xy_size),
             margin=dict(l=0, r=0, b=0, t=0),
             showlegend=False,
         )
         return fig
 
 
-def _create_mesh_sphere(center=np.array([0, 0, 0]), radius=1, color="red", resolution=np.pi / 8):
+def _create_mesh_sphere(
+    center: np.ndarray = np.array([0, 0, 0]),
+    radius: float = 1,
+    color: str = "red",
+    resolution: float = np.pi / 8,
+) -> go.Mesh3d:
     """
-    Creates a Plotly sphere mesh with customizable position, radius, and resolution.
+    Creates a 3D mesh representation of a sphere with customizable position, radius, and resolution.
 
     Args:
-        center (tuple, optional): (x, y, z) coordinates of the sphere's center. Defaults to (0, 0, 0).
-        radius (float, optional): Radius of the sphere. Defaults to 1.
-        resolution (float, optional): Angular resolution for generating the sphere.
-                                      Defaults to np.pi/32.
+        center (np.ndarray): (x, y, z) coordinates of the sphere's center. Defaults to np.array[(0, 0, 0)].
+        radius (float): Radius of the sphere. Defaults to 1.
+        color (str): Color of the sphere. Defaults to 'red'.
+        resolution (float): Angular resolution for generating the sphere. Defaults to np.pi/8.
 
     Returns:
-        plotly.graph_objects.Mesh3d: A Plotly Mesh3d object representing the sphere.
+        go.Mesh3d: A Plotly Mesh3d object representing the sphere.
     """
-
     d = resolution  # Angular spacing
 
     theta, phi = np.mgrid[0 : np.pi + d : d, 0 : 2 * np.pi : d]
     x = np.sin(theta) * np.cos(phi)  # Adjust for center
     y = np.sin(theta) * np.sin(phi)
     z = np.cos(theta)
 
@@ -280,25 +382,28 @@
 
     points = np.vstack([x.ravel(), y.ravel(), z.ravel()])
     x, y, z = points
 
     return go.Mesh3d(x=x, y=y, z=z, color=color, opacity=1.00, alphahull=0)
 
 
-def _create_floor(height=0, size=1, step=0.1, colors=["lightgrey", "darkgrey"]):
+def _create_floor(
+    height: float = 0.0, size: float = 1.0, step: float = 0.1, colors: list[str] = ["lightgrey", "darkgrey"]
+) -> go.Mesh3d:
     """
-    Creates a floor with a checkerboard pattern.
+    Creates a floor plane with a checkerboard pattern.
 
     Args:
-        height (float, optional): Height (z-coordinate) of the floor. Defaults to 0.
-        size (float, optional): Size of the floor along x and y directions. Defaults to 1.
-        colors (list, optional):  List of two colors for the checkerboard pattern. Defaults to ['lightgrey', 'darkgrey'].
+        height (float): Height (z-coordinate) of the floor. Defaults to 0.0.
+        size (float): Size of the floor along x and y directions. Defaults to 1.0.
+        step (float): Size of each checkerboard square. Defaults to 0.1.
+        colors (list[str]): A list of two colors for the checkerboard pattern. Defaults to ["lightgrey", "darkgrey"].
 
     Returns:
-        plotly.graph_objects.Mesh3d: Plotly Mesh3d object representing the floor.
+        go.Mesh3d: Plotly Mesh3d object representing the floor.
     """
 
     x = []
     y = []
     z = []
     i = []
     j = []
@@ -318,33 +423,38 @@
             j += [a_i + 1, a_i + 1]
             k += [a_i + 3, a_i + 2]
 
     return go.Mesh3d(x=x, y=y, z=z, i=i, j=j, k=k, opacity=1.0, delaunayaxis="z", vertexcolor=vertexcolor)
 
 
 def _create_skeleton(
-    joints,
-    parents,
-    color="red",
-    sphere_mode="scatter",
-    scatter_size=3.0,
-    line_width=2.0,
-    radius_joints=0.025,
-    resolution=np.pi / 8,
-):
+    joints: np.ndarray,
+    parents: np.ndarray,
+    color: str = "red",
+    sphere_mode: str = "scatter",
+    scatter_size: float = 3.0,
+    line_width: float = 2.0,
+    radius_joints: float = 0.025,
+    resolution: float = np.pi / 8,
+) -> list[go.Scatter3d | go.Mesh3d]:
     """
-    Creates a Plotly mesh for a skeleton using a NumPy array of joint positions.
+    Creates Plotly objects for a skeleton using a NumPy array of joint positions.
 
     Args:
-        data (np.array): A NumPy array of shape (num_joints, 3) containing the x, y, and z coordinates of the joints.
-        color (str, optional): Color of the skeleton. Defaults to "red".
-        resolution (float, optional): Angular resolution for generating the spheres. Defaults to np.pi/32.
+        joints (np.ndarray): NumPy array of shape (num_joints, 3) containing the x, y, and z coordinates of the joints.
+        parents (np.ndarray): NumPy array defining the parent joint for each joint, enabling line connections.
+        color (str): Color of the skeleton elements. Defaults to 'red'.
+        sphere_mode (str): Controls sphere representation ('scatter' or 'mesh'). Defaults to 'scatter'.
+        scatter_size (float): Size of scatter markers if 'sphere_mode' is 'scatter'. Defaults to 3.0.
+        line_width (float): Width of the lines connecting skeleton joints. Defaults to 2.0.
+        radius_joints (float): Radius of joints if represented as spheres ('mesh' mode). Defaults to 0.025.
+        resolution (float): Angular resolution for sphere meshes (`mesh` mode). Defaults to np.pi/8.
 
     Returns:
-        list: A list of Plotly go.Mesh3d objects representing the spheres.
+        list[go.Scatter3d | go.Mesh3d]: A list of Plotly go.Scatter3d and/or go.Mesh3d objects representing the skeleton.
     """
 
     sphere_data = []
     line_data = []
     for joint_idx, parent_idx in enumerate(parents):
         joint = joints[joint_idx]
         if sphere_mode == "scatter":
```

### Comparing `upc_pymotion-0.1.0/pymotion/rotations/dual_quat.py` & `upc_pymotion-0.1.1/pymotion/rotations/dual_quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/rotations/dual_quat_torch.py` & `upc_pymotion-0.1.1/pymotion/rotations/dual_quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/rotations/ortho6d.py` & `upc_pymotion-0.1.1/pymotion/rotations/ortho6d.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/rotations/ortho6d_torch.py` & `upc_pymotion-0.1.1/pymotion/rotations/ortho6d_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pymotion/rotations/quat.py` & `upc_pymotion-0.1.1/pymotion/rotations/quat.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,23 +181,17 @@
         "y": 1,
         "z": 2,
     }
 
     angle_first = 2
     angle_third = 0
 
-    i = np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 2:3])[
-        ..., np.newaxis
-    ]
-    j = np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 1:2])[
-        ..., np.newaxis
-    ]
-    k = np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 0:1])[
-        ..., np.newaxis
-    ]
+    i = np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 2:3])[..., np.newaxis]
+    j = np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 1:2])[..., np.newaxis]
+    k = np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 0:1])[..., np.newaxis]
 
     # check if permutation is even or odd
     sign = (i - j) * (j - k) * (k - i) // 2
 
     # euler angles
     euler = np.empty(quaternions.shape[:-1] + (3,))
 
@@ -453,17 +447,15 @@
         d1 = np.sum(-r[i] * r[i - 1], axis=-1)
         # if the distance with the flipped quaternion is smaller, use it
         r[i][d0 < d1] = -r[i][d0 < d1]
     r = r.swapaxes(0, axis)
     return r
 
 
-def slerp(
-    q0: np.array, q1: np.array, t: float or np.array, shortest: bool = True
-) -> np.array:
+def slerp(q0: np.array, q1: np.array, t: float | np.array, shortest: bool = True) -> np.array:
     """
     Perform spherical linear interpolation (SLERP) between two unit quaternions.
 
     Parameters
     ----------
     q0 : np.array[..., [w,x,y,z]]
     q1 : np.array[..., [w,x,y,z]]
@@ -489,17 +481,15 @@
     dot = np.clip(dot, -1, 1)
 
     # Compute the quaternion of the angle between the quaternions
     theta_0 = np.arccos(dot)  # theta_0 = angle between input vectors
     theta = theta_0 * t  # theta = angle between q0 vector and result
 
     q2 = q1 - q0 * dot
-    q2 /= np.linalg.norm(
-        q2 + 0.000001, axis=-1, keepdims=True
-    )  # {q0, q2} is now an orthonormal basis
+    q2 /= np.linalg.norm(q2 + 0.000001, axis=-1, keepdims=True)  # {q0, q2} is now an orthonormal basis
 
     return np.cos(theta) * q0 + np.sin(theta) * q2
 
 
 def _fast_cross(a: np.array, b: np.array) -> np.array:
     """
     Fast cross of two vectors
```

### Comparing `upc_pymotion-0.1.0/pymotion/rotations/quat_torch.py` & `upc_pymotion-0.1.1/pymotion/rotations/quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/.gitignore` & `upc_pymotion-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/LICENSE` & `upc_pymotion-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/README.md` & `upc_pymotion-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.0/pyproject.toml` & `upc_pymotion-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.hatch.build]
 include = ["pymotion/*"]
 exclude = ["*test*"]
 
 [project]
 name = "upc-pymotion"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python library for working with motion data in NumPy or PyTorch."
 readme = "README.md"
 authors = [{ name = "Jose Luis Ponton", email = "jose.luis.ponton@upc.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `upc_pymotion-0.1.0/PKG-INFO` & `upc_pymotion-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: upc-pymotion
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for working with motion data in NumPy or PyTorch.
 Project-URL: Homepage, https://github.com/UPC-ViRVIG/pymotion
 Author-email: Jose Luis Ponton <jose.luis.ponton@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 Jose Luis Ponton
```

