# Comparing `tmp/standardbots-2.20240212.9.tar.gz` & `tmp/standardbots-2.20240401.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standardbots-2.20240212.9.tar", last modified: Thu Mar 14 03:32:07 2024, max compression
+gzip compressed data, was "standardbots-2.20240401.1.tar", last modified: Mon Apr  1 15:40:22 2024, max compression
```

## Comparing `standardbots-2.20240212.9.tar` & `standardbots-2.20240401.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:32:07.228634 standardbots-2.20240212.9/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-14 03:32:07.228634 standardbots-2.20240212.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 03:32:07.228634 standardbots-2.20240212.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-14 03:32:06.000000 standardbots-2.20240212.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:32:07.224634 standardbots-2.20240212.9/standardbots/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-14 03:31:58.000000 standardbots-2.20240212.9/standardbots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:32:07.228634 standardbots-2.20240212.9/standardbots/auto_generated/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-14 03:31:58.000000 standardbots-2.20240212.9/standardbots/auto_generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26083 2024-03-14 03:31:58.000000 standardbots-2.20240212.9/standardbots/auto_generated/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-03-14 03:31:58.000000 standardbots-2.20240212.9/standardbots/auto_generated/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 03:32:07.228634 standardbots-2.20240212.9/standardbots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-14 03:32:07.000000 standardbots-2.20240212.9/standardbots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-14 03:32:07.000000 standardbots-2.20240212.9/standardbots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 03:32:07.000000 standardbots-2.20240212.9/standardbots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-14 03:32:07.000000 standardbots-2.20240212.9/standardbots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-14 03:32:07.000000 standardbots-2.20240212.9/standardbots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.872473 standardbots-2.20240401.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:40:22.872473 standardbots-2.20240401.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/standardbots/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/standardbots/auto_generated/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/auto_generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34791 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/auto_generated/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101836 2024-04-01 15:40:12.000000 standardbots-2.20240401.1/standardbots/auto_generated/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:40:22.868473 standardbots-2.20240401.1/standardbots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 15:40:22.000000 standardbots-2.20240401.1/standardbots.egg-info/top_level.txt
```

### Comparing `standardbots-2.20240212.9/setup.py` & `standardbots-2.20240401.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: support@standardbots.com
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "standardbots"
-VERSION = "2.20240212.9"
+VERSION = "2.20240401.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `standardbots-2.20240212.9/standardbots/auto_generated/apis.py` & `standardbots-2.20240401.1/standardbots/auto_generated/apis.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,14 +113,36 @@
               value=float(force),
             ),
             grip_direction=models.LinearGripDirectionEnum(direction),
           )
         )
       )
     
+    def dh_ag_grip(
+        self,
+        target_diameter: float,
+        target_force: float | None,
+        target_speed: float | None,
+    ):
+        """
+        Control the DH AG gripper.
+        Args:
+        - target_diameter: 0.0 - 1.0
+        - target_force: 0.2 - 1.0
+        - target_speed: 0.01 - 1.0
+        """
+        return self.control_gripper(
+            body=models.GripperCommandRequest(
+                kind=models.GripperKindEnum.DhAg,
+                dh_ag=models.DHAGGripperCommandRequest(
+                    target_diameter, target_force, target_speed
+                ),
+            ),
+        )
+    
 
     def control_gripper(
       self,
       body: models.GripperCommandRequest,
     ) -> Response[
       None,
       None
@@ -521,14 +543,223 @@
   position: Position
 
   def __init__(self, request_manager: RequestManager):
     self._request_manager = request_manager
     self.brakes = Movement.Brakes(request_manager)
     self.position = Movement.Position(request_manager)
 
+class Camera:
+  _request_manager: RequestManager
+  class Data:
+    def __init__(self, request_manager: RequestManager):
+      self._request_manager = request_manager
+
+
+    def get_color_frame(
+      self,
+      body: models.CameraFrameRequest,
+    ) -> Response[
+      None,
+      None
+    ]:
+      """
+      Retrieve the latest RGB frame from the camera.
+      """
+      path = "/api/v1/camera/frame/rgb"
+      response = self._request_manager.request(
+        "GET",
+        path,
+        headers=self._request_manager.json_headers(),
+        body=json.dumps(models.serialize_camera_frame_request(body)),
+      )
+      parsed = None
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+    def get_camera_intrinsics_color(
+      self,
+    ) -> Response[
+      None,
+      None
+    ]:
+      """
+      Retrieve the intrinsic parameters for the color camera.
+      """
+      path = "/api/v1/camera/intrinsics/rgb"
+      response = self._request_manager.request(
+        "GET",
+        path,
+        headers=self._request_manager.json_headers(),
+      )
+      parsed = None
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+    def get_camera_stream(
+      self,
+    ) -> Response[
+      None,
+      None
+    ]:
+      """
+      Retrieve the latest RGB frame from the camera.
+      """
+      path = "/api/v1/camera/stream"
+      response = self._request_manager.request(
+        "GET",
+        path,
+        headers=self._request_manager.json_headers(),
+      )
+      parsed = None
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+  class Settings:
+    def __init__(self, request_manager: RequestManager):
+      self._request_manager = request_manager
+
+
+    def set_camera_settings(
+      self,
+      body: models.CameraSettings,
+    ) -> Response[
+      None,
+      None
+    ]:
+      """
+      Set the camera settings.
+      """
+      path = "/api/v1/camera/settings"
+      response = self._request_manager.request(
+        "POST",
+        path,
+        headers=self._request_manager.json_headers(),
+        body=json.dumps(models.serialize_camera_settings(body)),
+      )
+      parsed = None
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+  data: Data
+  settings: Settings
+
+  def __init__(self, request_manager: RequestManager):
+    self._request_manager = request_manager
+    self.data = Camera.Data(request_manager)
+    self.settings = Camera.Settings(request_manager)
+
+class ChatGpt:
+  _request_manager: RequestManager
+  class Data:
+    def __init__(self, request_manager: RequestManager):
+      self._request_manager = request_manager
+
+
+    def speech_to_text(
+      self,
+      body: models.SpeechToTextRequest,
+    ) -> Response[
+      None,
+      None
+    ]:
+      """
+      Convert speech to text.
+      """
+      path = "/api/v1/internal-only/speech-to-text"
+      response = self._request_manager.request(
+        "POST",
+        path,
+        headers=self._request_manager.json_headers(),
+        body=json.dumps(models.serialize_speech_to_text_request(body)),
+      )
+      parsed = None
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+    def text_to_skill(
+      self,
+      body: models.TextToSkillRequest,
+    ) -> Response[
+      None,
+      None
+    ]:
+      """
+      Convert text to a skill.
+      """
+      path = "/api/v1/internal-only/text-to-skill"
+      response = self._request_manager.request(
+        "POST",
+        path,
+        headers=self._request_manager.json_headers(),
+        body=json.dumps(models.serialize_text_to_skill_request(body)),
+      )
+      parsed = None
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+  data: Data
+
+  def __init__(self, request_manager: RequestManager):
+    self._request_manager = request_manager
+    self.data = ChatGpt.Data(request_manager)
+
 class RoutineEditor:
   _request_manager: RequestManager
   class Routines:
     def __init__(self, request_manager: RequestManager):
       self._request_manager = request_manager
 
 
@@ -905,38 +1136,128 @@
   health: Health
 
   def __init__(self, request_manager: RequestManager):
     self._request_manager = request_manager
     self.control = Status.Control(request_manager)
     self.health = Status.Health(request_manager)
 
+class Teleoperation:
+  _request_manager: RequestManager
+  class Control:
+    def __init__(self, request_manager: RequestManager):
+      self._request_manager = request_manager
+
+
+    def update_teleop_state(
+      self,
+      body: models.TeleopStateUpdateRequest,
+    ) -> Response[
+      Union[
+        models.TeleopStateResponse,
+        models.ErrorResponse,
+        None
+      ],
+      models.TeleopStateResponse
+    ]:
+      """
+      Updates the state of teleoperation based on the provided action (&#x27;start&#x27; or &#x27;stop&#x27;).
+      """
+      path = "/api/v1/movement/teleop/state"
+      response = self._request_manager.request(
+        "POST",
+        path,
+        headers=self._request_manager.json_headers(),
+        body=json.dumps(models.serialize_teleop_state_update_request(body)),
+      )
+      parsed = None
+      if response.status == 200:
+        parsed = models.parse_teleop_state_response(json.loads(response.data))
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+  class Status:
+    def __init__(self, request_manager: RequestManager):
+      self._request_manager = request_manager
+
+
+    def get_teleop_state(
+      self,
+    ) -> Response[
+      None,
+      None
+    ]:
+      """
+      Retrieves the current state of teleoperation.
+      """
+      path = "/api/v1/movement/teleop/state"
+      response = self._request_manager.request(
+        "GET",
+        path,
+        headers=self._request_manager.json_headers(),
+      )
+      parsed = None
+
+      is_user_error = response.status >= 400 and response.status < 500
+      is_unavailable = response.status == 503
+      if parsed is None and (is_user_error or is_unavailable):
+        parsed = models.parse_error_response(json.loads(response.data))
+
+      return Response(
+        parsed,
+        response.status,
+        response
+      )
+
+  control: Control
+  status: Status
+
+  def __init__(self, request_manager: RequestManager):
+    self._request_manager = request_manager
+    self.control = Teleoperation.Control(request_manager)
+    self.status = Teleoperation.Status(request_manager)
+
 
 
 
 class StandardBotsRobot(Default):
   RobotKind = RobotKind
 
   movement: Movement
+  camera: Camera
+  chat_gpt: ChatGpt
   routine_editor: RoutineEditor
   status: Status
+  teleoperation: Teleoperation
   def __init__(
     self,
     url: str,
     token: str,
     robot_kind: Union[RobotKind, str] = RobotKind.Live,
     pools: int = 10
   ):
     super().__init__(RequestManager(
       urllib3.PoolManager(num_pools=2),
       token=token,
       host=url,
       robot_kind=RobotKind(robot_kind),
     ))
     self.movement = Movement(self._request_manager)
+    self.camera = Camera(self._request_manager)
+    self.chat_gpt = ChatGpt(self._request_manager)
     self.routine_editor = RoutineEditor(self._request_manager)
     self.status = Status(self._request_manager)
+    self.teleoperation = Teleoperation(self._request_manager)
 
   @contextmanager
   def connection(self):
     yield
     self._request_manager.close()
```

### Comparing `standardbots-2.20240212.9/standardbots/auto_generated/models.py` & `standardbots-2.20240401.1/standardbots/auto_generated/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -233,14 +233,345 @@
 def parse_brakes_state_enum(data: object) -> BrakesStateEnum:
   return BrakesStateEnum(data)
 
 def serialize_brakes_state_enum(data: Union[BrakesStateEnum, str]) -> object:
   return BrakesStateEnum(data).value
 
 @dataclass
+class CameraIntrinsics:
+  """Intrinsic parameters of the camera."""
+  width: Union[float, None] = None
+  height: Union[float, None] = None
+  fx: Union[float, None] = None
+  fy: Union[float, None] = None
+  ppx: Union[float, None] = None
+  ppy: Union[float, None] = None
+  error: Union[int, None] = None
+
+  def validate_width(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "width must be of type float for CameraIntrinsics, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_height(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "height must be of type float for CameraIntrinsics, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_fx(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "fx must be of type float for CameraIntrinsics, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_fy(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "fy must be of type float for CameraIntrinsics, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_ppx(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "ppx must be of type float for CameraIntrinsics, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_ppy(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "ppy must be of type float for CameraIntrinsics, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_error(self, value: int) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, int):
+      return [False, "error must be of type int for CameraIntrinsics, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_width(self.width)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_height(self.height)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_fx(self.fx)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_fy(self.fy)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_ppx(self.ppx)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_ppy(self.ppy)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_error(self.error)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_camera_intrinsics(data: object):
+  return CameraIntrinsics(
+    width=parse_f_64(data["width"]) if "width" in data else None,
+    height=parse_f_64(data["height"]) if "height" in data else None,
+    fx=parse_f_64(data["fx"]) if "fx" in data else None,
+    fy=parse_f_64(data["fy"]) if "fy" in data else None,
+    ppx=parse_f_64(data["ppx"]) if "ppx" in data else None,
+    ppy=parse_f_64(data["ppy"]) if "ppy" in data else None,
+    error=parse_i_8(data["error"]) if "error" in data else None,
+  )
+
+def serialize_camera_intrinsics(data: CameraIntrinsics) -> object:
+  return {
+    "width": None if data.width is None else serialize_f_64(data.width),
+    "height": None if data.height is None else serialize_f_64(data.height),
+    "fx": None if data.fx is None else serialize_f_64(data.fx),
+    "fy": None if data.fy is None else serialize_f_64(data.fy),
+    "ppx": None if data.ppx is None else serialize_f_64(data.ppx),
+    "ppy": None if data.ppy is None else serialize_f_64(data.ppy),
+    "error": None if data.error is None else serialize_i_8(data.error),
+  }
+
+@dataclass
+class CameraSettings:
+  """Settings for the camera."""
+  brightness: Union[int, None] = None
+  contrast: Union[int, None] = None
+  exposure: Union[int, None] = None
+  sharpness: Union[int, None] = None
+  hue: Union[int, None] = None
+  whiteBalance: Union[int, None] = None
+  autoWhiteBalance: Union[bool, None] = None
+
+  def validate_brightness(self, value: int) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, int):
+      return [False, "brightness must be of type int for CameraSettings, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_contrast(self, value: int) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, int):
+      return [False, "contrast must be of type int for CameraSettings, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_exposure(self, value: int) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, int):
+      return [False, "exposure must be of type int for CameraSettings, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_sharpness(self, value: int) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, int):
+      return [False, "sharpness must be of type int for CameraSettings, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_hue(self, value: int) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, int):
+      return [False, "hue must be of type int for CameraSettings, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_whiteBalance(self, value: int) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, int):
+      return [False, "whiteBalance must be of type int for CameraSettings, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_autoWhiteBalance(self, value: bool) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, bool):
+      return [False, "autoWhiteBalance must be of type bool for CameraSettings, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_brightness(self.brightness)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_contrast(self.contrast)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_exposure(self.exposure)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_sharpness(self.sharpness)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_hue(self.hue)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_whiteBalance(self.whiteBalance)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_autoWhiteBalance(self.autoWhiteBalance)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_camera_settings(data: object):
+  return CameraSettings(
+    brightness=parse_i_16(data["brightness"]) if "brightness" in data else None,
+    contrast=parse_i_16(data["contrast"]) if "contrast" in data else None,
+    exposure=parse_i_16(data["exposure"]) if "exposure" in data else None,
+    sharpness=parse_i_16(data["sharpness"]) if "sharpness" in data else None,
+    hue=parse_i_16(data["hue"]) if "hue" in data else None,
+    whiteBalance=parse_i_16(data["whiteBalance"]) if "whiteBalance" in data else None,
+    autoWhiteBalance=parse_bool(data["autoWhiteBalance"]) if "autoWhiteBalance" in data else None,
+  )
+
+def serialize_camera_settings(data: CameraSettings) -> object:
+  return {
+    "brightness": None if data.brightness is None else serialize_i_16(data.brightness),
+    "contrast": None if data.contrast is None else serialize_i_16(data.contrast),
+    "exposure": None if data.exposure is None else serialize_i_16(data.exposure),
+    "sharpness": None if data.sharpness is None else serialize_i_16(data.sharpness),
+    "hue": None if data.hue is None else serialize_i_16(data.hue),
+    "whiteBalance": None if data.whiteBalance is None else serialize_i_16(data.whiteBalance),
+    "autoWhiteBalance": None if data.autoWhiteBalance is None else serialize_bool(data.autoWhiteBalance),
+  }
+
+@dataclass
+class DHAGGripperCommandRequest:
+  """Control the DH AG gripper (end effector) of the robot
+"""
+  target_diameter: Union[float, None] = None
+  target_force: Union[float, None] = None
+  target_speed: Union[float, None] = None
+
+  def validate_target_diameter(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [False, "target_diameter is required for DHAGGripperCommandRequest"]
+
+    if not isinstance(value, float):
+      return [False, "target_diameter must be of type float for DHAGGripperCommandRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_target_force(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "target_force must be of type float for DHAGGripperCommandRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_target_speed(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, float):
+      return [False, "target_speed must be of type float for DHAGGripperCommandRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_target_diameter(self.target_diameter)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_target_force(self.target_force)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_target_speed(self.target_speed)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_dhag_gripper_command_request(data: object):
+  return DHAGGripperCommandRequest(
+    target_diameter=parse_f_64(data["target_diameter"]) if "target_diameter" in data else None,
+    target_force=parse_f_64(data["target_force"]) if "target_force" in data else None,
+    target_speed=parse_f_64(data["target_speed"]) if "target_speed" in data else None,
+  )
+
+def serialize_dhag_gripper_command_request(data: DHAGGripperCommandRequest) -> object:
+  return {
+    "target_diameter": serialize_f_64(data.target_diameter),
+    "target_force": None if data.target_force is None else serialize_f_64(data.target_force),
+    "target_speed": None if data.target_speed is None else serialize_f_64(data.target_speed),
+  }
+
+@dataclass
+class DHAGGripperConfiguration:
+  """Configuration for DH AG Gripper"""
+  diameter: Union[float, None] = None
+
+  def validate_diameter(self, value: float) -> Tuple[bool, str]:
+    if value is None:
+      return [False, "diameter is required for DHAGGripperConfiguration"]
+
+    if not isinstance(value, float):
+      return [False, "diameter must be of type float for DHAGGripperConfiguration, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_diameter(self.diameter)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_dhag_gripper_configuration(data: object):
+  return DHAGGripperConfiguration(
+    diameter=parse_f_64(data["diameter"]) if "diameter" in data else None,
+  )
+
+def serialize_dhag_gripper_configuration(data: DHAGGripperConfiguration) -> object:
+  return {
+    "diameter": serialize_f_64(data.diameter),
+  }
+
+@dataclass
 class EngageEmergencyStopRequest:
   """Engage Emergency Stop. This will immediately stop the robot and prevent it from moving until the robot is unbraked.
 """
   reason: Union[str, None] = None
 
   def validate_reason(self, value: str) -> Tuple[bool, str]:
     if value is None:
@@ -344,14 +675,24 @@
   """Brakes must be_engaged"""
   BrakesMustBeDisengaged = "brakes_must_be_disengaged"
   """Brakes must be disengaged"""
   EquipmentNoMatching = "equipment_no_matching"
   """No matching equipment found"""
   ServiceInitializing = "service_initializing"
   """The service is unavailable while initializing"""
+  CameraDisconnected = "camera_disconnected"
+  """Camera service running, but no camera is connected"""
+  SettingsValidationError = "settings_validation_error"
+  """Camera settings validation failed"""
+  SettingsTimeout = "settings_timeout"
+  """Camera settings timed out"""
+  InternalServerError = "internal_server_error"
+  """Internal server error occurred"""
+  NotFound = "not_found"
+  """Requested resource not found"""
 
 def parse_error_enum(data: object) -> ErrorEnum:
   return ErrorEnum(data)
 
 def serialize_error_enum(data: Union[ErrorEnum, str]) -> object:
   return ErrorEnum(data).value
 
@@ -368,14 +709,16 @@
   return ForceUnitKind(data).value
 
 class GripperKindEnum(Enum):
   Onrobot2Fg7 = "onrobot_2fg7"
   """An OnRobot 2FG7 Gripper is connected"""
   Onrobot3Fg15 = "onrobot_3fg15"
   """An OnRobot 3FG15 Gripper is connected"""
+  DhAg = "dh_ag"
+  """A DH AG Gripper is connected"""
   NoneConnected = "none_connected"
   """No gripper is connected"""
 
 def parse_gripper_kind_enum(data: object) -> GripperKindEnum:
   return GripperKindEnum(data)
 
 def serialize_gripper_kind_enum(data: Union[GripperKindEnum, str]) -> object:
@@ -685,14 +1028,52 @@
   )
 
 def serialize_runtime_variable(data: RuntimeVariable) -> object:
   return {
     "value": None if data.value is None else serialize_str(data.value),
   }
 
+SkillsList = List[str]
+
+def parse_skills_list(data: object) -> SkillsList:
+  return [parse_str(item) for item in data]
+
+def serialize_skills_list(data: SkillsList) -> List[object]:
+  return [serialize_str(item) for item in data]
+
+@dataclass
+class SpeechToTextRequest:
+  """Request to convert speech to text."""
+  encoded_audio_data: Union[str, None] = None
+
+  def validate_encoded_audio_data(self, value: str) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, str):
+      return [False, "encoded_audio_data must be of type str for SpeechToTextRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_encoded_audio_data(self.encoded_audio_data)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_speech_to_text_request(data: object):
+  return SpeechToTextRequest(
+    encoded_audio_data=parse_str(data["encoded_audio_data"]) if "encoded_audio_data" in data else None,
+  )
+
+def serialize_speech_to_text_request(data: SpeechToTextRequest) -> object:
+  return {
+    "encoded_audio_data": None if data.encoded_audio_data is None else serialize_str(data.encoded_audio_data),
+  }
+
 class StatusHealthEnum(Enum):
   Ok = "ok"
   """Enum Ok = `ok`"""
   Warning = "warning"
   """Enum Warning = `warning`"""
   Error = "error"
   """Enum Error = `error`"""
@@ -744,14 +1125,64 @@
 
 def serialize_status_version_data(data: StatusVersionData) -> object:
   return {
     "id": None if data.id is None else serialize_str(data.id),
     "name": None if data.name is None else serialize_str(data.name),
   }
 
+class TeleopStateEnum(Enum):
+  WaitForTeleop = "wait_for_teleop"
+  """The system is waiting to start teleoperation."""
+  Teleop = "teleop"
+  """Teleoperation is active, and the robot is being controlled remotely."""
+  Stopping = "stopping"
+  """The robot is stopping."""
+  Stopped = "stopped"
+  """Teleoperation is stopped, and the robot is not moving."""
+  Moving = "moving"
+  """The robot is moving but not under teleoperation."""
+  Unfrozen = "unfrozen"
+  """The mini-arm is unfrozen."""
+
+def parse_teleop_state_enum(data: object) -> TeleopStateEnum:
+  return TeleopStateEnum(data)
+
+def serialize_teleop_state_enum(data: Union[TeleopStateEnum, str]) -> object:
+  return TeleopStateEnum(data).value
+
+@dataclass
+class TeleopStateUpdateRequest:
+  """Request to update the state of teleoperation to either start or stop."""
+  action: Union[str, None] = None
+
+  def validate_action(self, value: str) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, str):
+      return [False, "action must be of type str for TeleopStateUpdateRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_action(self.action)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_teleop_state_update_request(data: object):
+  return TeleopStateUpdateRequest(
+    action=parse_str(data["action"]) if "action" in data else None,
+  )
+
+def serialize_teleop_state_update_request(data: TeleopStateUpdateRequest) -> object:
+  return {
+    "action": None if data.action is None else serialize_str(data.action),
+  }
+
 @dataclass
 class ArmPositionUpdateFailureEvent:
   """Move robot event when movement failed"""
   kind: Union[ArmPositionUpdateFailureEventKind, None] = None
   reason: Union[str, None] = None
   internal_reason: Union[str, None] = None
 
@@ -843,14 +1274,74 @@
   )
 
 def serialize_brakes_state(data: BrakesState) -> object:
   return {
     "state": serialize_brakes_state_enum(data.state),
   }
 
+@dataclass
+class CameraIntrinsicsResponse:
+  """Response with intrinsic parameters of the camera."""
+  intrinsics: Union[CameraIntrinsics, None] = None
+
+  def validate_intrinsics(self, value: CameraIntrinsics) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, CameraIntrinsics):
+      return [False, "intrinsics must be of type CameraIntrinsics for CameraIntrinsicsResponse, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_intrinsics(self.intrinsics)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_camera_intrinsics_response(data: object):
+  return CameraIntrinsicsResponse(
+    intrinsics=parse_camera_intrinsics(data["intrinsics"]) if "intrinsics" in data else None,
+  )
+
+def serialize_camera_intrinsics_response(data: CameraIntrinsicsResponse) -> object:
+  return {
+    "intrinsics": None if data.intrinsics is None else serialize_camera_intrinsics(data.intrinsics),
+  }
+
+@dataclass
+class CameraFrameRequest:
+  """Request for a single camera frame."""
+  camera_settings: Union[CameraSettings, None] = None
+
+  def validate_camera_settings(self, value: CameraSettings) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, CameraSettings):
+      return [False, "camera_settings must be of type CameraSettings for CameraFrameRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_camera_settings(self.camera_settings)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_camera_frame_request(data: object):
+  return CameraFrameRequest(
+    camera_settings=parse_camera_settings(data["camera_settings"]) if "camera_settings" in data else None,
+  )
+
+def serialize_camera_frame_request(data: CameraFrameRequest) -> object:
+  return {
+    "camera_settings": None if data.camera_settings is None else serialize_camera_settings(data.camera_settings),
+  }
+
 EnvironmentVariablesList = List[EnvironmentVariable]
 
 def parse_environment_variables_list(data: object) -> EnvironmentVariablesList:
   return [parse_environment_variable(item) for item in data]
 
 def serialize_environment_variables_list(data: EnvironmentVariablesList) -> List[object]:
   return [serialize_environment_variable(item) for item in data]
@@ -861,15 +1352,15 @@
   error: Union[ErrorEnum, None] = None
   message: Union[str, None] = None
 
   def validate_error(self, value: ErrorEnum) -> Tuple[bool, str]:
     if value is None:
       return [False, "error is required for ErrorResponse"]
 
-    if not ((isinstance(value, str) and ErrorEnum in ['authorization_required', 'routine_must_be_running', 'api_control_required', 'robot_brakes_disengage_failed', 'robot_brakes_engage_failed', 'request_failed_validation', 'brakes_must_be_engaged', 'brakes_must_be_disengaged', 'equipment_no_matching', 'service_initializing']) or isinstance(value, ErrorEnum)):
+    if not ((isinstance(value, str) and ErrorEnum in ['authorization_required', 'routine_must_be_running', 'api_control_required', 'robot_brakes_disengage_failed', 'robot_brakes_engage_failed', 'request_failed_validation', 'brakes_must_be_engaged', 'brakes_must_be_disengaged', 'equipment_no_matching', 'service_initializing', 'camera_disconnected', 'settings_validation_error', 'settings_timeout', 'internal_server_error', 'not_found']) or isinstance(value, ErrorEnum)):
       return [False, "error must be of type ErrorEnum for ErrorResponse, got " + type(value).__name__]
 
     return [True, ""]
 
   def validate_message(self, value: str) -> Tuple[bool, str]:
     if value is None:
       return [False, "message is required for ErrorResponse"]
@@ -946,38 +1437,53 @@
     "value": None if data.value is None else serialize_f_64(data.value),
   }
 
 @dataclass
 class GripperConfiguration:
   """Configuration of gripper, also known as End Effector"""
   kind: Union[GripperKindEnum, None] = None
+  dh_ag: Union[DHAGGripperConfiguration, None] = None
 
   def validate_kind(self, value: GripperKindEnum) -> Tuple[bool, str]:
     if value is None:
       return [False, "kind is required for GripperConfiguration"]
 
-    if not ((isinstance(value, str) and GripperKindEnum in ['onrobot_2fg7', 'onrobot_3fg15', 'none_connected']) or isinstance(value, GripperKindEnum)):
+    if not ((isinstance(value, str) and GripperKindEnum in ['onrobot_2fg7', 'onrobot_3fg15', 'dh_ag', 'none_connected']) or isinstance(value, GripperKindEnum)):
       return [False, "kind must be of type GripperKindEnum for GripperConfiguration, got " + type(value).__name__]
 
     return [True, ""]
 
+  def validate_dh_ag(self, value: DHAGGripperConfiguration) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, DHAGGripperConfiguration):
+      return [False, "dh_ag must be of type DHAGGripperConfiguration for GripperConfiguration, got " + type(value).__name__]
+
+    return [True, ""]
+
   def __post_init__(self):
     # Type check incoming model - raise error if invalid (required or wrong type)
     is_valid, error_str = self.validate_kind(self.kind)
     if not is_valid:
       raise TypeError(error_str)
+    is_valid, error_str = self.validate_dh_ag(self.dh_ag)
+    if not is_valid:
+      raise TypeError(error_str)
 
 def parse_gripper_configuration(data: object):
   return GripperConfiguration(
     kind=parse_gripper_kind_enum(data["kind"]) if "kind" in data else None,
+    dh_ag=parse_dhag_gripper_configuration(data["dh_ag"]) if "dh_ag" in data else None,
   )
 
 def serialize_gripper_configuration(data: GripperConfiguration) -> object:
   return {
     "kind": serialize_gripper_kind_enum(data.kind),
+    "dh_ag": None if data.dh_ag is None else serialize_dhag_gripper_configuration(data.dh_ag),
   }
 
 @dataclass
 class ArmJointRotations:
   """Rotational positions of arm joints"""
   joints: Union[JointRotations, None] = None
 
@@ -1237,14 +1743,59 @@
 
 def serialize_play_routine_request(data: PlayRoutineRequest) -> object:
   return {
     "variables": None if data.variables is None else serialize_routine_variables_state_map(data.variables),
   }
 
 @dataclass
+class TextToSkillRequest:
+  """Request to convert text to a skill."""
+  text: Union[str, None] = None
+  skills: Union[SkillsList, None] = None
+
+  def validate_text(self, value: str) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, str):
+      return [False, "text must be of type str for TextToSkillRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def validate_skills(self, value: SkillsList) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not (isinstance(value, list) and all(isinstance(x, str) for x in value)):
+      return [False, "skills must be of type SkillsList for TextToSkillRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_text(self.text)
+    if not is_valid:
+      raise TypeError(error_str)
+    is_valid, error_str = self.validate_skills(self.skills)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_text_to_skill_request(data: object):
+  return TextToSkillRequest(
+    text=parse_str(data["text"]) if "text" in data else None,
+    skills=parse_skills_list(data["skills"]) if "skills" in data else None,
+  )
+
+def serialize_text_to_skill_request(data: TextToSkillRequest) -> object:
+  return {
+    "text": None if data.text is None else serialize_str(data.text),
+    "skills": None if data.skills is None else serialize_skills_list(data.skills),
+  }
+
+@dataclass
 class StatusHealthResponse:
   """Status Health Response"""
   health: Union[StatusHealthEnum, None] = None
   build: Union[StatusVersionData, None] = None
 
   def validate_health(self, value: StatusHealthEnum) -> Tuple[bool, str]:
     if value is None:
@@ -1282,14 +1833,44 @@
 def serialize_status_health_response(data: StatusHealthResponse) -> object:
   return {
     "health": None if data.health is None else serialize_status_health_enum(data.health),
     "build": None if data.build is None else serialize_status_version_data(data.build),
   }
 
 @dataclass
+class TeleopStateResponse:
+  """Response to a query for the current state of teleoperation."""
+  state: Union[TeleopStateEnum, None] = None
+
+  def validate_state(self, value: TeleopStateEnum) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not ((isinstance(value, str) and TeleopStateEnum in ['wait_for_teleop', 'teleop', 'stopping', 'stopped', 'moving', 'unfrozen']) or isinstance(value, TeleopStateEnum)):
+      return [False, "state must be of type TeleopStateEnum for TeleopStateResponse, got " + type(value).__name__]
+
+    return [True, ""]
+
+  def __post_init__(self):
+    # Type check incoming model - raise error if invalid (required or wrong type)
+    is_valid, error_str = self.validate_state(self.state)
+    if not is_valid:
+      raise TypeError(error_str)
+
+def parse_teleop_state_response(data: object):
+  return TeleopStateResponse(
+    state=parse_teleop_state_enum(data["state"]) if "state" in data else None,
+  )
+
+def serialize_teleop_state_response(data: TeleopStateResponse) -> object:
+  return {
+    "state": None if data.state is None else serialize_teleop_state_enum(data.state),
+  }
+
+@dataclass
 class ArmPositionUpdateRequestResponseEventStreamDetails:
   """Specify how the response should be sent
 """
   subscriptions: Union[ArmPositionUpdateRequestResponseEventStreamSubscriptionsList, None] = None
 
   def validate_subscriptions(self, value: ArmPositionUpdateRequestResponseEventStreamSubscriptionsList) -> Tuple[bool, str]:
     if value is None:
@@ -1713,20 +2294,21 @@
 @dataclass
 class GripperCommandRequest:
   """Control the gripper (end effector) of the robot
 """
   kind: Union[GripperKindEnum, None] = None
   onrobot_2fg7: Union[OnRobot2FG7GripperCommandRequest, None] = None
   onrobot_3fg15: Union[OnRobot3FG15GripperCommandRequest, None] = None
+  dh_ag: Union[DHAGGripperCommandRequest, None] = None
 
   def validate_kind(self, value: GripperKindEnum) -> Tuple[bool, str]:
     if value is None:
       return [False, "kind is required for GripperCommandRequest"]
 
-    if not ((isinstance(value, str) and GripperKindEnum in ['onrobot_2fg7', 'onrobot_3fg15', 'none_connected']) or isinstance(value, GripperKindEnum)):
+    if not ((isinstance(value, str) and GripperKindEnum in ['onrobot_2fg7', 'onrobot_3fg15', 'dh_ag', 'none_connected']) or isinstance(value, GripperKindEnum)):
       return [False, "kind must be of type GripperKindEnum for GripperCommandRequest, got " + type(value).__name__]
 
     return [True, ""]
 
   def validate_onrobot_2fg7(self, value: OnRobot2FG7GripperCommandRequest) -> Tuple[bool, str]:
     if value is None:
       return [True, ""]
@@ -1741,38 +2323,52 @@
       return [True, ""]
 
     if not isinstance(value, OnRobot3FG15GripperCommandRequest):
       return [False, "onrobot_3fg15 must be of type OnRobot3FG15GripperCommandRequest for GripperCommandRequest, got " + type(value).__name__]
 
     return [True, ""]
 
+  def validate_dh_ag(self, value: DHAGGripperCommandRequest) -> Tuple[bool, str]:
+    if value is None:
+      return [True, ""]
+
+    if not isinstance(value, DHAGGripperCommandRequest):
+      return [False, "dh_ag must be of type DHAGGripperCommandRequest for GripperCommandRequest, got " + type(value).__name__]
+
+    return [True, ""]
+
   def __post_init__(self):
     # Type check incoming model - raise error if invalid (required or wrong type)
     is_valid, error_str = self.validate_kind(self.kind)
     if not is_valid:
       raise TypeError(error_str)
     is_valid, error_str = self.validate_onrobot_2fg7(self.onrobot_2fg7)
     if not is_valid:
       raise TypeError(error_str)
     is_valid, error_str = self.validate_onrobot_3fg15(self.onrobot_3fg15)
     if not is_valid:
       raise TypeError(error_str)
+    is_valid, error_str = self.validate_dh_ag(self.dh_ag)
+    if not is_valid:
+      raise TypeError(error_str)
 
 def parse_gripper_command_request(data: object):
   return GripperCommandRequest(
     kind=parse_gripper_kind_enum(data["kind"]) if "kind" in data else None,
     onrobot_2fg7=parse_on_robot_2_fg_7_gripper_command_request(data["onrobot_2fg7"]) if "onrobot_2fg7" in data else None,
     onrobot_3fg15=parse_on_robot_3_fg_15_gripper_command_request(data["onrobot_3fg15"]) if "onrobot_3fg15" in data else None,
+    dh_ag=parse_dhag_gripper_command_request(data["dh_ag"]) if "dh_ag" in data else None,
   )
 
 def serialize_gripper_command_request(data: GripperCommandRequest) -> object:
   return {
     "kind": serialize_gripper_kind_enum(data.kind),
     "onrobot_2fg7": None if data.onrobot_2fg7 is None else serialize_on_robot_2_fg_7_gripper_command_request(data.onrobot_2fg7),
     "onrobot_3fg15": None if data.onrobot_3fg15 is None else serialize_on_robot_3_fg_15_gripper_command_request(data.onrobot_3fg15),
+    "dh_ag": None if data.dh_ag is None else serialize_dhag_gripper_command_request(data.dh_ag),
   }
 
 @dataclass
 class CombinedArmPosition:
   """Combined tooltip position and joint rotations defining the arm&#x27;s position"""
   joint_rotations: Union[JointRotations, None] = None
   tooltip_position: Union[PositionAndOrientation, None] = None
```

