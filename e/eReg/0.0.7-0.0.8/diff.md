# Comparing `tmp/ereg-0.0.7-py3-none-any.whl.zip` & `tmp/ereg-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 20377 bytes, number of entries: 16
+Zip file size: 20675 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      171 b- defN 80-Jan-01 00:00 ereg/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ereg/cli/__init__.py
 -rw-r--r--  2.0 unx     4031 b- defN 80-Jan-01 00:00 ereg/cli/run.py
 -rw-r--r--  2.0 unx     3617 b- defN 80-Jan-01 00:00 ereg/configurations/default_rigid.yaml
 -rw-r--r--  2.0 unx     3600 b- defN 80-Jan-01 00:00 ereg/configurations/sample_config.yaml
 -rw-r--r--  2.0 unx     1575 b- defN 80-Jan-01 00:00 ereg/functional.py
--rw-r--r--  2.0 unx    31452 b- defN 80-Jan-01 00:00 ereg/registration.py
+-rw-r--r--  2.0 unx    33997 b- defN 80-Jan-01 00:00 ereg/registration.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 ereg/utils/__init__.py
 -rw-r--r--  2.0 unx      793 b- defN 80-Jan-01 00:00 ereg/utils/citation_reminder.py
 -rw-r--r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 ereg/utils/io.py
 -rw-r--r--  2.0 unx      866 b- defN 80-Jan-01 00:00 ereg/utils/metrics.py
--rw-r--r--  2.0 unx    11356 b- defN 80-Jan-01 00:00 ereg-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5874 b- defN 80-Jan-01 00:00 ereg-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ereg-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 ereg-0.0.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 ereg-0.0.7.dist-info/RECORD
-16 files, 66037 bytes uncompressed, 18335 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx    11356 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5874 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 ereg-0.0.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 ereg-0.0.8.dist-info/RECORD
+16 files, 68582 bytes uncompressed, 18633 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: ereg/utils/io.py
 Comment: 
 
 Filename: ereg/utils/metrics.py
 Comment: 
 
-Filename: ereg-0.0.7.dist-info/LICENSE
+Filename: ereg-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: ereg-0.0.7.dist-info/METADATA
+Filename: ereg-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: ereg-0.0.7.dist-info/WHEEL
+Filename: ereg-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: ereg-0.0.7.dist-info/entry_points.txt
+Filename: ereg-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: ereg-0.0.7.dist-info/RECORD
+Filename: ereg-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ereg/registration.py

```diff
@@ -175,24 +175,26 @@
                 target_image=target_image,
                 moving_image=moving_image,
             )
         if transform_file is not None:
             sitk.WriteTransform(self.transform, transform_file)
 
         # apply composite transform if provided
-        if self.parameters["composite_transform"] is not None:
+        self.parameters["composite_transform"] = self.parameters.get(
+            "composite_transform", None
+        )
+        if self.parameters.get("composite_transform"):
             self.logger.info("Applying composite transform.")
             transform_composite = sitk.ReadTransform(
                 self.parameters["composite_transform"]
             )
             self.transform = sitk.CompositeTransform(
                 transform_composite, self.transform
             )
 
-        if self.parameters["composite_transform"]:
             self.logger.info("Applying previous transforms.")
             current_transform = None
             for previous_transform in self.parameters["previous_transforms"]:
                 previous_transform = sitk.ReadTransform(previous_transform)
                 current_transform = (
                     sitk.CompositeTransform(previous_transform, self.transform)
                     if current_transform is None
@@ -252,15 +254,16 @@
                 target_image = read_image_and_cast_to_32bit_float(target_image)
                 moving_image = read_image_and_cast_to_32bit_float(moving_image)
 
                 self.logger.info("Resampling image.")
                 resampler = sitk.ResampleImageFilter()
                 resampler.SetReferenceImage(target_image)
                 interpolator_type = self.interpolator_type.get(
-                    self.parameters["interpolator"]
+                    self.parameters.get("interpolator", "linear").lower(),
+                    sitk.sitkLinear,
                 )
                 resampler.SetInterpolator(interpolator_type)
                 resampler.SetDefaultPixelValue(0)
                 resampler.SetTransform(self.transform)
                 output_image_struct = resampler.Execute(moving_image)
                 sitk.WriteImage(output_image_struct, output_image)
                 self.ssim_score = get_ssim(target_image, output_image_struct)
@@ -384,256 +387,329 @@
 
         physical_units = 1
         dimension = target_image.GetDimension()
         for dim in range(dimension):
             physical_units *= target_image.GetSpacing()[dim]
 
         self.logger.info("Initializing registration.")
-        R = sitk.ImageRegistrationMethod()
-        metric = self.parameters["metric"].lower()
+        registration = sitk.ImageRegistrationMethod()
+        self.parameters["metric_parameters"] = self.parameters.get(
+            "metric_parameters", {}
+        )
+        metric = (
+            self.parameters["metric_parameters"].get("type", "mean_squares").lower()
+        )
         if (
             (metric == "mattesmutualinformation")
             or (metric == "mattes")
             or (metric == "mmi")
             or ("mattes" in metric)
         ):
-            R.SetMetricAsMattesMutualInformation(
-                numberOfHistogramBins=self.parameters["metric_parameters"][
-                    "histogram_bins"
-                ]
+            registration.SetMetricAsMattesMutualInformation(
+                numberOfHistogramBins=self.parameters["metric_parameters"].get(
+                    "histogram_bins", 50
+                ),
             )
         elif (
             (metric == "antsneighborhoodcorrelation")
             or (metric == "ants")
             or ("ants" in metric)
         ):
-            R.SetMetricAsANTSNeighborhoodCorrelation(
-                radius=self.parameters["metric_parameters"]["radius"]
+            registration.SetMetricAsANTSNeighborhoodCorrelation(
+                radius=self.parameters["metric_parameters"].get("radius", 5)
             )
         elif metric == "correlation":
-            R.SetMetricAsCorrelation()
+            registration.SetMetricAsCorrelation()
         elif metric == "demons":
-            R.SetMetricAsDemons(
-                intensityDifferenceThreshold=self.parameters["metric_parameters"][
-                    "intensityDifferenceThreshold"
-                ]
+            registration.SetMetricAsDemons(
+                intensityDifferenceThreshold=self.parameters["metric_parameters"].get(
+                    "intensityDifferenceThreshold", 0.001
+                ),
             )
         elif (
             (metric == "joint_histogram_mutual_information")
             or (metric == "joint")
             or ("joint" in metric)
         ):
-            R.SetMetricAsJointHistogramMutualInformation(
-                numberOfHistogramBins=self.parameters["metric_parameters"][
-                    "histogram_bins"
-                ],
-                varianceForJointPDFSmoothing=self.parameters["metric_parameters"][
-                    "varianceForJointPDFSmoothing"
-                ],
+            registration.SetMetricAsJointHistogramMutualInformation(
+                numberOfHistogramBins=self.parameters["metric_parameters"].get(
+                    "histogram_bins", 50
+                ),
+                varianceForJointPDFSmoothing=self.parameters["metric_parameters"].get(
+                    "varianceForJointPDFSmoothing", 1.5
+                ),
             )
         else:
-            R.SetMetricAsMeanSquares()
+            registration.SetMetricAsMeanSquares()
 
         sampling_strategy_parsed = {
-            "random": R.RANDOM,
-            "regular": R.REGULAR,
-            "none": R.NONE,
+            "random": registration.RANDOM,
+            "regular": registration.REGULAR,
+            "none": registration.NONE,
         }
-        R.SetMetricSamplingStrategy(
-            sampling_strategy_parsed[self.parameters["sampling_strategy"]]
+        registration.SetMetricSamplingStrategy(
+            sampling_strategy_parsed[
+                self.parameters.get("sampling_strategy", "random").lower()
+            ]
         )
-        R.SetMetricSamplingPercentagePerLevel(self.parameters["sampling_percentage"])
-
-        if self.parameters["optimizer"] == "regular_step_gradient_descent":
-            R.SetOptimizerAsRegularStepGradientDescent(
-                minStep=self.parameters["optimizer_parameters"]["min_step"],
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                learningRate=self.parameters["optimizer_parameters"]["learningrate"],
-                # gradientMagnitudeTolerance=grad_tolerance,
-                relaxationFactor=self.parameters["optimizer_parameters"]["relaxation"],
-                gradientMagnitudeTolerance=self.parameters["optimizer_parameters"][
-                    "tolerance"
-                ],
-                estimateLearningRate=R.EachIteration,
-                maximumStepSizeInPhysicalUnits=self.parameters["optimizer_parameters"][
-                    "max_step"
-                ]
+        sampling_rate = self.parameters.get("sampling_percentage", 0.01)
+        if isinstance(sampling_rate, float):
+            registration.SetMetricSamplingPercentage(sampling_rate)
+        elif type(sampling_rate) in [np.ndarray, list]:
+            registration.SetMetricSamplingPercentagePerLevel(sampling_rate)
+
+        # initialize some defaults
+        self.parameters["optimizer_parameters"] = self.parameters.get(
+            "optimizer_parameters", {}
+        )
+        self.parameters["optimizer_parameters"]["type"] = self.parameters[
+            "optimizer_parameters"
+        ].get("type", "regular_step_gradient_descent")
+        # set the optimizer parameters as either floats or integers
+        for key in self.parameters["optimizer_parameters"]:
+            if key not in ["type"]:
+                self.parameters["optimizer_parameters"][key] = float(
+                    self.parameters["optimizer_parameters"][key]
+                )
+                if key == "iterations":
+                    self.parameters["optimizer_parameters"][key] = int(
+                        self.parameters["optimizer_parameters"][key]
+                    )
+        if (
+            self.parameters["optimizer_parameters"].get("type").lower()
+            == "regular_step_gradient_descent"
+        ):
+            registration.SetOptimizerAsRegularStepGradientDescent(
+                minStep=self.parameters["optimizer_parameters"].get("min_step", 1e-6),
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                learningRate=self.parameters["optimizer_parameters"].get(
+                    "learningrate", 1.0
+                ),
+                relaxationFactor=self.parameters["optimizer_parameters"].get(
+                    "relaxation", 0.5
+                ),
+                gradientMagnitudeTolerance=self.parameters["optimizer_parameters"].get(
+                    "tolerance", 1e-4
+                ),
+                estimateLearningRate=registration.EachIteration,
+                maximumStepSizeInPhysicalUnits=self.parameters[
+                    "optimizer_parameters"
+                ].get("max_step", 1.0)
                 * physical_units,
             )
-        elif self.parameters["optimizer"] == "gradient_descent":
-            R.SetOptimizerAsGradientDescent(
-                learningRate=self.parameters["optimizer_parameters"]["learningrate"],
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                convergenceMinimumValue=self.parameters["optimizer_parameters"][
-                    "convergence_minimum"
-                ],
-                convergenceWindowSize=self.parameters["optimizer_parameters"][
-                    "convergence_window_size"
-                ],
-                estimateLearningRate=R.EachIteration,
-                maximumStepSizeInPhysicalUnits=self.parameters["optimizer_parameters"][
-                    "max_step"
-                ]
+        elif (
+            self.parameters["optimizer_parameters"].get("type").lower()
+            == "gradient_descent"
+        ):
+            registration.SetOptimizerAsGradientDescent(
+                learningRate=self.parameters["optimizer_parameters"].get(
+                    "learningrate", 1.0
+                ),
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                convergenceMinimumValue=self.parameters["optimizer_parameters"].get(
+                    "convergence_minimum", 1e-6
+                ),
+                convergenceWindowSize=self.parameters["optimizer_parameters"].get(
+                    "convergence_window_size", 10
+                ),
+                estimateLearningRate=registration.EachIteration,
+                maximumStepSizeInPhysicalUnits=self.parameters[
+                    "optimizer_parameters"
+                ].get("max_step", 1.0)
                 * physical_units,
             )
-        elif self.parameters["optimizer"] == "gradient_descent_line_search":
-            R.SetOptimizerAsGradientDescentLineSearch(
-                learningRate=self.parameters["optimizer_parameters"]["learningrate"],
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                convergenceMinimumValue=self.parameters["optimizer_parameters"][
-                    "convergence_minimum"
-                ],
-                convergenceWindowSize=self.parameters["optimizer_parameters"][
-                    "convergence_window_size"
-                ],
-                lineSearchLowerLimit=self.parameters["optimizer_parameters"][
-                    "line_search_lower_limit"
-                ],
-                lineSearchUpperLimit=self.parameters["optimizer_parameters"][
-                    "line_search_upper_limit"
-                ],
-                lineSearchEpsilon=self.parameters["optimizer_parameters"][
-                    "line_search_epsilon"
-                ],
-                lineSearchMaximumIterations=self.parameters["optimizer_parameters"][
-                    "line_search_maximum_iterations"
-                ],
-                estimateLearningRate=R.EachIteration,
-                maximumStepSizeInPhysicalUnits=self.parameters["optimizer_parameters"][
-                    "max_step"
-                ]
+        elif (
+            self.parameters["optimizer_parameters"].get("type").lower()
+            == "gradient_descent_line_search"
+        ):
+            registration.SetOptimizerAsGradientDescentLineSearch(
+                learningRate=self.parameters["optimizer_parameters"].get(
+                    "learningrate", 1.0
+                ),
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                convergenceMinimumValue=self.parameters["optimizer_parameters"].get(
+                    "convergence_minimum", 1e-6
+                ),
+                convergenceWindowSize=self.parameters["optimizer_parameters"].get(
+                    "convergence_window_size", 10
+                ),
+                lineSearchLowerLimit=self.parameters["optimizer_parameters"].get(
+                    "line_search_lower_limit", 0.0
+                ),
+                lineSearchUpperLimit=self.parameters["optimizer_parameters"].get(
+                    "line_search_upper_limit", 1.0
+                ),
+                lineSearchEpsilon=self.parameters["optimizer_parameters"].get(
+                    "line_search_epsilon", 0.01
+                ),
+                lineSearchMaximumIterations=self.parameters["optimizer_parameters"].get(
+                    "line_search_maximum_iterations", 20
+                ),
+                estimateLearningRate=registration.EachIteration,
+                maximumStepSizeInPhysicalUnits=self.parameters[
+                    "optimizer_parameters"
+                ].get("max_step", 1.0)
                 * physical_units,
             )
         elif (
-            self.parameters["optimizer"]
+            self.parameters["optimizer_parameters"].get("type").lower()
             == "Conjugate_step_gradient_descent_line_search"
         ):
-            R.SetOptimizerAsConjugateGradientLineSearch(
-                learningRate=self.parameters["optimizer_parameters"]["learningrate"],
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                convergenceMinimumValue=self.parameters["optimizer_parameters"][
-                    "convergence_minimum"
-                ],
-                convergenceWindowSize=self.parameters["optimizer_parameters"][
-                    "convergence_window_size"
-                ],
-                lineSearchLowerLimit=self.parameters["optimizer_parameters"][
-                    "line_search_lower_limit"
-                ],
-                lineSearchUpperLimit=self.parameters["optimizer_parameters"][
-                    "line_search_upper_limit"
-                ],
-                lineSearchEpsilon=self.parameters["optimizer_parameters"][
-                    "line_search_epsilon"
-                ],
-                lineSearchMaximumIterations=self.parameters["optimizer_parameters"][
-                    "line_search_maximum_iterations"
-                ],
-                estimateLearningRate=R.EachIteration,
-                maximumStepSizeInPhysicalUnits=self.parameters["optimizer_parameters"][
-                    "max_step"
-                ]
+            registration.SetOptimizerAsConjugateGradientLineSearch(
+                learningRate=self.parameters["optimizer_parameters"].get(
+                    "learningrate", 1.0
+                ),
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                convergenceMinimumValue=self.parameters["optimizer_parameters"].get(
+                    "convergence_minimum", 1e-6
+                ),
+                convergenceWindowSize=self.parameters["optimizer_parameters"].get(
+                    "convergence_window_size", 10
+                ),
+                lineSearchLowerLimit=self.parameters["optimizer_parameters"].get(
+                    "line_search_lower_limit", 0.0
+                ),
+                lineSearchUpperLimit=self.parameters["optimizer_parameters"].get(
+                    "line_search_upper_limit", 1.0
+                ),
+                lineSearchEpsilon=self.parameters["optimizer_parameters"].get(
+                    "line_search_epsilon", 0.01
+                ),
+                lineSearchMaximumIterations=self.parameters["optimizer_parameters"].get(
+                    "line_search_maximum_iterations", 20
+                ),
+                estimateLearningRate=registration.EachIteration,
+                maximumStepSizeInPhysicalUnits=self.parameters[
+                    "optimizer_parameters"
+                ].get("max_step", 1.0)
                 * physical_units,
             )
-        elif self.parameters["optimizer"] == "exhaustive":
-            R.SetOptimizerAsExhaustive(
-                numberOfSteps=self.parameters["optimizer_parameters"]["iterations"],
-                stepLength=self.parameters["optimizer_parameters"]["step_length"],
+        elif (
+            self.parameters["optimizer_parameters"].get("type").lower() == "exhaustive"
+        ):
+            registration.SetOptimizerAsExhaustive(
+                numberOfSteps=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                stepLength=self.parameters["optimizer_parameters"].get(
+                    "step_length", 0.1
+                ),
             )
-        elif self.parameters["optimizer"] == "amoeba":
-            R.SetOptimizerAsAmoeba(
+        elif self.parameters["optimizer_parameters"].get("type").lower() == "amoeba":
+            registration.SetOptimizerAsAmoeba(
                 numberOfIterations=self.parameters["optimizer_parameters"][
                     "iterations"
                 ],
                 simplexDelta=self.parameters["optimizer_parameters"]["simplex_delta"],
             )
-        elif self.parameters["optimizer"] == "lbfgsb":
-            R.SetOptimizerAsLBFGSB(
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                maximumNumberOfCorrections=self.parameters["optimizer_parameters"][
-                    "maximum_number_of_corrections"
-                ],
+        elif self.parameters["optimizer_parameters"].get("type").lower() == "lbfgsb":
+            registration.SetOptimizerAsLBFGSB(
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                maximumNumberOfCorrections=self.parameters["optimizer_parameters"].get(
+                    "maximum_number_of_corrections", 5
+                ),
                 maximumNumberOfFunctionEvaluations=self.parameters[
                     "optimizer_parameters"
-                ]["maximum_number_of_function_evaluations"],
-                costFunctionConvergenceFactor=self.parameters["optimizer_parameters"][
-                    "cost_function_convergence_factor"
-                ],
-            )
-        elif self.parameters["optimizer"] == "lbfgs2":
-            R.SetOptimizerAsLBFGS2(
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                solutionAccuracy=self.parameters["optimizer_parameters"][
-                    "solution_accuracy"
-                ],
-                hessianApproximateAccuracy=self.parameters["optimizer_parameters"][
-                    "hessian_approximate_accuracy"
-                ],
-                deltaConvergenceDistance=self.parameters["optimizer_parameters"][
-                    "delta_convergence_distance"
-                ],
-                deltaConvergenceTolerance=self.parameters["optimizer_parameters"][
-                    "delta_convergence_tolerance"
-                ],
-                lineSearchMaximumEvaluations=self.parameters["optimizer_parameters"][
-                    "line_search_maximum_evaluations"
-                ],
-                lineSearchMinimumStep=self.parameters["optimizer_parameters"][
-                    "line_search_minimum_step"
-                ],
-                lineSearchMaximumStep=self.parameters["optimizer_parameters"][
-                    "line_search_maximum_step"
-                ],
-                lineSearchAccuracy=self.parameters["optimizer_parameters"][
-                    "line_search_accuracy"
-                ],
+                ].get("maximum_number_of_function_evaluations", 2000),
+                costFunctionConvergenceFactor=self.parameters[
+                    "optimizer_parameters"
+                ].get("cost_function_convergence_factor", 1e7),
             )
-        elif self.parameters["optimizer"] == "one_plus_one_evolutionary":
-            R.SetOptimizerAsOnePlusOneEvolutionary(
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                epsilon=self.parameters["optimizer_parameters"]["epsilon"],
-                initialRadius=self.parameters["optimizer_parameters"]["initial_radius"],
-                growthFactor=self.parameters["optimizer_parameters"]["growth_factor"],
-                shrinkFactor=self.parameters["optimizer_parameters"]["shrink_factor"],
+        elif self.parameters["optimizer_parameters"].get("type").lower() == "lbfgs2":
+            registration.SetOptimizerAsLBFGS2(
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                solutionAccuracy=self.parameters["optimizer_parameters"].get(
+                    "solution_accuracy", 1e-7
+                ),
+                hessianApproximateAccuracy=self.parameters["optimizer_parameters"].get(
+                    "hessian_approximate_accuracy", 1e-7
+                ),
+                deltaConvergenceDistance=self.parameters["optimizer_parameters"].get(
+                    "delta_convergence_distance", 1e-5
+                ),
+                deltaConvergenceTolerance=self.parameters["optimizer_parameters"].get(
+                    "delta_convergence_tolerance", 1e-4
+                ),
+                lineSearchMaximumEvaluations=self.parameters[
+                    "optimizer_parameters"
+                ].get("line_search_maximum_evaluations", 20),
+                lineSearchMinimumStep=self.parameters["optimizer_parameters"].get(
+                    "line_search_minimum_step", 1e-20
+                ),
+                lineSearchMaximumStep=self.parameters["optimizer_parameters"].get(
+                    "line_search_maximum_step", 1e20
+                ),
+                lineSearchAccuracy=self.parameters["optimizer_parameters"].get(
+                    "line_search_accuracy", 0.9
+                ),
             )
-        elif self.parameters["optimizer"] == "powell":
-            R.SetOptimizerAsPowell(
-                numberOfIterations=self.parameters["optimizer_parameters"][
-                    "iterations"
-                ],
-                maximumLineIterations=self.parameters["optimizer_parameters"][
-                    "maximum_line_iterations"
-                ],
-                stepLength=self.parameters["optimizer_parameters"]["step_length"],
-                stepTolerance=self.parameters["optimizer_parameters"]["step_tolerance"],
-                valueTolerance=self.parameters["optimizer_parameters"][
-                    "value_tolerance"
-                ],
+        elif (
+            self.parameters["optimizer_parameters"].get("type").lower()
+            == "one_plus_one_evolutionary"
+        ):
+            registration.SetOptimizerAsOnePlusOneEvolutionary(
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                epsilon=self.parameters["optimizer_parameters"].get("epsilon", 1e-6),
+                initialRadius=self.parameters["optimizer_parameters"].get(
+                    "initial_radius", 1.0
+                ),
+                growthFactor=self.parameters["optimizer_parameters"].get(
+                    "growth_factor", 2.0
+                ),
+                shrinkFactor=self.parameters["optimizer_parameters"].get(
+                    "shrink_factor", 0.7
+                ),
+            )
+        elif self.parameters["optimizer_parameters"].get("type").lower() == "powell":
+            registration.SetOptimizerAsPowell(
+                numberOfIterations=self.parameters["optimizer_parameters"].get(
+                    "iterations", 200
+                ),
+                maximumLineIterations=self.parameters["optimizer_parameters"].get(
+                    "maximum_line_iterations", 20
+                ),
+                stepLength=self.parameters["optimizer_parameters"].get(
+                    "step_length", 1.0
+                ),
+                stepTolerance=self.parameters["optimizer_parameters"].get(
+                    "step_tolerance", 0.001
+                ),
+                valueTolerance=self.parameters["optimizer_parameters"].get(
+                    "value_tolerance", 0.001
+                ),
             )
 
-        # R.SetOptimizerScalesFromJacobian()
-        R.SetOptimizerScalesFromPhysicalShift()
+        # registration.SetOptimizerScalesFromJacobian()
+        registration.SetOptimizerScalesFromPhysicalShift()
 
-        R.SetShrinkFactorsPerLevel(self.parameters["shrink_factors"])
-        R.SetSmoothingSigmasPerLevel(self.parameters["smoothing_sigmas"])
-        R.SmoothingSigmasAreSpecifiedInPhysicalUnitsOn()
+        registration.SetShrinkFactorsPerLevel(
+            self.parameters.get("shrink_factors", [8, 4, 2])
+        )
+        registration.SetSmoothingSigmasPerLevel(
+            self.parameters.get("smoothing_sigmas", [3, 2, 1])
+        )
+        registration.SmoothingSigmasAreSpecifiedInPhysicalUnitsOn()
+
+        assert (
+            self.parameters.get("transform", "") in self.available_transforms
+        ), f"`transform`needs to be set to one of the following: {self.available_transforms}"
         transform_function = self._get_transform_wrapper(
             self.parameters["transform"], dimension
         )
         ## todo: evaluate the viability of having default options for "rigid", "affine", and "deformable" registrations
         # rigid_registration = False
         # # euler transforms need special processing
         # if isinstance(transform_function, sitk.Euler3DTransform) or isinstance(
@@ -654,14 +730,15 @@
         #     final_transform = sitk.CenteredTransformInitializer(
         #         target_image,
         #         moving_image,
         #         transform_function,
         #         self.initialization_type.get(initialization.lower(), "geometry"),
         #     )
 
+        self.parameters["initialization"] = self.parameters.get("initialization", None)
         if self.parameters["initialization"] is not None:
             temp_moving = moving_image
             temp_initialization = self.parameters["initialization"].upper()
             # check for self initialization
             if "SELF" in temp_initialization:
                 temp_moving = target_image
                 temp_initialization.replace("SELF", "")
@@ -674,37 +751,42 @@
                 )
             final_transform = sitk.CenteredTransformInitializer(
                 target_image,
                 temp_moving,
                 transform_function,
                 eval("sitk.CenteredTransformInitializerFilter.%s" % (initializer_type)),
             )
-        R.SetInitialTransform(final_transform, inPlace=False)
+        registration.SetInitialTransform(final_transform, inPlace=False)
         ## set the interpolator - all options: https://simpleitk.org/doxygen/latest/html/namespaceitk_1_1simple.html#a7cb1ef8bd02c669c02ea2f9f5aa374e5
         # this should be linear to optimize results and computational efficacy
-        R.SetInterpolator(sitk.sitkLinear)
+        registration.SetInterpolator(sitk.sitkLinear)
 
-        # R.AddCommand(sitk.sitkIterationEvent, lambda: R)
+        # registration.AddCommand(sitk.sitkIterationEvent, lambda: R)
         self.logger.info("Starting registration.")
         output_transform = None
         for _ in range(self.parameters["attempts"]):
             try:
-                output_transform = R.Execute(target_image, moving_image)
+                output_transform = registration.Execute(target_image, moving_image)
                 break
             except RuntimeError as e:
                 self.logger.warning(
                     "Registration failed with error: %s. Retrying." % (e)
                 )
                 continue
 
-        if output_transform is None:
-            raise RuntimeError("Registration failed.")
+        assert output_transform is not None, "Registration failed."
+
+        self.logger.info(
+            f"Final Optimizer Parameters:: convergence={registration.GetOptimizerConvergenceValue()}, iterations={registration.GetOptimizerIteration()}, metric={registration.GetMetricValue()}, stop condition={registration.GetOptimizerStopConditionDescription()}"
+        )
 
         registration_transform_sitk = output_transform
         # if user is requesting a rigid registration, convert the transform to a rigid transform
+        if isinstance(output_transform, sitk.CompositeTransform):
+            registration_transform_sitk = output_transform.GetNthTransform(0)
         if self.parameters["transform"] in ["euler", "versorrigid"]:
             try:
                 # Euler Transform used:
                 registration_transform_sitk = eval(
                     "sitk.Euler%dDTransform(registration_transform_sitk)" % (dimension)
                 )
             except:
@@ -714,39 +796,8 @@
                     % (dimension)
                 )
                 tmp = eval("sitk.Euler%dDTransform()" % (dimension))
                 tmp.SetMatrix(registration_transform_sitk.GetMatrix())
                 tmp.SetTranslation(registration_transform_sitk.GetTranslation())
                 tmp.SetCenter(registration_transform_sitk.GetCenter())
                 registration_transform_sitk = tmp
-        ## additional information
-        # print("Metric: ", R.MetricEvaluate(target_image, moving_image), flush=True)
-        # print(
-        #     "Optimizer stop condition: ",
-        #     R.GetOptimizerStopConditionDescription(),
-        #     flush=True,
-        # )
-        # print("Number of iterations: ", R.GetOptimizerIteration(), flush=True)
-        # print("Final metric value: ", R.GetMetricValue(), flush=True)
-
-        # if rigid_registration:
-        #     if target_image.GetDimension() == 2:
-        #         output_transform = eval(
-        #             "sitk.Euler%dDTransform(output_transform)"
-        #             % (target_image.GetDimension())
-        #         )
-        #     elif target_image.GetDimension() == 3:
-        #         output_transform = eval(
-        #             "sitk.Euler%dDTransform(output_transform)"
-        #             % (target_image.GetDimension())
-        #         )
-        # # VersorRigid used: Transform from VersorRigid to Euler
-        # output_transform = eval(
-        #     "sitk.VersorRigid%dDTransform(output_transform)"
-        #     % (target_image.GetDimension())
-        # )
-        # tmp = eval("sitk.Euler%dDTransform()" % (target_image.GetDimension()))
-        # tmp.SetMatrix(output_transform.GetMatrix())
-        # tmp.SetTranslation(output_transform.GetTranslation())
-        # tmp.SetCenter(output_transform.GetCenter())
-        # output_transform = tmp
         return registration_transform_sitk
```

## Comparing `ereg-0.0.7.dist-info/LICENSE` & `ereg-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ereg-0.0.7.dist-info/METADATA` & `ereg-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eReg
-Version: 0.0.7
+Version: 0.0.8
 Summary: efficient, pythonic cross-platform image registrations
 Home-page: https://github.com/BrainLesion/eReg
 Author: Sarthak Pati
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `ereg-0.0.7.dist-info/RECORD` & `ereg-0.0.8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ereg/__init__.py,sha256=8inCCaHIF9Q0HfwHcRlSV0Ihl-fXHI5djEf6XoYl0FQ,171
 ereg/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ereg/cli/run.py,sha256=lqtXfshrOFsBlsZC_AngWWhR0Zt6YL0Ec_gSvIxrx1I,4031
 ereg/configurations/default_rigid.yaml,sha256=OmoW3LrDOOyjjSvzcOWwxKJzV0ylazZQRixCrapB-VM,3617
 ereg/configurations/sample_config.yaml,sha256=v_KqDOlNjmzqcaO5rfv8sM9cP_4upjwU2wY89nmq7ck,3600
 ereg/functional.py,sha256=VO2WYCc1-cQ9d17t8hF3t0wrJvsirWszBtEsFBW8fCM,1575
-ereg/registration.py,sha256=ALvJOiocYIgDzhnn7XX7DeuT33aPzAAIFvFrLKIzLuo,31452
+ereg/registration.py,sha256=VvcldvSzemBlwB4PIkCMxQoCtg7TQF2NT99eNyQTo08,33997
 ereg/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ereg/utils/citation_reminder.py,sha256=JV1Ey0StYPCnsBpPx4yXSCfbnaAK2kxI1gLlHLNZ5Bs,793
 ereg/utils/io.py,sha256=946FhtfQJaF_5uziQ-FrEYUW5-WpaH6FGgV6FeYrEzU,1296
 ereg/utils/metrics.py,sha256=HzUctS0r_Tv7bdSo_7nhFiam0adWCsNpX_1yjibHhzo,866
-ereg-0.0.7.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-ereg-0.0.7.dist-info/METADATA,sha256=-rSlPiS2tpm4CKPvQ_STaKWiNAhmQEe6tXlGIaLZh14,5874
-ereg-0.0.7.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-ereg-0.0.7.dist-info/entry_points.txt,sha256=1W3fHbgIIvRc178p2ovIAzyoURXHluISleo29PEHcsw,69
-ereg-0.0.7.dist-info/RECORD,,
+ereg-0.0.8.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+ereg-0.0.8.dist-info/METADATA,sha256=fKGdr2dAfb_tNAw9IUrZVlwBPBDG6f4BrcqcnCLAJGo,5874
+ereg-0.0.8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+ereg-0.0.8.dist-info/entry_points.txt,sha256=1W3fHbgIIvRc178p2ovIAzyoURXHluISleo29PEHcsw,69
+ereg-0.0.8.dist-info/RECORD,,
```

