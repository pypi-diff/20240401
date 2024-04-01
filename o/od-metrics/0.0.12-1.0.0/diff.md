# Comparing `tmp/od-metrics-0.0.12.tar.gz` & `tmp/od-metrics-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "od-metrics-0.0.12.tar", last modified: Sun Dec 24 08:53:41 2023, max compression
+gzip compressed data, was "od-metrics-1.0.0.tar", last modified: Mon Apr  1 21:50:04 2024, max compression
```

## Comparing `od-metrics-0.0.12.tar` & `od-metrics-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 08:53:41.262063 od-metrics-0.0.12/
--rw-r--r--   0 root         (0) root         (0)     1068 2023-12-24 08:53:21.000000 od-metrics-0.0.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4344 2023-12-24 08:53:41.262063 od-metrics-0.0.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3819 2023-12-24 08:53:21.000000 od-metrics-0.0.12/README.md
--rw-r--r--   0 root         (0) root         (0)       49 2023-12-24 08:53:21.000000 od-metrics-0.0.12/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      782 2023-12-24 08:53:41.262063 od-metrics-0.0.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       69 2023-12-24 08:53:21.000000 od-metrics-0.0.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 08:53:41.258063 od-metrics-0.0.12/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 08:53:41.262063 od-metrics-0.0.12/src/od_metrics/
--rw-r--r--   0 root         (0) root         (0)      111 2023-12-24 08:53:21.000000 od-metrics-0.0.12/src/od_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2199 2023-12-24 08:53:21.000000 od-metrics-0.0.12/src/od_metrics/constants.py
--rw-r--r--   0 root         (0) root         (0)    46625 2023-12-24 08:53:21.000000 od-metrics-0.0.12/src/od_metrics/od_metrics.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-12-24 08:53:21.000000 od-metrics-0.0.12/src/od_metrics/utils.py
--rw-r--r--   0 root         (0) root         (0)    23147 2023-12-24 08:53:21.000000 od-metrics-0.0.12/src/od_metrics/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 08:53:41.262063 od-metrics-0.0.12/src/od_metrics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4344 2023-12-24 08:53:41.000000 od-metrics-0.0.12/src/od_metrics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2023-12-24 08:53:41.000000 od-metrics-0.0.12/src/od_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-24 08:53:41.000000 od-metrics-0.0.12/src/od_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-12-24 08:53:41.000000 od-metrics-0.0.12/src/od_metrics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-12-24 08:53:41.000000 od-metrics-0.0.12/src/od_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-24 08:53:41.262063 od-metrics-0.0.12/tests/
--rw-r--r--   0 root         (0) root         (0)    12196 2023-12-24 08:53:21.000000 od-metrics-0.0.12/tests/test_pycoco_equivalence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.769223 od-metrics-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-01 21:49:53.000000 od-metrics-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4343 2024-04-01 21:50:04.769223 od-metrics-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-04-01 21:49:53.000000 od-metrics-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-01 21:49:53.000000 od-metrics-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      781 2024-04-01 21:50:04.769223 od-metrics-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-01 21:49:53.000000 od-metrics-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.765223 od-metrics-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.765223 od-metrics-1.0.0/src/od_metrics/
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/constants.py
+-rw-r--r--   0 root         (0) root         (0)    46890 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/od_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/utils.py
+-rw-r--r--   0 root         (0) root         (0)    23209 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.769223 od-metrics-1.0.0/src/od_metrics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4343 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.769223 od-metrics-1.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)    12219 2024-04-01 21:49:53.000000 od-metrics-1.0.0/tests/test_pycoco_equivalence.py
```

### Comparing `od-metrics-0.0.12/LICENSE` & `od-metrics-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `od-metrics-0.0.12/PKG-INFO` & `od-metrics-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-metrics
-Version: 0.0.12
+Version: 1.0.0
 Summary: Object Detection metrics.
 Home-page: https://github.com/EMalagoli92/OD-metrics
 Author: EMalagoli92
 Author-email: emala.892@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 0.0.12 Summary: Object
-Detection metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
+Metadata-Version: 2.1 Name: od-metrics Version: 1.0.0 Summary: Object Detection
+metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
 EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
                                 logo_light.svg]
```

### Comparing `od-metrics-0.0.12/README.md` & `od-metrics-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `od-metrics-0.0.12/setup.cfg` & `od-metrics-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = od-metrics
-version = 0.0.12
+version = 1.0.0
 author = EMalagoli92
 author_email = emala.892@gmail.com
 description = Object Detection metrics.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/EMalagoli92/OD-metrics
 classifiers =
```

### Comparing `od-metrics-0.0.12/src/od_metrics/constants.py` & `od-metrics-1.0.0/src/od_metrics/constants.py`

 * *Files identical despite different names*

### Comparing `od-metrics-0.0.12/src/od_metrics/od_metrics.py` & `od-metrics-1.0.0/src/od_metrics/od_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,34 +77,34 @@
                 "small": [0 ** 2, 32 ** 2],
                 "medium": [32 ** 2, 96 ** 2],
                 "large": [96 ** 2, 1e5 ** 2]
                 }`
             If `None`, no area range limits will be set.
             The default is `_Missing`.
         class_metrics : bool, optional
-            Option to enable per-class metrics. (See `compute`).
+            Option to enable per-class metrics (See `compute()` method).
             Has a performance impact.
             The default is `False`.
         box_format: Literal["xyxy", "xywh", "cxcywh"], optional
             Bounding box format.
             Supported formats are:<br>
-                - `xyxy`: boxes are represented via corners,
+                - `"xyxy"`: boxes are represented via corners,
                         x1, y1 being top left and x2, y2
                         being bottom right.<br>
                 - `xywh`: boxes are represented via corner,
                         width and height, x1, y2 being top
                         left, w, h being width and height.
                         This is the default format; all
                         input formats will be converted
                         to this.<br>
-                - `cxcywh`: boxes are represented via centre,
-                          width and height, cx, cy being
-                          center of box, w, h being width
-                          and height.<br>
-            The default is `xywh`.
+                - `"cxcywh"`: boxes are represented via centre,
+                        width and height, cx, cy being
+                        center of box, w, h being width
+                        and height.<br>
+            The default is `"xywh"`.
 
         Returns
         -------
         None
         """
         constructor_model = ConstructorModel.model_validate(
             {
@@ -143,146 +143,148 @@
         y_true : list[dict]
             A list consisting of dictionaries each containing
             the key-values: each dictionary corresponds to the ground truth
             of a single image.
             Parameters that should be provided per dict:
 
                 boxes : list[list[float]] | np.ndarray
-                    List of floats lists or np.ndarray; the length of the
+                    List of floats lists or `np.ndarray`; the length of the
                     list/array correspond to the number of boxes and each
                     list/array is 4-float specifying the box coordinates in
                     the format specified in the constructor.
                 labels : list[int] | np.ndarray
-                    List of integers or np.ndarray specifying the ground
+                    List of integers or `np.ndarray` specifying the ground
                     truth classes for the boxes: the length corresponds to
                     the number of boxes.
                 iscrowd : list[bool | Literal[0, 1]] | np.ndarray
-                    List of integers or np.ndarray specifying crowd regions:
+                    List of integers or `np.ndarray` specifying crowd regions:
                     the length corresponds to the number of boxes.
-                    The values can be bool or 0/1 indicating whether the
+                    The values can be `bool` or `0`/`1` indicating whether the
                     bounding box indicates a crowd of objects.
                     Value is optional, and if not provided it will
-                    automatically be set to False.
+                    automatically be set to `False`.
                 area : list[float] | np.ndarray
-                    A list of float or np.ndarray specifying the area of
+                    A list of `float` or `np.ndarray` specifying the area of
                     the objects: the length corresponds to the number of
                     boxes.
                     Value is optional, and if not provided will
                     be automatically calculated based on
                     the bounding box provided.
                     Only affects which samples contribute the specific
                     area range.
         y_pred : list[dict]
             A list consisting of dictionaries each containing
             the key-values: each dictionary corresponds to the predictions
             of a single image.
             Parameters that should be provided per dict:
 
                 boxes : list[list[float]] | np.ndarray
-                    List of float lists or np.ndarray; the length of the
+                    List of float lists or `np.ndarray`; the length of the
                     list/array correspond to the number of boxes and each
                     list/array is 4-float specifying the box coordinates in
                     the format specified in the constructor.
                 scores : list[float] | np.ndarray
-                    List of floats or np.ndarray specifying for the boxes:
-                    the length corresponds to the number of boxes.
+                    List of floats or `np.ndarray` specifying the score for
+                    the boxes: the length corresponds to the number of boxes.
                 labels : list[int] | np.ndarray
-                    List of integers or np.ndarray specifying the ground
+                    List of integers or `np.ndarray` specifying the ground
                     truth classes for the boxes: the length corresponds to
                     the number of boxes.
         extended_summary : bool, optional
             Option to enable extended summary with additional metrics
             including `IoU`, `AP` (Average Precision), `AR` (Average Recall)
             and `mean_evaluator` (`Callable`).
             The output dictionary will contain the following extra key-values:
 
                 IoU : dict[tuple[int, int], np.ndarray]
                        A dictionary containing the IoU values for every
-                       image/class combination e.g. ious[(0,0)]
-                       would contain the IoU for image 0 and class 0.
-                       Each value is a np.ndarray with shape (n, m)
-                       where n is the number of detections and m is the number
-                       of ground truth boxes for that image/class combination.
+                       image/class combination e.g. `IoU[(0,0)]`
+                       would contain the IoU for image `0` and class `0`.
+                       Each value is a `np.ndarray` with shape `(n, m)`
+                       where `n` is the number of detections and `m` is
+                       the number of ground truth boxes for that image/class
+                       combination.
                 AP : np.ndarray
-                      Average precision: a np.ndarray of shape (T, R, K, A, M)
-                      containing the precision values.
+                      Average precision: a `np.ndarray` of shape
+                      `(T, R, K, A, M)` containing the precision values.
                       Here:
-                          - T is the number of IoU thresholds
-                          - R is the number of recall thresholds
-                          - K is the number of classes
-                          - A is the number of areas
-                          - M is the number of max detections per image
+                          - `T` is the number of IoU thresholds
+                          - `R` is the number of recall thresholds
+                          - `K` is the number of classes
+                          - `A` is the number of areas
+                          - `M` is the number of max detections per image
                 AR : np.ndarray
-                     A np.ndarray of shape (T, K, A, M) containing the
+                     A `np.ndarray` of shape `(T, K, A, M)` containing the
                      averag recall values.
                      Here:
-                         - T is the number of IoU thresholds
-                         - K is the number of classes
-                         - A is the number of areas
-                         - M is the number of max detections per image
+                         - `T` is the number of IoU thresholds
+                         - `K` is the number of classes
+                         - `A` is the number of areas
+                         - `M` is the number of max detections per image
                 mean_evaluator : Callable
                     Mean evaluator function.
                     Parameters are:
                         iou_threshold : (float | list[float] | np.ndarray
                                          | None), optional
                             IoU threshold on which calculate the mean.
-                            It can be a float, a list of floats, np.ndarray
-                            or None; all values must be inlcuded in the
+                            It can be a `float`, a list of floats, `np.ndarray`
+                            or `None`; all values must be inlcuded in the
                             constructor argument `iou_thresholds`.
-                            If None, all input `iou_thresholds` will be used.
-                            The default is None.
+                            If `None`, all input `iou_thresholds` will be used.
+                            The default is `None`.
                         area_range_key : (str | list[str] | np.ndarray
                                           | None), optional
                             Area range key on which calculate the mean.
-                            It can be a str, a list of strings, np.ndarray,
-                            or None; all values must be included in the
+                            It can be a `str`, a list of strings, `np.ndarray`,
+                            or `None`; all values must be included in the
                             constructor argument `area_ranges`.
-                            If None, all input `area_ranges` keys will be used.
-                            The default is None.
+                            If `None`, all input `area_ranges` keys will be
+                            used.
+                            The default is `None`.
                         max_detection_threshold : (int | list[int] |
                                                    np.ndarray | None), optional
                             Threshold on maxiumum detections per image on
                             which calculate the mean.
-                            It can be a int, a list of ints, np.ndarray
-                            or None; all values must be inlcuded in the
+                            It can be a `int`, a list of integers, `np.ndarray`
+                            or `None`; all values must be inlcuded in the
                             constructor argument `max_detection_thresholds`.
-                            If None, all input `max_detection_thresholds`
+                            If `None`, all input `max_detection_thresholds`
                             will be used.
-                            The default is None.
+                            The default is `None`.
                         label_id : (int | list[int] | np.ndarray
                                     | None), optional
                             Label ids on which calculate the mean.
-                            If `class_metrics` is True, `label_id` must be
+                            If `class_metrics` is `True`, `label_id` must be
                             included in the label ids of the provided `y_true`.
-                            If `class_metrics` is False, `label_id` must be -1
-                            (in this case equivalent to None).
-                            If None, all labels will be used.
-                            The default is None.
+                            If `class_metrics` is `False`, `label_id` must be
+                            `-1` (in this case equivalent to `None`).
+                            If `None`, all labels will be used.
+                            The default is `None`.
                         metrics : (Literal["AP", "AR"]
                                    | list[Literal["AP", "AR"]] | None),
                                    optional
                             Metrics on which calculate the mean.
-                            If None, both "AP" and "AR" will be used.
-                            The default is None.
+                            If `None`, both `"AP"` and `"AR"` will be used.
+                            The default is `None`.
                         include_spec : bool, optional
                             Whether to include mean settings specification.
-                            The default is False.
+                            The default is `False`.
                         prefix : str, optional
                             Prefix to add to metrics keys.
                             The default is `m`.
 
         Returns
         -------
         dict[str, float | int | list[int] | dict | np.ndarray | partial]
             The format of the output string metric ids is defined as:
 
             `{metric}@[{iou_thresholds} | {area_ranges}
                       | {max_detection_thresholds}]`
 
-            If a field is None, the corresponding string field will be emtpy,
+            If a field is `None`, the corresponding string field will be emtpy,
             e.g., `{metric}@[{iou_thresholds} | {area_ranges}]`
             indicate metrics calculated without limit to detections per image,
             i.e. `max_detections_thresholds` set to `None`.
             Assuming that the parameters passed to the constructor
             are the default ones (COCO), the output dictionary will
             contain the following key-values: <br>
                 `mAP@[.5 | all | 100]` <br>
@@ -441,15 +443,15 @@
             Label id.
         label_ids : list[int]
             Overall label ids.
 
         Returns
         -------
         np.ndarray
-            np.ndarray containing IoU values between `y_true` and `y_pred`.
+            `np.ndarray` containing IoU values between `y_true` and `y_pred`.
         """
         if self.class_metrics:
             y_true_ = y_true[image_id, label_id]
             y_pred_ = y_pred[image_id, label_id]
         else:
             y_true_ = reduce(
                 lambda x, y: x+y,
@@ -515,15 +517,15 @@
         ious : dict
             IoU dictionary.
 
         Returns
         -------
         dict[str, Any] | None
             Dictionary containing results given image and label.
-            None if there is no ground-truths and detections for that
+            `None` if there is no ground-truths and detections for that
             specific `image_id` and `label_id`.
         """
         if self.class_metrics:
             y_true_ = y_true[image_id, label_id]
             y_pred_ = y_pred[image_id, label_id]
         else:
             y_true_ = reduce(
@@ -825,63 +827,63 @@
         """
         Calculate mean for Average-Precision (mAP) and Average-Recall (mAR).
 
         Parameters
         ----------
         iou_threshold : float | list[float] | np.ndarray | None, optional
             IoU threshold on which calculate the mean.
-            It can be a float, a list of floats, np.ndarray
-            or None; all values must be inlcuded in the
+            It can be a `float`, a list of floats, `np.ndarray`
+            or `None`; all values must be inlcuded in the
             constructor argument `iou_thresholds`.
-            If None, all input `iou_thresholds` will be used.
-            The default is None.
+            If `None`, all input `iou_thresholds` will be used.
+            The default is `None`.
         area_range_key : str | list[str] | np.ndarray | None, optional
             Area range key on which calculate the mean.
-            It can be a str, a list of strings, np.ndarray,
-            or None; all values must be included in the
+            It can be a `str`, a list of strings, `np.ndarray`,
+            or `None`; all values must be included in the
             constructor argument `area_ranges`.
-            If None, all input `area_ranges` keys will be used.
-            The default is None.
+            If `None`, all input `area_ranges` keys will be used.
+            The default is `None`.
         max_detection_threshold : int | list[int] |
                                    np.ndarray | None), optional
-            Threshold on maxiumum detections per image on
+            Threshold on maximum detections per image on
             which calculate the mean.
-            It can be a int, a list of ints, np.ndarray
-            or None; all values must be inlcuded in the
+            It can be a `int`, a list of integers, `np.ndarray`
+            or `None`; all values must be inlcuded in the
             constructor argument `max_detection_thresholds`.
-            If None, all input `max_detection_thresholds`
+            If `None`, all input `max_detection_thresholds`
             will be used.
-            The default is None.
+            The default is `None`.
         label_id : int | list[int] | np.ndarray | None, optional
             Label ids on which calculate the mean.
-            If `class_metrics` is True, `label_id` must be
+            If `class_metrics` is `True`, `label_id` must be
             included in the label ids of the provided `y_true`.
-            If `class_metrics` is False, `label_id` must be -1 (in this case
-            equivalent to None).
-            If None, all labels will be used.
-            The default is None.
+            If `class_metrics` is `False`, `label_id` must be `-1`
+            (in this case equivalent to `None`).
+            If `None`, all labels will be used.
+            The default is `None`.
         metrics : Literal["AP", "AR"] | list[Literal["AP", "AR"]] | None,
                   optional
             Metrics on which calculate the mean.
-            If None, both "AP" and "AR" will be used.
-            The default is None.
+            If `None`, both `"AP"` and `"AR"` will be used.
+            The default is `None`.
         include_spec : bool, optional
             Whether to include mean settings specification.
-            The default is False.
+            The default is `False`.
         prefix : str, optional
             Prefix to add to metrics keys.
             The default is `m`.
         results : dict[str, Any] | type[_Missing], optional
             Dictionary containing aggregated images results.
-            If _Missing an error will be raised.
-            The default is _Missing.
+            If `_Missing` an error will be raised.
+            The default is `_Missing`.
         label_ids : list[int] | np.ndarray | type[_Missing], optional
-            All label ids found in y_true.
-            If _Missing an error will be raised.
-            The default is _Missing.
+            All label ids found in `y_true`.
+            If `_Missing` an error will be raised.
+            The default is `_Missing`.
 
         Returns
         -------
         dict[str, float | dict[str, list]]
             Dictionary containing the values of precision and recall.
             If `include_spec` input parameters info will be added.
         """
@@ -1002,16 +1004,16 @@
 
         Parameters
         ----------
         mean_evaluator : Callable
             Mean evaluator function.
         label_id : int | list[int] | np.ndarray | None
             Label ids.
-            If None, all labels will be used.
-            The default is None.
+            If `None`, all labels will be used.
+            The default is `None`.
         prefix : str
             Prefix to add to metrics keys.
 
         Returns
         -------
         dict[str, float | dict[str, list]]
             Dictionary with metrics output.
@@ -1048,15 +1050,15 @@
         y_true: np.ndarray | list,
         y_pred: np.ndarray | list,
         iscrowd: np.ndarray | list[bool] | list[int] | None = None,
         ) -> np.ndarray:
     """
     Calculate IoU between bounding boxes.
 
-    Single bounding boxes must be in `xywh` format, i.e.
+    Single bounding boxes must be in `"xywh"` format, i.e.
         [xmin, ymin, width, height]
 
     The standard iou of a ground truth `y_true` and detected
     `y_pred` object is:
 
     $$iou(\\text{y_true}, \\text{y_pred}) =
         \\frac{\\text{y_true} \\bigcap \\text{y_pred}}
```

### Comparing `od-metrics-0.0.12/src/od_metrics/utils.py` & `od-metrics-1.0.0/src/od_metrics/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     """Sentinel class for missing values."""
 
 
 def to_array(
         input_: Any,
         ) -> np.ndarray:
     """
-    Trasform input to np.ndarray.
+    Trasform input to `np.ndarray`.
 
     Parameters
     ----------
     input_ : Any | None, optional
         Input to be converted.
 
     Returns
     -------
     np.ndarray
-        Input converted to numpy array.
+        Input converted to `np.ndarray`.
     """
     if not isinstance(input_, np.ndarray):
         output = np.array(input_)
     else:
         output = input_
 
     if output.ndim == 0:
@@ -52,22 +52,22 @@
 
     Returns a list of indices where elements from `array1` are present
     in `array2`.
 
     Parameters
     ----------
     array1 : np.ndarray
-        The np.ndarray to search for elements.
+        The `np.ndarray` to search for elements.
     array2 : np.ndarray
-        The np.ndarray to search for matches.
+        The `np.ndarray` to search for matches.
 
     Returns
     -------
     np.ndarray
-        A np.ndarray of indices where elements from `array1` are
+        A `np.ndarray` of indices where elements from `array1` are
         present in `array2`.
     """
     return np.sort(np.where(np.isin(
         array1, array2))[0])
 
 
 def xyxy_xywh(bbox: list[float]) -> list[float]:
@@ -78,78 +78,78 @@
     ----------
     bbox : list[float]
         Input bounding box.
 
     Returns
     -------
     list[float]
-        Bounding box in `xywh` format.
+        Bounding box in `"xywh"` format.
     """
     return [
         bbox[0],
         bbox[1],
         bbox[2] - bbox[0],
         bbox[3] - bbox[1]
         ]
 
 
 def cxcywh_xywh(bbox: list[float]) -> list[float]:
     """
-    Change bounding box format from `cxcywh` to `xywh`.
+    Change bounding box format from `"cxcywh"` to `"xywh"`.
 
     Parameters
     ----------
     bbox : list[float]
         Input bounding box.
 
     Returns
     -------
     list[float]
-        Bounding box in `xywh` format.
+        Bounding box in `"xywh"` format.
     """
     return [
         bbox[0] - bbox[2] / 2,
         bbox[1] - bbox[3] / 2,
         bbox[2],
         bbox[3]
         ]
 
 
 def to_xywh(
         bbox: list[float],
         box_format: Literal["xyxy", "xywh", "cxcywh"],
         ) -> list[float]:
     """
-    Change bounding box format to `xywh`.
+    Change bounding box format to `"xywh"`.
 
     Parameters
     ----------
     bbox : list[float]
         Input bounding box.
     box_format : Literal["xyxy", "xywh", "cxcywh"]
         Input bounding box format.
-        It can be `xyxy`, `xywh` or `cxcywh`.
+        It can be `"xyxy"`, `"xywh"` or `"cxcywh"`.
 
     Raises
     ------
     ValueError
-        If `box_format` not in `xyxy`, `xywh`, `cxcywh`.
+        If `box_format` not one of `"xyxy"`, `"xywh"`, `"cxcywh"`.
 
     Returns
     -------
     list[float]
-        Bounding box in `xywh` format.
+        Bounding box in `"xywh"` format.
     """
     if box_format == "xywh":
         return bbox
     if box_format == "xyxy":
         return xyxy_xywh(bbox)
     if box_format == "cxcywh":
         return cxcywh_xywh(bbox)
-    raise ValueError("`box_format` can be `xyxy`, `xywh`, `cxcywh`. "
+    raise ValueError("`box_format` can be `'xyxy'`, `'xywh'`, `'cxcywh'`. "
                      f"Found {box_format}")
 
 
 def get_suffix(
         iou_threshold: np.ndarray,
         area_range_key: np.ndarray,
         max_detection_threshold: np.ndarray,
```

### Comparing `od-metrics-0.0.12/src/od_metrics/validators.py` & `od-metrics-1.0.0/src/od_metrics/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,21 +40,21 @@
     default_flag : Any
         Flag for default value.
     default_value : np.ndarray
         Default value.
     dtype : type[int] | type[str] | type[float]
         Value dtypes.
     allow_none : bool
-        Whether to allow None values.
+        Whether to allow `None` values.
 
     Raises
     ------
     ValueError
         If `value` is neither a `dtype`, a list of `dtype` or
-        a 1-dimensional np.ndarray, or None if `allow_none` is True.
+        a 1-dimensional `np.ndarray`, or `None` if `allow_none=True`.
         If `value` contains duplicate values.
 
     Returns
     -------
     np.ndarray
     """
     # dtype
@@ -80,17 +80,17 @@
     elif (value is None) and allow_none:
         _value = np.array([None])
 
     else:
         _msg = (
             f"Invalid value for {name}. "
             f"{name} should be a {dtype.__name__}, list of {dtype.__name__} "
-            "or a 1-dimensional np.ndarray"
+            "or a 1-dimensional `np.ndarray`."
             )
-        _msg += "or None." if allow_none else "."
+        _msg += "or `None`." if allow_none else "."
         raise ValueError(_msg)
 
     # Check duplicates
     has_duplicates = any(count > 1 for count in
                          np.unique(_value, return_counts=True)[1])
 
     if has_duplicates:
@@ -122,16 +122,16 @@
     default_value :  dict[str, list[float]]
         Default value.
 
     Raises
     ------
     ValueError
         If `value` is neither a dictionary with string keys and values
-        as lists/np.ndarray of 2 integers/floats, with first element less or
-        equal than second, or None.
+        as lists/`np.ndarray` of 2 integers/floats, with first element less or
+        equal than second, or `None`.
         If `value` contains duplicate values.
 
     Returns
     -------
     dict[str | None, list[float]]
     """
     # dict[,np.ndarray] --> dict[, list]
@@ -157,18 +157,18 @@
     # Missing
     elif value is default_flag:
         _value = default_value
     else:
         raise ValueError(
             f"Invalid value for {name}. "
             f"{name} should be either:\n"
-            "- A dictionary with string keys and values as lists/np.ndarray "
+            "- A dictionary with string keys and values as lists/`np.ndarray` "
             "of 2 integers/floats, with first element less or equal than "
             "second.\n"
-            "- None.\n"
+            "- `None`.\n"
             )
     # Check duplicates in .values()
     _values = [tuple(x) if isinstance(x, list) else tuple([x])
                for x in _value.values()]
     has_duplicates = any(
         count > 1 for count in Counter(_values).values())
 
@@ -177,15 +177,15 @@
             f"Duplicate values found in {name}. "
             f"{name} should not contain any duplicate values."
             )
     return _value
 
 
 class ConstructorModel(BaseModel):
-    """`__init__` method Model."""
+    """`__init__()` method Model."""
 
     iou_thresholds: np.ndarray
     recall_thresholds: np.ndarray
     max_detection_thresholds: np.ndarray
     area_ranges: dict[Optional[str], list[float]]
     class_metrics: bool
     box_format: Literal["xyxy", "xywh", "cxcywh"]
@@ -206,15 +206,15 @@
         Validate `iou_thresholds` and `recall_thresholds` fields.
 
         Parameters
         ----------
         value : Any
             Input value.
         info : ValidationInfo
-            Pydantic ValidationInfo
+            Pydantic `ValidationInfo`.
 
         Raises
         ------
         ValueError
             If context or field name informations are missing.
 
         Returns
@@ -250,15 +250,15 @@
         Validate `max_detection_thresholds` field.
 
         Parameters
         ----------
         value : Any
             Input value.
         info : ValidationInfo
-            Pydantic ValidationInfo
+            Pydantic `ValidationInfo`.
 
         Raises
         ------
         ValueError
             If context or field name informations are missing.
 
         Returns
@@ -294,15 +294,15 @@
         Validate `area_ranges` field.
 
         Parameters
         ----------
         value : Any
             Input value.
         info : ValidationInfo
-            Pydantic ValidationInfo.
+            Pydantic `ValidationInfo`.
 
         Raises
         ------
         ValueError
             If context or field name informations are missing.
 
         Returns
@@ -551,27 +551,27 @@
 
 
 def _convert_y_true(
         data: list[YTrueInputModel],
         box_format: Literal["xyxy", "xywh", "cxcywh"],
         ) -> list[YTrueOutputModel]:
     """
-    Convert a list YTrueInputModel to a list of YTrueOutputModel.
+    Convert a list of `YTrueInputModel` to a list of `YTrueOutputModel`.
 
     Parameters
     ----------
     data : list[YTrueInputModel]
-        List of YTrueInputModel.
+        List of `YTrueInputModel`.
     box_format : Literal["xyxy", "xywh", "cxcywh"]
         Input format of given boxes.
 
     Returns
     -------
     list[YTrueOutputModel]
-        YTrueOutputModel list.
+        List of `YTrueOutputModel`.
     """
     annotations = []
     id_ = 1
     for image_id, image_anns in enumerate(data):
         n_annotations = len(image_anns.boxes)
         for i in range(n_annotations):
             # Common
@@ -600,27 +600,27 @@
 
 
 def _convert_y_pred(
         data: list[YPredInputModel],
         box_format: Literal["xyxy", "xywh", "cxcywh"],
         ) -> list[YPredOutputModel]:
     """
-    Convert a list of YPredInputModel to a list of YPredOutputModel.
+    Convert a list of `YPredInputModel` to a list of `YPredOutputModel`.
 
     Parameters
     ----------
     data : list[YPredInputModel]
-        List of YPredInputModel.
+        List of `YPredInputModel`.
     box_format : Literal["xyxy", "xywh", "cxcywh"]
         Input format of given boxes.
 
     Returns
     -------
     list[YPredOutputModel]
-        YPredOutputModel list.
+        List of `YPredOutputModel`.
     """
     annotations = []
     id_ = 1
     for image_id, image_anns in enumerate(data):
         n_annotations = len(image_anns.boxes)
         for i in range(n_annotations):
             # Common
@@ -668,15 +668,15 @@
         Parse annotations.
 
         Parameters
         ----------
         data : dict
             Input annotations.
         info : ValidationInfo
-            Pydantic ValidationInfo.
+            Pydantic `ValidationInfo`.
 
         Returns
         -------
         dict
             Ground truth or predictions annotations.
         """
         if info.context is None or "box_format" not in info.context:
@@ -734,15 +734,15 @@
         Validate `iou_threshold` field.
 
         Parameters
         ----------
         value : Any
             Input value.
         info : ValidationInfo
-            Pydantic ValidationInfo
+            Pydantic `ValidationInfo`.
 
         Returns
         -------
         np.ndarray
         """
         if (
                 info.context is None
@@ -773,15 +773,15 @@
         Validate `area_range_key` field.
 
         Parameters
         ----------
         value : Any
             Input value.
         info : ValidationInfo
-            Pydantic ValidationInfo
+            Pydantic `ValidationInfo`.
 
         Returns
         -------
         np.ndarray
         """
         if (
                 info.context is None
@@ -812,15 +812,15 @@
         Validate `max_detection_threshold` field.
 
         Parameters
         ----------
         value : Any
             Input value.
         info : ValidationInfo
-            Pydantic ValidationInfo
+            Pydantic `ValidationInfo`.
 
         Returns
         -------
         np.ndarray
         """
         if (
                 info.context is None
```

### Comparing `od-metrics-0.0.12/src/od_metrics.egg-info/PKG-INFO` & `od-metrics-1.0.0/src/od_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-metrics
-Version: 0.0.12
+Version: 1.0.0
 Summary: Object Detection metrics.
 Home-page: https://github.com/EMalagoli92/OD-metrics
 Author: EMalagoli92
 Author-email: emala.892@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 0.0.12 Summary: Object
-Detection metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
+Metadata-Version: 2.1 Name: od-metrics Version: 1.0.0 Summary: Object Detection
+metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
 EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
                                 logo_light.svg]
```

### Comparing `od-metrics-0.0.12/tests/test_pycoco_equivalence.py` & `od-metrics-1.0.0/tests/test_pycoco_equivalence.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,29 +29,29 @@
 @unittest.skipUnless(
     _PYCOCOTOOLS_AVAILABLE,
     "This unittest needs `pycocotools`. Please intall by "
     "running `pip install pycocotools`"
     )
 @parameterized_class(TESTS)
 class TestPyCocoEquivalenceMetrics(unittest.TestCase):
-    """Test equivalence: ODMetrics and pycocotools.COCOeval"""
+    """Test equivalence: ODMetrics and `pycocotools.COCOeval()` method."""
 
     metrics_settings: dict
     compute_settings: dict
     annotations_settings: dict
     mean_evaluator_settings: dict
     exceptions: dict
 
     def get_pycoco_params(
             self,
             od_metrics_params: dict[str, Any],
             pycoco_params: pycocotools.cocoeval.Params,
             real_max_detections: int | None,
             ) -> pycocotools.cocoeval.Params:
-        """Set pycocotools.cocoeval.Params."""
+        """Set `pycocotools.cocoeval.Params`."""
         pycoco_params.iouThrs = od_metrics_params["iou_thresholds"]
         pycoco_params.recThrs = od_metrics_params["recall_thresholds"]
         # Handle max_detection_thresholds case
         pycoco_params.maxDets = (
             od_metrics_params["max_detection_thresholds"]
             if not np.equal(
                     od_metrics_params["max_detection_thresholds"],
@@ -67,15 +67,15 @@
         return pycoco_params
 
     @staticmethod
     def _test_ious(
             od_metrics_ious: dict,
             pycoco_ious: dict,
             ) -> bool:
-        """Test equivalence: od-metrics ious and pycocotools.ious."""
+        """Test equivalence: od-metrics ious and `pycocotools.ious`."""
         od_metrics_ious = dict(map(
             lambda x: (x[0], [] if np.array_equal(x[1], np.array([]))
                        else x[1]), od_metrics_ious.items()
             )
         )
         return test_equality(
             od_metrics_ious,
@@ -83,15 +83,15 @@
             )
 
     @staticmethod
     def _test_aggregate(
             od_metrics_output: dict,
             pycoco_eval: dict,
             ) -> bool:
-        """Test equivalence: od-metrics and pycocotools aggregated results."""
+        """Test equivalence: od-metrics and `pycocotools` aggregated result."""
         od_metrics_output = copy.deepcopy(od_metrics_output)
         pycoco_eval = copy.deepcopy(pycoco_eval)
 
         _keys = ["precision", "recall"]
         od_metrics_output = rename_dict(
             dict_=od_metrics_output,
             rename_dict_keys={"AP": "precision",
@@ -104,15 +104,15 @@
 
     @staticmethod
     def _test_summary(
             od_metrics_output: dict,
             pycoco_stats: np.ndarray,
             is_default_coco: bool,
             ) -> bool:
-        """Test equivalence: od-metrics summary and pycocotools summary."""
+        """Test equivalence: od-metrics summary and `pycocotools` summary."""
         # Check default settings
         if is_default_coco:
             od_metrics_stats = np.array([
                 od_metrics_output["mAP@[.5:.95 | all | 100]"],
                 od_metrics_output["mAP@[.5 | all | 100]"],
                 od_metrics_output["mAP@[.75 | all | 100]"],
                 od_metrics_output["mAP@[.5:.95 | small | 100]"],
@@ -131,15 +131,15 @@
                 pycoco_stats,
                 od_metrics_stats,
                 )
         return True
 
     # pylint: disable=R0915, R0912, R0914
     def test_equivalence(self) -> None:
-        """Test equivalence: od-metrics and pycocotools."""
+        """Test equivalence: od-metrics and `pycocotools`."""
         # Get annotations
         y_true_od_metrics = annotations_generator(
             **self.annotations_settings["y_true"])
         y_pred_od_metrics = annotations_generator(
             **self.annotations_settings["y_pred"], include_score=True)
         # max detections: Only used for max_detections_thresholds=None case
         real_max_detections = (
@@ -297,15 +297,15 @@
 
 @unittest.skipUnless(
     _PYCOCOTOOLS_AVAILABLE,
     "This unittest needs `pycocotools`. Please intall by "
     "running `pip install pycocotools`"
     )
 class TestPyCocoEquivalenceIoU(unittest.TestCase):
-    """Test equivalence: od-metrics and pycocotools iou function."""
+    """Test equivalence: od-metrics and `pycocotools` iou function."""
 
     HIGH = 100000
     SIZE = 3000
 
     def test_iou(self) -> None:
         """Test IoU."""
         iscrowd = list(map(
```

