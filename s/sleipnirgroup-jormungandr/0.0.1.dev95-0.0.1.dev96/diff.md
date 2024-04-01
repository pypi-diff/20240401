# Comparing `tmp/sleipnirgroup_jormungandr-0.0.1.dev95.tar.gz` & `tmp/sleipnirgroup_jormungandr-0.0.1.dev96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleipnirgroup_jormungandr-0.0.1.dev95.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sleipnirgroup_jormungandr-0.0.1.dev96.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sleipnirgroup_jormungandr-0.0.1.dev95.tar` & `sleipnirgroup_jormungandr-0.0.1.dev96.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0    11689 2024-04-01 15:49:18.615798 sleipnirgroup_jormungandr-0.0.1.dev95/CMakeLists.txt
--rw-r--r--   0        0        0     1465 2024-04-01 15:49:18.616038 sleipnirgroup_jormungandr-0.0.1.dev95/LICENSE.txt
--rw-r--r--   0        0        0     8573 2024-04-01 15:49:18.616402 sleipnirgroup_jormungandr-0.0.1.dev95/README.md
--rw-r--r--   0        0        0       68 2024-04-01 15:49:18.616637 sleipnirgroup_jormungandr-0.0.1.dev95/SleipnirConfig.cmake.in
--rw-r--r--   0        0        0     1163 2024-04-01 15:49:18.621037 sleipnirgroup_jormungandr-0.0.1.dev95/cmake/eigen-disable-fortran-support.patch
--rw-r--r--   0        0        0      991 2024-04-01 15:49:18.621222 sleipnirgroup_jormungandr-0.0.1.dev95/cmake/modules/Pybind11Mkdoc.cmake
--rw-r--r--   0        0        0      769 2024-04-01 15:49:18.621369 sleipnirgroup_jormungandr-0.0.1.dev95/cmake/modules/Pybind11Stubgen.cmake
--rw-r--r--   0        0        0     3848 2024-04-01 15:49:18.621662 sleipnirgroup_jormungandr-0.0.1.dev95/cmake/modules/SleipnirBuildTypes.cmake
--rw-r--r--   0        0        0      599 2024-04-01 15:49:18.621858 sleipnirgroup_jormungandr-0.0.1.dev95/cmake/modules/SleipnirCompilerFlags.cmake
--rw-r--r--   0        0        0      308 2024-04-01 15:49:18.622084 sleipnirgroup_jormungandr-0.0.1.dev95/cmake/modules/SleipnirSubdirList.cmake
--rw-r--r--   0        0        0    33588 2024-04-01 15:49:18.628116 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Expression.hpp
--rw-r--r--   0        0        0     7557 2024-04-01 15:49:18.628377 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/ExpressionGraph.hpp
--rw-r--r--   0        0        0      536 2024-04-01 15:49:18.628625 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/ExpressionType.hpp
--rw-r--r--   0        0        0     1872 2024-04-01 15:49:18.628816 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Gradient.hpp
--rw-r--r--   0        0        0     2237 2024-04-01 15:49:18.629027 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Hessian.hpp
--rw-r--r--   0        0        0     4349 2024-04-01 15:49:18.629312 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Jacobian.hpp
--rw-r--r--   0        0        0     2165 2024-04-01 15:49:18.629531 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Profiler.hpp
--rw-r--r--   0        0        0    11634 2024-04-01 15:49:18.629739 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Variable.hpp
--rw-r--r--   0        0        0    15699 2024-04-01 15:49:18.630081 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/VariableBlock.hpp
--rw-r--r--   0        0        0    26943 2024-04-01 15:49:18.630322 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/VariableMatrix.hpp
--rw-r--r--   0        0        0    13118 2024-04-01 15:49:18.630621 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/control/OCPSolver.hpp
--rw-r--r--   0        0        0     7457 2024-04-01 15:49:18.630877 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/Constraints.hpp
--rw-r--r--   0        0        0    18482 2024-04-01 15:49:18.631137 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/OptimizationProblem.hpp
--rw-r--r--   0        0        0     1774 2024-04-01 15:49:18.631384 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/SolverConfig.hpp
--rw-r--r--   0        0        0     2719 2024-04-01 15:49:18.631590 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/SolverExitCondition.hpp
--rw-r--r--   0        0        0      763 2024-04-01 15:49:18.631795 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/SolverIterationInfo.hpp
--rw-r--r--   0        0        0      904 2024-04-01 15:49:18.632086 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/SolverStatus.hpp
--rw-r--r--   0        0        0     1778 2024-04-01 15:49:18.632304 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/solver/InteriorPoint.hpp
--rw-r--r--   0        0        0      843 2024-04-01 15:49:18.632492 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Assert.hpp
--rw-r--r--   0        0        0      743 2024-04-01 15:49:18.632629 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Concepts.hpp
--rw-r--r--   0        0        0     2773 2024-04-01 15:49:18.632888 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Formatters.hpp
--rw-r--r--   0        0        0     6089 2024-04-01 15:49:18.633039 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/IntrusiveSharedPtr.hpp
--rw-r--r--   0        0        0     4160 2024-04-01 15:49:18.633200 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Pool.hpp
--rw-r--r--   0        0        0     1290 2024-04-01 15:49:18.633332 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Print.hpp
--rw-r--r--   0        0        0     2198 2024-04-01 15:49:18.633700 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Spy.hpp
--rw-r--r--   0        0        0     7128 2024-04-01 15:49:18.633885 sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/SymbolExports.hpp
--rw-r--r--   0        0        0      154 2024-04-01 15:49:18.634069 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/__init__.py
--rw-r--r--   0        0        0     1416 2024-04-01 15:49:18.634251 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/autodiff/__init__.py
--rw-r--r--   0        0        0      741 2024-04-01 15:49:18.634422 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/Binders.hpp
--rw-r--r--   0        0        0    70351 2024-04-01 15:49:18.634920 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/Docstrings.hpp
--rw-r--r--   0        0        0      899 2024-04-01 15:49:18.635129 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/Main.cpp
--rw-r--r--   0        0        0      483 2024-04-01 15:49:18.635635 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/NumPy.hpp
--rw-r--r--   0        0        0      959 2024-04-01 15:49:18.635895 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindExpressionType.cpp
--rw-r--r--   0        0        0      855 2024-04-01 15:49:18.636093 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindGradient.cpp
--rw-r--r--   0        0        0      641 2024-04-01 15:49:18.636307 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindHessian.cpp
--rw-r--r--   0        0        0      670 2024-04-01 15:49:18.636499 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindJacobian.cpp
--rw-r--r--   0        0        0     8942 2024-04-01 15:49:18.636844 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindVariable.cpp
--rw-r--r--   0        0        0    19493 2024-04-01 15:49:18.637198 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindVariableBlock.cpp
--rw-r--r--   0        0        0    22512 2024-04-01 15:49:18.637415 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindVariableMatrix.cpp
--rw-r--r--   0        0        0      972 2024-04-01 15:49:18.637914 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/optimization/BindConstraints.cpp
--rw-r--r--   0        0        0     3910 2024-04-01 15:49:18.638191 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/optimization/BindOptimizationProblem.cpp
--rw-r--r--   0        0        0     1944 2024-04-01 15:49:18.638420 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/optimization/BindSolverExitCondition.cpp
--rw-r--r--   0        0        0     1371 2024-04-01 15:49:18.638798 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/optimization/BindSolverIterationInfo.cpp
--rw-r--r--   0        0        0     1467 2024-04-01 15:49:18.639137 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/optimization/BindSolverStatus.cpp
--rw-r--r--   0        0        0       42 2024-04-01 15:49:18.639323 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/optimization/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:49:18.639525 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/py.typed
--rw-r--r--   0        0        0    15046 2024-04-01 15:49:18.640034 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/autodiff/gradient_test.py
--rw-r--r--   0        0        0     6144 2024-04-01 15:49:18.640236 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/autodiff/hessian_test.py
--rw-r--r--   0        0        0     3531 2024-04-01 15:49:18.640596 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/autodiff/jacobian_test.py
--rw-r--r--   0        0        0     4712 2024-04-01 15:49:18.640924 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/autodiff/variable_matrix_test.py
--rw-r--r--   0        0        0      185 2024-04-01 15:49:18.641230 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/autodiff/variable_test.py
--rw-r--r--   0        0        0     6029 2024-04-01 15:49:18.641648 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/constraints_test.py
--rw-r--r--   0        0        0     2368 2024-04-01 15:49:18.641973 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/decision_variable_test.py
--rw-r--r--   0        0        0      969 2024-04-01 15:49:18.642321 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/linear_problem_test.py
--rw-r--r--   0        0        0     4213 2024-04-01 15:49:18.642596 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/nonlinear_problem_test.py
--rw-r--r--   0        0        0     3181 2024-04-01 15:49:18.642934 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py
--rw-r--r--   0        0        0     6874 2024-04-01 15:49:18.643304 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_cart_pole_test.py
--rw-r--r--   0        0        0     5452 2024-04-01 15:49:18.643646 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_differential_drive_test.py
--rw-r--r--   0        0        0     3791 2024-04-01 15:49:18.644013 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_double_integrator_test.py
--rw-r--r--   0        0        0     3247 2024-04-01 15:49:18.644369 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_flywheel_test.py
--rw-r--r--   0        0        0     3985 2024-04-01 15:49:18.644619 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/quadratic_problem_test.py
--rw-r--r--   0        0        0     4643 2024-04-01 15:49:18.644908 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/solver_exit_condition_test.py
--rw-r--r--   0        0        0     1624 2024-04-01 15:49:18.645160 sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/trivial_problem_test.py
--rw-r--r--   0        0        0     1198 2024-04-01 15:49:19.071641 sleipnirgroup_jormungandr-0.0.1.dev95/pyproject.toml
--rw-r--r--   0        0        0      346 2024-04-01 15:49:18.647007 sleipnirgroup_jormungandr-0.0.1.dev95/src/autodiff/Expression.cpp
--rw-r--r--   0        0        0     1406 2024-04-01 15:49:18.647343 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/Inertia.hpp
--rw-r--r--   0        0        0     5066 2024-04-01 15:49:18.647516 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/RegularizedLDLT.hpp
--rw-r--r--   0        0        0    30260 2024-04-01 15:49:18.647887 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/InteriorPoint.cpp
--rw-r--r--   0        0        0     2843 2024-04-01 15:49:18.648103 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/ErrorEstimate.hpp
--rw-r--r--   0        0        0     7944 2024-04-01 15:49:18.648295 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/FeasibilityRestoration.hpp
--rw-r--r--   0        0        0     4844 2024-04-01 15:49:18.648640 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/Filter.hpp
--rw-r--r--   0        0        0     1166 2024-04-01 15:49:18.648789 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/FractionToTheBoundaryRule.hpp
--rw-r--r--   0        0        0     1895 2024-04-01 15:49:18.649070 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/IsLocallyInfeasible.hpp
--rw-r--r--   0        0        0     1803 2024-04-01 15:49:18.649256 sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/KKTError.hpp
--rw-r--r--   0        0        0      615 2024-04-01 15:49:18.649476 sleipnirgroup_jormungandr-0.0.1.dev95/src/util/ScopeExit.hpp
--rw-r--r--   0        0        0      504 2024-04-01 15:49:18.649625 sleipnirgroup_jormungandr-0.0.1.dev95/src/util/ToMilliseconds.hpp
--rw-r--r--   0        0        0     8977 1970-01-01 00:00:00.000000 sleipnirgroup_jormungandr-0.0.1.dev95/PKG-INFO
+-rw-r--r--   0        0        0    12063 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/CMakeLists.txt
+-rw-r--r--   0        0        0     1476 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/LICENSE.txt
+-rw-r--r--   0        0        0     8813 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/README.md
+-rw-r--r--   0        0        0       71 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/SleipnirConfig.cmake.in
+-rw-r--r--   0        0        0     1194 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/cmake/eigen-disable-fortran-support.patch
+-rw-r--r--   0        0        0     1017 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/cmake/modules/Pybind11Mkdoc.cmake
+-rw-r--r--   0        0        0      793 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/cmake/modules/Pybind11Stubgen.cmake
+-rw-r--r--   0        0        0     3960 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/cmake/modules/SleipnirBuildTypes.cmake
+-rw-r--r--   0        0        0      617 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/cmake/modules/SleipnirCompilerFlags.cmake
+-rw-r--r--   0        0        0      318 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/cmake/modules/SleipnirSubdirList.cmake
+-rw-r--r--   0        0        0    34761 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Expression.hpp
+-rw-r--r--   0        0        0     7788 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/ExpressionGraph.hpp
+-rw-r--r--   0        0        0      561 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/ExpressionType.hpp
+-rw-r--r--   0        0        0     1950 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Gradient.hpp
+-rw-r--r--   0        0        0     2321 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Hessian.hpp
+-rw-r--r--   0        0        0     4511 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Jacobian.hpp
+-rw-r--r--   0        0        0     2244 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Profiler.hpp
+-rw-r--r--   0        0        0    12101 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Variable.hpp
+-rw-r--r--   0        0        0    16315 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/VariableBlock.hpp
+-rw-r--r--   0        0        0    27949 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/VariableMatrix.hpp
+-rw-r--r--   0        0        0    13524 2024-04-01 19:29:30.369741 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/control/OCPSolver.hpp
+-rw-r--r--   0        0        0     7708 2024-04-01 19:29:30.385367 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/Constraints.hpp
+-rw-r--r--   0        0        0    19041 2024-04-01 19:29:30.385367 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/OptimizationProblem.hpp
+-rw-r--r--   0        0        0     1828 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/SolverConfig.hpp
+-rw-r--r--   0        0        0     2797 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/SolverExitCondition.hpp
+-rw-r--r--   0        0        0      799 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/SolverIterationInfo.hpp
+-rw-r--r--   0        0        0      933 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/SolverStatus.hpp
+-rw-r--r--   0        0        0     1833 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/solver/InteriorPoint.hpp
+-rw-r--r--   0        0        0      869 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Assert.hpp
+-rw-r--r--   0        0        0      773 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Concepts.hpp
+-rw-r--r--   0        0        0     2878 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Formatters.hpp
+-rw-r--r--   0        0        0     6305 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/IntrusiveSharedPtr.hpp
+-rw-r--r--   0        0        0     4313 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Pool.hpp
+-rw-r--r--   0        0        0     1346 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Print.hpp
+-rw-r--r--   0        0        0     2287 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Spy.hpp
+-rw-r--r--   0        0        0     7320 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/SymbolExports.hpp
+-rw-r--r--   0        0        0      160 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/__init__.py
+-rw-r--r--   0        0        0     1474 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/autodiff/__init__.py
+-rw-r--r--   0        0        0      766 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/Binders.hpp
+-rw-r--r--   0        0        0    72513 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/Docstrings.hpp
+-rw-r--r--   0        0        0      932 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/Main.cpp
+-rw-r--r--   0        0        0      504 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/NumPy.hpp
+-rw-r--r--   0        0        0      987 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindExpressionType.cpp
+-rw-r--r--   0        0        0      883 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindGradient.cpp
+-rw-r--r--   0        0        0      662 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindHessian.cpp
+-rw-r--r--   0        0        0      692 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindJacobian.cpp
+-rw-r--r--   0        0        0     9154 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindVariable.cpp
+-rw-r--r--   0        0        0    19970 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindVariableBlock.cpp
+-rw-r--r--   0        0        0    23087 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindVariableMatrix.cpp
+-rw-r--r--   0        0        0     1001 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/optimization/BindConstraints.cpp
+-rw-r--r--   0        0        0     4014 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/optimization/BindOptimizationProblem.cpp
+-rw-r--r--   0        0        0     1987 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/optimization/BindSolverExitCondition.cpp
+-rw-r--r--   0        0        0     1409 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/optimization/BindSolverIterationInfo.cpp
+-rw-r--r--   0        0        0     1503 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/optimization/BindSolverStatus.cpp
+-rw-r--r--   0        0        0       43 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/optimization/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/py.typed
+-rw-r--r--   0        0        0    15557 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/autodiff/gradient_test.py
+-rw-r--r--   0        0        0     6395 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/autodiff/hessian_test.py
+-rw-r--r--   0        0        0     3693 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/autodiff/jacobian_test.py
+-rw-r--r--   0        0        0     4891 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/autodiff/variable_matrix_test.py
+-rw-r--r--   0        0        0      193 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/autodiff/variable_test.py
+-rw-r--r--   0        0        0     6167 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/constraints_test.py
+-rw-r--r--   0        0        0     2456 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/decision_variable_test.py
+-rw-r--r--   0        0        0     1001 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/linear_problem_test.py
+-rw-r--r--   0        0        0     4334 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/nonlinear_problem_test.py
+-rw-r--r--   0        0        0     3275 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py
+-rw-r--r--   0        0        0     7122 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_cart_pole_test.py
+-rw-r--r--   0        0        0     5624 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_differential_drive_test.py
+-rw-r--r--   0        0        0     3917 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_double_integrator_test.py
+-rw-r--r--   0        0        0     3362 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_flywheel_test.py
+-rw-r--r--   0        0        0     4129 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/quadratic_problem_test.py
+-rw-r--r--   0        0        0     4778 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/solver_exit_condition_test.py
+-rw-r--r--   0        0        0     1673 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/trivial_problem_test.py
+-rw-r--r--   0        0        0     1246 2024-04-01 19:29:32.715522 sleipnirgroup_jormungandr-0.0.1.dev96/pyproject.toml
+-rw-r--r--   0        0        0      357 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/autodiff/Expression.cpp
+-rw-r--r--   0        0        0     1464 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/Inertia.hpp
+-rw-r--r--   0        0        0     5245 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/RegularizedLDLT.hpp
+-rw-r--r--   0        0        0    31134 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/InteriorPoint.cpp
+-rw-r--r--   0        0        0     2923 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/ErrorEstimate.hpp
+-rw-r--r--   0        0        0     8183 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/FeasibilityRestoration.hpp
+-rw-r--r--   0        0        0     5032 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/Filter.hpp
+-rw-r--r--   0        0        0     1211 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/FractionToTheBoundaryRule.hpp
+-rw-r--r--   0        0        0     1958 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/IsLocallyInfeasible.hpp
+-rw-r--r--   0        0        0     1854 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/KKTError.hpp
+-rw-r--r--   0        0        0      650 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/util/ScopeExit.hpp
+-rw-r--r--   0        0        0      525 2024-04-01 19:29:30.400993 sleipnirgroup_jormungandr-0.0.1.dev96/src/util/ToMilliseconds.hpp
+-rw-r--r--   0        0        0     8977 1970-01-01 00:00:00.000000 sleipnirgroup_jormungandr-0.0.1.dev96/PKG-INFO
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/CMakeLists.txt` & `sleipnirgroup_jormungandr-0.0.1.dev96/CMakeLists.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,374 +1,374 @@
-# Disable in-source builds to prevent source tree corruption
-if("${CMAKE_CURRENT_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_BINARY_DIR}")
-    message(
-        FATAL_ERROR
-        "
-FATAL: In-source builds are not allowed.
-       You should create a separate directory for build files.
-"
-    )
-endif()
-
-cmake_minimum_required(VERSION 3.21)
-set(CMAKE_MODULE_PATH
-    ${CMAKE_MODULE_PATH}
-    "${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules"
-)
-
-# Make `GIT_SUBMODULES ""` initialize no submodules
-cmake_policy(SET CMP0097 NEW)
-
-project(Sleipnir)
-
-set_property(GLOBAL PROPERTY USE_FOLDERS ON)
-
-# Use, i.e. don't skip the full RPATH for the build tree
-set(CMAKE_SKIP_BUILD_RPATH FALSE)
-
-# When building, don't use the install RPATH already (but later on when
-# installing)
-set(CMAKE_BUILD_WITH_INSTALL_RPATH FALSE)
-
-# Add the automatically determined parts of the RPATH which point to directories
-# outside the build tree to the install RPATH
-set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
-
-# The RPATH to be used when installing, but only if it's not a system directory
-list(
-    FIND
-    CMAKE_PLATFORM_IMPLICIT_LINK_DIRECTORIES
-    "${CMAKE_INSTALL_PREFIX}/lib"
-    isSystemDir
-)
-if("${isSystemDir}" STREQUAL "-1")
-    list(APPEND CMAKE_INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/lib")
-endif()
-
-# Set default build type to release with debug info (i.e. release mode
-# optimizations are performed, but debug info still exists).
-if(NOT CMAKE_BUILD_TYPE)
-    set(CMAKE_BUILD_TYPE "RelWithDebInfo" CACHE STRING "" FORCE)
-endif()
-
-# Generate compile_commands.json by default
-if(NOT CMAKE_EXPORT_COMPILE_COMMANDS)
-    set(CMAKE_EXPORT_COMPILE_COMMANDS "YES" CACHE STRING "" FORCE)
-endif()
-
-include(SleipnirBuildTypes)
-
-# Control where the static and shared libraries are built so that on Windows,
-# we don't need to tinker with the path to run the executable
-set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")
-set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")
-set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")
-
-option(BUILD_SHARED_LIBS "Build using shared libraries" ON)
-
-set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS FALSE)
-
-option(BUILD_BENCHMARKING "Build CasADi and Sleipnir benchmarks" OFF)
-option(BUILD_EXAMPLES "Build examples" OFF)
-option(BUILD_PYTHON "Build Python module" OFF)
-
-include(SleipnirCompilerFlags)
-
-file(GLOB_RECURSE Sleipnir_src src/*.cpp)
-add_library(Sleipnir ${Sleipnir_src})
-add_library(Sleipnir::Sleipnir ALIAS Sleipnir)
-sleipnir_compiler_flags(Sleipnir)
-target_include_directories(Sleipnir PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/src)
-
-set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS TRUE)
-
-set_target_properties(Sleipnir PROPERTIES DEBUG_POSTFIX "d")
-
-set_property(TARGET Sleipnir PROPERTY FOLDER "libraries")
-target_compile_definitions(Sleipnir PRIVATE SLEIPNIR_EXPORTS)
-
-include(CTest)
-include(FetchContent)
-
-# Options for using a package manager (e.g., vcpkg) for certain dependencies
-option(USE_SYSTEM_EIGEN "Use system eigen" OFF)
-option(USE_SYSTEM_FMT "Use system fmt" OFF)
-option(USE_SYSTEM_PYBIND "Use system pybind" OFF)
-
-# Eigen dependency
-if(NOT USE_SYSTEM_EIGEN)
-    fetchcontent_declare(
-        Eigen3
-        GIT_REPOSITORY https://gitlab.com/libeigen/eigen.git
-        # master on 2024-03-06
-        GIT_TAG 17f3bf8985021c242eedc9fa26c5c66d43a300f2
-        PATCH_COMMAND
-            git apply
-            ${CMAKE_CURRENT_SOURCE_DIR}/cmake/eigen-disable-fortran-support.patch
-        UPDATE_DISCONNECTED 1
-    )
-    fetchcontent_makeavailable(Eigen3)
-else()
-    find_package(Eigen3 CONFIG REQUIRED)
-endif()
-
-target_link_libraries(Sleipnir PUBLIC Eigen3::Eigen)
-
-# Prevent Eigen tests from running
-add_custom_command(
-    TARGET Sleipnir
-    PRE_BUILD
-    COMMAND
-        ${CMAKE_COMMAND} -E rm -f
-        ${CMAKE_BINARY_DIR}/_deps/eigen3-build/CTestTestfile.cmake
-    WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
-)
-
-# fmt dependency
-if(NOT USE_SYSTEM_FMT)
-    fetchcontent_declare(
-        fmt
-        GIT_REPOSITORY https://github.com/fmtlib/fmt.git
-        GIT_TAG 10.2.1
-    )
-    fetchcontent_makeavailable(fmt)
-else()
-    find_package(fmt CONFIG REQUIRED)
-endif()
-
-target_link_libraries(Sleipnir PUBLIC fmt::fmt)
-
-if(BUILD_TESTING)
-    # Catch2 dependency
-    fetchcontent_declare(
-        Catch2
-        GIT_REPOSITORY https://github.com/catchorg/Catch2.git
-        GIT_TAG v3.5.3
-        CMAKE_ARGS
-    )
-    fetchcontent_makeavailable(Catch2)
-endif()
-
-target_include_directories(
-    Sleipnir
-    PUBLIC
-        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
-        $<INSTALL_INTERFACE:include>
-)
-
-install(
-    TARGETS Sleipnir
-    COMPONENT Sleipnir
-    EXPORT SleipnirTargets
-    LIBRARY
-    DESTINATION lib
-    ARCHIVE
-    DESTINATION lib
-    RUNTIME
-    DESTINATION bin
-    INCLUDES DESTINATION include
-)
-export(TARGETS Sleipnir FILE Sleipnir.cmake NAMESPACE Sleipnir::)
-install(DIRECTORY include/ COMPONENT Sleipnir DESTINATION "include")
-install(
-    EXPORT SleipnirTargets
-    FILE Sleipnir.cmake
-    NAMESPACE Sleipnir::
-    DESTINATION lib/cmake/Sleipnir
-)
-
-include(CMakePackageConfigHelpers)
-
-# Generate the config file that includes the exports
-configure_package_config_file(
-    ${CMAKE_CURRENT_SOURCE_DIR}/SleipnirConfig.cmake.in
-    ${CMAKE_CURRENT_BINARY_DIR}/SleipnirConfig.cmake
-    INSTALL_DESTINATION "lib/cmake/Sleipnir"
-    NO_SET_AND_CHECK_MACRO
-    NO_CHECK_REQUIRED_COMPONENTS_MACRO
-)
-
-# Install the config file
-install(
-    FILES ${CMAKE_CURRENT_BINARY_DIR}/SleipnirConfig.cmake
-    COMPONENT Sleipnir
-    DESTINATION lib/cmake/Sleipnir
-)
-
-# Add benchmark executables if CasADi exists
-if(BUILD_BENCHMARKING)
-    find_package(casadi QUIET)
-    if(casadi_FOUND)
-        foreach(benchmark "CartPole" "Flywheel")
-            file(
-                GLOB ${benchmark}ScalabilityBenchmark_src
-                benchmarks/scalability/*.cpp
-                benchmarks/scalability/${benchmark}/*.cpp
-            )
-            add_executable(
-                ${benchmark}ScalabilityBenchmark
-                ${${benchmark}ScalabilityBenchmark_src}
-            )
-            sleipnir_compiler_flags(${benchmark}ScalabilityBenchmark)
-            target_include_directories(
-                ${benchmark}ScalabilityBenchmark
-                PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/benchmarks/scalability
-            )
-            target_link_libraries(
-                ${benchmark}ScalabilityBenchmark
-                PRIVATE Sleipnir casadi
-            )
-        endforeach()
-    endif()
-endif()
-
-if(BUILD_TESTING)
-    enable_testing()
-    list(APPEND CMAKE_MODULE_PATH ${Catch2_SOURCE_DIR}/extras)
-    include(Catch)
-endif()
-
-# Build Sleipnir tests
-if(BUILD_TESTING)
-    file(GLOB_RECURSE Sleipnir_test_src test/src/*.cpp)
-    add_executable(SleipnirTest ${Sleipnir_test_src})
-    sleipnir_compiler_flags(SleipnirTest)
-    target_include_directories(
-        SleipnirTest
-        PRIVATE
-            ${CMAKE_CURRENT_SOURCE_DIR}/src
-            ${CMAKE_CURRENT_SOURCE_DIR}/test/include
-    )
-    target_link_libraries(SleipnirTest PRIVATE Sleipnir Catch2::Catch2)
-    if(NOT CMAKE_TOOLCHAIN_FILE)
-        catch_discover_tests(SleipnirTest)
-    endif()
-endif()
-
-# Build examples and example tests
-if(BUILD_EXAMPLES)
-    include(SleipnirSubdirList)
-    sleipnir_subdir_list(EXAMPLES ${CMAKE_CURRENT_SOURCE_DIR}/examples)
-    foreach(example ${EXAMPLES})
-        # Build example
-        file(GLOB_RECURSE sources examples/${example}/src/*.cpp)
-        add_executable(${example} ${sources})
-        sleipnir_compiler_flags(${example})
-        target_include_directories(
-            ${example}
-            PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/include
-        )
-        target_link_libraries(${example} PRIVATE Sleipnir)
-
-        # Build example test if files exist for it
-        if(
-            BUILD_TESTING
-            AND EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/test
-        )
-            file(GLOB_RECURSE test_sources examples/${example}/test/*.cpp)
-            add_executable(${example}Test ${sources} ${test_sources})
-            target_include_directories(
-                ${example}Test
-                PRIVATE
-                    ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/src
-                    ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/test
-            )
-            sleipnir_compiler_flags(${example}Test)
-            target_compile_definitions(${example}Test PUBLIC RUNNING_TESTS)
-            target_include_directories(
-                ${example}Test
-                PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/include
-            )
-            target_link_libraries(
-                ${example}Test
-                PRIVATE Sleipnir Catch2::Catch2WithMain
-            )
-            if(NOT CMAKE_TOOLCHAIN_FILE)
-                catch_discover_tests(${example}Test)
-            endif()
-        endif()
-    endforeach()
-endif()
-
-if(BUILD_PYTHON)
-    find_package(Python REQUIRED COMPONENTS Interpreter Development)
-    if(DEFINED PY_BUILD_CMAKE_MODULE_NAME)
-        set(PY_DEST ${PY_BUILD_CMAKE_MODULE_NAME})
-    else()
-        set(PY_DEST lib/python${Python_VERSION_MAJOR}.${Python_VERSION_MINOR})
-    endif()
-
-    # pybind11 dependency
-    if(NOT USE_SYSTEM_PYBIND)
-        fetchcontent_declare(
-            pybind11
-            GIT_REPOSITORY https://github.com/pybind/pybind11.git
-            GIT_TAG v2.12.0
-        )
-        fetchcontent_makeavailable(pybind11)
-    else()
-        find_package(pybind11 CONFIG REQUIRED)
-    endif()
-
-    file(GLOB_RECURSE jormungandr_src jormungandr/cpp/*.cpp)
-
-    # Build fmt and Sleipnir dependencies directly into the wheel to avoid having
-    # to configure RPATHs
-    set(fmt_src ${fmt_SOURCE_DIR}/src/format.cc ${fmt_SOURCE_DIR}/src/os.cc)
-    pybind11_add_module(_jormungandr ${jormungandr_src} ${fmt_src} ${Sleipnir_src})
-    sleipnir_compiler_flags(_jormungandr)
-    target_compile_definitions(_jormungandr PRIVATE JORMUNGANDR=1)
-    target_include_directories(
-        _jormungandr
-        PRIVATE
-            ${CMAKE_CURRENT_SOURCE_DIR}/src
-            ${CMAKE_CURRENT_SOURCE_DIR}/include
-            ${fmt_SOURCE_DIR}/include
-            ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp
-    )
-    target_link_libraries(_jormungandr PUBLIC pybind11::module Eigen3::Eigen)
-
-    install(
-        TARGETS _jormungandr
-        COMPONENT python_modules
-        LIBRARY
-        DESTINATION ${PY_DEST}
-    )
-
-    # pybind11-stubgen and pybind11_mkdoc don't support Windows
-    if(NOT WIN32 AND NOT CMAKE_CROSSCOMPILING)
-        # pybind11-stubgen dependency
-        fetchcontent_declare(
-            pybind11-stubgen
-            GIT_REPOSITORY https://github.com/sizmailov/pybind11-stubgen.git
-            GIT_TAG v.2.5
-            GIT_SUBMODULES ""
-        )
-        fetchcontent_makeavailable(pybind11-stubgen)
-
-        # Generate stubs for the Python module
-        include(cmake/modules/Pybind11Stubgen.cmake)
-        pybind11_stubgen(_jormungandr)
-        pybind11_stubgen_install(_jormungandr ${PY_DEST})
-
-        # pybind11_mkdoc dependency
-        fetchcontent_declare(
-            pybind11_mkdoc
-            GIT_REPOSITORY https://github.com/pybind/pybind11_mkdoc.git
-            GIT_TAG master
-            GIT_SUBMODULES ""
-        )
-        fetchcontent_makeavailable(pybind11_mkdoc)
-
-        file(
-            GLOB_RECURSE sleipnir_headers
-            include/sleipnir/autodiff/*.hpp
-            include/sleipnir/control/*.hpp
-            include/sleipnir/optimization/*.hpp
-        )
-
-        # Generate docs for the Python module
-        include(cmake/modules/Pybind11Mkdoc.cmake)
-        pybind11_mkdoc(_jormungandr "${sleipnir_headers}")
-        add_dependencies(_jormungandr _jormungandr_docstrings)
-    endif()
-endif()
+# Disable in-source builds to prevent source tree corruption
+if("${CMAKE_CURRENT_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_BINARY_DIR}")
+    message(
+        FATAL_ERROR
+        "
+FATAL: In-source builds are not allowed.
+       You should create a separate directory for build files.
+"
+    )
+endif()
+
+cmake_minimum_required(VERSION 3.21)
+set(CMAKE_MODULE_PATH
+    ${CMAKE_MODULE_PATH}
+    "${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules"
+)
+
+# Make `GIT_SUBMODULES ""` initialize no submodules
+cmake_policy(SET CMP0097 NEW)
+
+project(Sleipnir)
+
+set_property(GLOBAL PROPERTY USE_FOLDERS ON)
+
+# Use, i.e. don't skip the full RPATH for the build tree
+set(CMAKE_SKIP_BUILD_RPATH FALSE)
+
+# When building, don't use the install RPATH already (but later on when
+# installing)
+set(CMAKE_BUILD_WITH_INSTALL_RPATH FALSE)
+
+# Add the automatically determined parts of the RPATH which point to directories
+# outside the build tree to the install RPATH
+set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
+
+# The RPATH to be used when installing, but only if it's not a system directory
+list(
+    FIND
+    CMAKE_PLATFORM_IMPLICIT_LINK_DIRECTORIES
+    "${CMAKE_INSTALL_PREFIX}/lib"
+    isSystemDir
+)
+if("${isSystemDir}" STREQUAL "-1")
+    list(APPEND CMAKE_INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/lib")
+endif()
+
+# Set default build type to release with debug info (i.e. release mode
+# optimizations are performed, but debug info still exists).
+if(NOT CMAKE_BUILD_TYPE)
+    set(CMAKE_BUILD_TYPE "RelWithDebInfo" CACHE STRING "" FORCE)
+endif()
+
+# Generate compile_commands.json by default
+if(NOT CMAKE_EXPORT_COMPILE_COMMANDS)
+    set(CMAKE_EXPORT_COMPILE_COMMANDS "YES" CACHE STRING "" FORCE)
+endif()
+
+include(SleipnirBuildTypes)
+
+# Control where the static and shared libraries are built so that on Windows,
+# we don't need to tinker with the path to run the executable
+set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")
+set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")
+set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")
+
+option(BUILD_SHARED_LIBS "Build using shared libraries" ON)
+
+set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS FALSE)
+
+option(BUILD_BENCHMARKING "Build CasADi and Sleipnir benchmarks" OFF)
+option(BUILD_EXAMPLES "Build examples" OFF)
+option(BUILD_PYTHON "Build Python module" OFF)
+
+include(SleipnirCompilerFlags)
+
+file(GLOB_RECURSE Sleipnir_src src/*.cpp)
+add_library(Sleipnir ${Sleipnir_src})
+add_library(Sleipnir::Sleipnir ALIAS Sleipnir)
+sleipnir_compiler_flags(Sleipnir)
+target_include_directories(Sleipnir PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/src)
+
+set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS TRUE)
+
+set_target_properties(Sleipnir PROPERTIES DEBUG_POSTFIX "d")
+
+set_property(TARGET Sleipnir PROPERTY FOLDER "libraries")
+target_compile_definitions(Sleipnir PRIVATE SLEIPNIR_EXPORTS)
+
+include(CTest)
+include(FetchContent)
+
+# Options for using a package manager (e.g., vcpkg) for certain dependencies
+option(USE_SYSTEM_EIGEN "Use system eigen" OFF)
+option(USE_SYSTEM_FMT "Use system fmt" OFF)
+option(USE_SYSTEM_PYBIND "Use system pybind" OFF)
+
+# Eigen dependency
+if(NOT USE_SYSTEM_EIGEN)
+    fetchcontent_declare(
+        Eigen3
+        GIT_REPOSITORY https://gitlab.com/libeigen/eigen.git
+        # master on 2024-03-06
+        GIT_TAG 17f3bf8985021c242eedc9fa26c5c66d43a300f2
+        PATCH_COMMAND
+            git apply
+            ${CMAKE_CURRENT_SOURCE_DIR}/cmake/eigen-disable-fortran-support.patch
+        UPDATE_DISCONNECTED 1
+    )
+    fetchcontent_makeavailable(Eigen3)
+else()
+    find_package(Eigen3 CONFIG REQUIRED)
+endif()
+
+target_link_libraries(Sleipnir PUBLIC Eigen3::Eigen)
+
+# Prevent Eigen tests from running
+add_custom_command(
+    TARGET Sleipnir
+    PRE_BUILD
+    COMMAND
+        ${CMAKE_COMMAND} -E rm -f
+        ${CMAKE_BINARY_DIR}/_deps/eigen3-build/CTestTestfile.cmake
+    WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
+)
+
+# fmt dependency
+if(NOT USE_SYSTEM_FMT)
+    fetchcontent_declare(
+        fmt
+        GIT_REPOSITORY https://github.com/fmtlib/fmt.git
+        GIT_TAG 10.2.1
+    )
+    fetchcontent_makeavailable(fmt)
+else()
+    find_package(fmt CONFIG REQUIRED)
+endif()
+
+target_link_libraries(Sleipnir PUBLIC fmt::fmt)
+
+if(BUILD_TESTING)
+    # Catch2 dependency
+    fetchcontent_declare(
+        Catch2
+        GIT_REPOSITORY https://github.com/catchorg/Catch2.git
+        GIT_TAG v3.5.3
+        CMAKE_ARGS
+    )
+    fetchcontent_makeavailable(Catch2)
+endif()
+
+target_include_directories(
+    Sleipnir
+    PUBLIC
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
+        $<INSTALL_INTERFACE:include>
+)
+
+install(
+    TARGETS Sleipnir
+    COMPONENT Sleipnir
+    EXPORT SleipnirTargets
+    LIBRARY
+    DESTINATION lib
+    ARCHIVE
+    DESTINATION lib
+    RUNTIME
+    DESTINATION bin
+    INCLUDES DESTINATION include
+)
+export(TARGETS Sleipnir FILE Sleipnir.cmake NAMESPACE Sleipnir::)
+install(DIRECTORY include/ COMPONENT Sleipnir DESTINATION "include")
+install(
+    EXPORT SleipnirTargets
+    FILE Sleipnir.cmake
+    NAMESPACE Sleipnir::
+    DESTINATION lib/cmake/Sleipnir
+)
+
+include(CMakePackageConfigHelpers)
+
+# Generate the config file that includes the exports
+configure_package_config_file(
+    ${CMAKE_CURRENT_SOURCE_DIR}/SleipnirConfig.cmake.in
+    ${CMAKE_CURRENT_BINARY_DIR}/SleipnirConfig.cmake
+    INSTALL_DESTINATION "lib/cmake/Sleipnir"
+    NO_SET_AND_CHECK_MACRO
+    NO_CHECK_REQUIRED_COMPONENTS_MACRO
+)
+
+# Install the config file
+install(
+    FILES ${CMAKE_CURRENT_BINARY_DIR}/SleipnirConfig.cmake
+    COMPONENT Sleipnir
+    DESTINATION lib/cmake/Sleipnir
+)
+
+# Add benchmark executables if CasADi exists
+if(BUILD_BENCHMARKING)
+    find_package(casadi QUIET)
+    if(casadi_FOUND)
+        foreach(benchmark "CartPole" "Flywheel")
+            file(
+                GLOB ${benchmark}ScalabilityBenchmark_src
+                benchmarks/scalability/*.cpp
+                benchmarks/scalability/${benchmark}/*.cpp
+            )
+            add_executable(
+                ${benchmark}ScalabilityBenchmark
+                ${${benchmark}ScalabilityBenchmark_src}
+            )
+            sleipnir_compiler_flags(${benchmark}ScalabilityBenchmark)
+            target_include_directories(
+                ${benchmark}ScalabilityBenchmark
+                PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/benchmarks/scalability
+            )
+            target_link_libraries(
+                ${benchmark}ScalabilityBenchmark
+                PRIVATE Sleipnir casadi
+            )
+        endforeach()
+    endif()
+endif()
+
+if(BUILD_TESTING)
+    enable_testing()
+    list(APPEND CMAKE_MODULE_PATH ${Catch2_SOURCE_DIR}/extras)
+    include(Catch)
+endif()
+
+# Build Sleipnir tests
+if(BUILD_TESTING)
+    file(GLOB_RECURSE Sleipnir_test_src test/src/*.cpp)
+    add_executable(SleipnirTest ${Sleipnir_test_src})
+    sleipnir_compiler_flags(SleipnirTest)
+    target_include_directories(
+        SleipnirTest
+        PRIVATE
+            ${CMAKE_CURRENT_SOURCE_DIR}/src
+            ${CMAKE_CURRENT_SOURCE_DIR}/test/include
+    )
+    target_link_libraries(SleipnirTest PRIVATE Sleipnir Catch2::Catch2)
+    if(NOT CMAKE_TOOLCHAIN_FILE)
+        catch_discover_tests(SleipnirTest)
+    endif()
+endif()
+
+# Build examples and example tests
+if(BUILD_EXAMPLES)
+    include(SleipnirSubdirList)
+    sleipnir_subdir_list(EXAMPLES ${CMAKE_CURRENT_SOURCE_DIR}/examples)
+    foreach(example ${EXAMPLES})
+        # Build example
+        file(GLOB_RECURSE sources examples/${example}/src/*.cpp)
+        add_executable(${example} ${sources})
+        sleipnir_compiler_flags(${example})
+        target_include_directories(
+            ${example}
+            PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/include
+        )
+        target_link_libraries(${example} PRIVATE Sleipnir)
+
+        # Build example test if files exist for it
+        if(
+            BUILD_TESTING
+            AND EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/test
+        )
+            file(GLOB_RECURSE test_sources examples/${example}/test/*.cpp)
+            add_executable(${example}Test ${sources} ${test_sources})
+            target_include_directories(
+                ${example}Test
+                PRIVATE
+                    ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/src
+                    ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/test
+            )
+            sleipnir_compiler_flags(${example}Test)
+            target_compile_definitions(${example}Test PUBLIC RUNNING_TESTS)
+            target_include_directories(
+                ${example}Test
+                PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/examples/${example}/include
+            )
+            target_link_libraries(
+                ${example}Test
+                PRIVATE Sleipnir Catch2::Catch2WithMain
+            )
+            if(NOT CMAKE_TOOLCHAIN_FILE)
+                catch_discover_tests(${example}Test)
+            endif()
+        endif()
+    endforeach()
+endif()
+
+if(BUILD_PYTHON)
+    find_package(Python REQUIRED COMPONENTS Interpreter Development)
+    if(DEFINED PY_BUILD_CMAKE_MODULE_NAME)
+        set(PY_DEST ${PY_BUILD_CMAKE_MODULE_NAME})
+    else()
+        set(PY_DEST lib/python${Python_VERSION_MAJOR}.${Python_VERSION_MINOR})
+    endif()
+
+    # pybind11 dependency
+    if(NOT USE_SYSTEM_PYBIND)
+        fetchcontent_declare(
+            pybind11
+            GIT_REPOSITORY https://github.com/pybind/pybind11.git
+            GIT_TAG v2.12.0
+        )
+        fetchcontent_makeavailable(pybind11)
+    else()
+        find_package(pybind11 CONFIG REQUIRED)
+    endif()
+
+    file(GLOB_RECURSE jormungandr_src jormungandr/cpp/*.cpp)
+
+    # Build fmt and Sleipnir dependencies directly into the wheel to avoid having
+    # to configure RPATHs
+    set(fmt_src ${fmt_SOURCE_DIR}/src/format.cc ${fmt_SOURCE_DIR}/src/os.cc)
+    pybind11_add_module(_jormungandr ${jormungandr_src} ${fmt_src} ${Sleipnir_src})
+    sleipnir_compiler_flags(_jormungandr)
+    target_compile_definitions(_jormungandr PRIVATE JORMUNGANDR=1)
+    target_include_directories(
+        _jormungandr
+        PRIVATE
+            ${CMAKE_CURRENT_SOURCE_DIR}/src
+            ${CMAKE_CURRENT_SOURCE_DIR}/include
+            ${fmt_SOURCE_DIR}/include
+            ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp
+    )
+    target_link_libraries(_jormungandr PUBLIC pybind11::module Eigen3::Eigen)
+
+    install(
+        TARGETS _jormungandr
+        COMPONENT python_modules
+        LIBRARY
+        DESTINATION ${PY_DEST}
+    )
+
+    # pybind11-stubgen and pybind11_mkdoc don't support Windows
+    if(NOT WIN32 AND NOT CMAKE_CROSSCOMPILING)
+        # pybind11-stubgen dependency
+        fetchcontent_declare(
+            pybind11-stubgen
+            GIT_REPOSITORY https://github.com/sizmailov/pybind11-stubgen.git
+            GIT_TAG v.2.5
+            GIT_SUBMODULES ""
+        )
+        fetchcontent_makeavailable(pybind11-stubgen)
+
+        # Generate stubs for the Python module
+        include(cmake/modules/Pybind11Stubgen.cmake)
+        pybind11_stubgen(_jormungandr)
+        pybind11_stubgen_install(_jormungandr ${PY_DEST})
+
+        # pybind11_mkdoc dependency
+        fetchcontent_declare(
+            pybind11_mkdoc
+            GIT_REPOSITORY https://github.com/pybind/pybind11_mkdoc.git
+            GIT_TAG master
+            GIT_SUBMODULES ""
+        )
+        fetchcontent_makeavailable(pybind11_mkdoc)
+
+        file(
+            GLOB_RECURSE sleipnir_headers
+            include/sleipnir/autodiff/*.hpp
+            include/sleipnir/control/*.hpp
+            include/sleipnir/optimization/*.hpp
+        )
+
+        # Generate docs for the Python module
+        include(cmake/modules/Pybind11Mkdoc.cmake)
+        pybind11_mkdoc(_jormungandr "${sleipnir_headers}")
+        add_dependencies(_jormungandr _jormungandr_docstrings)
+    endif()
+endif()
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/LICENSE.txt` & `sleipnirgroup_jormungandr-0.0.1.dev96/LICENSE.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Copyright (c) Sleipnir contributors
-
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) Sleipnir contributors
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/README.md` & `sleipnirgroup_jormungandr-0.0.1.dev96/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: sleipnirgroup-jormungandr
+Version: 0.0.1.dev96
+Summary: A linearity-exploiting sparse nonlinear constrained optimization problem solver that uses the interior-point method.
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Project-URL: Documentation, https://sleipnirgroup.github.io/Sleipnir/
+
 # Sleipnir
 
 ![Build](https://github.com/SleipnirGroup/Sleipnir/actions/workflows/build.yml/badge.svg)
 [![C++ Documentation](https://img.shields.io/badge/documentation-c%2B%2B-blue)](https://sleipnirgroup.github.io/Sleipnir/)
 [![Discord](https://img.shields.io/discord/975739302933856277?color=%23738ADB&label=Join%20our%20Discord&logo=discord&logoColor=white)](https://discord.gg/ad2EEZZwsS)
 
 > Sparsity and Linearity-Exploiting Interior-Point solver - Now Internally Readable
@@ -234,7 +245,8 @@
     <th>Yellow</th>
   </tr>
   <tr>
     <td style="background-color: #6d3d94; color: white;">6D3D94</td>
     <td style="background-color: #fdb813; color: white;">FDB813</td>
   </tr>
 </table>
+
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/cmake/eigen-disable-fortran-support.patch` & `sleipnirgroup_jormungandr-0.0.1.dev96/cmake/eigen-disable-fortran-support.patch`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-diff --git a/CMakeLists.txt b/CMakeLists.txt
-index 8477d8122..f0e9f8d3e 100644
---- a/CMakeLists.txt
-+++ b/CMakeLists.txt
-@@ -572,16 +572,16 @@ if(EIGEN_BUILD_TESTING)
-   add_subdirectory(failtest)
- endif()
- 
--include(CMakeDetermineFortranCompiler)
--option(EIGEN_BUILD_BLAS "Toggles the building of the Eigen Blas library" ${CMAKE_Fortran_COMPILER})
--option(EIGEN_BUILD_LAPACK "Toggles the building of the included Eigen LAPACK library" ${CMAKE_Fortran_COMPILER})
--if(EIGEN_LEAVE_TEST_IN_ALL_TARGET)
--  add_subdirectory(blas)
--  add_subdirectory(lapack)
--else()
--  add_subdirectory(blas EXCLUDE_FROM_ALL)
--  add_subdirectory(lapack EXCLUDE_FROM_ALL)
--endif()
-+# include(CMakeDetermineFortranCompiler)
-+# option(EIGEN_BUILD_BLAS "Toggles the building of the Eigen Blas library" ${CMAKE_Fortran_COMPILER})
-+# option(EIGEN_BUILD_LAPACK "Toggles the building of the included Eigen LAPACK library" ${CMAKE_Fortran_COMPILER})
-+# if(EIGEN_LEAVE_TEST_IN_ALL_TARGET)
-+#   add_subdirectory(blas)
-+#   add_subdirectory(lapack)
-+# else()
-+#   add_subdirectory(blas EXCLUDE_FROM_ALL)
-+#   add_subdirectory(lapack EXCLUDE_FROM_ALL)
-+# endif()
- 
- add_subdirectory(unsupported)
- 
+diff --git a/CMakeLists.txt b/CMakeLists.txt
+index 8477d8122..f0e9f8d3e 100644
+--- a/CMakeLists.txt
++++ b/CMakeLists.txt
+@@ -572,16 +572,16 @@ if(EIGEN_BUILD_TESTING)
+   add_subdirectory(failtest)
+ endif()
+ 
+-include(CMakeDetermineFortranCompiler)
+-option(EIGEN_BUILD_BLAS "Toggles the building of the Eigen Blas library" ${CMAKE_Fortran_COMPILER})
+-option(EIGEN_BUILD_LAPACK "Toggles the building of the included Eigen LAPACK library" ${CMAKE_Fortran_COMPILER})
+-if(EIGEN_LEAVE_TEST_IN_ALL_TARGET)
+-  add_subdirectory(blas)
+-  add_subdirectory(lapack)
+-else()
+-  add_subdirectory(blas EXCLUDE_FROM_ALL)
+-  add_subdirectory(lapack EXCLUDE_FROM_ALL)
+-endif()
++# include(CMakeDetermineFortranCompiler)
++# option(EIGEN_BUILD_BLAS "Toggles the building of the Eigen Blas library" ${CMAKE_Fortran_COMPILER})
++# option(EIGEN_BUILD_LAPACK "Toggles the building of the included Eigen LAPACK library" ${CMAKE_Fortran_COMPILER})
++# if(EIGEN_LEAVE_TEST_IN_ALL_TARGET)
++#   add_subdirectory(blas)
++#   add_subdirectory(lapack)
++# else()
++#   add_subdirectory(blas EXCLUDE_FROM_ALL)
++#   add_subdirectory(lapack EXCLUDE_FROM_ALL)
++# endif()
+ 
+ add_subdirectory(unsupported)
+
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/cmake/modules/Pybind11Mkdoc.cmake` & `sleipnirgroup_jormungandr-0.0.1.dev96/cmake/modules/Pybind11Mkdoc.cmake`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-function(pybind11_mkdoc target headers)
-    find_package(Python3 REQUIRED COMPONENTS Interpreter)
-    if(UNIX AND NOT APPLE)
-        set(env_vars LLVM_DIR_PATH=/usr/lib LIBCLANG_PATH=/usr/lib/libclang.so)
-    endif()
-
-    get_target_property(target_dirs ${target} INCLUDE_DIRECTORIES)
-    list(TRANSFORM target_dirs PREPEND "-I")
-
-    get_target_property(eigen_dirs Eigen3::Eigen INCLUDE_DIRECTORIES)
-    list(TRANSFORM eigen_dirs PREPEND "-I")
-
-    add_custom_command(
-        OUTPUT ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp/Docstrings.hpp
-        COMMAND
-            ${env_vars} ${Python3_EXECUTABLE} -m pybind11_mkdoc ${headers} -o
-            ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp/Docstrings.hpp
-            -I/usr/lib/clang/17/include ${target_dirs} ${eigen_dirs} -std=c++20
-        DEPENDS ${headers}
-        USES_TERMINAL
-    )
-    add_custom_target(
-        ${target}_docstrings
-        DEPENDS ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp/Docstrings.hpp
-    )
-endfunction()
+function(pybind11_mkdoc target headers)
+    find_package(Python3 REQUIRED COMPONENTS Interpreter)
+    if(UNIX AND NOT APPLE)
+        set(env_vars LLVM_DIR_PATH=/usr/lib LIBCLANG_PATH=/usr/lib/libclang.so)
+    endif()
+
+    get_target_property(target_dirs ${target} INCLUDE_DIRECTORIES)
+    list(TRANSFORM target_dirs PREPEND "-I")
+
+    get_target_property(eigen_dirs Eigen3::Eigen INCLUDE_DIRECTORIES)
+    list(TRANSFORM eigen_dirs PREPEND "-I")
+
+    add_custom_command(
+        OUTPUT ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp/Docstrings.hpp
+        COMMAND
+            ${env_vars} ${Python3_EXECUTABLE} -m pybind11_mkdoc ${headers} -o
+            ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp/Docstrings.hpp
+            -I/usr/lib/clang/17/include ${target_dirs} ${eigen_dirs} -std=c++20
+        DEPENDS ${headers}
+        USES_TERMINAL
+    )
+    add_custom_target(
+        ${target}_docstrings
+        DEPENDS ${CMAKE_CURRENT_SOURCE_DIR}/jormungandr/cpp/Docstrings.hpp
+    )
+endfunction()
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/cmake/modules/Pybind11Stubgen.cmake` & `sleipnirgroup_jormungandr-0.0.1.dev96/cmake/modules/Pybind11Stubgen.cmake`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-function(pybind11_stubgen target)
-    find_package(Python3 REQUIRED COMPONENTS Interpreter)
-    add_custom_command(
-        TARGET ${target}
-        POST_BUILD
-        COMMAND
-            ${Python3_EXECUTABLE} -m pybind11_stubgen --ignore-all-errors
-            --print-invalid-expressions-as-is --exit-code
-            $<TARGET_FILE_BASE_NAME:${target}> -o
-            $<TARGET_FILE_DIR:${target}>-stubs
-        WORKING_DIRECTORY $<TARGET_FILE_DIR:${target}>
-        USES_TERMINAL
-    )
-endfunction()
-
-function(pybind11_stubgen_install target destination)
-    install(
-        DIRECTORY $<TARGET_FILE_DIR:${target}>-stubs/${target}/
-        COMPONENT python_modules
-        DESTINATION ${destination}
-        FILES_MATCHING
-        PATTERN "*.pyi"
-    )
-endfunction()
+function(pybind11_stubgen target)
+    find_package(Python3 REQUIRED COMPONENTS Interpreter)
+    add_custom_command(
+        TARGET ${target}
+        POST_BUILD
+        COMMAND
+            ${Python3_EXECUTABLE} -m pybind11_stubgen --ignore-all-errors
+            --print-invalid-expressions-as-is --exit-code
+            $<TARGET_FILE_BASE_NAME:${target}> -o
+            $<TARGET_FILE_DIR:${target}>-stubs
+        WORKING_DIRECTORY $<TARGET_FILE_DIR:${target}>
+        USES_TERMINAL
+    )
+endfunction()
+
+function(pybind11_stubgen_install target destination)
+    install(
+        DIRECTORY $<TARGET_FILE_DIR:${target}>-stubs/${target}/
+        COMPONENT python_modules
+        DESTINATION ${destination}
+        FILES_MATCHING
+        PATTERN "*.pyi"
+    )
+endfunction()
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Expression.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Expression.hpp`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1173 +1,1173 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <stdint.h>
-
-#include <algorithm>
-#include <array>
-#include <cmath>
-#include <memory>
-#include <numbers>
-#include <utility>
-#include <vector>
-
-#include "sleipnir/autodiff/ExpressionType.hpp"
-#include "sleipnir/util/IntrusiveSharedPtr.hpp"
-#include "sleipnir/util/Pool.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir::detail {
-
-struct SLEIPNIR_DLLEXPORT Expression;
-
-inline constexpr void IntrusiveSharedPtrIncRefCount(Expression* expr);
-// FIXME: Make constexpr after upgrading to GCC 12+
-inline void IntrusiveSharedPtrDecRefCount(Expression* expr);
-
-/**
- * Typedef for intrusive shared pointer to Expression.
- */
-using ExpressionPtr = IntrusiveSharedPtr<Expression>;
-
-/**
- * Creates an intrusive shared pointer to an expression from the global pool
- * allocator.
- *
- * @param args Constructor arguments for Expression.
- */
-template <typename... Args>
-static ExpressionPtr MakeExpressionPtr(Args&&... args) {
-  return AllocateIntrusiveShared<Expression>(GlobalPoolAllocator<Expression>(),
-                                             std::forward<Args>(args)...);
-}
-
-/**
- * An autodiff expression node.
- */
-struct SLEIPNIR_DLLEXPORT Expression {
-  /**
-   * Binary function taking two doubles and returning a double.
-   */
-  using BinaryFuncDouble = double (*)(double, double);
-
-  /**
-   * Trinary function taking three doubles and returning a double.
-   */
-  using TrinaryFuncDouble = double (*)(double, double, double);
-
-  /**
-   * Trinary function taking three expressions and returning an expression.
-   */
-  using TrinaryFuncExpr = ExpressionPtr (*)(const ExpressionPtr&,
-                                            const ExpressionPtr&,
-                                            const ExpressionPtr&);
-
-  /// The value of the expression node.
-  double value = 0.0;
-
-  /// The adjoint of the expression node used during autodiff.
-  double adjoint = 0.0;
-
-  /// Tracks the number of instances of this expression yet to be encountered in
-  /// an expression tree.
-  int duplications = 0;
-
-  /// This expression's row in wrt for autodiff gradient, Jacobian, or Hessian.
-  /// This is -1 if the expression isn't in wrt.
-  int row = -1;
-
-  /// The adjoint of the expression node used during gradient expression tree
-  /// generation.
-  ExpressionPtr adjointExpr;
-
-  /// Expression argument type.
-  ExpressionType type = ExpressionType::kConstant;
-
-  /// Either nullary operator with no arguments, unary operator with one
-  /// argument, or binary operator with two arguments. This operator is
-  /// used to update the node's value.
-  BinaryFuncDouble valueFunc = nullptr;
-
-  /// Functions returning double adjoints of the children expressions.
-  ///
-  /// Parameters:
-  /// <ul>
-  ///   <li>lhs: Left argument to binary operator.</li>
-  ///   <li>rhs: Right argument to binary operator.</li>
-  ///   <li>parentAdjoint: Adjoint of parent expression.</li>
-  /// </ul>
-  std::array<TrinaryFuncDouble, 2> gradientValueFuncs{
-      [](double, double, double) { return 0.0; },
-      [](double, double, double) { return 0.0; }};
-
-  /// Functions returning Variable adjoints of the children expressions.
-  ///
-  /// Parameters:
-  /// <ul>
-  ///   <li>lhs: Left argument to binary operator.</li>
-  ///   <li>rhs: Right argument to binary operator.</li>
-  ///   <li>parentAdjoint: Adjoint of parent expression.</li>
-  /// </ul>
-  std::array<TrinaryFuncExpr, 2> gradientFuncs{
-      [](const ExpressionPtr&, const ExpressionPtr&,
-         const ExpressionPtr&) -> ExpressionPtr {
-        // Return zero
-        return nullptr;
-      },
-      [](const ExpressionPtr&, const ExpressionPtr&,
-         const ExpressionPtr&) -> ExpressionPtr {
-        // Return zero
-        return nullptr;
-      }};
-
-  /// Expression arguments.
-  std::array<ExpressionPtr, 2> args{nullptr, nullptr};
-
-  /// Reference count for intrusive shared pointer.
-  uint32_t refCount = 0;
-
-  /**
-   * Constructs a constant expression with a value of zero.
-   */
-  constexpr Expression() = default;
-
-  /**
-   * Constructs a nullary expression (an operator with no arguments).
-   *
-   * @param value The expression value.
-   * @param type The expression type. It should be either constant (the default)
-   *             or linear.
-   */
-  explicit constexpr Expression(double value,
-                                ExpressionType type = ExpressionType::kConstant)
-      : value{value}, type{type} {}
-
-  /**
-   * Constructs an unary expression (an operator with one argument).
-   *
-   * @param type The expression's type.
-   * @param valueFunc Unary operator that produces this expression's value.
-   * @param lhsGradientValueFunc Gradient with respect to the operand.
-   * @param lhsGradientFunc Gradient with respect to the operand.
-   * @param lhs Unary operator's operand.
-   */
-  constexpr Expression(ExpressionType type, BinaryFuncDouble valueFunc,
-                       TrinaryFuncDouble lhsGradientValueFunc,
-                       TrinaryFuncExpr lhsGradientFunc, ExpressionPtr lhs)
-      : value{valueFunc(lhs->value, 0.0)},
-        type{type},
-        valueFunc{valueFunc},
-        gradientValueFuncs{lhsGradientValueFunc,
-                           [](double, double, double) { return 0.0; }},
-        gradientFuncs{
-            lhsGradientFunc,
-            [](const ExpressionPtr&, const ExpressionPtr&,
-               const ExpressionPtr&) -> ExpressionPtr { return nullptr; }},
-        args{lhs, nullptr} {}
-
-  /**
-   * Constructs a binary expression (an operator with two arguments).
-   *
-   * @param type The expression's type.
-   * @param valueFunc Unary operator that produces this expression's value.
-   * @param lhsGradientValueFunc Gradient with respect to the left operand.
-   * @param rhsGradientValueFunc Gradient with respect to the right operand.
-   * @param lhsGradientFunc Gradient with respect to the left operand.
-   * @param rhsGradientFunc Gradient with respect to the right operand.
-   * @param lhs Binary operator's left operand.
-   * @param rhs Binary operator's right operand.
-   */
-  constexpr Expression(ExpressionType type, BinaryFuncDouble valueFunc,
-                       TrinaryFuncDouble lhsGradientValueFunc,
-                       TrinaryFuncDouble rhsGradientValueFunc,
-                       TrinaryFuncExpr lhsGradientFunc,
-                       TrinaryFuncExpr rhsGradientFunc, ExpressionPtr lhs,
-                       ExpressionPtr rhs)
-      : value{valueFunc(lhs->value, rhs->value)},
-        type{type},
-        valueFunc{valueFunc},
-        gradientValueFuncs{lhsGradientValueFunc, rhsGradientValueFunc},
-        gradientFuncs{lhsGradientFunc, rhsGradientFunc},
-        args{lhs, rhs} {}
-
-  /**
-   * Returns true if the expression is the given constant.
-   *
-   * @param constant The constant.
-   */
-  constexpr bool IsConstant(double constant) const {
-    return type == ExpressionType::kConstant && value == constant;
-  }
-
-  /**
-   * Expression-Expression multiplication operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator*(const ExpressionPtr& lhs,
-                                                    const ExpressionPtr& rhs) {
-    using enum ExpressionType;
-
-    // Prune expression
-    if (lhs->IsConstant(0.0)) {
-      // Return zero
-      return lhs;
-    } else if (rhs->IsConstant(0.0)) {
-      // Return zero
-      return rhs;
-    } else if (lhs->IsConstant(1.0)) {
-      return rhs;
-    } else if (rhs->IsConstant(1.0)) {
-      return lhs;
-    }
-
-    // Evaluate constant
-    if (lhs->type == kConstant && rhs->type == kConstant) {
-      return MakeExpressionPtr(lhs->value * rhs->value);
-    }
-
-    // Evaluate expression type
-    ExpressionType type;
-    if (lhs->type == kConstant) {
-      type = rhs->type;
-    } else if (rhs->type == kConstant) {
-      type = lhs->type;
-    } else if (lhs->type == kLinear && rhs->type == kLinear) {
-      type = ExpressionType::kQuadratic;
-    } else {
-      type = ExpressionType::kNonlinear;
-    }
-
-    return MakeExpressionPtr(
-        type, [](double lhs, double rhs) { return lhs * rhs; },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return parentAdjoint * rhs;
-        },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return parentAdjoint * lhs;
-        },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return parentAdjoint * rhs; },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return parentAdjoint * lhs; },
-        lhs, rhs);
-  }
-
-  /**
-   * Expression-Expression division operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator/(const ExpressionPtr& lhs,
-                                                    const ExpressionPtr& rhs) {
-    using enum ExpressionType;
-
-    // Prune expression
-    if (lhs->IsConstant(0.0)) {
-      // Return zero
-      return lhs;
-    } else if (rhs->IsConstant(1.0)) {
-      return lhs;
-    }
-
-    // Evaluate constant
-    if (lhs->type == kConstant && rhs->type == kConstant) {
-      return MakeExpressionPtr(lhs->value / rhs->value);
-    }
-
-    // Evaluate expression type
-    ExpressionType type;
-    if (rhs->type == kConstant) {
-      type = lhs->type;
-    } else {
-      type = ExpressionType::kNonlinear;
-    }
-
-    return MakeExpressionPtr(
-        type, [](double lhs, double rhs) { return lhs / rhs; },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return parentAdjoint / rhs;
-        },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return parentAdjoint * -lhs / (rhs * rhs);
-        },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return parentAdjoint / rhs; },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) {
-          return parentAdjoint * -lhs / (rhs * rhs);
-        },
-        lhs, rhs);
-  }
-
-  /**
-   * Expression-Expression addition operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator+(const ExpressionPtr& lhs,
-                                                    const ExpressionPtr& rhs) {
-    using enum ExpressionType;
-
-    // Prune expression
-    if (lhs == nullptr || lhs->IsConstant(0.0)) {
-      return rhs;
-    } else if (rhs == nullptr || rhs->IsConstant(0.0)) {
-      return lhs;
-    }
-
-    // Evaluate constant
-    if (lhs->type == kConstant && rhs->type == kConstant) {
-      return MakeExpressionPtr(lhs->value + rhs->value);
-    }
-
-    return MakeExpressionPtr(
-        std::max(lhs->type, rhs->type),
-        [](double lhs, double rhs) { return lhs + rhs; },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return parentAdjoint;
-        },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return parentAdjoint;
-        },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return parentAdjoint; },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return parentAdjoint; },
-        lhs, rhs);
-  }
-
-  /**
-   * Expression-Expression subtraction operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator-(const ExpressionPtr& lhs,
-                                                    const ExpressionPtr& rhs) {
-    using enum ExpressionType;
-
-    // Prune expression
-    if (lhs->IsConstant(0.0)) {
-      if (rhs->IsConstant(0.0)) {
-        // Return zero
-        return rhs;
-      } else {
-        return -rhs;
-      }
-    } else if (rhs->IsConstant(0.0)) {
-      return lhs;
-    }
-
-    // Evaluate constant
-    if (lhs->type == kConstant && rhs->type == kConstant) {
-      return MakeExpressionPtr(lhs->value - rhs->value);
-    }
-
-    return MakeExpressionPtr(
-        std::max(lhs->type, rhs->type),
-        [](double lhs, double rhs) { return lhs - rhs; },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return parentAdjoint;
-        },
-        [](double lhs, double rhs, double parentAdjoint) {
-          return -parentAdjoint;
-        },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return parentAdjoint; },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return -parentAdjoint; },
-        lhs, rhs);
-  }
-
-  /**
-   * Unary minus operator.
-   *
-   * @param lhs Operand of unary minus.
-   */
-  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator-(const ExpressionPtr& lhs) {
-    using enum ExpressionType;
-
-    // Prune expression
-    if (lhs->IsConstant(0.0)) {
-      // Return zero
-      return lhs;
-    }
-
-    // Evaluate constant
-    if (lhs->type == kConstant) {
-      return MakeExpressionPtr(-lhs->value);
-    }
-
-    return MakeExpressionPtr(
-        lhs->type, [](double lhs, double) { return -lhs; },
-        [](double lhs, double, double parentAdjoint) { return -parentAdjoint; },
-        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
-           const ExpressionPtr& parentAdjoint) { return -parentAdjoint; },
-        lhs);
-  }
-
-  /**
-   * Unary plus operator.
-   *
-   * @param lhs Operand of unary plus.
-   */
-  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator+(const ExpressionPtr& lhs) {
-    return lhs;
-  }
-};
-
-SLEIPNIR_DLLEXPORT inline ExpressionPtr exp(const ExpressionPtr& x);
-SLEIPNIR_DLLEXPORT inline ExpressionPtr sin(const ExpressionPtr& x);
-SLEIPNIR_DLLEXPORT inline ExpressionPtr sinh(const ExpressionPtr& x);
-SLEIPNIR_DLLEXPORT inline ExpressionPtr sqrt(const ExpressionPtr& x);
-
-/**
- * Refcount increment for intrusive shared pointer.
- *
- * @param expr The shared pointer's managed object.
- */
-inline constexpr void IntrusiveSharedPtrIncRefCount(Expression* expr) {
-  ++expr->refCount;
-}
-
-/**
- * Refcount decrement for intrusive shared pointer.
- *
- * @param expr The shared pointer's managed object.
- */
-// FIXME: Make constexpr after upgrading to GCC 12+
-inline void IntrusiveSharedPtrDecRefCount(Expression* expr) {
-  // If a deeply nested tree is being deallocated all at once, calling the
-  // Expression destructor when expr's refcount reaches zero can cause a stack
-  // overflow. Instead, we iterate over its children to decrement their
-  // refcounts and deallocate them.
-  std::vector<Expression*> stack;
-  stack.emplace_back(expr);
-
-  while (!stack.empty()) {
-    auto elem = stack.back();
-    stack.pop_back();
-
-    // Decrement the current node's refcount. If it reaches zero, deallocate the
-    // node and enqueue its children so their refcounts are decremented too.
-    if (--elem->refCount == 0) {
-      if (elem->adjointExpr != nullptr) {
-        stack.emplace_back(elem->adjointExpr.Get());
-      }
-      for (auto&& arg : elem->args) {
-        if (arg != nullptr) {
-          stack.emplace_back(arg.Get());
-        }
-      }
-
-      // Not calling the destructor here is safe because it only decrements
-      // refcounts, which was already done above.
-      auto alloc = GlobalPoolAllocator<Expression>();
-      std::allocator_traits<decltype(alloc)>::deallocate(alloc, elem,
-                                                         sizeof(Expression));
-    }
-  }
-}
-
-/**
- * std::abs() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr abs(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::abs(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::abs(x); },
-      [](double x, double, double parentAdjoint) {
-        if (x < 0.0) {
-          return -parentAdjoint;
-        } else if (x > 0.0) {
-          return parentAdjoint;
-        } else {
-          return 0.0;
-        }
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        if (x->value < 0.0) {
-          return -parentAdjoint;
-        } else if (x->value > 0.0) {
-          return parentAdjoint;
-        } else {
-          // Return zero
-          return MakeExpressionPtr();
-        }
-      },
-      x);
-}
-
-/**
- * std::acos() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr acos(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    return MakeExpressionPtr(std::numbers::pi / 2.0);
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::acos(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::acos(x); },
-      [](double x, double, double parentAdjoint) {
-        return -parentAdjoint / std::sqrt(1.0 - x * x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return -parentAdjoint /
-               sleipnir::detail::sqrt(MakeExpressionPtr(1.0) - x * x);
-      },
-      x);
-}
-
-/**
- * std::asin() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr asin(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::asin(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::asin(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint / std::sqrt(1.0 - x * x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint /
-               sleipnir::detail::sqrt(MakeExpressionPtr(1.0) - x * x);
-      },
-      x);
-}
-
-/**
- * std::atan() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr atan(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::atan(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::atan(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint / (1.0 + x * x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint / (MakeExpressionPtr(1.0) + x * x);
-      },
-      x);
-}
-
-/**
- * std::atan2() for Expressions.
- *
- * @param y The y argument.
- * @param x The x argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr atan2(  // NOLINT
-    const ExpressionPtr& y, const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (y->IsConstant(0.0)) {
-    // Return zero
-    return y;
-  } else if (x->IsConstant(0.0)) {
-    return MakeExpressionPtr(std::numbers::pi / 2.0);
-  }
-
-  // Evaluate constant
-  if (y->type == kConstant && x->type == kConstant) {
-    return MakeExpressionPtr(std::atan2(y->value, x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double y, double x) { return std::atan2(y, x); },
-      [](double y, double x, double parentAdjoint) {
-        return parentAdjoint * x / (y * y + x * x);
-      },
-      [](double y, double x, double parentAdjoint) {
-        return parentAdjoint * -y / (y * y + x * x);
-      },
-      [](const ExpressionPtr& y, const ExpressionPtr& x,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * x / (y * y + x * x);
-      },
-      [](const ExpressionPtr& y, const ExpressionPtr& x,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * -y / (y * y + x * x);
-      },
-      y, x);
-}
-
-/**
- * std::cos() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr cos(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    return MakeExpressionPtr(1.0);
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::cos(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::cos(x); },
-      [](double x, double, double parentAdjoint) {
-        return -parentAdjoint * std::sin(x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * -sleipnir::detail::sin(x);
-      },
-      x);
-}
-
-/**
- * std::cosh() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr cosh(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    return MakeExpressionPtr(1.0);
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::cosh(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::cosh(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint * std::sinh(x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * sleipnir::detail::sinh(x);
-      },
-      x);
-}
-
-/**
- * std::erf() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr erf(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::erf(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::erf(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint * 2.0 * std::numbers::inv_sqrtpi *
-               std::exp(-x * x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint *
-               MakeExpressionPtr(2.0 * std::numbers::inv_sqrtpi) *
-               sleipnir::detail::exp(-x * x);
-      },
-      x);
-}
-
-/**
- * std::exp() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr exp(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    return MakeExpressionPtr(1.0);
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::exp(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::exp(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint * std::exp(x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * sleipnir::detail::exp(x);
-      },
-      x);
-}
-
-/**
- * std::hypot() for Expressions.
- *
- * @param x The x argument.
- * @param y The y argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr hypot(  // NOLINT
-    const ExpressionPtr& x, const ExpressionPtr& y) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    return y;
-  } else if (y->IsConstant(0.0)) {
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant && y->type == kConstant) {
-    return MakeExpressionPtr(std::hypot(x->value, y->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double y) { return std::hypot(x, y); },
-      [](double x, double y, double parentAdjoint) {
-        return parentAdjoint * x / std::hypot(x, y);
-      },
-      [](double x, double y, double parentAdjoint) {
-        return parentAdjoint * y / std::hypot(x, y);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr& y,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * x / sleipnir::detail::hypot(x, y);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr& y,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * y / sleipnir::detail::hypot(x, y);
-      },
-      x, y);
-}
-
-/**
- * std::log() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr log(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::log(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::log(x); },
-      [](double x, double, double parentAdjoint) { return parentAdjoint / x; },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) { return parentAdjoint / x; },
-      x);
-}
-
-/**
- * std::log10() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr log10(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::log10(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::log10(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint / (std::numbers::ln10 * x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint / (MakeExpressionPtr(std::numbers::ln10) * x);
-      },
-      x);
-}
-
-/**
- * std::pow() for Expressions.
- *
- * @param base The base.
- * @param power The power.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr pow(  // NOLINT
-    const ExpressionPtr& base, const ExpressionPtr& power) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (base->IsConstant(0.0)) {
-    // Return zero
-    return base;
-  } else if (base->IsConstant(1.0)) {
-    return base;
-  }
-  if (power->IsConstant(0.0)) {
-    return MakeExpressionPtr(1.0);
-  } else if (power->IsConstant(1.0)) {
-    return base;
-  }
-
-  // Evaluate constant
-  if (base->type == kConstant && power->type == kConstant) {
-    return MakeExpressionPtr(std::pow(base->value, power->value));
-  }
-
-  return MakeExpressionPtr(
-      base->type == kLinear && power->IsConstant(2.0) ? kQuadratic : kNonlinear,
-      [](double base, double power) { return std::pow(base, power); },
-      [](double base, double power, double parentAdjoint) {
-        return parentAdjoint * std::pow(base, power - 1) * power;
-      },
-      [](double base, double power, double parentAdjoint) {
-        // Since x * std::log(x) -> 0 as x -> 0
-        if (base == 0.0) {
-          return 0.0;
-        } else {
-          return parentAdjoint * std::pow(base, power - 1) * base *
-                 std::log(base);
-        }
-      },
-      [](const ExpressionPtr& base, const ExpressionPtr& power,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint *
-               sleipnir::detail::pow(base, power - MakeExpressionPtr(1.0)) *
-               power;
-      },
-      [](const ExpressionPtr& base, const ExpressionPtr& power,
-         const ExpressionPtr& parentAdjoint) {
-        // Since x * std::log(x) -> 0 as x -> 0
-        if (base->value == 0.0) {
-          // Return zero
-          return base;
-        } else {
-          return parentAdjoint *
-                 sleipnir::detail::pow(base, power - MakeExpressionPtr(1.0)) *
-                 base * sleipnir::detail::log(base);
-        }
-      },
-      base, power);
-}
-
-/**
- * sign() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr sign(const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    if (x->value < 0.0) {
-      return MakeExpressionPtr(-1.0);
-    } else if (x->value == 0.0) {
-      // Return zero
-      return x;
-    } else {
-      return MakeExpressionPtr(1.0);
-    }
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear,
-      [](double x, double) {
-        if (x < 0.0) {
-          return -1.0;
-        } else if (x == 0.0) {
-          return 0.0;
-        } else {
-          return 1.0;
-        }
-      },
-      [](double x, double, double parentAdjoint) { return 0.0; },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        // Return zero
-        return MakeExpressionPtr();
-      },
-      x);
-}
-
-/**
- * std::sin() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr sin(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::sin(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::sin(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint * std::cos(x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * sleipnir::detail::cos(x);
-      },
-      x);
-}
-
-/**
- * std::sinh() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr sinh(const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::sinh(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::sinh(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint * std::cosh(x);
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint * sleipnir::detail::cosh(x);
-      },
-      x);
-}
-
-/**
- * std::sqrt() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr sqrt(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    if (x->value == 0.0) {
-      // Return zero
-      return x;
-    } else if (x->value == 1.0) {
-      return x;
-    } else {
-      return MakeExpressionPtr(std::sqrt(x->value));
-    }
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::sqrt(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint / (2.0 * std::sqrt(x));
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint /
-               (MakeExpressionPtr(2.0) * sleipnir::detail::sqrt(x));
-      },
-      x);
-}
-
-/**
- * std::tan() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr tan(  // NOLINT
-    const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::tan(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::tan(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint / (std::cos(x) * std::cos(x));
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint /
-               (sleipnir::detail::cos(x) * sleipnir::detail::cos(x));
-      },
-      x);
-}
-
-/**
- * std::tanh() for Expressions.
- *
- * @param x The argument.
- */
-SLEIPNIR_DLLEXPORT inline ExpressionPtr tanh(const ExpressionPtr& x) {
-  using enum ExpressionType;
-
-  // Prune expression
-  if (x->IsConstant(0.0)) {
-    // Return zero
-    return x;
-  }
-
-  // Evaluate constant
-  if (x->type == kConstant) {
-    return MakeExpressionPtr(std::tanh(x->value));
-  }
-
-  return MakeExpressionPtr(
-      kNonlinear, [](double x, double) { return std::tanh(x); },
-      [](double x, double, double parentAdjoint) {
-        return parentAdjoint / (std::cosh(x) * std::cosh(x));
-      },
-      [](const ExpressionPtr& x, const ExpressionPtr&,
-         const ExpressionPtr& parentAdjoint) {
-        return parentAdjoint /
-               (sleipnir::detail::cosh(x) * sleipnir::detail::cosh(x));
-      },
-      x);
-}
-
-}  // namespace sleipnir::detail
-
-namespace sleipnir {
-
-// FIXME: Doxygen is confused:
-//
-//   Found ';' while parsing initializer list! (doxygen could be confused by a
-//   macro call without semicolon)
-
-//! @cond Doxygen_Suppress
-
-// Instantiate Expression pool in Expression.cpp instead to avoid ODR violation
-extern template EXPORT_TEMPLATE_DECLARE(SLEIPNIR_DLLEXPORT)
-    PoolAllocator<detail::Expression> GlobalPoolAllocator<detail::Expression>();
-
-//! @endcond
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <stdint.h>
+
+#include <algorithm>
+#include <array>
+#include <cmath>
+#include <memory>
+#include <numbers>
+#include <utility>
+#include <vector>
+
+#include "sleipnir/autodiff/ExpressionType.hpp"
+#include "sleipnir/util/IntrusiveSharedPtr.hpp"
+#include "sleipnir/util/Pool.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir::detail {
+
+struct SLEIPNIR_DLLEXPORT Expression;
+
+inline constexpr void IntrusiveSharedPtrIncRefCount(Expression* expr);
+// FIXME: Make constexpr after upgrading to GCC 12+
+inline void IntrusiveSharedPtrDecRefCount(Expression* expr);
+
+/**
+ * Typedef for intrusive shared pointer to Expression.
+ */
+using ExpressionPtr = IntrusiveSharedPtr<Expression>;
+
+/**
+ * Creates an intrusive shared pointer to an expression from the global pool
+ * allocator.
+ *
+ * @param args Constructor arguments for Expression.
+ */
+template <typename... Args>
+static ExpressionPtr MakeExpressionPtr(Args&&... args) {
+  return AllocateIntrusiveShared<Expression>(GlobalPoolAllocator<Expression>(),
+                                             std::forward<Args>(args)...);
+}
+
+/**
+ * An autodiff expression node.
+ */
+struct SLEIPNIR_DLLEXPORT Expression {
+  /**
+   * Binary function taking two doubles and returning a double.
+   */
+  using BinaryFuncDouble = double (*)(double, double);
+
+  /**
+   * Trinary function taking three doubles and returning a double.
+   */
+  using TrinaryFuncDouble = double (*)(double, double, double);
+
+  /**
+   * Trinary function taking three expressions and returning an expression.
+   */
+  using TrinaryFuncExpr = ExpressionPtr (*)(const ExpressionPtr&,
+                                            const ExpressionPtr&,
+                                            const ExpressionPtr&);
+
+  /// The value of the expression node.
+  double value = 0.0;
+
+  /// The adjoint of the expression node used during autodiff.
+  double adjoint = 0.0;
+
+  /// Tracks the number of instances of this expression yet to be encountered in
+  /// an expression tree.
+  int duplications = 0;
+
+  /// This expression's row in wrt for autodiff gradient, Jacobian, or Hessian.
+  /// This is -1 if the expression isn't in wrt.
+  int row = -1;
+
+  /// The adjoint of the expression node used during gradient expression tree
+  /// generation.
+  ExpressionPtr adjointExpr;
+
+  /// Expression argument type.
+  ExpressionType type = ExpressionType::kConstant;
+
+  /// Either nullary operator with no arguments, unary operator with one
+  /// argument, or binary operator with two arguments. This operator is
+  /// used to update the node's value.
+  BinaryFuncDouble valueFunc = nullptr;
+
+  /// Functions returning double adjoints of the children expressions.
+  ///
+  /// Parameters:
+  /// <ul>
+  ///   <li>lhs: Left argument to binary operator.</li>
+  ///   <li>rhs: Right argument to binary operator.</li>
+  ///   <li>parentAdjoint: Adjoint of parent expression.</li>
+  /// </ul>
+  std::array<TrinaryFuncDouble, 2> gradientValueFuncs{
+      [](double, double, double) { return 0.0; },
+      [](double, double, double) { return 0.0; }};
+
+  /// Functions returning Variable adjoints of the children expressions.
+  ///
+  /// Parameters:
+  /// <ul>
+  ///   <li>lhs: Left argument to binary operator.</li>
+  ///   <li>rhs: Right argument to binary operator.</li>
+  ///   <li>parentAdjoint: Adjoint of parent expression.</li>
+  /// </ul>
+  std::array<TrinaryFuncExpr, 2> gradientFuncs{
+      [](const ExpressionPtr&, const ExpressionPtr&,
+         const ExpressionPtr&) -> ExpressionPtr {
+        // Return zero
+        return nullptr;
+      },
+      [](const ExpressionPtr&, const ExpressionPtr&,
+         const ExpressionPtr&) -> ExpressionPtr {
+        // Return zero
+        return nullptr;
+      }};
+
+  /// Expression arguments.
+  std::array<ExpressionPtr, 2> args{nullptr, nullptr};
+
+  /// Reference count for intrusive shared pointer.
+  uint32_t refCount = 0;
+
+  /**
+   * Constructs a constant expression with a value of zero.
+   */
+  constexpr Expression() = default;
+
+  /**
+   * Constructs a nullary expression (an operator with no arguments).
+   *
+   * @param value The expression value.
+   * @param type The expression type. It should be either constant (the default)
+   *             or linear.
+   */
+  explicit constexpr Expression(double value,
+                                ExpressionType type = ExpressionType::kConstant)
+      : value{value}, type{type} {}
+
+  /**
+   * Constructs an unary expression (an operator with one argument).
+   *
+   * @param type The expression's type.
+   * @param valueFunc Unary operator that produces this expression's value.
+   * @param lhsGradientValueFunc Gradient with respect to the operand.
+   * @param lhsGradientFunc Gradient with respect to the operand.
+   * @param lhs Unary operator's operand.
+   */
+  constexpr Expression(ExpressionType type, BinaryFuncDouble valueFunc,
+                       TrinaryFuncDouble lhsGradientValueFunc,
+                       TrinaryFuncExpr lhsGradientFunc, ExpressionPtr lhs)
+      : value{valueFunc(lhs->value, 0.0)},
+        type{type},
+        valueFunc{valueFunc},
+        gradientValueFuncs{lhsGradientValueFunc,
+                           [](double, double, double) { return 0.0; }},
+        gradientFuncs{
+            lhsGradientFunc,
+            [](const ExpressionPtr&, const ExpressionPtr&,
+               const ExpressionPtr&) -> ExpressionPtr { return nullptr; }},
+        args{lhs, nullptr} {}
+
+  /**
+   * Constructs a binary expression (an operator with two arguments).
+   *
+   * @param type The expression's type.
+   * @param valueFunc Unary operator that produces this expression's value.
+   * @param lhsGradientValueFunc Gradient with respect to the left operand.
+   * @param rhsGradientValueFunc Gradient with respect to the right operand.
+   * @param lhsGradientFunc Gradient with respect to the left operand.
+   * @param rhsGradientFunc Gradient with respect to the right operand.
+   * @param lhs Binary operator's left operand.
+   * @param rhs Binary operator's right operand.
+   */
+  constexpr Expression(ExpressionType type, BinaryFuncDouble valueFunc,
+                       TrinaryFuncDouble lhsGradientValueFunc,
+                       TrinaryFuncDouble rhsGradientValueFunc,
+                       TrinaryFuncExpr lhsGradientFunc,
+                       TrinaryFuncExpr rhsGradientFunc, ExpressionPtr lhs,
+                       ExpressionPtr rhs)
+      : value{valueFunc(lhs->value, rhs->value)},
+        type{type},
+        valueFunc{valueFunc},
+        gradientValueFuncs{lhsGradientValueFunc, rhsGradientValueFunc},
+        gradientFuncs{lhsGradientFunc, rhsGradientFunc},
+        args{lhs, rhs} {}
+
+  /**
+   * Returns true if the expression is the given constant.
+   *
+   * @param constant The constant.
+   */
+  constexpr bool IsConstant(double constant) const {
+    return type == ExpressionType::kConstant && value == constant;
+  }
+
+  /**
+   * Expression-Expression multiplication operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator*(const ExpressionPtr& lhs,
+                                                    const ExpressionPtr& rhs) {
+    using enum ExpressionType;
+
+    // Prune expression
+    if (lhs->IsConstant(0.0)) {
+      // Return zero
+      return lhs;
+    } else if (rhs->IsConstant(0.0)) {
+      // Return zero
+      return rhs;
+    } else if (lhs->IsConstant(1.0)) {
+      return rhs;
+    } else if (rhs->IsConstant(1.0)) {
+      return lhs;
+    }
+
+    // Evaluate constant
+    if (lhs->type == kConstant && rhs->type == kConstant) {
+      return MakeExpressionPtr(lhs->value * rhs->value);
+    }
+
+    // Evaluate expression type
+    ExpressionType type;
+    if (lhs->type == kConstant) {
+      type = rhs->type;
+    } else if (rhs->type == kConstant) {
+      type = lhs->type;
+    } else if (lhs->type == kLinear && rhs->type == kLinear) {
+      type = ExpressionType::kQuadratic;
+    } else {
+      type = ExpressionType::kNonlinear;
+    }
+
+    return MakeExpressionPtr(
+        type, [](double lhs, double rhs) { return lhs * rhs; },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return parentAdjoint * rhs;
+        },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return parentAdjoint * lhs;
+        },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return parentAdjoint * rhs; },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return parentAdjoint * lhs; },
+        lhs, rhs);
+  }
+
+  /**
+   * Expression-Expression division operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator/(const ExpressionPtr& lhs,
+                                                    const ExpressionPtr& rhs) {
+    using enum ExpressionType;
+
+    // Prune expression
+    if (lhs->IsConstant(0.0)) {
+      // Return zero
+      return lhs;
+    } else if (rhs->IsConstant(1.0)) {
+      return lhs;
+    }
+
+    // Evaluate constant
+    if (lhs->type == kConstant && rhs->type == kConstant) {
+      return MakeExpressionPtr(lhs->value / rhs->value);
+    }
+
+    // Evaluate expression type
+    ExpressionType type;
+    if (rhs->type == kConstant) {
+      type = lhs->type;
+    } else {
+      type = ExpressionType::kNonlinear;
+    }
+
+    return MakeExpressionPtr(
+        type, [](double lhs, double rhs) { return lhs / rhs; },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return parentAdjoint / rhs;
+        },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return parentAdjoint * -lhs / (rhs * rhs);
+        },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return parentAdjoint / rhs; },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) {
+          return parentAdjoint * -lhs / (rhs * rhs);
+        },
+        lhs, rhs);
+  }
+
+  /**
+   * Expression-Expression addition operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator+(const ExpressionPtr& lhs,
+                                                    const ExpressionPtr& rhs) {
+    using enum ExpressionType;
+
+    // Prune expression
+    if (lhs == nullptr || lhs->IsConstant(0.0)) {
+      return rhs;
+    } else if (rhs == nullptr || rhs->IsConstant(0.0)) {
+      return lhs;
+    }
+
+    // Evaluate constant
+    if (lhs->type == kConstant && rhs->type == kConstant) {
+      return MakeExpressionPtr(lhs->value + rhs->value);
+    }
+
+    return MakeExpressionPtr(
+        std::max(lhs->type, rhs->type),
+        [](double lhs, double rhs) { return lhs + rhs; },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return parentAdjoint;
+        },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return parentAdjoint;
+        },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return parentAdjoint; },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return parentAdjoint; },
+        lhs, rhs);
+  }
+
+  /**
+   * Expression-Expression subtraction operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator-(const ExpressionPtr& lhs,
+                                                    const ExpressionPtr& rhs) {
+    using enum ExpressionType;
+
+    // Prune expression
+    if (lhs->IsConstant(0.0)) {
+      if (rhs->IsConstant(0.0)) {
+        // Return zero
+        return rhs;
+      } else {
+        return -rhs;
+      }
+    } else if (rhs->IsConstant(0.0)) {
+      return lhs;
+    }
+
+    // Evaluate constant
+    if (lhs->type == kConstant && rhs->type == kConstant) {
+      return MakeExpressionPtr(lhs->value - rhs->value);
+    }
+
+    return MakeExpressionPtr(
+        std::max(lhs->type, rhs->type),
+        [](double lhs, double rhs) { return lhs - rhs; },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return parentAdjoint;
+        },
+        [](double lhs, double rhs, double parentAdjoint) {
+          return -parentAdjoint;
+        },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return parentAdjoint; },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return -parentAdjoint; },
+        lhs, rhs);
+  }
+
+  /**
+   * Unary minus operator.
+   *
+   * @param lhs Operand of unary minus.
+   */
+  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator-(const ExpressionPtr& lhs) {
+    using enum ExpressionType;
+
+    // Prune expression
+    if (lhs->IsConstant(0.0)) {
+      // Return zero
+      return lhs;
+    }
+
+    // Evaluate constant
+    if (lhs->type == kConstant) {
+      return MakeExpressionPtr(-lhs->value);
+    }
+
+    return MakeExpressionPtr(
+        lhs->type, [](double lhs, double) { return -lhs; },
+        [](double lhs, double, double parentAdjoint) { return -parentAdjoint; },
+        [](const ExpressionPtr& lhs, const ExpressionPtr& rhs,
+           const ExpressionPtr& parentAdjoint) { return -parentAdjoint; },
+        lhs);
+  }
+
+  /**
+   * Unary plus operator.
+   *
+   * @param lhs Operand of unary plus.
+   */
+  friend SLEIPNIR_DLLEXPORT ExpressionPtr operator+(const ExpressionPtr& lhs) {
+    return lhs;
+  }
+};
+
+SLEIPNIR_DLLEXPORT inline ExpressionPtr exp(const ExpressionPtr& x);
+SLEIPNIR_DLLEXPORT inline ExpressionPtr sin(const ExpressionPtr& x);
+SLEIPNIR_DLLEXPORT inline ExpressionPtr sinh(const ExpressionPtr& x);
+SLEIPNIR_DLLEXPORT inline ExpressionPtr sqrt(const ExpressionPtr& x);
+
+/**
+ * Refcount increment for intrusive shared pointer.
+ *
+ * @param expr The shared pointer's managed object.
+ */
+inline constexpr void IntrusiveSharedPtrIncRefCount(Expression* expr) {
+  ++expr->refCount;
+}
+
+/**
+ * Refcount decrement for intrusive shared pointer.
+ *
+ * @param expr The shared pointer's managed object.
+ */
+// FIXME: Make constexpr after upgrading to GCC 12+
+inline void IntrusiveSharedPtrDecRefCount(Expression* expr) {
+  // If a deeply nested tree is being deallocated all at once, calling the
+  // Expression destructor when expr's refcount reaches zero can cause a stack
+  // overflow. Instead, we iterate over its children to decrement their
+  // refcounts and deallocate them.
+  std::vector<Expression*> stack;
+  stack.emplace_back(expr);
+
+  while (!stack.empty()) {
+    auto elem = stack.back();
+    stack.pop_back();
+
+    // Decrement the current node's refcount. If it reaches zero, deallocate the
+    // node and enqueue its children so their refcounts are decremented too.
+    if (--elem->refCount == 0) {
+      if (elem->adjointExpr != nullptr) {
+        stack.emplace_back(elem->adjointExpr.Get());
+      }
+      for (auto&& arg : elem->args) {
+        if (arg != nullptr) {
+          stack.emplace_back(arg.Get());
+        }
+      }
+
+      // Not calling the destructor here is safe because it only decrements
+      // refcounts, which was already done above.
+      auto alloc = GlobalPoolAllocator<Expression>();
+      std::allocator_traits<decltype(alloc)>::deallocate(alloc, elem,
+                                                         sizeof(Expression));
+    }
+  }
+}
+
+/**
+ * std::abs() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr abs(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::abs(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::abs(x); },
+      [](double x, double, double parentAdjoint) {
+        if (x < 0.0) {
+          return -parentAdjoint;
+        } else if (x > 0.0) {
+          return parentAdjoint;
+        } else {
+          return 0.0;
+        }
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        if (x->value < 0.0) {
+          return -parentAdjoint;
+        } else if (x->value > 0.0) {
+          return parentAdjoint;
+        } else {
+          // Return zero
+          return MakeExpressionPtr();
+        }
+      },
+      x);
+}
+
+/**
+ * std::acos() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr acos(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    return MakeExpressionPtr(std::numbers::pi / 2.0);
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::acos(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::acos(x); },
+      [](double x, double, double parentAdjoint) {
+        return -parentAdjoint / std::sqrt(1.0 - x * x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return -parentAdjoint /
+               sleipnir::detail::sqrt(MakeExpressionPtr(1.0) - x * x);
+      },
+      x);
+}
+
+/**
+ * std::asin() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr asin(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::asin(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::asin(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint / std::sqrt(1.0 - x * x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint /
+               sleipnir::detail::sqrt(MakeExpressionPtr(1.0) - x * x);
+      },
+      x);
+}
+
+/**
+ * std::atan() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr atan(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::atan(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::atan(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint / (1.0 + x * x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint / (MakeExpressionPtr(1.0) + x * x);
+      },
+      x);
+}
+
+/**
+ * std::atan2() for Expressions.
+ *
+ * @param y The y argument.
+ * @param x The x argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr atan2(  // NOLINT
+    const ExpressionPtr& y, const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (y->IsConstant(0.0)) {
+    // Return zero
+    return y;
+  } else if (x->IsConstant(0.0)) {
+    return MakeExpressionPtr(std::numbers::pi / 2.0);
+  }
+
+  // Evaluate constant
+  if (y->type == kConstant && x->type == kConstant) {
+    return MakeExpressionPtr(std::atan2(y->value, x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double y, double x) { return std::atan2(y, x); },
+      [](double y, double x, double parentAdjoint) {
+        return parentAdjoint * x / (y * y + x * x);
+      },
+      [](double y, double x, double parentAdjoint) {
+        return parentAdjoint * -y / (y * y + x * x);
+      },
+      [](const ExpressionPtr& y, const ExpressionPtr& x,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * x / (y * y + x * x);
+      },
+      [](const ExpressionPtr& y, const ExpressionPtr& x,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * -y / (y * y + x * x);
+      },
+      y, x);
+}
+
+/**
+ * std::cos() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr cos(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    return MakeExpressionPtr(1.0);
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::cos(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::cos(x); },
+      [](double x, double, double parentAdjoint) {
+        return -parentAdjoint * std::sin(x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * -sleipnir::detail::sin(x);
+      },
+      x);
+}
+
+/**
+ * std::cosh() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr cosh(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    return MakeExpressionPtr(1.0);
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::cosh(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::cosh(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint * std::sinh(x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * sleipnir::detail::sinh(x);
+      },
+      x);
+}
+
+/**
+ * std::erf() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr erf(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::erf(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::erf(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint * 2.0 * std::numbers::inv_sqrtpi *
+               std::exp(-x * x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint *
+               MakeExpressionPtr(2.0 * std::numbers::inv_sqrtpi) *
+               sleipnir::detail::exp(-x * x);
+      },
+      x);
+}
+
+/**
+ * std::exp() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr exp(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    return MakeExpressionPtr(1.0);
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::exp(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::exp(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint * std::exp(x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * sleipnir::detail::exp(x);
+      },
+      x);
+}
+
+/**
+ * std::hypot() for Expressions.
+ *
+ * @param x The x argument.
+ * @param y The y argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr hypot(  // NOLINT
+    const ExpressionPtr& x, const ExpressionPtr& y) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    return y;
+  } else if (y->IsConstant(0.0)) {
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant && y->type == kConstant) {
+    return MakeExpressionPtr(std::hypot(x->value, y->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double y) { return std::hypot(x, y); },
+      [](double x, double y, double parentAdjoint) {
+        return parentAdjoint * x / std::hypot(x, y);
+      },
+      [](double x, double y, double parentAdjoint) {
+        return parentAdjoint * y / std::hypot(x, y);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr& y,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * x / sleipnir::detail::hypot(x, y);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr& y,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * y / sleipnir::detail::hypot(x, y);
+      },
+      x, y);
+}
+
+/**
+ * std::log() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr log(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::log(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::log(x); },
+      [](double x, double, double parentAdjoint) { return parentAdjoint / x; },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) { return parentAdjoint / x; },
+      x);
+}
+
+/**
+ * std::log10() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr log10(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::log10(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::log10(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint / (std::numbers::ln10 * x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint / (MakeExpressionPtr(std::numbers::ln10) * x);
+      },
+      x);
+}
+
+/**
+ * std::pow() for Expressions.
+ *
+ * @param base The base.
+ * @param power The power.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr pow(  // NOLINT
+    const ExpressionPtr& base, const ExpressionPtr& power) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (base->IsConstant(0.0)) {
+    // Return zero
+    return base;
+  } else if (base->IsConstant(1.0)) {
+    return base;
+  }
+  if (power->IsConstant(0.0)) {
+    return MakeExpressionPtr(1.0);
+  } else if (power->IsConstant(1.0)) {
+    return base;
+  }
+
+  // Evaluate constant
+  if (base->type == kConstant && power->type == kConstant) {
+    return MakeExpressionPtr(std::pow(base->value, power->value));
+  }
+
+  return MakeExpressionPtr(
+      base->type == kLinear && power->IsConstant(2.0) ? kQuadratic : kNonlinear,
+      [](double base, double power) { return std::pow(base, power); },
+      [](double base, double power, double parentAdjoint) {
+        return parentAdjoint * std::pow(base, power - 1) * power;
+      },
+      [](double base, double power, double parentAdjoint) {
+        // Since x * std::log(x) -> 0 as x -> 0
+        if (base == 0.0) {
+          return 0.0;
+        } else {
+          return parentAdjoint * std::pow(base, power - 1) * base *
+                 std::log(base);
+        }
+      },
+      [](const ExpressionPtr& base, const ExpressionPtr& power,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint *
+               sleipnir::detail::pow(base, power - MakeExpressionPtr(1.0)) *
+               power;
+      },
+      [](const ExpressionPtr& base, const ExpressionPtr& power,
+         const ExpressionPtr& parentAdjoint) {
+        // Since x * std::log(x) -> 0 as x -> 0
+        if (base->value == 0.0) {
+          // Return zero
+          return base;
+        } else {
+          return parentAdjoint *
+                 sleipnir::detail::pow(base, power - MakeExpressionPtr(1.0)) *
+                 base * sleipnir::detail::log(base);
+        }
+      },
+      base, power);
+}
+
+/**
+ * sign() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr sign(const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    if (x->value < 0.0) {
+      return MakeExpressionPtr(-1.0);
+    } else if (x->value == 0.0) {
+      // Return zero
+      return x;
+    } else {
+      return MakeExpressionPtr(1.0);
+    }
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear,
+      [](double x, double) {
+        if (x < 0.0) {
+          return -1.0;
+        } else if (x == 0.0) {
+          return 0.0;
+        } else {
+          return 1.0;
+        }
+      },
+      [](double x, double, double parentAdjoint) { return 0.0; },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        // Return zero
+        return MakeExpressionPtr();
+      },
+      x);
+}
+
+/**
+ * std::sin() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr sin(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::sin(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::sin(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint * std::cos(x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * sleipnir::detail::cos(x);
+      },
+      x);
+}
+
+/**
+ * std::sinh() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr sinh(const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::sinh(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::sinh(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint * std::cosh(x);
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint * sleipnir::detail::cosh(x);
+      },
+      x);
+}
+
+/**
+ * std::sqrt() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr sqrt(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    if (x->value == 0.0) {
+      // Return zero
+      return x;
+    } else if (x->value == 1.0) {
+      return x;
+    } else {
+      return MakeExpressionPtr(std::sqrt(x->value));
+    }
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::sqrt(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint / (2.0 * std::sqrt(x));
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint /
+               (MakeExpressionPtr(2.0) * sleipnir::detail::sqrt(x));
+      },
+      x);
+}
+
+/**
+ * std::tan() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr tan(  // NOLINT
+    const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::tan(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::tan(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint / (std::cos(x) * std::cos(x));
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint /
+               (sleipnir::detail::cos(x) * sleipnir::detail::cos(x));
+      },
+      x);
+}
+
+/**
+ * std::tanh() for Expressions.
+ *
+ * @param x The argument.
+ */
+SLEIPNIR_DLLEXPORT inline ExpressionPtr tanh(const ExpressionPtr& x) {
+  using enum ExpressionType;
+
+  // Prune expression
+  if (x->IsConstant(0.0)) {
+    // Return zero
+    return x;
+  }
+
+  // Evaluate constant
+  if (x->type == kConstant) {
+    return MakeExpressionPtr(std::tanh(x->value));
+  }
+
+  return MakeExpressionPtr(
+      kNonlinear, [](double x, double) { return std::tanh(x); },
+      [](double x, double, double parentAdjoint) {
+        return parentAdjoint / (std::cosh(x) * std::cosh(x));
+      },
+      [](const ExpressionPtr& x, const ExpressionPtr&,
+         const ExpressionPtr& parentAdjoint) {
+        return parentAdjoint /
+               (sleipnir::detail::cosh(x) * sleipnir::detail::cosh(x));
+      },
+      x);
+}
+
+}  // namespace sleipnir::detail
+
+namespace sleipnir {
+
+// FIXME: Doxygen is confused:
+//
+//   Found ';' while parsing initializer list! (doxygen could be confused by a
+//   macro call without semicolon)
+
+//! @cond Doxygen_Suppress
+
+// Instantiate Expression pool in Expression.cpp instead to avoid ODR violation
+extern template EXPORT_TEMPLATE_DECLARE(SLEIPNIR_DLLEXPORT)
+    PoolAllocator<detail::Expression> GlobalPoolAllocator<detail::Expression>();
+
+//! @endcond
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/Gradient.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/Hessian.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,84 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <utility>
-
-#include <Eigen/SparseCore>
-
-#include "sleipnir/autodiff/Jacobian.hpp"
-#include "sleipnir/autodiff/Profiler.hpp"
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/autodiff/VariableMatrix.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * This class calculates the gradient of a a variable with respect to a vector
- * of variables.
- *
- * The gradient is only recomputed if the variable expression is quadratic or
- * higher order.
- */
-class SLEIPNIR_DLLEXPORT Gradient {
- public:
-  /**
-   * Constructs a Gradient object.
-   *
-   * @param variable Variable of which to compute the gradient.
-   * @param wrt Variable with respect to which to compute the gradient.
-   */
-  Gradient(Variable variable, Variable wrt) noexcept
-      : Gradient{std::move(variable), VariableMatrix{wrt}} {}
-
-  /**
-   * Constructs a Gradient object.
-   *
-   * @param variable Variable of which to compute the gradient.
-   * @param wrt Vector of variables with respect to which to compute the
-   *   gradient.
-   */
-  Gradient(Variable variable, const VariableMatrix& wrt) noexcept
-      : m_jacobian{variable, wrt} {}
-
-  /**
-   * Returns the gradient as a VariableMatrix.
-   *
-   * This is useful when constructing optimization problems with derivatives in
-   * them.
-   */
-  VariableMatrix Get() const { return m_jacobian.Get().T(); }
-
-  /**
-   * Evaluates the gradient at wrt's value.
-   */
-  const Eigen::SparseVector<double>& Value() {
-    m_g = m_jacobian.Value();
-
-    return m_g;
-  }
-
-  /**
-   * Updates the value of the variable.
-   */
-  void Update() { m_jacobian.Update(); }
-
-  /**
-   * Returns the profiler.
-   */
-  Profiler& GetProfiler() { return m_jacobian.GetProfiler(); }
-
- private:
-  Eigen::SparseVector<double> m_g;
-
-  Jacobian m_jacobian;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <utility>
+#include <vector>
+
+#include <Eigen/Core>
+#include <Eigen/SparseCore>
+
+#include "sleipnir/autodiff/ExpressionGraph.hpp"
+#include "sleipnir/autodiff/Jacobian.hpp"
+#include "sleipnir/autodiff/Profiler.hpp"
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/autodiff/VariableMatrix.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * This class calculates the Hessian of a variable with respect to a vector of
+ * variables.
+ *
+ * The gradient tree is cached so subsequent Hessian calculations are faster,
+ * and the Hessian is only recomputed if the variable expression is nonlinear.
+ */
+class SLEIPNIR_DLLEXPORT Hessian {
+ public:
+  /**
+   * Constructs a Hessian object.
+   *
+   * @param variable Variable of which to compute the Hessian.
+   * @param wrt Vector of variables with respect to which to compute the
+   *   Hessian.
+   */
+  Hessian(Variable variable, const VariableMatrix& wrt) noexcept
+      : m_jacobian{
+            [&] {
+              std::vector<detail::ExpressionPtr> wrtVec;
+              wrtVec.reserve(wrt.size());
+              for (auto& elem : wrt) {
+                wrtVec.emplace_back(elem.expr);
+              }
+
+              auto grad =
+                  detail::ExpressionGraph{variable.expr}.GenerateGradientTree(
+                      wrtVec);
+
+              VariableMatrix ret{wrt.Rows()};
+              for (int row = 0; row < ret.Rows(); ++row) {
+                ret(row) = Variable{std::move(grad[row])};
+              }
+              return ret;
+            }(),
+            wrt} {}
+
+  /**
+   * Returns the Hessian as a VariableMatrix.
+   *
+   * This is useful when constructing optimization problems with derivatives in
+   * them.
+   */
+  VariableMatrix Get() const { return m_jacobian.Get(); }
+
+  /**
+   * Evaluates the Hessian at wrt's value.
+   */
+  const Eigen::SparseMatrix<double>& Value() { return m_jacobian.Value(); }
+
+  /**
+   * Updates the values of the gradient tree.
+   */
+  void Update() { m_jacobian.Update(); }
+
+  /**
+   * Returns the profiler.
+   */
+  Profiler& GetProfiler() { return m_jacobian.GetProfiler(); }
+
+ private:
+  Jacobian m_jacobian;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/VariableBlock.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/VariableBlock.hpp`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,616 +1,616 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <concepts>
-#include <type_traits>
-#include <utility>
-
-#include <Eigen/Core>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/util/Assert.hpp"
-
-namespace sleipnir {
-
-/**
- * A submatrix of autodiff variables with reference semantics.
- *
- * @tparam Mat The type of the matrix whose storage this class points to.
- */
-template <typename Mat>
-class VariableBlock {
- public:
-  VariableBlock(const VariableBlock<Mat>& values) = default;
-
-  /**
-   * Assigns a VariableBlock to the block.
-   */
-  VariableBlock<Mat>& operator=(const VariableBlock<Mat>& values) {
-    if (this == &values) {
-      return *this;
-    }
-
-    if (m_mat == nullptr) {
-      m_mat = values.m_mat;
-      m_rowOffset = values.m_rowOffset;
-      m_colOffset = values.m_colOffset;
-      m_blockRows = values.m_blockRows;
-      m_blockCols = values.m_blockCols;
-    } else {
-      Assert(Rows() == values.Rows());
-      Assert(Cols() == values.Cols());
-
-      for (int row = 0; row < Rows(); ++row) {
-        for (int col = 0; col < Cols(); ++col) {
-          (*this)(row, col) = values(row, col);
-        }
-      }
-    }
-
-    return *this;
-  }
-
-  VariableBlock(VariableBlock<Mat>&&) = default;
-
-  /**
-   * Assigns a VariableBlock to the block.
-   */
-  VariableBlock<Mat>& operator=(VariableBlock<Mat>&& values) {
-    if (this == &values) {
-      return *this;
-    }
-
-    if (m_mat == nullptr) {
-      m_mat = values.m_mat;
-      m_rowOffset = values.m_rowOffset;
-      m_colOffset = values.m_colOffset;
-      m_blockRows = values.m_blockRows;
-      m_blockCols = values.m_blockCols;
-    } else {
-      Assert(Rows() == values.Rows());
-      Assert(Cols() == values.Cols());
-
-      for (int row = 0; row < Rows(); ++row) {
-        for (int col = 0; col < Cols(); ++col) {
-          (*this)(row, col) = values(row, col);
-        }
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Constructs a Variable block pointing to all of the given matrix.
-   *
-   * @param mat The matrix to which to point.
-   */
-  VariableBlock(Mat& mat)  // NOLINT
-      : m_mat{&mat}, m_blockRows{mat.Rows()}, m_blockCols{mat.Cols()} {}
-
-  /**
-   * Constructs a Variable block pointing to a subset of the given matrix.
-   *
-   * @param mat The matrix to which to point.
-   * @param rowOffset The block's row offset.
-   * @param colOffset The block's column offset.
-   * @param blockRows The number of rows in the block.
-   * @param blockCols The number of columns in the block.
-   */
-  VariableBlock(Mat& mat, int rowOffset, int colOffset, int blockRows,
-                int blockCols)
-      : m_mat{&mat},
-        m_rowOffset{rowOffset},
-        m_colOffset{colOffset},
-        m_blockRows{blockRows},
-        m_blockCols{blockCols} {}
-
-  /**
-   * Assigns a double to the block.
-   *
-   * This only works for blocks with one row and one column.
-   */
-  VariableBlock<Mat>& operator=(double value) {
-    Assert(Rows() == 1 && Cols() == 1);
-
-    (*this)(0, 0) = value;
-
-    return *this;
-  }
-
-  /**
-   * Assigns a double to the block.
-   *
-   * This only works for blocks with one row and one column.
-   */
-  VariableBlock<Mat>& SetValue(double value) {
-    Assert(Rows() == 1 && Cols() == 1);
-
-    (*this)(0, 0).SetValue(value);
-
-    return *this;
-  }
-
-  /**
-   * Assigns an Eigen matrix to the block.
-   */
-  template <typename Derived>
-  VariableBlock<Mat>& operator=(const Eigen::MatrixBase<Derived>& values) {
-    Assert(Rows() == values.rows());
-    Assert(Cols() == values.cols());
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) = values(row, col);
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Sets block's internal values.
-   */
-  template <typename Derived>
-    requires std::same_as<typename Derived::Scalar, double>
-  VariableBlock<Mat>& SetValue(const Eigen::MatrixBase<Derived>& values) {
-    Assert(Rows() == values.rows());
-    Assert(Cols() == values.cols());
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col).SetValue(values(row, col));
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Assigns a VariableMatrix to the block.
-   */
-  VariableBlock<Mat>& operator=(const Mat& values) {
-    Assert(Rows() == values.Rows());
-    Assert(Cols() == values.Cols());
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) = values(row, col);
-      }
-    }
-    return *this;
-  }
-
-  /**
-   * Assigns a VariableMatrix to the block.
-   */
-  VariableBlock<Mat>& operator=(Mat&& values) {
-    Assert(Rows() == values.Rows());
-    Assert(Cols() == values.Cols());
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) = std::move(values(row, col));
-      }
-    }
-    return *this;
-  }
-
-  /**
-   * Returns a scalar subblock at the given row and column.
-   *
-   * @param row The scalar subblock's row.
-   * @param col The scalar subblock's column.
-   */
-  template <typename Mat2 = Mat>
-    requires(!std::is_const_v<Mat2>)
-  Variable& operator()(int row, int col) {
-    Assert(row >= 0 && row < Rows());
-    Assert(col >= 0 && col < Cols());
-    return (*m_mat)(m_rowOffset + row, m_colOffset + col);
-  }
-
-  /**
-   * Returns a scalar subblock at the given row and column.
-   *
-   * @param row The scalar subblock's row.
-   * @param col The scalar subblock's column.
-   */
-  const Variable& operator()(int row, int col) const {
-    Assert(row >= 0 && row < Rows());
-    Assert(col >= 0 && col < Cols());
-    return (*m_mat)(m_rowOffset + row, m_colOffset + col);
-  }
-
-  /**
-   * Returns a scalar subblock at the given row.
-   *
-   * @param row The scalar subblock's row.
-   */
-  template <typename Mat2 = Mat>
-    requires(!std::is_const_v<Mat2>)
-  Variable& operator()(int row) {
-    Assert(row >= 0 && row < Rows() * Cols());
-    return (*this)(row / Cols(), row % Cols());
-  }
-
-  /**
-   * Returns a scalar subblock at the given row.
-   *
-   * @param row The scalar subblock's row.
-   */
-  const Variable& operator()(int row) const {
-    Assert(row >= 0 && row < Rows() * Cols());
-    return (*this)(row / Cols(), row % Cols());
-  }
-
-  /**
-   * Returns a block slice of the variable matrix.
-   *
-   * @param rowOffset The row offset of the block selection.
-   * @param colOffset The column offset of the block selection.
-   * @param blockRows The number of rows in the block selection.
-   * @param blockCols The number of columns in the block selection.
-   */
-  VariableBlock<Mat> Block(int rowOffset, int colOffset, int blockRows,
-                           int blockCols) {
-    Assert(rowOffset >= 0 && rowOffset <= Rows());
-    Assert(colOffset >= 0 && colOffset <= Cols());
-    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
-    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
-    return VariableBlock{*m_mat, m_rowOffset + rowOffset,
-                         m_colOffset + colOffset, blockRows, blockCols};
-  }
-
-  /**
-   * Returns a block slice of the variable matrix.
-   *
-   * @param rowOffset The row offset of the block selection.
-   * @param colOffset The column offset of the block selection.
-   * @param blockRows The number of rows in the block selection.
-   * @param blockCols The number of columns in the block selection.
-   */
-  const VariableBlock<const Mat> Block(int rowOffset, int colOffset,
-                                       int blockRows, int blockCols) const {
-    Assert(rowOffset >= 0 && rowOffset <= Rows());
-    Assert(colOffset >= 0 && colOffset <= Cols());
-    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
-    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
-    return VariableBlock{*m_mat, m_rowOffset + rowOffset,
-                         m_colOffset + colOffset, blockRows, blockCols};
-  }
-
-  /**
-   * Returns a row slice of the variable matrix.
-   *
-   * @param row The row to slice.
-   */
-  VariableBlock<Mat> Row(int row) {
-    Assert(row >= 0 && row < Rows());
-    return Block(row, 0, 1, Cols());
-  }
-
-  /**
-   * Returns a row slice of the variable matrix.
-   *
-   * @param row The row to slice.
-   */
-  VariableBlock<const Mat> Row(int row) const {
-    Assert(row >= 0 && row < Rows());
-    return Block(row, 0, 1, Cols());
-  }
-
-  /**
-   * Returns a column slice of the variable matrix.
-   *
-   * @param col The column to slice.
-   */
-  VariableBlock<Mat> Col(int col) {
-    Assert(col >= 0 && col < Cols());
-    return Block(0, col, Rows(), 1);
-  }
-
-  /**
-   * Returns a column slice of the variable matrix.
-   *
-   * @param col The column to slice.
-   */
-  VariableBlock<const Mat> Col(int col) const {
-    Assert(col >= 0 && col < Cols());
-    return Block(0, col, Rows(), 1);
-  }
-
-  /**
-   * Compound matrix multiplication-assignment operator.
-   *
-   * @param rhs Variable to multiply.
-   */
-  VariableBlock<Mat>& operator*=(const VariableBlock<Mat>& rhs) {
-    Assert(Cols() == rhs.Rows() && Cols() == rhs.Cols());
-
-    for (int i = 0; i < Rows(); ++i) {
-      for (int j = 0; j < rhs.Cols(); ++j) {
-        Variable sum;
-        for (int k = 0; k < Cols(); ++k) {
-          sum += (*this)(i, k) * rhs(k, j);
-        }
-        (*this)(i, j) = sum;
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Compound matrix multiplication-assignment operator (only enabled when lhs
-   * is a scalar).
-   *
-   * @param rhs Variable to multiply.
-   */
-  VariableBlock& operator*=(double rhs) {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) *= rhs;
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Compound matrix division-assignment operator (only enabled when rhs
-   * is a scalar).
-   *
-   * @param rhs Variable to divide.
-   */
-  VariableBlock<Mat>& operator/=(const VariableBlock<Mat>& rhs) {
-    Assert(rhs.Rows() == 1 && rhs.Cols() == 1);
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) /= rhs(0, 0);
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Compound matrix division-assignment operator (only enabled when rhs
-   * is a scalar).
-   *
-   * @param rhs Variable to divide.
-   */
-  VariableBlock<Mat>& operator/=(double rhs) {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) /= rhs;
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Compound addition-assignment operator.
-   *
-   * @param rhs Variable to add.
-   */
-  VariableBlock<Mat>& operator+=(const VariableBlock<Mat>& rhs) {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) += rhs(row, col);
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Compound subtraction-assignment operator.
-   *
-   * @param rhs Variable to subtract.
-   */
-  VariableBlock<Mat>& operator-=(const VariableBlock<Mat>& rhs) {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) -= rhs(row, col);
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Returns the transpose of the variable matrix.
-   */
-  std::remove_cv_t<Mat> T() const {
-    std::remove_cv_t<Mat> result{Cols(), Rows()};
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        result(col, row) = (*this)(row, col);
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Returns number of rows in the matrix.
-   */
-  int Rows() const { return m_blockRows; }
-
-  /**
-   * Returns number of columns in the matrix.
-   */
-  int Cols() const { return m_blockCols; }
-
-  /**
-   * Returns an element of the variable matrix.
-   *
-   * @param row The row of the element to return.
-   * @param col The column of the element to return.
-   */
-  double Value(int row, int col) const {
-    Assert(row >= 0 && row < Rows());
-    Assert(col >= 0 && col < Cols());
-    return (*m_mat)(m_rowOffset + row, m_colOffset + col).Value();
-  }
-
-  /**
-   * Returns a row of the variable column vector.
-   *
-   * @param index The index of the element to return.
-   */
-  double Value(int index) const {
-    Assert(index >= 0 && index < Rows() * Cols());
-    return (*m_mat)(m_rowOffset + index / m_blockCols,
-                    m_colOffset + index % m_blockCols)
-        .Value();
-  }
-
-  /**
-   * Returns the contents of the variable matrix.
-   */
-  Eigen::MatrixXd Value() const {
-    Eigen::MatrixXd result{Rows(), Cols()};
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        result(row, col) = Value(row, col);
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Transforms the matrix coefficient-wise with an unary operator.
-   *
-   * @param unaryOp The unary operator to use for the transform operation.
-   */
-  template <std::invocable<const Variable&> UnaryOp>
-  std::remove_cv_t<Mat> CwiseTransform(UnaryOp&& unaryOp) const {
-    std::remove_cv_t<Mat> result{Rows(), Cols()};
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        result(row, col) = unaryOp((*this)(row, col));
-      }
-    }
-
-    return result;
-  }
-
-  class iterator {
-   public:
-    using iterator_category = std::forward_iterator_tag;
-    using value_type = Variable;
-    using difference_type = std::ptrdiff_t;
-    using pointer = Variable*;
-    using reference = Variable&;
-
-    iterator(VariableBlock<Mat>* mat, int row, int col)
-        : m_mat{mat}, m_row{row}, m_col{col} {}
-
-    iterator& operator++() {
-      ++m_col;
-      if (m_col == m_mat->Cols()) {
-        m_col = 0;
-        ++m_row;
-      }
-      return *this;
-    }
-    iterator operator++(int) {
-      iterator retval = *this;
-      ++(*this);
-      return retval;
-    }
-    bool operator==(const iterator&) const = default;
-    reference operator*() { return (*m_mat)(m_row, m_col); }
-
-   private:
-    VariableBlock<Mat>* m_mat;
-    int m_row;
-    int m_col;
-  };
-
-  class const_iterator {
-   public:
-    using iterator_category = std::forward_iterator_tag;
-    using value_type = Variable;
-    using difference_type = std::ptrdiff_t;
-    using pointer = Variable*;
-    using const_reference = const Variable&;
-
-    const_iterator(const VariableBlock<Mat>* mat, int row, int col)
-        : m_mat{mat}, m_row{row}, m_col{col} {}
-
-    const_iterator& operator++() {
-      ++m_col;
-      if (m_col == m_mat->Cols()) {
-        m_col = 0;
-        ++m_row;
-      }
-      return *this;
-    }
-    const_iterator operator++(int) {
-      const_iterator retval = *this;
-      ++(*this);
-      return retval;
-    }
-    bool operator==(const const_iterator&) const = default;
-    const_reference operator*() const { return (*m_mat)(m_row, m_col); }
-
-   private:
-    const VariableBlock<Mat>* m_mat;
-    int m_row;
-    int m_col;
-  };
-
-  /**
-   * Returns begin iterator.
-   */
-  iterator begin() { return iterator(this, 0, 0); }
-
-  /**
-   * Returns end iterator.
-   */
-  iterator end() { return iterator(this, Rows(), 0); }
-
-  /**
-   * Returns begin iterator.
-   */
-  const_iterator begin() const { return const_iterator(this, 0, 0); }
-
-  /**
-   * Returns end iterator.
-   */
-  const_iterator end() const { return const_iterator(this, Rows(), 0); }
-
-  /**
-   * Returns begin iterator.
-   */
-  const_iterator cbegin() const { return const_iterator(this, 0, 0); }
-
-  /**
-   * Returns end iterator.
-   */
-  const_iterator cend() const { return const_iterator(this, Rows(), 0); }
-
-  /**
-   * Returns number of elements in matrix.
-   */
-  size_t size() const { return m_blockRows * m_blockCols; }
-
- private:
-  Mat* m_mat = nullptr;
-  int m_rowOffset = 0;
-  int m_colOffset = 0;
-  int m_blockRows = 0;
-  int m_blockCols = 0;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <concepts>
+#include <type_traits>
+#include <utility>
+
+#include <Eigen/Core>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/util/Assert.hpp"
+
+namespace sleipnir {
+
+/**
+ * A submatrix of autodiff variables with reference semantics.
+ *
+ * @tparam Mat The type of the matrix whose storage this class points to.
+ */
+template <typename Mat>
+class VariableBlock {
+ public:
+  VariableBlock(const VariableBlock<Mat>& values) = default;
+
+  /**
+   * Assigns a VariableBlock to the block.
+   */
+  VariableBlock<Mat>& operator=(const VariableBlock<Mat>& values) {
+    if (this == &values) {
+      return *this;
+    }
+
+    if (m_mat == nullptr) {
+      m_mat = values.m_mat;
+      m_rowOffset = values.m_rowOffset;
+      m_colOffset = values.m_colOffset;
+      m_blockRows = values.m_blockRows;
+      m_blockCols = values.m_blockCols;
+    } else {
+      Assert(Rows() == values.Rows());
+      Assert(Cols() == values.Cols());
+
+      for (int row = 0; row < Rows(); ++row) {
+        for (int col = 0; col < Cols(); ++col) {
+          (*this)(row, col) = values(row, col);
+        }
+      }
+    }
+
+    return *this;
+  }
+
+  VariableBlock(VariableBlock<Mat>&&) = default;
+
+  /**
+   * Assigns a VariableBlock to the block.
+   */
+  VariableBlock<Mat>& operator=(VariableBlock<Mat>&& values) {
+    if (this == &values) {
+      return *this;
+    }
+
+    if (m_mat == nullptr) {
+      m_mat = values.m_mat;
+      m_rowOffset = values.m_rowOffset;
+      m_colOffset = values.m_colOffset;
+      m_blockRows = values.m_blockRows;
+      m_blockCols = values.m_blockCols;
+    } else {
+      Assert(Rows() == values.Rows());
+      Assert(Cols() == values.Cols());
+
+      for (int row = 0; row < Rows(); ++row) {
+        for (int col = 0; col < Cols(); ++col) {
+          (*this)(row, col) = values(row, col);
+        }
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Constructs a Variable block pointing to all of the given matrix.
+   *
+   * @param mat The matrix to which to point.
+   */
+  VariableBlock(Mat& mat)  // NOLINT
+      : m_mat{&mat}, m_blockRows{mat.Rows()}, m_blockCols{mat.Cols()} {}
+
+  /**
+   * Constructs a Variable block pointing to a subset of the given matrix.
+   *
+   * @param mat The matrix to which to point.
+   * @param rowOffset The block's row offset.
+   * @param colOffset The block's column offset.
+   * @param blockRows The number of rows in the block.
+   * @param blockCols The number of columns in the block.
+   */
+  VariableBlock(Mat& mat, int rowOffset, int colOffset, int blockRows,
+                int blockCols)
+      : m_mat{&mat},
+        m_rowOffset{rowOffset},
+        m_colOffset{colOffset},
+        m_blockRows{blockRows},
+        m_blockCols{blockCols} {}
+
+  /**
+   * Assigns a double to the block.
+   *
+   * This only works for blocks with one row and one column.
+   */
+  VariableBlock<Mat>& operator=(double value) {
+    Assert(Rows() == 1 && Cols() == 1);
+
+    (*this)(0, 0) = value;
+
+    return *this;
+  }
+
+  /**
+   * Assigns a double to the block.
+   *
+   * This only works for blocks with one row and one column.
+   */
+  VariableBlock<Mat>& SetValue(double value) {
+    Assert(Rows() == 1 && Cols() == 1);
+
+    (*this)(0, 0).SetValue(value);
+
+    return *this;
+  }
+
+  /**
+   * Assigns an Eigen matrix to the block.
+   */
+  template <typename Derived>
+  VariableBlock<Mat>& operator=(const Eigen::MatrixBase<Derived>& values) {
+    Assert(Rows() == values.rows());
+    Assert(Cols() == values.cols());
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) = values(row, col);
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Sets block's internal values.
+   */
+  template <typename Derived>
+    requires std::same_as<typename Derived::Scalar, double>
+  VariableBlock<Mat>& SetValue(const Eigen::MatrixBase<Derived>& values) {
+    Assert(Rows() == values.rows());
+    Assert(Cols() == values.cols());
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col).SetValue(values(row, col));
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Assigns a VariableMatrix to the block.
+   */
+  VariableBlock<Mat>& operator=(const Mat& values) {
+    Assert(Rows() == values.Rows());
+    Assert(Cols() == values.Cols());
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) = values(row, col);
+      }
+    }
+    return *this;
+  }
+
+  /**
+   * Assigns a VariableMatrix to the block.
+   */
+  VariableBlock<Mat>& operator=(Mat&& values) {
+    Assert(Rows() == values.Rows());
+    Assert(Cols() == values.Cols());
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) = std::move(values(row, col));
+      }
+    }
+    return *this;
+  }
+
+  /**
+   * Returns a scalar subblock at the given row and column.
+   *
+   * @param row The scalar subblock's row.
+   * @param col The scalar subblock's column.
+   */
+  template <typename Mat2 = Mat>
+    requires(!std::is_const_v<Mat2>)
+  Variable& operator()(int row, int col) {
+    Assert(row >= 0 && row < Rows());
+    Assert(col >= 0 && col < Cols());
+    return (*m_mat)(m_rowOffset + row, m_colOffset + col);
+  }
+
+  /**
+   * Returns a scalar subblock at the given row and column.
+   *
+   * @param row The scalar subblock's row.
+   * @param col The scalar subblock's column.
+   */
+  const Variable& operator()(int row, int col) const {
+    Assert(row >= 0 && row < Rows());
+    Assert(col >= 0 && col < Cols());
+    return (*m_mat)(m_rowOffset + row, m_colOffset + col);
+  }
+
+  /**
+   * Returns a scalar subblock at the given row.
+   *
+   * @param row The scalar subblock's row.
+   */
+  template <typename Mat2 = Mat>
+    requires(!std::is_const_v<Mat2>)
+  Variable& operator()(int row) {
+    Assert(row >= 0 && row < Rows() * Cols());
+    return (*this)(row / Cols(), row % Cols());
+  }
+
+  /**
+   * Returns a scalar subblock at the given row.
+   *
+   * @param row The scalar subblock's row.
+   */
+  const Variable& operator()(int row) const {
+    Assert(row >= 0 && row < Rows() * Cols());
+    return (*this)(row / Cols(), row % Cols());
+  }
+
+  /**
+   * Returns a block slice of the variable matrix.
+   *
+   * @param rowOffset The row offset of the block selection.
+   * @param colOffset The column offset of the block selection.
+   * @param blockRows The number of rows in the block selection.
+   * @param blockCols The number of columns in the block selection.
+   */
+  VariableBlock<Mat> Block(int rowOffset, int colOffset, int blockRows,
+                           int blockCols) {
+    Assert(rowOffset >= 0 && rowOffset <= Rows());
+    Assert(colOffset >= 0 && colOffset <= Cols());
+    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
+    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
+    return VariableBlock{*m_mat, m_rowOffset + rowOffset,
+                         m_colOffset + colOffset, blockRows, blockCols};
+  }
+
+  /**
+   * Returns a block slice of the variable matrix.
+   *
+   * @param rowOffset The row offset of the block selection.
+   * @param colOffset The column offset of the block selection.
+   * @param blockRows The number of rows in the block selection.
+   * @param blockCols The number of columns in the block selection.
+   */
+  const VariableBlock<const Mat> Block(int rowOffset, int colOffset,
+                                       int blockRows, int blockCols) const {
+    Assert(rowOffset >= 0 && rowOffset <= Rows());
+    Assert(colOffset >= 0 && colOffset <= Cols());
+    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
+    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
+    return VariableBlock{*m_mat, m_rowOffset + rowOffset,
+                         m_colOffset + colOffset, blockRows, blockCols};
+  }
+
+  /**
+   * Returns a row slice of the variable matrix.
+   *
+   * @param row The row to slice.
+   */
+  VariableBlock<Mat> Row(int row) {
+    Assert(row >= 0 && row < Rows());
+    return Block(row, 0, 1, Cols());
+  }
+
+  /**
+   * Returns a row slice of the variable matrix.
+   *
+   * @param row The row to slice.
+   */
+  VariableBlock<const Mat> Row(int row) const {
+    Assert(row >= 0 && row < Rows());
+    return Block(row, 0, 1, Cols());
+  }
+
+  /**
+   * Returns a column slice of the variable matrix.
+   *
+   * @param col The column to slice.
+   */
+  VariableBlock<Mat> Col(int col) {
+    Assert(col >= 0 && col < Cols());
+    return Block(0, col, Rows(), 1);
+  }
+
+  /**
+   * Returns a column slice of the variable matrix.
+   *
+   * @param col The column to slice.
+   */
+  VariableBlock<const Mat> Col(int col) const {
+    Assert(col >= 0 && col < Cols());
+    return Block(0, col, Rows(), 1);
+  }
+
+  /**
+   * Compound matrix multiplication-assignment operator.
+   *
+   * @param rhs Variable to multiply.
+   */
+  VariableBlock<Mat>& operator*=(const VariableBlock<Mat>& rhs) {
+    Assert(Cols() == rhs.Rows() && Cols() == rhs.Cols());
+
+    for (int i = 0; i < Rows(); ++i) {
+      for (int j = 0; j < rhs.Cols(); ++j) {
+        Variable sum;
+        for (int k = 0; k < Cols(); ++k) {
+          sum += (*this)(i, k) * rhs(k, j);
+        }
+        (*this)(i, j) = sum;
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Compound matrix multiplication-assignment operator (only enabled when lhs
+   * is a scalar).
+   *
+   * @param rhs Variable to multiply.
+   */
+  VariableBlock& operator*=(double rhs) {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) *= rhs;
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Compound matrix division-assignment operator (only enabled when rhs
+   * is a scalar).
+   *
+   * @param rhs Variable to divide.
+   */
+  VariableBlock<Mat>& operator/=(const VariableBlock<Mat>& rhs) {
+    Assert(rhs.Rows() == 1 && rhs.Cols() == 1);
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) /= rhs(0, 0);
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Compound matrix division-assignment operator (only enabled when rhs
+   * is a scalar).
+   *
+   * @param rhs Variable to divide.
+   */
+  VariableBlock<Mat>& operator/=(double rhs) {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) /= rhs;
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Compound addition-assignment operator.
+   *
+   * @param rhs Variable to add.
+   */
+  VariableBlock<Mat>& operator+=(const VariableBlock<Mat>& rhs) {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) += rhs(row, col);
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Compound subtraction-assignment operator.
+   *
+   * @param rhs Variable to subtract.
+   */
+  VariableBlock<Mat>& operator-=(const VariableBlock<Mat>& rhs) {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) -= rhs(row, col);
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Returns the transpose of the variable matrix.
+   */
+  std::remove_cv_t<Mat> T() const {
+    std::remove_cv_t<Mat> result{Cols(), Rows()};
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        result(col, row) = (*this)(row, col);
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Returns number of rows in the matrix.
+   */
+  int Rows() const { return m_blockRows; }
+
+  /**
+   * Returns number of columns in the matrix.
+   */
+  int Cols() const { return m_blockCols; }
+
+  /**
+   * Returns an element of the variable matrix.
+   *
+   * @param row The row of the element to return.
+   * @param col The column of the element to return.
+   */
+  double Value(int row, int col) const {
+    Assert(row >= 0 && row < Rows());
+    Assert(col >= 0 && col < Cols());
+    return (*m_mat)(m_rowOffset + row, m_colOffset + col).Value();
+  }
+
+  /**
+   * Returns a row of the variable column vector.
+   *
+   * @param index The index of the element to return.
+   */
+  double Value(int index) const {
+    Assert(index >= 0 && index < Rows() * Cols());
+    return (*m_mat)(m_rowOffset + index / m_blockCols,
+                    m_colOffset + index % m_blockCols)
+        .Value();
+  }
+
+  /**
+   * Returns the contents of the variable matrix.
+   */
+  Eigen::MatrixXd Value() const {
+    Eigen::MatrixXd result{Rows(), Cols()};
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        result(row, col) = Value(row, col);
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Transforms the matrix coefficient-wise with an unary operator.
+   *
+   * @param unaryOp The unary operator to use for the transform operation.
+   */
+  template <std::invocable<const Variable&> UnaryOp>
+  std::remove_cv_t<Mat> CwiseTransform(UnaryOp&& unaryOp) const {
+    std::remove_cv_t<Mat> result{Rows(), Cols()};
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        result(row, col) = unaryOp((*this)(row, col));
+      }
+    }
+
+    return result;
+  }
+
+  class iterator {
+   public:
+    using iterator_category = std::forward_iterator_tag;
+    using value_type = Variable;
+    using difference_type = std::ptrdiff_t;
+    using pointer = Variable*;
+    using reference = Variable&;
+
+    iterator(VariableBlock<Mat>* mat, int row, int col)
+        : m_mat{mat}, m_row{row}, m_col{col} {}
+
+    iterator& operator++() {
+      ++m_col;
+      if (m_col == m_mat->Cols()) {
+        m_col = 0;
+        ++m_row;
+      }
+      return *this;
+    }
+    iterator operator++(int) {
+      iterator retval = *this;
+      ++(*this);
+      return retval;
+    }
+    bool operator==(const iterator&) const = default;
+    reference operator*() { return (*m_mat)(m_row, m_col); }
+
+   private:
+    VariableBlock<Mat>* m_mat;
+    int m_row;
+    int m_col;
+  };
+
+  class const_iterator {
+   public:
+    using iterator_category = std::forward_iterator_tag;
+    using value_type = Variable;
+    using difference_type = std::ptrdiff_t;
+    using pointer = Variable*;
+    using const_reference = const Variable&;
+
+    const_iterator(const VariableBlock<Mat>* mat, int row, int col)
+        : m_mat{mat}, m_row{row}, m_col{col} {}
+
+    const_iterator& operator++() {
+      ++m_col;
+      if (m_col == m_mat->Cols()) {
+        m_col = 0;
+        ++m_row;
+      }
+      return *this;
+    }
+    const_iterator operator++(int) {
+      const_iterator retval = *this;
+      ++(*this);
+      return retval;
+    }
+    bool operator==(const const_iterator&) const = default;
+    const_reference operator*() const { return (*m_mat)(m_row, m_col); }
+
+   private:
+    const VariableBlock<Mat>* m_mat;
+    int m_row;
+    int m_col;
+  };
+
+  /**
+   * Returns begin iterator.
+   */
+  iterator begin() { return iterator(this, 0, 0); }
+
+  /**
+   * Returns end iterator.
+   */
+  iterator end() { return iterator(this, Rows(), 0); }
+
+  /**
+   * Returns begin iterator.
+   */
+  const_iterator begin() const { return const_iterator(this, 0, 0); }
+
+  /**
+   * Returns end iterator.
+   */
+  const_iterator end() const { return const_iterator(this, Rows(), 0); }
+
+  /**
+   * Returns begin iterator.
+   */
+  const_iterator cbegin() const { return const_iterator(this, 0, 0); }
+
+  /**
+   * Returns end iterator.
+   */
+  const_iterator cend() const { return const_iterator(this, Rows(), 0); }
+
+  /**
+   * Returns number of elements in matrix.
+   */
+  size_t size() const { return m_blockRows * m_blockCols; }
+
+ private:
+  Mat* m_mat = nullptr;
+  int m_rowOffset = 0;
+  int m_colOffset = 0;
+  int m_blockRows = 0;
+  int m_blockCols = 0;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/autodiff/VariableMatrix.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/autodiff/VariableMatrix.hpp`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,1006 +1,1006 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <algorithm>
-#include <concepts>
-#include <initializer_list>
-#include <iterator>
-#include <span>
-#include <utility>
-#include <vector>
-
-#include <Eigen/Core>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/autodiff/VariableBlock.hpp"
-#include "sleipnir/util/Assert.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * A matrix of autodiff variables.
- */
-class SLEIPNIR_DLLEXPORT VariableMatrix {
- public:
-  /**
-   * Constructs an empty VariableMatrix.
-   */
-  VariableMatrix() = default;
-
-  /**
-   * Constructs a VariableMatrix column vector with the given rows.
-   *
-   * @param rows The number of matrix rows.
-   */
-  explicit VariableMatrix(int rows) : m_rows{rows}, m_cols{1} {
-    for (int row = 0; row < rows; ++row) {
-      m_storage.emplace_back();
-    }
-  }
-
-  /**
-   * Constructs a VariableMatrix with the given dimensions.
-   *
-   * @param rows The number of matrix rows.
-   * @param cols The number of matrix columns.
-   */
-  VariableMatrix(int rows, int cols) : m_rows{rows}, m_cols{cols} {
-    for (int row = 0; row < rows; ++row) {
-      for (int col = 0; col < cols; ++col) {
-        m_storage.emplace_back();
-      }
-    }
-  }
-
-  /**
-   * Constructs a scalar VariableMatrix from a nested list of Variables.
-   *
-   * @param list The nested list of Variables.
-   */
-  VariableMatrix(  // NOLINT
-      std::initializer_list<std::initializer_list<Variable>> list) {
-    // Get row and column counts for destination matrix
-    m_rows = list.size();
-    m_cols = 0;
-    if (list.size() > 0) {
-      m_cols = list.begin()->size();
-    }
-
-    // Assert the first and latest column counts are the same
-    for ([[maybe_unused]]
-         const auto& row : list) {
-      Assert(list.begin()->size() == row.size());
-    }
-
-    m_storage.reserve(Rows() * Cols());
-    for (const auto& row : list) {
-      std::copy(row.begin(), row.end(), std::back_inserter(m_storage));
-    }
-  }
-
-  /**
-   * Constructs a scalar VariableMatrix from a nested list of doubles.
-   *
-   * This overload is for Python bindings only.
-   *
-   * @param list The nested list of Variables.
-   */
-  VariableMatrix(std::vector<std::vector<double>> list) {  // NOLINT
-    // Get row and column counts for destination matrix
-    m_rows = list.size();
-    m_cols = 0;
-    if (list.size() > 0) {
-      m_cols = list.begin()->size();
-    }
-
-    // Assert the first and latest column counts are the same
-    for ([[maybe_unused]]
-         const auto& row : list) {
-      Assert(list.begin()->size() == row.size());
-    }
-
-    m_storage.reserve(Rows() * Cols());
-    for (const auto& row : list) {
-      std::copy(row.begin(), row.end(), std::back_inserter(m_storage));
-    }
-  }
-
-  /**
-   * Constructs a scalar VariableMatrix from a nested list of Variables.
-   *
-   * This overload is for Python bindings only.
-   *
-   * @param list The nested list of Variables.
-   */
-  VariableMatrix(std::vector<std::vector<Variable>> list) {  // NOLINT
-    // Get row and column counts for destination matrix
-    m_rows = list.size();
-    m_cols = 0;
-    if (list.size() > 0) {
-      m_cols = list.begin()->size();
-    }
-
-    // Assert the first and latest column counts are the same
-    for ([[maybe_unused]]
-         const auto& row : list) {
-      Assert(list.begin()->size() == row.size());
-    }
-
-    m_storage.reserve(Rows() * Cols());
-    for (const auto& row : list) {
-      std::copy(row.begin(), row.end(), std::back_inserter(m_storage));
-    }
-  }
-
-  /**
-   * Constructs a VariableMatrix from an Eigen matrix.
-   */
-  template <typename Derived>
-  VariableMatrix(const Eigen::MatrixBase<Derived>& values)  // NOLINT
-      : m_rows{static_cast<int>(values.rows())},
-        m_cols{static_cast<int>(values.cols())} {
-    m_storage.reserve(values.rows() * values.cols());
-    for (int row = 0; row < values.rows(); ++row) {
-      for (int col = 0; col < values.cols(); ++col) {
-        m_storage.emplace_back(values(row, col));
-      }
-    }
-  }
-
-  /**
-   * Constructs a VariableMatrix from an Eigen diagonal matrix.
-   */
-  template <typename Derived>
-  VariableMatrix(const Eigen::DiagonalBase<Derived>& values)  // NOLINT
-      : m_rows{static_cast<int>(values.rows())},
-        m_cols{static_cast<int>(values.cols())} {
-    m_storage.reserve(values.rows() * values.cols());
-    for (int row = 0; row < values.rows(); ++row) {
-      for (int col = 0; col < values.cols(); ++col) {
-        if (row == col) {
-          m_storage.emplace_back(values.diagonal()(row));
-        } else {
-          m_storage.emplace_back(0.0);
-        }
-      }
-    }
-  }
-
-  /**
-   * Assigns an Eigen matrix to a VariableMatrix.
-   */
-  template <typename Derived>
-  VariableMatrix& operator=(const Eigen::MatrixBase<Derived>& values) {
-    Assert(Rows() == values.rows());
-    Assert(Cols() == values.cols());
-
-    for (int row = 0; row < values.rows(); ++row) {
-      for (int col = 0; col < values.cols(); ++col) {
-        (*this)(row, col) = values(row, col);
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Sets the VariableMatrix's internal values.
-   */
-  template <typename Derived>
-    requires std::same_as<typename Derived::Scalar, double>
-  VariableMatrix& SetValue(const Eigen::MatrixBase<Derived>& values) {
-    Assert(Rows() == values.rows());
-    Assert(Cols() == values.cols());
-
-    for (int row = 0; row < values.rows(); ++row) {
-      for (int col = 0; col < values.cols(); ++col) {
-        (*this)(row, col).SetValue(values(row, col));
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Constructs a scalar VariableMatrix from a Variable.
-   */
-  VariableMatrix(const Variable& variable)  // NOLINT
-      : m_rows{1}, m_cols{1} {
-    m_storage.emplace_back(variable);
-  }
-
-  /**
-   * Constructs a scalar VariableMatrix from a Variable.
-   */
-  VariableMatrix(Variable&& variable) : m_rows{1}, m_cols{1} {  // NOLINT
-    m_storage.emplace_back(std::move(variable));
-  }
-
-  /**
-   * Constructs a VariableMatrix from a VariableBlock.
-   */
-  VariableMatrix(const VariableBlock<VariableMatrix>& values)  // NOLINT
-      : m_rows{values.Rows()}, m_cols{values.Cols()} {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        m_storage.emplace_back(values(row, col));
-      }
-    }
-  }
-
-  /**
-   * Constructs a VariableMatrix from a VariableBlock.
-   */
-  VariableMatrix(const VariableBlock<const VariableMatrix>& values)  // NOLINT
-      : m_rows{values.Rows()}, m_cols{values.Cols()} {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        m_storage.emplace_back(values(row, col));
-      }
-    }
-  }
-
-  /**
-   * Constructs a column vector wrapper around a Variable array.
-   *
-   * @param values Variable array to wrap.
-   */
-  explicit VariableMatrix(std::span<const Variable> values)
-      : m_rows{static_cast<int>(values.size())}, m_cols{1} {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        m_storage.emplace_back(values[row * Cols() + col]);
-      }
-    }
-  }
-
-  /**
-   * Constructs a matrix wrapper around a Variable array.
-   *
-   * @param values Variable array to wrap.
-   * @param rows The number of matrix rows.
-   * @param cols The number of matrix columns.
-   */
-  VariableMatrix(std::span<const Variable> values, int rows, int cols)
-      : m_rows{rows}, m_cols{cols} {
-    Assert(static_cast<int>(values.size()) == Rows() * Cols());
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        m_storage.emplace_back(values[row * Cols() + col]);
-      }
-    }
-  }
-
-  /**
-   * Returns a block pointing to the given row and column.
-   *
-   * @param row The block row.
-   * @param col The block column.
-   */
-  Variable& operator()(int row, int col) {
-    Assert(row >= 0 && row < Rows());
-    Assert(col >= 0 && col < Cols());
-    return m_storage[row * Cols() + col];
-  }
-
-  /**
-   * Returns a block pointing to the given row and column.
-   *
-   * @param row The block row.
-   * @param col The block column.
-   */
-  const Variable& operator()(int row, int col) const {
-    Assert(row >= 0 && row < Rows());
-    Assert(col >= 0 && col < Cols());
-    return m_storage[row * Cols() + col];
-  }
-
-  /**
-   * Returns a block pointing to the given row.
-   *
-   * @param row The block row.
-   */
-  Variable& operator()(int row) {
-    Assert(row >= 0 && row < Rows() * Cols());
-    return m_storage[row];
-  }
-
-  /**
-   * Returns a block pointing to the given row.
-   *
-   * @param row The block row.
-   */
-  const Variable& operator()(int row) const {
-    Assert(row >= 0 && row < Rows() * Cols());
-    return m_storage[row];
-  }
-
-  /**
-   * Returns a block slice of the variable matrix.
-   *
-   * @param rowOffset The row offset of the block selection.
-   * @param colOffset The column offset of the block selection.
-   * @param blockRows The number of rows in the block selection.
-   * @param blockCols The number of columns in the block selection.
-   */
-  VariableBlock<VariableMatrix> Block(int rowOffset, int colOffset,
-                                      int blockRows, int blockCols) {
-    Assert(rowOffset >= 0 && rowOffset <= Rows());
-    Assert(colOffset >= 0 && colOffset <= Cols());
-    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
-    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
-    return VariableBlock{*this, rowOffset, colOffset, blockRows, blockCols};
-  }
-
-  /**
-   * Returns a block slice of the variable matrix.
-   *
-   * @param rowOffset The row offset of the block selection.
-   * @param colOffset The column offset of the block selection.
-   * @param blockRows The number of rows in the block selection.
-   * @param blockCols The number of columns in the block selection.
-   */
-  const VariableBlock<const VariableMatrix> Block(int rowOffset, int colOffset,
-                                                  int blockRows,
-                                                  int blockCols) const {
-    Assert(rowOffset >= 0 && rowOffset <= Rows());
-    Assert(colOffset >= 0 && colOffset <= Cols());
-    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
-    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
-    return VariableBlock{*this, rowOffset, colOffset, blockRows, blockCols};
-  }
-
-  /**
-   * Returns a segment of the variable vector.
-   *
-   * @param offset The offset of the segment.
-   * @param length The length of the segment.
-   */
-  VariableBlock<VariableMatrix> Segment(int offset, int length) {
-    Assert(offset >= 0 && offset < Rows() * Cols());
-    Assert(length >= 0 && length <= Rows() * Cols() - offset);
-    return Block(offset, 0, length, 1);
-  }
-
-  /**
-   * Returns a segment of the variable vector.
-   *
-   * @param offset The offset of the segment.
-   * @param length The length of the segment.
-   */
-  const VariableBlock<const VariableMatrix> Segment(int offset,
-                                                    int length) const {
-    Assert(offset >= 0 && offset < Rows() * Cols());
-    Assert(length >= 0 && length <= Rows() * Cols() - offset);
-    return Block(offset, 0, length, 1);
-  }
-
-  /**
-   * Returns a row slice of the variable matrix.
-   *
-   * @param row The row to slice.
-   */
-  VariableBlock<VariableMatrix> Row(int row) {
-    Assert(row >= 0 && row < Rows());
-    return Block(row, 0, 1, Cols());
-  }
-
-  /**
-   * Returns a row slice of the variable matrix.
-   *
-   * @param row The row to slice.
-   */
-  const VariableBlock<const VariableMatrix> Row(int row) const {
-    Assert(row >= 0 && row < Rows());
-    return Block(row, 0, 1, Cols());
-  }
-
-  /**
-   * Returns a column slice of the variable matrix.
-   *
-   * @param col The column to slice.
-   */
-  VariableBlock<VariableMatrix> Col(int col) {
-    Assert(col >= 0 && col < Cols());
-    return Block(0, col, Rows(), 1);
-  }
-
-  /**
-   * Returns a column slice of the variable matrix.
-   *
-   * @param col The column to slice.
-   */
-  const VariableBlock<const VariableMatrix> Col(int col) const {
-    Assert(col >= 0 && col < Cols());
-    return Block(0, col, Rows(), 1);
-  }
-
-  /**
-   * Matrix multiplication operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix
-  operator*(const VariableMatrix& lhs, const VariableMatrix& rhs) {
-    Assert(lhs.Cols() == rhs.Rows());
-
-    VariableMatrix result{lhs.Rows(), rhs.Cols()};
-
-    for (int i = 0; i < lhs.Rows(); ++i) {
-      for (int j = 0; j < rhs.Cols(); ++j) {
-        Variable sum;
-        for (int k = 0; k < lhs.Cols(); ++k) {
-          sum += lhs(i, k) * rhs(k, j);
-        }
-        result(i, j) = sum;
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Matrix-scalar multiplication operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix operator*(const VariableMatrix& lhs,
-                                                     const Variable& rhs) {
-    VariableMatrix result{lhs.Rows(), lhs.Cols()};
-
-    for (int row = 0; row < result.Rows(); ++row) {
-      for (int col = 0; col < result.Cols(); ++col) {
-        result(row, col) = lhs(row, col) * rhs;
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Matrix-scalar multiplication operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix operator*(const VariableMatrix& lhs,
-                                                     double rhs) {
-    return lhs * Variable{rhs};
-  }
-
-  /**
-   * Scalar-matrix multiplication operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix
-  operator*(const Variable& lhs, const VariableMatrix& rhs) {
-    VariableMatrix result{rhs.Rows(), rhs.Cols()};
-
-    for (int row = 0; row < result.Rows(); ++row) {
-      for (int col = 0; col < result.Cols(); ++col) {
-        result(row, col) = rhs(row, col) * lhs;
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Scalar-matrix multiplication operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix
-  operator*(double lhs, const VariableMatrix& rhs) {
-    return Variable{lhs} * rhs;
-  }
-
-  /**
-   * Compound matrix multiplication-assignment operator.
-   *
-   * @param rhs Variable to multiply.
-   */
-  VariableMatrix& operator*=(const VariableMatrix& rhs) {
-    Assert(Cols() == rhs.Rows() && Cols() == rhs.Cols());
-
-    for (int i = 0; i < Rows(); ++i) {
-      for (int j = 0; j < rhs.Cols(); ++j) {
-        Variable sum;
-        for (int k = 0; k < Cols(); ++k) {
-          sum += (*this)(i, k) * rhs(k, j);
-        }
-        (*this)(i, j) = sum;
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Binary division operator (only enabled when rhs is a scalar).
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix operator/(const VariableMatrix& lhs,
-                                                     const Variable& rhs) {
-    VariableMatrix result{lhs.Rows(), lhs.Cols()};
-
-    for (int row = 0; row < result.Rows(); ++row) {
-      for (int col = 0; col < result.Cols(); ++col) {
-        result(row, col) = lhs(row, col) / rhs;
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Compound matrix division-assignment operator (only enabled when rhs
-   * is a scalar).
-   *
-   * @param rhs Variable to divide.
-   */
-  VariableMatrix& operator/=(const Variable& rhs) {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) /= rhs;
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Binary addition operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix
-  operator+(const VariableMatrix& lhs, const VariableMatrix& rhs) {
-    VariableMatrix result{lhs.Rows(), lhs.Cols()};
-
-    for (int row = 0; row < result.Rows(); ++row) {
-      for (int col = 0; col < result.Cols(); ++col) {
-        result(row, col) = lhs(row, col) + rhs(row, col);
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Compound addition-assignment operator.
-   *
-   * @param rhs Variable to add.
-   */
-  VariableMatrix& operator+=(const VariableMatrix& rhs) {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) += rhs(row, col);
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Binary subtraction operator.
-   *
-   * @param lhs Operator left-hand side.
-   * @param rhs Operator right-hand side.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix
-  operator-(const VariableMatrix& lhs, const VariableMatrix& rhs) {
-    VariableMatrix result{lhs.Rows(), lhs.Cols()};
-
-    for (int row = 0; row < result.Rows(); ++row) {
-      for (int col = 0; col < result.Cols(); ++col) {
-        result(row, col) = lhs(row, col) - rhs(row, col);
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Compound subtraction-assignment operator.
-   *
-   * @param rhs Variable to subtract.
-   */
-  VariableMatrix& operator-=(const VariableMatrix& rhs) {
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        (*this)(row, col) -= rhs(row, col);
-      }
-    }
-
-    return *this;
-  }
-
-  /**
-   * Unary minus operator.
-   *
-   * @param lhs Operand for unary minus.
-   */
-  friend SLEIPNIR_DLLEXPORT VariableMatrix
-  operator-(const VariableMatrix& lhs) {
-    VariableMatrix result{lhs.Rows(), lhs.Cols()};
-
-    for (int row = 0; row < result.Rows(); ++row) {
-      for (int col = 0; col < result.Cols(); ++col) {
-        result(row, col) = -lhs(row, col);
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Implicit conversion operator from 1x1 VariableMatrix to Variable.
-   */
-  operator Variable() const {  // NOLINT
-    Assert(Rows() == 1 && Cols() == 1);
-    return (*this)(0, 0);
-  }
-
-  /**
-   * Returns the transpose of the variable matrix.
-   */
-  VariableMatrix T() const {
-    VariableMatrix result{Cols(), Rows()};
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        result(col, row) = (*this)(row, col);
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Returns number of rows in the matrix.
-   */
-  int Rows() const { return m_rows; }
-
-  /**
-   * Returns number of columns in the matrix.
-   */
-  int Cols() const { return m_cols; }
-
-  /**
-   * Returns an element of the variable matrix.
-   *
-   * @param row The row of the element to return.
-   * @param col The column of the element to return.
-   */
-  double Value(int row, int col) const {
-    Assert(row >= 0 && row < Rows());
-    Assert(col >= 0 && col < Cols());
-    return m_storage[row * Cols() + col].Value();
-  }
-
-  /**
-   * Returns a row of the variable column vector.
-   *
-   * @param index The index of the element to return.
-   */
-  double Value(int index) const {
-    Assert(index >= 0 && index < Rows() * Cols());
-    return m_storage[index].Value();
-  }
-
-  /**
-   * Returns the contents of the variable matrix.
-   */
-  Eigen::MatrixXd Value() const {
-    Eigen::MatrixXd result{Rows(), Cols()};
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        result(row, col) = Value(row, col);
-      }
-    }
-
-    return result;
-  }
-
-  /**
-   * Transforms the matrix coefficient-wise with an unary operator.
-   *
-   * @param unaryOp The unary operator to use for the transform operation.
-   */
-  template <std::invocable<const Variable&> UnaryOp>
-  VariableMatrix CwiseTransform(UnaryOp&& unaryOp) const {
-    VariableMatrix result{Rows(), Cols()};
-
-    for (int row = 0; row < Rows(); ++row) {
-      for (int col = 0; col < Cols(); ++col) {
-        result(row, col) = unaryOp((*this)(row, col));
-      }
-    }
-
-    return result;
-  }
-
-  class iterator {
-   public:
-    using iterator_category = std::forward_iterator_tag;
-    using value_type = Variable;
-    using difference_type = std::ptrdiff_t;
-    using pointer = Variable*;
-    using reference = Variable&;
-
-    iterator(VariableMatrix* mat, int row, int col)
-        : m_mat{mat}, m_row{row}, m_col{col} {}
-
-    iterator& operator++() {
-      ++m_col;
-      if (m_col == m_mat->Cols()) {
-        m_col = 0;
-        ++m_row;
-      }
-      return *this;
-    }
-    iterator operator++(int) {
-      iterator retval = *this;
-      ++(*this);
-      return retval;
-    }
-    bool operator==(const iterator&) const = default;
-    reference operator*() { return (*m_mat)(m_row, m_col); }
-
-   private:
-    VariableMatrix* m_mat;
-    int m_row;
-    int m_col;
-  };
-
-  class const_iterator {
-   public:
-    using iterator_category = std::forward_iterator_tag;
-    using value_type = Variable;
-    using difference_type = std::ptrdiff_t;
-    using pointer = Variable*;
-    using const_reference = const Variable&;
-
-    const_iterator(const VariableMatrix* mat, int row, int col)
-        : m_mat{mat}, m_row{row}, m_col{col} {}
-
-    const_iterator& operator++() {
-      ++m_col;
-      if (m_col == m_mat->Cols()) {
-        m_col = 0;
-        ++m_row;
-      }
-      return *this;
-    }
-    const_iterator operator++(int) {
-      const_iterator retval = *this;
-      ++(*this);
-      return retval;
-    }
-    bool operator==(const const_iterator&) const = default;
-    const_reference operator*() const { return (*m_mat)(m_row, m_col); }
-
-   private:
-    const VariableMatrix* m_mat;
-    int m_row;
-    int m_col;
-  };
-
-  /**
-   * Returns begin iterator.
-   */
-  iterator begin() { return iterator(this, 0, 0); }
-
-  /**
-   * Returns end iterator.
-   */
-  iterator end() { return iterator(this, Rows(), 0); }
-
-  /**
-   * Returns begin iterator.
-   */
-  const_iterator begin() const { return const_iterator(this, 0, 0); }
-
-  /**
-   * Returns end iterator.
-   */
-  const_iterator end() const { return const_iterator(this, Rows(), 0); }
-
-  /**
-   * Returns begin iterator.
-   */
-  const_iterator cbegin() const { return const_iterator(this, 0, 0); }
-
-  /**
-   * Returns end iterator.
-   */
-  const_iterator cend() const { return const_iterator(this, Rows(), 0); }
-
-  /**
-   * Returns number of elements in matrix.
-   */
-  size_t size() const { return m_rows * m_cols; }
-
-  /**
-   * Returns a variable matrix filled with zeroes.
-   *
-   * @param rows The number of matrix rows.
-   * @param cols The number of matrix columns.
-   */
-  static VariableMatrix Zero(int rows, int cols) {
-    VariableMatrix result{rows, cols};
-
-    for (auto& elem : result) {
-      elem = 0.0;
-    }
-
-    return result;
-  }
-
-  /**
-   * Returns a variable matrix filled with ones.
-   *
-   * @param rows The number of matrix rows.
-   * @param cols The number of matrix columns.
-   */
-  static VariableMatrix Ones(int rows, int cols) {
-    VariableMatrix result{rows, cols};
-
-    for (auto& elem : result) {
-      elem = 1.0;
-    }
-
-    return result;
-  }
-
- private:
-  std::vector<Variable> m_storage;
-  int m_rows = 0;
-  int m_cols = 0;
-};
-
-/**
- * Applies a coefficient-wise reduce operation to two matrices.
- *
- * @param lhs The left-hand side of the binary operator.
- * @param rhs The right-hand side of the binary operator.
- * @param binaryOp The binary operator to use for the reduce operation.
- */
-template <std::invocable<const Variable&, const Variable&> BinaryOp>
-VariableMatrix CwiseReduce(const VariableMatrix& lhs, const VariableMatrix& rhs,
-                           BinaryOp&& binaryOp) {
-  Assert(lhs.Rows() == rhs.Rows());
-  Assert(lhs.Rows() == rhs.Rows());
-
-  VariableMatrix result{lhs.Rows(), lhs.Cols()};
-
-  for (int row = 0; row < lhs.Rows(); ++row) {
-    for (int col = 0; col < lhs.Cols(); ++col) {
-      result(row, col) = binaryOp(lhs(row, col), rhs(row, col));
-    }
-  }
-
-  return result;
-}
-
-/**
- * Assemble a VariableMatrix from a nested list of blocks.
- *
- * Each row's blocks must have the same height, and the assembled block rows
- * must have the same width. For example, for the block matrix [[A, B], [C]] to
- * be constructible, the number of rows in A and B must match, and the number of
- * columns in [A, B] and [C] must match.
- *
- * @param list The nested list of blocks.
- */
-SLEIPNIR_DLLEXPORT inline VariableMatrix Block(
-    std::initializer_list<std::initializer_list<VariableMatrix>> list) {
-  // Get row and column counts for destination matrix
-  int rows = 0;
-  int cols = -1;
-  for (const auto& row : list) {
-    if (row.size() > 0) {
-      rows += row.begin()->Rows();
-    }
-
-    // Get number of columns in this row
-    int latestCols = 0;
-    for (const auto& elem : row) {
-      // Assert the first and latest row have the same height
-      Assert(row.begin()->Rows() == elem.Rows());
-
-      latestCols += elem.Cols();
-    }
-
-    // If this is the first row, record the column count. Otherwise, assert the
-    // first and latest column counts are the same.
-    if (cols == -1) {
-      cols = latestCols;
-    } else {
-      Assert(cols == latestCols);
-    }
-  }
-
-  VariableMatrix result{rows, cols};
-
-  int rowOffset = 0;
-  for (const auto& row : list) {
-    int colOffset = 0;
-    for (const auto& elem : row) {
-      result.Block(rowOffset, colOffset, elem.Rows(), elem.Cols()) = elem;
-      colOffset += elem.Cols();
-    }
-    rowOffset += row.begin()->Rows();
-  }
-
-  return result;
-}
-
-/**
- * Assemble a VariableMatrix from a nested list of blocks.
- *
- * Each row's blocks must have the same height, and the assembled block rows
- * must have the same width. For example, for the block matrix [[A, B], [C]] to
- * be constructible, the number of rows in A and B must match, and the number of
- * columns in [A, B] and [C] must match.
- *
- * This overload is for Python bindings only.
- *
- * @param list The nested list of blocks.
- */
-SLEIPNIR_DLLEXPORT inline VariableMatrix Block(
-    std::vector<std::vector<VariableMatrix>> list) {
-  // Get row and column counts for destination matrix
-  int rows = 0;
-  int cols = -1;
-  for (const auto& row : list) {
-    if (row.size() > 0) {
-      rows += row.begin()->Rows();
-    }
-
-    // Get number of columns in this row
-    int latestCols = 0;
-    for (const auto& elem : row) {
-      // Assert the first and latest row have the same height
-      Assert(row.begin()->Rows() == elem.Rows());
-
-      latestCols += elem.Cols();
-    }
-
-    // If this is the first row, record the column count. Otherwise, assert the
-    // first and latest column counts are the same.
-    if (cols == -1) {
-      cols = latestCols;
-    } else {
-      Assert(cols == latestCols);
-    }
-  }
-
-  VariableMatrix result{rows, cols};
-
-  int rowOffset = 0;
-  for (const auto& row : list) {
-    int colOffset = 0;
-    for (const auto& elem : row) {
-      result.Block(rowOffset, colOffset, elem.Rows(), elem.Cols()) = elem;
-      colOffset += elem.Cols();
-    }
-    rowOffset += row.begin()->Rows();
-  }
-
-  return result;
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <algorithm>
+#include <concepts>
+#include <initializer_list>
+#include <iterator>
+#include <span>
+#include <utility>
+#include <vector>
+
+#include <Eigen/Core>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/autodiff/VariableBlock.hpp"
+#include "sleipnir/util/Assert.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * A matrix of autodiff variables.
+ */
+class SLEIPNIR_DLLEXPORT VariableMatrix {
+ public:
+  /**
+   * Constructs an empty VariableMatrix.
+   */
+  VariableMatrix() = default;
+
+  /**
+   * Constructs a VariableMatrix column vector with the given rows.
+   *
+   * @param rows The number of matrix rows.
+   */
+  explicit VariableMatrix(int rows) : m_rows{rows}, m_cols{1} {
+    for (int row = 0; row < rows; ++row) {
+      m_storage.emplace_back();
+    }
+  }
+
+  /**
+   * Constructs a VariableMatrix with the given dimensions.
+   *
+   * @param rows The number of matrix rows.
+   * @param cols The number of matrix columns.
+   */
+  VariableMatrix(int rows, int cols) : m_rows{rows}, m_cols{cols} {
+    for (int row = 0; row < rows; ++row) {
+      for (int col = 0; col < cols; ++col) {
+        m_storage.emplace_back();
+      }
+    }
+  }
+
+  /**
+   * Constructs a scalar VariableMatrix from a nested list of Variables.
+   *
+   * @param list The nested list of Variables.
+   */
+  VariableMatrix(  // NOLINT
+      std::initializer_list<std::initializer_list<Variable>> list) {
+    // Get row and column counts for destination matrix
+    m_rows = list.size();
+    m_cols = 0;
+    if (list.size() > 0) {
+      m_cols = list.begin()->size();
+    }
+
+    // Assert the first and latest column counts are the same
+    for ([[maybe_unused]]
+         const auto& row : list) {
+      Assert(list.begin()->size() == row.size());
+    }
+
+    m_storage.reserve(Rows() * Cols());
+    for (const auto& row : list) {
+      std::copy(row.begin(), row.end(), std::back_inserter(m_storage));
+    }
+  }
+
+  /**
+   * Constructs a scalar VariableMatrix from a nested list of doubles.
+   *
+   * This overload is for Python bindings only.
+   *
+   * @param list The nested list of Variables.
+   */
+  VariableMatrix(std::vector<std::vector<double>> list) {  // NOLINT
+    // Get row and column counts for destination matrix
+    m_rows = list.size();
+    m_cols = 0;
+    if (list.size() > 0) {
+      m_cols = list.begin()->size();
+    }
+
+    // Assert the first and latest column counts are the same
+    for ([[maybe_unused]]
+         const auto& row : list) {
+      Assert(list.begin()->size() == row.size());
+    }
+
+    m_storage.reserve(Rows() * Cols());
+    for (const auto& row : list) {
+      std::copy(row.begin(), row.end(), std::back_inserter(m_storage));
+    }
+  }
+
+  /**
+   * Constructs a scalar VariableMatrix from a nested list of Variables.
+   *
+   * This overload is for Python bindings only.
+   *
+   * @param list The nested list of Variables.
+   */
+  VariableMatrix(std::vector<std::vector<Variable>> list) {  // NOLINT
+    // Get row and column counts for destination matrix
+    m_rows = list.size();
+    m_cols = 0;
+    if (list.size() > 0) {
+      m_cols = list.begin()->size();
+    }
+
+    // Assert the first and latest column counts are the same
+    for ([[maybe_unused]]
+         const auto& row : list) {
+      Assert(list.begin()->size() == row.size());
+    }
+
+    m_storage.reserve(Rows() * Cols());
+    for (const auto& row : list) {
+      std::copy(row.begin(), row.end(), std::back_inserter(m_storage));
+    }
+  }
+
+  /**
+   * Constructs a VariableMatrix from an Eigen matrix.
+   */
+  template <typename Derived>
+  VariableMatrix(const Eigen::MatrixBase<Derived>& values)  // NOLINT
+      : m_rows{static_cast<int>(values.rows())},
+        m_cols{static_cast<int>(values.cols())} {
+    m_storage.reserve(values.rows() * values.cols());
+    for (int row = 0; row < values.rows(); ++row) {
+      for (int col = 0; col < values.cols(); ++col) {
+        m_storage.emplace_back(values(row, col));
+      }
+    }
+  }
+
+  /**
+   * Constructs a VariableMatrix from an Eigen diagonal matrix.
+   */
+  template <typename Derived>
+  VariableMatrix(const Eigen::DiagonalBase<Derived>& values)  // NOLINT
+      : m_rows{static_cast<int>(values.rows())},
+        m_cols{static_cast<int>(values.cols())} {
+    m_storage.reserve(values.rows() * values.cols());
+    for (int row = 0; row < values.rows(); ++row) {
+      for (int col = 0; col < values.cols(); ++col) {
+        if (row == col) {
+          m_storage.emplace_back(values.diagonal()(row));
+        } else {
+          m_storage.emplace_back(0.0);
+        }
+      }
+    }
+  }
+
+  /**
+   * Assigns an Eigen matrix to a VariableMatrix.
+   */
+  template <typename Derived>
+  VariableMatrix& operator=(const Eigen::MatrixBase<Derived>& values) {
+    Assert(Rows() == values.rows());
+    Assert(Cols() == values.cols());
+
+    for (int row = 0; row < values.rows(); ++row) {
+      for (int col = 0; col < values.cols(); ++col) {
+        (*this)(row, col) = values(row, col);
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Sets the VariableMatrix's internal values.
+   */
+  template <typename Derived>
+    requires std::same_as<typename Derived::Scalar, double>
+  VariableMatrix& SetValue(const Eigen::MatrixBase<Derived>& values) {
+    Assert(Rows() == values.rows());
+    Assert(Cols() == values.cols());
+
+    for (int row = 0; row < values.rows(); ++row) {
+      for (int col = 0; col < values.cols(); ++col) {
+        (*this)(row, col).SetValue(values(row, col));
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Constructs a scalar VariableMatrix from a Variable.
+   */
+  VariableMatrix(const Variable& variable)  // NOLINT
+      : m_rows{1}, m_cols{1} {
+    m_storage.emplace_back(variable);
+  }
+
+  /**
+   * Constructs a scalar VariableMatrix from a Variable.
+   */
+  VariableMatrix(Variable&& variable) : m_rows{1}, m_cols{1} {  // NOLINT
+    m_storage.emplace_back(std::move(variable));
+  }
+
+  /**
+   * Constructs a VariableMatrix from a VariableBlock.
+   */
+  VariableMatrix(const VariableBlock<VariableMatrix>& values)  // NOLINT
+      : m_rows{values.Rows()}, m_cols{values.Cols()} {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        m_storage.emplace_back(values(row, col));
+      }
+    }
+  }
+
+  /**
+   * Constructs a VariableMatrix from a VariableBlock.
+   */
+  VariableMatrix(const VariableBlock<const VariableMatrix>& values)  // NOLINT
+      : m_rows{values.Rows()}, m_cols{values.Cols()} {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        m_storage.emplace_back(values(row, col));
+      }
+    }
+  }
+
+  /**
+   * Constructs a column vector wrapper around a Variable array.
+   *
+   * @param values Variable array to wrap.
+   */
+  explicit VariableMatrix(std::span<const Variable> values)
+      : m_rows{static_cast<int>(values.size())}, m_cols{1} {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        m_storage.emplace_back(values[row * Cols() + col]);
+      }
+    }
+  }
+
+  /**
+   * Constructs a matrix wrapper around a Variable array.
+   *
+   * @param values Variable array to wrap.
+   * @param rows The number of matrix rows.
+   * @param cols The number of matrix columns.
+   */
+  VariableMatrix(std::span<const Variable> values, int rows, int cols)
+      : m_rows{rows}, m_cols{cols} {
+    Assert(static_cast<int>(values.size()) == Rows() * Cols());
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        m_storage.emplace_back(values[row * Cols() + col]);
+      }
+    }
+  }
+
+  /**
+   * Returns a block pointing to the given row and column.
+   *
+   * @param row The block row.
+   * @param col The block column.
+   */
+  Variable& operator()(int row, int col) {
+    Assert(row >= 0 && row < Rows());
+    Assert(col >= 0 && col < Cols());
+    return m_storage[row * Cols() + col];
+  }
+
+  /**
+   * Returns a block pointing to the given row and column.
+   *
+   * @param row The block row.
+   * @param col The block column.
+   */
+  const Variable& operator()(int row, int col) const {
+    Assert(row >= 0 && row < Rows());
+    Assert(col >= 0 && col < Cols());
+    return m_storage[row * Cols() + col];
+  }
+
+  /**
+   * Returns a block pointing to the given row.
+   *
+   * @param row The block row.
+   */
+  Variable& operator()(int row) {
+    Assert(row >= 0 && row < Rows() * Cols());
+    return m_storage[row];
+  }
+
+  /**
+   * Returns a block pointing to the given row.
+   *
+   * @param row The block row.
+   */
+  const Variable& operator()(int row) const {
+    Assert(row >= 0 && row < Rows() * Cols());
+    return m_storage[row];
+  }
+
+  /**
+   * Returns a block slice of the variable matrix.
+   *
+   * @param rowOffset The row offset of the block selection.
+   * @param colOffset The column offset of the block selection.
+   * @param blockRows The number of rows in the block selection.
+   * @param blockCols The number of columns in the block selection.
+   */
+  VariableBlock<VariableMatrix> Block(int rowOffset, int colOffset,
+                                      int blockRows, int blockCols) {
+    Assert(rowOffset >= 0 && rowOffset <= Rows());
+    Assert(colOffset >= 0 && colOffset <= Cols());
+    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
+    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
+    return VariableBlock{*this, rowOffset, colOffset, blockRows, blockCols};
+  }
+
+  /**
+   * Returns a block slice of the variable matrix.
+   *
+   * @param rowOffset The row offset of the block selection.
+   * @param colOffset The column offset of the block selection.
+   * @param blockRows The number of rows in the block selection.
+   * @param blockCols The number of columns in the block selection.
+   */
+  const VariableBlock<const VariableMatrix> Block(int rowOffset, int colOffset,
+                                                  int blockRows,
+                                                  int blockCols) const {
+    Assert(rowOffset >= 0 && rowOffset <= Rows());
+    Assert(colOffset >= 0 && colOffset <= Cols());
+    Assert(blockRows >= 0 && blockRows <= Rows() - rowOffset);
+    Assert(blockCols >= 0 && blockCols <= Cols() - colOffset);
+    return VariableBlock{*this, rowOffset, colOffset, blockRows, blockCols};
+  }
+
+  /**
+   * Returns a segment of the variable vector.
+   *
+   * @param offset The offset of the segment.
+   * @param length The length of the segment.
+   */
+  VariableBlock<VariableMatrix> Segment(int offset, int length) {
+    Assert(offset >= 0 && offset < Rows() * Cols());
+    Assert(length >= 0 && length <= Rows() * Cols() - offset);
+    return Block(offset, 0, length, 1);
+  }
+
+  /**
+   * Returns a segment of the variable vector.
+   *
+   * @param offset The offset of the segment.
+   * @param length The length of the segment.
+   */
+  const VariableBlock<const VariableMatrix> Segment(int offset,
+                                                    int length) const {
+    Assert(offset >= 0 && offset < Rows() * Cols());
+    Assert(length >= 0 && length <= Rows() * Cols() - offset);
+    return Block(offset, 0, length, 1);
+  }
+
+  /**
+   * Returns a row slice of the variable matrix.
+   *
+   * @param row The row to slice.
+   */
+  VariableBlock<VariableMatrix> Row(int row) {
+    Assert(row >= 0 && row < Rows());
+    return Block(row, 0, 1, Cols());
+  }
+
+  /**
+   * Returns a row slice of the variable matrix.
+   *
+   * @param row The row to slice.
+   */
+  const VariableBlock<const VariableMatrix> Row(int row) const {
+    Assert(row >= 0 && row < Rows());
+    return Block(row, 0, 1, Cols());
+  }
+
+  /**
+   * Returns a column slice of the variable matrix.
+   *
+   * @param col The column to slice.
+   */
+  VariableBlock<VariableMatrix> Col(int col) {
+    Assert(col >= 0 && col < Cols());
+    return Block(0, col, Rows(), 1);
+  }
+
+  /**
+   * Returns a column slice of the variable matrix.
+   *
+   * @param col The column to slice.
+   */
+  const VariableBlock<const VariableMatrix> Col(int col) const {
+    Assert(col >= 0 && col < Cols());
+    return Block(0, col, Rows(), 1);
+  }
+
+  /**
+   * Matrix multiplication operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix
+  operator*(const VariableMatrix& lhs, const VariableMatrix& rhs) {
+    Assert(lhs.Cols() == rhs.Rows());
+
+    VariableMatrix result{lhs.Rows(), rhs.Cols()};
+
+    for (int i = 0; i < lhs.Rows(); ++i) {
+      for (int j = 0; j < rhs.Cols(); ++j) {
+        Variable sum;
+        for (int k = 0; k < lhs.Cols(); ++k) {
+          sum += lhs(i, k) * rhs(k, j);
+        }
+        result(i, j) = sum;
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Matrix-scalar multiplication operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix operator*(const VariableMatrix& lhs,
+                                                     const Variable& rhs) {
+    VariableMatrix result{lhs.Rows(), lhs.Cols()};
+
+    for (int row = 0; row < result.Rows(); ++row) {
+      for (int col = 0; col < result.Cols(); ++col) {
+        result(row, col) = lhs(row, col) * rhs;
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Matrix-scalar multiplication operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix operator*(const VariableMatrix& lhs,
+                                                     double rhs) {
+    return lhs * Variable{rhs};
+  }
+
+  /**
+   * Scalar-matrix multiplication operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix
+  operator*(const Variable& lhs, const VariableMatrix& rhs) {
+    VariableMatrix result{rhs.Rows(), rhs.Cols()};
+
+    for (int row = 0; row < result.Rows(); ++row) {
+      for (int col = 0; col < result.Cols(); ++col) {
+        result(row, col) = rhs(row, col) * lhs;
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Scalar-matrix multiplication operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix
+  operator*(double lhs, const VariableMatrix& rhs) {
+    return Variable{lhs} * rhs;
+  }
+
+  /**
+   * Compound matrix multiplication-assignment operator.
+   *
+   * @param rhs Variable to multiply.
+   */
+  VariableMatrix& operator*=(const VariableMatrix& rhs) {
+    Assert(Cols() == rhs.Rows() && Cols() == rhs.Cols());
+
+    for (int i = 0; i < Rows(); ++i) {
+      for (int j = 0; j < rhs.Cols(); ++j) {
+        Variable sum;
+        for (int k = 0; k < Cols(); ++k) {
+          sum += (*this)(i, k) * rhs(k, j);
+        }
+        (*this)(i, j) = sum;
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Binary division operator (only enabled when rhs is a scalar).
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix operator/(const VariableMatrix& lhs,
+                                                     const Variable& rhs) {
+    VariableMatrix result{lhs.Rows(), lhs.Cols()};
+
+    for (int row = 0; row < result.Rows(); ++row) {
+      for (int col = 0; col < result.Cols(); ++col) {
+        result(row, col) = lhs(row, col) / rhs;
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Compound matrix division-assignment operator (only enabled when rhs
+   * is a scalar).
+   *
+   * @param rhs Variable to divide.
+   */
+  VariableMatrix& operator/=(const Variable& rhs) {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) /= rhs;
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Binary addition operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix
+  operator+(const VariableMatrix& lhs, const VariableMatrix& rhs) {
+    VariableMatrix result{lhs.Rows(), lhs.Cols()};
+
+    for (int row = 0; row < result.Rows(); ++row) {
+      for (int col = 0; col < result.Cols(); ++col) {
+        result(row, col) = lhs(row, col) + rhs(row, col);
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Compound addition-assignment operator.
+   *
+   * @param rhs Variable to add.
+   */
+  VariableMatrix& operator+=(const VariableMatrix& rhs) {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) += rhs(row, col);
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Binary subtraction operator.
+   *
+   * @param lhs Operator left-hand side.
+   * @param rhs Operator right-hand side.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix
+  operator-(const VariableMatrix& lhs, const VariableMatrix& rhs) {
+    VariableMatrix result{lhs.Rows(), lhs.Cols()};
+
+    for (int row = 0; row < result.Rows(); ++row) {
+      for (int col = 0; col < result.Cols(); ++col) {
+        result(row, col) = lhs(row, col) - rhs(row, col);
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Compound subtraction-assignment operator.
+   *
+   * @param rhs Variable to subtract.
+   */
+  VariableMatrix& operator-=(const VariableMatrix& rhs) {
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        (*this)(row, col) -= rhs(row, col);
+      }
+    }
+
+    return *this;
+  }
+
+  /**
+   * Unary minus operator.
+   *
+   * @param lhs Operand for unary minus.
+   */
+  friend SLEIPNIR_DLLEXPORT VariableMatrix
+  operator-(const VariableMatrix& lhs) {
+    VariableMatrix result{lhs.Rows(), lhs.Cols()};
+
+    for (int row = 0; row < result.Rows(); ++row) {
+      for (int col = 0; col < result.Cols(); ++col) {
+        result(row, col) = -lhs(row, col);
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Implicit conversion operator from 1x1 VariableMatrix to Variable.
+   */
+  operator Variable() const {  // NOLINT
+    Assert(Rows() == 1 && Cols() == 1);
+    return (*this)(0, 0);
+  }
+
+  /**
+   * Returns the transpose of the variable matrix.
+   */
+  VariableMatrix T() const {
+    VariableMatrix result{Cols(), Rows()};
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        result(col, row) = (*this)(row, col);
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Returns number of rows in the matrix.
+   */
+  int Rows() const { return m_rows; }
+
+  /**
+   * Returns number of columns in the matrix.
+   */
+  int Cols() const { return m_cols; }
+
+  /**
+   * Returns an element of the variable matrix.
+   *
+   * @param row The row of the element to return.
+   * @param col The column of the element to return.
+   */
+  double Value(int row, int col) const {
+    Assert(row >= 0 && row < Rows());
+    Assert(col >= 0 && col < Cols());
+    return m_storage[row * Cols() + col].Value();
+  }
+
+  /**
+   * Returns a row of the variable column vector.
+   *
+   * @param index The index of the element to return.
+   */
+  double Value(int index) const {
+    Assert(index >= 0 && index < Rows() * Cols());
+    return m_storage[index].Value();
+  }
+
+  /**
+   * Returns the contents of the variable matrix.
+   */
+  Eigen::MatrixXd Value() const {
+    Eigen::MatrixXd result{Rows(), Cols()};
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        result(row, col) = Value(row, col);
+      }
+    }
+
+    return result;
+  }
+
+  /**
+   * Transforms the matrix coefficient-wise with an unary operator.
+   *
+   * @param unaryOp The unary operator to use for the transform operation.
+   */
+  template <std::invocable<const Variable&> UnaryOp>
+  VariableMatrix CwiseTransform(UnaryOp&& unaryOp) const {
+    VariableMatrix result{Rows(), Cols()};
+
+    for (int row = 0; row < Rows(); ++row) {
+      for (int col = 0; col < Cols(); ++col) {
+        result(row, col) = unaryOp((*this)(row, col));
+      }
+    }
+
+    return result;
+  }
+
+  class iterator {
+   public:
+    using iterator_category = std::forward_iterator_tag;
+    using value_type = Variable;
+    using difference_type = std::ptrdiff_t;
+    using pointer = Variable*;
+    using reference = Variable&;
+
+    iterator(VariableMatrix* mat, int row, int col)
+        : m_mat{mat}, m_row{row}, m_col{col} {}
+
+    iterator& operator++() {
+      ++m_col;
+      if (m_col == m_mat->Cols()) {
+        m_col = 0;
+        ++m_row;
+      }
+      return *this;
+    }
+    iterator operator++(int) {
+      iterator retval = *this;
+      ++(*this);
+      return retval;
+    }
+    bool operator==(const iterator&) const = default;
+    reference operator*() { return (*m_mat)(m_row, m_col); }
+
+   private:
+    VariableMatrix* m_mat;
+    int m_row;
+    int m_col;
+  };
+
+  class const_iterator {
+   public:
+    using iterator_category = std::forward_iterator_tag;
+    using value_type = Variable;
+    using difference_type = std::ptrdiff_t;
+    using pointer = Variable*;
+    using const_reference = const Variable&;
+
+    const_iterator(const VariableMatrix* mat, int row, int col)
+        : m_mat{mat}, m_row{row}, m_col{col} {}
+
+    const_iterator& operator++() {
+      ++m_col;
+      if (m_col == m_mat->Cols()) {
+        m_col = 0;
+        ++m_row;
+      }
+      return *this;
+    }
+    const_iterator operator++(int) {
+      const_iterator retval = *this;
+      ++(*this);
+      return retval;
+    }
+    bool operator==(const const_iterator&) const = default;
+    const_reference operator*() const { return (*m_mat)(m_row, m_col); }
+
+   private:
+    const VariableMatrix* m_mat;
+    int m_row;
+    int m_col;
+  };
+
+  /**
+   * Returns begin iterator.
+   */
+  iterator begin() { return iterator(this, 0, 0); }
+
+  /**
+   * Returns end iterator.
+   */
+  iterator end() { return iterator(this, Rows(), 0); }
+
+  /**
+   * Returns begin iterator.
+   */
+  const_iterator begin() const { return const_iterator(this, 0, 0); }
+
+  /**
+   * Returns end iterator.
+   */
+  const_iterator end() const { return const_iterator(this, Rows(), 0); }
+
+  /**
+   * Returns begin iterator.
+   */
+  const_iterator cbegin() const { return const_iterator(this, 0, 0); }
+
+  /**
+   * Returns end iterator.
+   */
+  const_iterator cend() const { return const_iterator(this, Rows(), 0); }
+
+  /**
+   * Returns number of elements in matrix.
+   */
+  size_t size() const { return m_rows * m_cols; }
+
+  /**
+   * Returns a variable matrix filled with zeroes.
+   *
+   * @param rows The number of matrix rows.
+   * @param cols The number of matrix columns.
+   */
+  static VariableMatrix Zero(int rows, int cols) {
+    VariableMatrix result{rows, cols};
+
+    for (auto& elem : result) {
+      elem = 0.0;
+    }
+
+    return result;
+  }
+
+  /**
+   * Returns a variable matrix filled with ones.
+   *
+   * @param rows The number of matrix rows.
+   * @param cols The number of matrix columns.
+   */
+  static VariableMatrix Ones(int rows, int cols) {
+    VariableMatrix result{rows, cols};
+
+    for (auto& elem : result) {
+      elem = 1.0;
+    }
+
+    return result;
+  }
+
+ private:
+  std::vector<Variable> m_storage;
+  int m_rows = 0;
+  int m_cols = 0;
+};
+
+/**
+ * Applies a coefficient-wise reduce operation to two matrices.
+ *
+ * @param lhs The left-hand side of the binary operator.
+ * @param rhs The right-hand side of the binary operator.
+ * @param binaryOp The binary operator to use for the reduce operation.
+ */
+template <std::invocable<const Variable&, const Variable&> BinaryOp>
+VariableMatrix CwiseReduce(const VariableMatrix& lhs, const VariableMatrix& rhs,
+                           BinaryOp&& binaryOp) {
+  Assert(lhs.Rows() == rhs.Rows());
+  Assert(lhs.Rows() == rhs.Rows());
+
+  VariableMatrix result{lhs.Rows(), lhs.Cols()};
+
+  for (int row = 0; row < lhs.Rows(); ++row) {
+    for (int col = 0; col < lhs.Cols(); ++col) {
+      result(row, col) = binaryOp(lhs(row, col), rhs(row, col));
+    }
+  }
+
+  return result;
+}
+
+/**
+ * Assemble a VariableMatrix from a nested list of blocks.
+ *
+ * Each row's blocks must have the same height, and the assembled block rows
+ * must have the same width. For example, for the block matrix [[A, B], [C]] to
+ * be constructible, the number of rows in A and B must match, and the number of
+ * columns in [A, B] and [C] must match.
+ *
+ * @param list The nested list of blocks.
+ */
+SLEIPNIR_DLLEXPORT inline VariableMatrix Block(
+    std::initializer_list<std::initializer_list<VariableMatrix>> list) {
+  // Get row and column counts for destination matrix
+  int rows = 0;
+  int cols = -1;
+  for (const auto& row : list) {
+    if (row.size() > 0) {
+      rows += row.begin()->Rows();
+    }
+
+    // Get number of columns in this row
+    int latestCols = 0;
+    for (const auto& elem : row) {
+      // Assert the first and latest row have the same height
+      Assert(row.begin()->Rows() == elem.Rows());
+
+      latestCols += elem.Cols();
+    }
+
+    // If this is the first row, record the column count. Otherwise, assert the
+    // first and latest column counts are the same.
+    if (cols == -1) {
+      cols = latestCols;
+    } else {
+      Assert(cols == latestCols);
+    }
+  }
+
+  VariableMatrix result{rows, cols};
+
+  int rowOffset = 0;
+  for (const auto& row : list) {
+    int colOffset = 0;
+    for (const auto& elem : row) {
+      result.Block(rowOffset, colOffset, elem.Rows(), elem.Cols()) = elem;
+      colOffset += elem.Cols();
+    }
+    rowOffset += row.begin()->Rows();
+  }
+
+  return result;
+}
+
+/**
+ * Assemble a VariableMatrix from a nested list of blocks.
+ *
+ * Each row's blocks must have the same height, and the assembled block rows
+ * must have the same width. For example, for the block matrix [[A, B], [C]] to
+ * be constructible, the number of rows in A and B must match, and the number of
+ * columns in [A, B] and [C] must match.
+ *
+ * This overload is for Python bindings only.
+ *
+ * @param list The nested list of blocks.
+ */
+SLEIPNIR_DLLEXPORT inline VariableMatrix Block(
+    std::vector<std::vector<VariableMatrix>> list) {
+  // Get row and column counts for destination matrix
+  int rows = 0;
+  int cols = -1;
+  for (const auto& row : list) {
+    if (row.size() > 0) {
+      rows += row.begin()->Rows();
+    }
+
+    // Get number of columns in this row
+    int latestCols = 0;
+    for (const auto& elem : row) {
+      // Assert the first and latest row have the same height
+      Assert(row.begin()->Rows() == elem.Rows());
+
+      latestCols += elem.Cols();
+    }
+
+    // If this is the first row, record the column count. Otherwise, assert the
+    // first and latest column counts are the same.
+    if (cols == -1) {
+      cols = latestCols;
+    } else {
+      Assert(cols == latestCols);
+    }
+  }
+
+  VariableMatrix result{rows, cols};
+
+  int rowOffset = 0;
+  for (const auto& row : list) {
+    int colOffset = 0;
+    for (const auto& elem : row) {
+      result.Block(rowOffset, colOffset, elem.Rows(), elem.Cols()) = elem;
+      colOffset += elem.Cols();
+    }
+    rowOffset += row.begin()->Rows();
+  }
+
+  return result;
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/control/OCPSolver.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/control/OCPSolver.hpp`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,406 +1,406 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <chrono>
-#include <functional>
-#include <utility>
-
-#include "sleipnir/autodiff/VariableMatrix.hpp"
-#include "sleipnir/optimization/OptimizationProblem.hpp"
-#include "sleipnir/util/Assert.hpp"
-#include "sleipnir/util/Concepts.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * Function representing an explicit or implicit ODE, or a discrete state
- * transition function.
- *
- * - Explicit: dx/dt = f(t, x, u, *)
- * - Implicit: f(t, [x dx/dt]', u, *) = 0
- * - State transition: xₖ₊₁ = f(t, xₖ, uₖ, dt)
- */
-using DynamicsFunction =
-    std::function<VariableMatrix(const Variable&, const VariableMatrix&,
-                                 const VariableMatrix&, const Variable&)>;
-
-/**
- * Performs 4th order Runge-Kutta integration of dx/dt = f(t, x, u) for dt.
- *
- * @param f  The function to integrate. It must take two arguments x and u.
- * @param x  The initial value of x.
- * @param u  The value u held constant over the integration period.
- * @param t0 The initial time.
- * @param dt The time over which to integrate.
- */
-template <typename F, typename State, typename Input, typename Time>
-State RK4(F&& f, State x, Input u, Time t0, Time dt) {
-  auto halfdt = dt * 0.5;
-  State k1 = f(t0, x, u, dt);
-  State k2 = f(t0 + halfdt, x + k1 * halfdt, u, dt);
-  State k3 = f(t0 + halfdt, x + k2 * halfdt, u, dt);
-  State k4 = f(t0 + dt, x + k3 * dt, u, dt);
-
-  return x + (k1 + k2 * 2.0 + k3 * 2.0 + k4) * (dt / 6.0);
-}
-
-/**
- * Enum describing an OCP transcription method.
- */
-enum class TranscriptionMethod {
-  /// Each state is a decision variable constrained to the integrated dynamics
-  /// of the previous state.
-  kDirectTranscription,
-  /// The trajectory is modeled as a series of cubic polynomials where the
-  /// centerpoint slope is constrained.
-  kDirectCollocation,
-  /// States depend explicitly as a function of all previous states and all
-  /// previous inputs.
-  kSingleShooting
-};
-
-/**
- * Enum describing a type of system dynamics constraints.
- */
-enum class DynamicsType {
-  /// The dynamics are a function in the form dx/dt = f(t, x, u).
-  kExplicitODE,
-  /// The dynamics are a function in the form xₖ₊₁ = f(t, xₖ, uₖ).
-  kDiscrete
-};
-
-/**
- * Enum describing the type of system timestep.
- */
-enum class TimestepMethod {
-  /// The timestep is a fixed constant.
-  kFixed,
-  /// The timesteps are allowed to vary as independent decision variables.
-  kVariable,
-  /// The timesteps are equal length but allowed to vary as a single decision
-  /// variable.
-  kVariableSingle
-};
-
-/**
- * This class allows the user to pose and solve a constrained optimal control
- * problem (OCP) in a variety of ways.
- *
- * The system is transcripted by one of three methods (direct transcription,
- * direct collocation, or single-shooting) and additional constraints can be
- * added.
- *
- * In direct transcription, each state is a decision variable constrained to the
- * integrated dynamics of the previous state. In direct collocation, the
- * trajectory is modeled as a series of cubic polynomials where the centerpoint
- * slope is constrained. In single-shooting, states depend explicitly as a
- * function of all previous states and all previous inputs.
- *
- * Explicit ODEs are integrated using RK4.
- *
- * For explicit ODEs, the function must be in the form dx/dt = f(t, x, u).
- * For discrete state transition functions, the function must be in the form
- * xₖ₊₁ = f(t, xₖ, uₖ).
- *
- * Direct collocation requires an explicit ODE. Direct transcription and
- * single-shooting can use either an ODE or state transition function.
- *
- * https://underactuated.mit.edu/trajopt.html goes into more detail on each
- * transcription method.
- */
-class SLEIPNIR_DLLEXPORT OCPSolver : public OptimizationProblem {
- public:
-  /**
-   * Build an optimization problem using a system evolution function (explicit
-   * ODE or discrete state transition function).
-   *
-   * @param numStates The number of system states.
-   * @param numInputs The number of system inputs.
-   * @param dt The timestep for fixed-step integration.
-   * @param numSteps The number of control points.
-   * @param dynamics The system evolution function, either an explicit ODE or a
-   * discrete state transition function.
-   * @param dynamicsType The type of system evolution function.
-   * @param timestepMethod The timestep method.
-   * @param method The transcription method.
-   */
-  OCPSolver(
-      int numStates, int numInputs, std::chrono::duration<double> dt,
-      int numSteps, DynamicsFunction dynamics,
-      DynamicsType dynamicsType = DynamicsType::kExplicitODE,
-      TimestepMethod timestepMethod = TimestepMethod::kFixed,
-      TranscriptionMethod method = TranscriptionMethod::kDirectTranscription)
-      : m_numStates{numStates},
-        m_numInputs{numInputs},
-        m_dt{dt},
-        m_numSteps{numSteps},
-        m_transcriptionMethod{method},
-        m_dynamicsType{dynamicsType},
-        m_dynamicsFunction{std::move(dynamics)},
-        m_timestepMethod{timestepMethod} {
-    // u is numSteps + 1 so that the final constraintFunction evaluation works
-    m_U = DecisionVariable(m_numInputs, m_numSteps + 1);
-
-    if (m_timestepMethod == TimestepMethod::kFixed) {
-      m_DT = VariableMatrix{1, m_numSteps + 1};
-      for (int i = 0; i < numSteps + 1; ++i) {
-        m_DT(0, i) = m_dt.count();
-      }
-    } else if (m_timestepMethod == TimestepMethod::kVariableSingle) {
-      Variable DT = DecisionVariable();
-      DT.SetValue(m_dt.count());
-
-      // Set the member variable matrix to track the decision variable
-      m_DT = VariableMatrix{1, m_numSteps + 1};
-      for (int i = 0; i < numSteps + 1; ++i) {
-        m_DT(0, i) = DT;
-      }
-    } else if (m_timestepMethod == TimestepMethod::kVariable) {
-      m_DT = DecisionVariable(1, m_numSteps + 1);
-      for (int i = 0; i < numSteps + 1; ++i) {
-        m_DT(0, i).SetValue(m_dt.count());
-      }
-    }
-
-    if (m_transcriptionMethod == TranscriptionMethod::kDirectTranscription) {
-      m_X = DecisionVariable(m_numStates, m_numSteps + 1);
-      ConstrainDirectTranscription();
-    } else if (m_transcriptionMethod ==
-               TranscriptionMethod::kDirectCollocation) {
-      m_X = DecisionVariable(m_numStates, m_numSteps + 1);
-      ConstrainDirectCollocation();
-    } else if (m_transcriptionMethod == TranscriptionMethod::kSingleShooting) {
-      // In single-shooting the states aren't decision variables, but instead
-      // depend on the input and previous states
-      m_X = VariableMatrix{m_numStates, m_numSteps + 1};
-      ConstrainSingleShooting();
-    }
-  }
-
-  /**
-   * Utility function to constrain the initial state.
-   *
-   * @param initialState the initial state to constrain to.
-   */
-  template <typename T>
-    requires ScalarLike<T> || MatrixLike<T>
-  void ConstrainInitialState(const T& initialState) {
-    SubjectTo(InitialState() == initialState);
-  }
-
-  /**
-   * Utility function to constrain the final state.
-   *
-   * @param finalState the final state to constrain to.
-   */
-  template <typename T>
-    requires ScalarLike<T> || MatrixLike<T>
-  void ConstrainFinalState(const T& finalState) {
-    SubjectTo(FinalState() == finalState);
-  }
-
-  /**
-   * Set the constraint evaluation function. This function is called
-   * `numSteps+1` times, with the corresponding state and input
-   * VariableMatrices.
-   *
-   * @param callback The callback f(t, x, u, dt) where t is time, x is the state
-   *   vector, u is the input vector, and dt is the timestep duration.
-   */
-  void ForEachStep(
-      const std::function<void(const Variable&, const VariableMatrix&,
-                               const VariableMatrix&, const Variable&)>&
-          callback) {
-    Variable time = 0.0;
-
-    for (int i = 0; i < m_numSteps + 1; ++i) {
-      auto x = X().Col(i);
-      auto u = U().Col(i);
-      auto dt = DT()(0, i);
-      callback(time, x, u, dt);
-
-      time += dt;
-    }
-  }
-
-  /**
-   * Convenience function to set a lower bound on the input.
-   *
-   * @param lowerBound The lower bound that inputs must always be above. Must be
-   * shaped (numInputs)x1.
-   */
-  template <typename T>
-    requires ScalarLike<T> || MatrixLike<T>
-  void SetLowerInputBound(const T& lowerBound) {
-    for (int i = 0; i < m_numSteps + 1; ++i) {
-      SubjectTo(U().Col(i) >= lowerBound);
-    }
-  }
-
-  /**
-   * Convenience function to set an upper bound on the input.
-   *
-   * @param upperBound The upper bound that inputs must always be below. Must be
-   * shaped (numInputs)x1.
-   */
-  template <typename T>
-    requires ScalarLike<T> || MatrixLike<T>
-  void SetUpperInputBound(const T& upperBound) {
-    for (int i = 0; i < m_numSteps + 1; ++i) {
-      SubjectTo(U().Col(i) <= upperBound);
-    }
-  }
-
-  /**
-   * Convenience function to set an upper bound on the timestep.
-   *
-   * @param maxTimestep The maximum timestep.
-   */
-  void SetMaxTimestep(std::chrono::duration<double> maxTimestep) {
-    SubjectTo(DT() <= maxTimestep.count());
-  }
-
-  /**
-   * Convenience function to set a lower bound on the timestep.
-   *
-   * @param minTimestep The minimum timestep.
-   */
-  void SetMinTimestep(std::chrono::duration<double> minTimestep) {
-    SubjectTo(DT() >= minTimestep.count());
-  }
-
-  /**
-   * Get the state variables. After the problem is solved, this will contain the
-   * optimized trajectory.
-   *
-   * Shaped (numStates)x(numSteps+1).
-   *
-   * @returns The state variable matrix.
-   */
-  VariableMatrix& X() { return m_X; };
-
-  /**
-   * Get the input variables. After the problem is solved, this will contain the
-   * inputs corresponding to the optimized trajectory.
-   *
-   * Shaped (numInputs)x(numSteps+1), although the last input step is unused in
-   * the trajectory.
-   *
-   * @returns The input variable matrix.
-   */
-  VariableMatrix& U() { return m_U; };
-
-  /**
-   * Get the timestep variables. After the problem is solved, this will contain
-   * the timesteps corresponding to the optimized trajectory.
-   *
-   * Shaped 1x(numSteps+1), although the last timestep is unused in
-   * the trajectory.
-   *
-   * @returns The timestep variable matrix.
-   */
-  VariableMatrix& DT() { return m_DT; };
-
-  /**
-   * Convenience function to get the initial state in the trajectory.
-   *
-   * @returns The initial state of the trajectory.
-   */
-  VariableMatrix InitialState() { return m_X.Col(0); }
-
-  /**
-   * Convenience function to get the final state in the trajectory.
-   *
-   * @returns The final state of the trajectory.
-   */
-  VariableMatrix FinalState() { return m_X.Col(m_numSteps); }
-
- private:
-  void ConstrainDirectCollocation() {
-    Assert(m_dynamicsType == DynamicsType::kExplicitODE);
-
-    Variable time = 0.0;
-
-    for (int i = 0; i < m_numSteps; ++i) {
-      auto x_begin = X().Col(i);
-      auto x_end = X().Col(i + 1);
-      auto u_begin = U().Col(i);
-      Variable dt = DT()(0, i);
-      auto t_begin = time;
-      auto t_end = time + dt;
-      auto t_c = t_begin + dt / 2.0;
-
-      time += dt;
-
-      // Use u_begin on the end point as well because we are approaching a
-      // discontinuity from the left
-      auto f_begin = m_dynamicsFunction(t_begin, x_begin, u_begin, dt);
-      auto f_end = m_dynamicsFunction(t_end, x_end, u_begin, dt);
-      auto x_c = (x_begin + x_end) / 2.0 + (f_begin - f_end) * (dt / 8.0);
-      auto xprime_c =
-          (x_begin - x_end) * (-3.0 / (2.0 * dt)) - (f_begin + f_end) / 4.0;
-      auto f_c = m_dynamicsFunction(t_c, x_c, u_begin, dt);
-      SubjectTo(f_c == xprime_c);
-    }
-  }
-
-  void ConstrainDirectTranscription() {
-    Variable time = 0.0;
-
-    for (int i = 0; i < m_numSteps; ++i) {
-      auto x_begin = X().Col(i);
-      auto x_end = X().Col(i + 1);
-      auto u = U().Col(i);
-      Variable dt = DT()(0, i);
-
-      if (m_dynamicsType == DynamicsType::kExplicitODE) {
-        SubjectTo(x_end ==
-                  RK4<const DynamicsFunction&, VariableMatrix, VariableMatrix,
-                      Variable>(m_dynamicsFunction, x_begin, u, time, dt));
-      } else if (m_dynamicsType == DynamicsType::kDiscrete) {
-        SubjectTo(x_end == m_dynamicsFunction(time, x_begin, u, dt));
-      }
-
-      time += dt;
-    }
-  }
-
-  void ConstrainSingleShooting() {
-    Variable time = 0.0;
-
-    for (int i = 0; i < m_numSteps; ++i) {
-      auto x_begin = X().Col(i);
-      auto x_end = X().Col(i + 1);
-      auto u = U().Col(i);
-      Variable dt = DT()(0, i);
-
-      if (m_dynamicsType == DynamicsType::kExplicitODE) {
-        x_end = RK4<const DynamicsFunction&, VariableMatrix, VariableMatrix,
-                    Variable>(m_dynamicsFunction, x_begin, u, time, dt);
-      } else if (m_dynamicsType == DynamicsType::kDiscrete) {
-        x_end = m_dynamicsFunction(time, x_begin, u, dt);
-      }
-
-      time += dt;
-    }
-  }
-
-  int m_numStates;
-  int m_numInputs;
-  std::chrono::duration<double> m_dt;
-  int m_numSteps;
-  TranscriptionMethod m_transcriptionMethod;
-
-  DynamicsType m_dynamicsType;
-  DynamicsFunction m_dynamicsFunction;
-
-  TimestepMethod m_timestepMethod;
-
-  VariableMatrix m_X;
-  VariableMatrix m_U;
-  VariableMatrix m_DT;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <chrono>
+#include <functional>
+#include <utility>
+
+#include "sleipnir/autodiff/VariableMatrix.hpp"
+#include "sleipnir/optimization/OptimizationProblem.hpp"
+#include "sleipnir/util/Assert.hpp"
+#include "sleipnir/util/Concepts.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * Function representing an explicit or implicit ODE, or a discrete state
+ * transition function.
+ *
+ * - Explicit: dx/dt = f(t, x, u, *)
+ * - Implicit: f(t, [x dx/dt]', u, *) = 0
+ * - State transition: xₖ₊₁ = f(t, xₖ, uₖ, dt)
+ */
+using DynamicsFunction =
+    std::function<VariableMatrix(const Variable&, const VariableMatrix&,
+                                 const VariableMatrix&, const Variable&)>;
+
+/**
+ * Performs 4th order Runge-Kutta integration of dx/dt = f(t, x, u) for dt.
+ *
+ * @param f  The function to integrate. It must take two arguments x and u.
+ * @param x  The initial value of x.
+ * @param u  The value u held constant over the integration period.
+ * @param t0 The initial time.
+ * @param dt The time over which to integrate.
+ */
+template <typename F, typename State, typename Input, typename Time>
+State RK4(F&& f, State x, Input u, Time t0, Time dt) {
+  auto halfdt = dt * 0.5;
+  State k1 = f(t0, x, u, dt);
+  State k2 = f(t0 + halfdt, x + k1 * halfdt, u, dt);
+  State k3 = f(t0 + halfdt, x + k2 * halfdt, u, dt);
+  State k4 = f(t0 + dt, x + k3 * dt, u, dt);
+
+  return x + (k1 + k2 * 2.0 + k3 * 2.0 + k4) * (dt / 6.0);
+}
+
+/**
+ * Enum describing an OCP transcription method.
+ */
+enum class TranscriptionMethod {
+  /// Each state is a decision variable constrained to the integrated dynamics
+  /// of the previous state.
+  kDirectTranscription,
+  /// The trajectory is modeled as a series of cubic polynomials where the
+  /// centerpoint slope is constrained.
+  kDirectCollocation,
+  /// States depend explicitly as a function of all previous states and all
+  /// previous inputs.
+  kSingleShooting
+};
+
+/**
+ * Enum describing a type of system dynamics constraints.
+ */
+enum class DynamicsType {
+  /// The dynamics are a function in the form dx/dt = f(t, x, u).
+  kExplicitODE,
+  /// The dynamics are a function in the form xₖ₊₁ = f(t, xₖ, uₖ).
+  kDiscrete
+};
+
+/**
+ * Enum describing the type of system timestep.
+ */
+enum class TimestepMethod {
+  /// The timestep is a fixed constant.
+  kFixed,
+  /// The timesteps are allowed to vary as independent decision variables.
+  kVariable,
+  /// The timesteps are equal length but allowed to vary as a single decision
+  /// variable.
+  kVariableSingle
+};
+
+/**
+ * This class allows the user to pose and solve a constrained optimal control
+ * problem (OCP) in a variety of ways.
+ *
+ * The system is transcripted by one of three methods (direct transcription,
+ * direct collocation, or single-shooting) and additional constraints can be
+ * added.
+ *
+ * In direct transcription, each state is a decision variable constrained to the
+ * integrated dynamics of the previous state. In direct collocation, the
+ * trajectory is modeled as a series of cubic polynomials where the centerpoint
+ * slope is constrained. In single-shooting, states depend explicitly as a
+ * function of all previous states and all previous inputs.
+ *
+ * Explicit ODEs are integrated using RK4.
+ *
+ * For explicit ODEs, the function must be in the form dx/dt = f(t, x, u).
+ * For discrete state transition functions, the function must be in the form
+ * xₖ₊₁ = f(t, xₖ, uₖ).
+ *
+ * Direct collocation requires an explicit ODE. Direct transcription and
+ * single-shooting can use either an ODE or state transition function.
+ *
+ * https://underactuated.mit.edu/trajopt.html goes into more detail on each
+ * transcription method.
+ */
+class SLEIPNIR_DLLEXPORT OCPSolver : public OptimizationProblem {
+ public:
+  /**
+   * Build an optimization problem using a system evolution function (explicit
+   * ODE or discrete state transition function).
+   *
+   * @param numStates The number of system states.
+   * @param numInputs The number of system inputs.
+   * @param dt The timestep for fixed-step integration.
+   * @param numSteps The number of control points.
+   * @param dynamics The system evolution function, either an explicit ODE or a
+   * discrete state transition function.
+   * @param dynamicsType The type of system evolution function.
+   * @param timestepMethod The timestep method.
+   * @param method The transcription method.
+   */
+  OCPSolver(
+      int numStates, int numInputs, std::chrono::duration<double> dt,
+      int numSteps, DynamicsFunction dynamics,
+      DynamicsType dynamicsType = DynamicsType::kExplicitODE,
+      TimestepMethod timestepMethod = TimestepMethod::kFixed,
+      TranscriptionMethod method = TranscriptionMethod::kDirectTranscription)
+      : m_numStates{numStates},
+        m_numInputs{numInputs},
+        m_dt{dt},
+        m_numSteps{numSteps},
+        m_transcriptionMethod{method},
+        m_dynamicsType{dynamicsType},
+        m_dynamicsFunction{std::move(dynamics)},
+        m_timestepMethod{timestepMethod} {
+    // u is numSteps + 1 so that the final constraintFunction evaluation works
+    m_U = DecisionVariable(m_numInputs, m_numSteps + 1);
+
+    if (m_timestepMethod == TimestepMethod::kFixed) {
+      m_DT = VariableMatrix{1, m_numSteps + 1};
+      for (int i = 0; i < numSteps + 1; ++i) {
+        m_DT(0, i) = m_dt.count();
+      }
+    } else if (m_timestepMethod == TimestepMethod::kVariableSingle) {
+      Variable DT = DecisionVariable();
+      DT.SetValue(m_dt.count());
+
+      // Set the member variable matrix to track the decision variable
+      m_DT = VariableMatrix{1, m_numSteps + 1};
+      for (int i = 0; i < numSteps + 1; ++i) {
+        m_DT(0, i) = DT;
+      }
+    } else if (m_timestepMethod == TimestepMethod::kVariable) {
+      m_DT = DecisionVariable(1, m_numSteps + 1);
+      for (int i = 0; i < numSteps + 1; ++i) {
+        m_DT(0, i).SetValue(m_dt.count());
+      }
+    }
+
+    if (m_transcriptionMethod == TranscriptionMethod::kDirectTranscription) {
+      m_X = DecisionVariable(m_numStates, m_numSteps + 1);
+      ConstrainDirectTranscription();
+    } else if (m_transcriptionMethod ==
+               TranscriptionMethod::kDirectCollocation) {
+      m_X = DecisionVariable(m_numStates, m_numSteps + 1);
+      ConstrainDirectCollocation();
+    } else if (m_transcriptionMethod == TranscriptionMethod::kSingleShooting) {
+      // In single-shooting the states aren't decision variables, but instead
+      // depend on the input and previous states
+      m_X = VariableMatrix{m_numStates, m_numSteps + 1};
+      ConstrainSingleShooting();
+    }
+  }
+
+  /**
+   * Utility function to constrain the initial state.
+   *
+   * @param initialState the initial state to constrain to.
+   */
+  template <typename T>
+    requires ScalarLike<T> || MatrixLike<T>
+  void ConstrainInitialState(const T& initialState) {
+    SubjectTo(InitialState() == initialState);
+  }
+
+  /**
+   * Utility function to constrain the final state.
+   *
+   * @param finalState the final state to constrain to.
+   */
+  template <typename T>
+    requires ScalarLike<T> || MatrixLike<T>
+  void ConstrainFinalState(const T& finalState) {
+    SubjectTo(FinalState() == finalState);
+  }
+
+  /**
+   * Set the constraint evaluation function. This function is called
+   * `numSteps+1` times, with the corresponding state and input
+   * VariableMatrices.
+   *
+   * @param callback The callback f(t, x, u, dt) where t is time, x is the state
+   *   vector, u is the input vector, and dt is the timestep duration.
+   */
+  void ForEachStep(
+      const std::function<void(const Variable&, const VariableMatrix&,
+                               const VariableMatrix&, const Variable&)>&
+          callback) {
+    Variable time = 0.0;
+
+    for (int i = 0; i < m_numSteps + 1; ++i) {
+      auto x = X().Col(i);
+      auto u = U().Col(i);
+      auto dt = DT()(0, i);
+      callback(time, x, u, dt);
+
+      time += dt;
+    }
+  }
+
+  /**
+   * Convenience function to set a lower bound on the input.
+   *
+   * @param lowerBound The lower bound that inputs must always be above. Must be
+   * shaped (numInputs)x1.
+   */
+  template <typename T>
+    requires ScalarLike<T> || MatrixLike<T>
+  void SetLowerInputBound(const T& lowerBound) {
+    for (int i = 0; i < m_numSteps + 1; ++i) {
+      SubjectTo(U().Col(i) >= lowerBound);
+    }
+  }
+
+  /**
+   * Convenience function to set an upper bound on the input.
+   *
+   * @param upperBound The upper bound that inputs must always be below. Must be
+   * shaped (numInputs)x1.
+   */
+  template <typename T>
+    requires ScalarLike<T> || MatrixLike<T>
+  void SetUpperInputBound(const T& upperBound) {
+    for (int i = 0; i < m_numSteps + 1; ++i) {
+      SubjectTo(U().Col(i) <= upperBound);
+    }
+  }
+
+  /**
+   * Convenience function to set an upper bound on the timestep.
+   *
+   * @param maxTimestep The maximum timestep.
+   */
+  void SetMaxTimestep(std::chrono::duration<double> maxTimestep) {
+    SubjectTo(DT() <= maxTimestep.count());
+  }
+
+  /**
+   * Convenience function to set a lower bound on the timestep.
+   *
+   * @param minTimestep The minimum timestep.
+   */
+  void SetMinTimestep(std::chrono::duration<double> minTimestep) {
+    SubjectTo(DT() >= minTimestep.count());
+  }
+
+  /**
+   * Get the state variables. After the problem is solved, this will contain the
+   * optimized trajectory.
+   *
+   * Shaped (numStates)x(numSteps+1).
+   *
+   * @returns The state variable matrix.
+   */
+  VariableMatrix& X() { return m_X; };
+
+  /**
+   * Get the input variables. After the problem is solved, this will contain the
+   * inputs corresponding to the optimized trajectory.
+   *
+   * Shaped (numInputs)x(numSteps+1), although the last input step is unused in
+   * the trajectory.
+   *
+   * @returns The input variable matrix.
+   */
+  VariableMatrix& U() { return m_U; };
+
+  /**
+   * Get the timestep variables. After the problem is solved, this will contain
+   * the timesteps corresponding to the optimized trajectory.
+   *
+   * Shaped 1x(numSteps+1), although the last timestep is unused in
+   * the trajectory.
+   *
+   * @returns The timestep variable matrix.
+   */
+  VariableMatrix& DT() { return m_DT; };
+
+  /**
+   * Convenience function to get the initial state in the trajectory.
+   *
+   * @returns The initial state of the trajectory.
+   */
+  VariableMatrix InitialState() { return m_X.Col(0); }
+
+  /**
+   * Convenience function to get the final state in the trajectory.
+   *
+   * @returns The final state of the trajectory.
+   */
+  VariableMatrix FinalState() { return m_X.Col(m_numSteps); }
+
+ private:
+  void ConstrainDirectCollocation() {
+    Assert(m_dynamicsType == DynamicsType::kExplicitODE);
+
+    Variable time = 0.0;
+
+    for (int i = 0; i < m_numSteps; ++i) {
+      auto x_begin = X().Col(i);
+      auto x_end = X().Col(i + 1);
+      auto u_begin = U().Col(i);
+      Variable dt = DT()(0, i);
+      auto t_begin = time;
+      auto t_end = time + dt;
+      auto t_c = t_begin + dt / 2.0;
+
+      time += dt;
+
+      // Use u_begin on the end point as well because we are approaching a
+      // discontinuity from the left
+      auto f_begin = m_dynamicsFunction(t_begin, x_begin, u_begin, dt);
+      auto f_end = m_dynamicsFunction(t_end, x_end, u_begin, dt);
+      auto x_c = (x_begin + x_end) / 2.0 + (f_begin - f_end) * (dt / 8.0);
+      auto xprime_c =
+          (x_begin - x_end) * (-3.0 / (2.0 * dt)) - (f_begin + f_end) / 4.0;
+      auto f_c = m_dynamicsFunction(t_c, x_c, u_begin, dt);
+      SubjectTo(f_c == xprime_c);
+    }
+  }
+
+  void ConstrainDirectTranscription() {
+    Variable time = 0.0;
+
+    for (int i = 0; i < m_numSteps; ++i) {
+      auto x_begin = X().Col(i);
+      auto x_end = X().Col(i + 1);
+      auto u = U().Col(i);
+      Variable dt = DT()(0, i);
+
+      if (m_dynamicsType == DynamicsType::kExplicitODE) {
+        SubjectTo(x_end ==
+                  RK4<const DynamicsFunction&, VariableMatrix, VariableMatrix,
+                      Variable>(m_dynamicsFunction, x_begin, u, time, dt));
+      } else if (m_dynamicsType == DynamicsType::kDiscrete) {
+        SubjectTo(x_end == m_dynamicsFunction(time, x_begin, u, dt));
+      }
+
+      time += dt;
+    }
+  }
+
+  void ConstrainSingleShooting() {
+    Variable time = 0.0;
+
+    for (int i = 0; i < m_numSteps; ++i) {
+      auto x_begin = X().Col(i);
+      auto x_end = X().Col(i + 1);
+      auto u = U().Col(i);
+      Variable dt = DT()(0, i);
+
+      if (m_dynamicsType == DynamicsType::kExplicitODE) {
+        x_end = RK4<const DynamicsFunction&, VariableMatrix, VariableMatrix,
+                    Variable>(m_dynamicsFunction, x_begin, u, time, dt);
+      } else if (m_dynamicsType == DynamicsType::kDiscrete) {
+        x_end = m_dynamicsFunction(time, x_begin, u, dt);
+      }
+
+      time += dt;
+    }
+  }
+
+  int m_numStates;
+  int m_numInputs;
+  std::chrono::duration<double> m_dt;
+  int m_numSteps;
+  TranscriptionMethod m_transcriptionMethod;
+
+  DynamicsType m_dynamicsType;
+  DynamicsFunction m_dynamicsFunction;
+
+  TimestepMethod m_timestepMethod;
+
+  VariableMatrix m_X;
+  VariableMatrix m_U;
+  VariableMatrix m_DT;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/Constraints.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/Constraints.hpp`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <algorithm>
-#include <concepts>
-#include <vector>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/util/Assert.hpp"
-#include "sleipnir/util/Concepts.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * Make a list of constraints.
- *
- * The standard form for equality constraints is c(x) = 0, and the standard form
- * for inequality constraints is c(x) ≥ 0. This function takes constraints of
- * the form lhs = rhs or lhs ≥ rhs and converts them to lhs - rhs = 0 or
- * lhs - rhs ≥ 0.
- *
- * @param lhs Left-hand side.
- * @param rhs Right-hand side.
- */
-template <typename LHS, typename RHS>
-  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-          (ScalarLike<RHS> || MatrixLike<RHS>) &&
-          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-std::vector<Variable> MakeConstraints(const LHS& lhs, const RHS& rhs) {
-  std::vector<Variable> constraints;
-
-  if constexpr (ScalarLike<LHS> && ScalarLike<RHS>) {
-    constraints.emplace_back(lhs - rhs);
-  } else if constexpr (ScalarLike<LHS> && MatrixLike<RHS>) {
-    int rows;
-    int cols;
-    if constexpr (EigenMatrixLike<RHS>) {
-      rows = rhs.rows();
-      cols = rhs.cols();
-    } else {
-      rows = rhs.Rows();
-      cols = rhs.Cols();
-    }
-
-    constraints.reserve(rows * cols);
-
-    for (int row = 0; row < rows; ++row) {
-      for (int col = 0; col < cols; ++col) {
-        // Make right-hand side zero
-        constraints.emplace_back(lhs - rhs(row, col));
-      }
-    }
-  } else if constexpr (MatrixLike<LHS> && ScalarLike<RHS>) {
-    int rows;
-    int cols;
-    if constexpr (EigenMatrixLike<LHS>) {
-      rows = lhs.rows();
-      cols = lhs.cols();
-    } else {
-      rows = lhs.Rows();
-      cols = lhs.Cols();
-    }
-
-    constraints.reserve(rows * cols);
-
-    for (int row = 0; row < rows; ++row) {
-      for (int col = 0; col < cols; ++col) {
-        // Make right-hand side zero
-        constraints.emplace_back(lhs(row, col) - rhs);
-      }
-    }
-  } else if constexpr (MatrixLike<LHS> && MatrixLike<RHS>) {
-    int lhsRows;
-    int lhsCols;
-    if constexpr (EigenMatrixLike<LHS>) {
-      lhsRows = lhs.rows();
-      lhsCols = lhs.cols();
-    } else {
-      lhsRows = lhs.Rows();
-      lhsCols = lhs.Cols();
-    }
-
-    [[maybe_unused]]
-    int rhsRows;
-    [[maybe_unused]]
-    int rhsCols;
-    if constexpr (EigenMatrixLike<RHS>) {
-      rhsRows = rhs.rows();
-      rhsCols = rhs.cols();
-    } else {
-      rhsRows = rhs.Rows();
-      rhsCols = rhs.Cols();
-    }
-
-    Assert(lhsRows == rhsRows && lhsCols == rhsCols);
-    constraints.reserve(lhsRows * lhsCols);
-
-    for (int row = 0; row < lhsRows; ++row) {
-      for (int col = 0; col < lhsCols; ++col) {
-        // Make right-hand side zero
-        constraints.emplace_back(lhs(row, col) - rhs(row, col));
-      }
-    }
-  }
-
-  return constraints;
-}
-
-/**
- * A vector of equality constraints of the form cₑ(x) = 0.
- */
-struct SLEIPNIR_DLLEXPORT EqualityConstraints {
-  /// A vector of scalar equality constraints.
-  std::vector<Variable> constraints;
-
-  /**
-   * Constructs an equality constraint from a left and right side.
-   *
-   * The standard form for equality constraints is c(x) = 0. This function takes
-   * a constraint of the form lhs = rhs and converts it to lhs - rhs = 0.
-   *
-   * @param lhs Left-hand side.
-   * @param rhs Right-hand side.
-   */
-  template <typename LHS, typename RHS>
-    requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-            (ScalarLike<RHS> || MatrixLike<RHS>) &&
-            (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-  EqualityConstraints(const LHS& lhs, const RHS& rhs)
-      : constraints{MakeConstraints(lhs, rhs)} {}
-
-  /**
-   * Implicit conversion operator to bool.
-   */
-  operator bool() const {  // NOLINT
-    return std::all_of(
-        constraints.begin(), constraints.end(),
-        [](const auto& constraint) { return constraint.Value() == 0.0; });
-  }
-};
-
-/**
- * A vector of inequality constraints of the form cᵢ(x) ≥ 0.
- */
-struct SLEIPNIR_DLLEXPORT InequalityConstraints {
-  /// A vector of scalar inequality constraints.
-  std::vector<Variable> constraints;
-
-  /**
-   * Constructs an inequality constraint from a left and right side.
-   *
-   * The standard form for inequality constraints is c(x) ≥ 0. This function
-   * takes a constraints of the form lhs ≥ rhs and converts it to lhs - rhs ≥ 0.
-   *
-   * @param lhs Left-hand side.
-   * @param rhs Right-hand side.
-   */
-  template <typename LHS, typename RHS>
-    requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-            (ScalarLike<RHS> || MatrixLike<RHS>) &&
-            (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-  InequalityConstraints(const LHS& lhs, const RHS& rhs)
-      : constraints{MakeConstraints(lhs, rhs)} {}
-
-  /**
-   * Implicit conversion operator to bool.
-   */
-  operator bool() const {  // NOLINT
-    return std::all_of(
-        constraints.begin(), constraints.end(),
-        [](const auto& constraint) { return constraint.Value() >= 0.0; });
-  }
-};
-
-/**
- * Equality operator that returns an equality constraint for two Variables.
- *
- * @param lhs Left-hand side.
- * @param rhs Left-hand side.
- */
-template <typename LHS, typename RHS>
-  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-          (ScalarLike<RHS> || MatrixLike<RHS>) &&
-          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-EqualityConstraints operator==(const LHS& lhs, const RHS& rhs) {
-  return EqualityConstraints{lhs, rhs};
-}
-
-/**
- * Less-than comparison operator that returns an inequality constraint for two
- * Variables.
- *
- * @param lhs Left-hand side.
- * @param rhs Left-hand side.
- */
-template <typename LHS, typename RHS>
-  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-          (ScalarLike<RHS> || MatrixLike<RHS>) &&
-          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-InequalityConstraints operator<(const LHS& lhs, const RHS& rhs) {
-  return rhs >= lhs;
-}
-
-/**
- * Less-than-or-equal-to comparison operator that returns an inequality
- * constraint for two Variables.
- *
- * @param lhs Left-hand side.
- * @param rhs Left-hand side.
- */
-template <typename LHS, typename RHS>
-  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-          (ScalarLike<RHS> || MatrixLike<RHS>) &&
-          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-InequalityConstraints operator<=(const LHS& lhs, const RHS& rhs) {
-  return rhs >= lhs;
-}
-
-/**
- * Greater-than comparison operator that returns an inequality constraint for
- * two Variables.
- *
- * @param lhs Left-hand side.
- * @param rhs Left-hand side.
- */
-template <typename LHS, typename RHS>
-  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-          (ScalarLike<RHS> || MatrixLike<RHS>) &&
-          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-InequalityConstraints operator>(const LHS& lhs, const RHS& rhs) {
-  return lhs >= rhs;
-}
-
-/**
- * Greater-than-or-equal-to comparison operator that returns an inequality
- * constraint for two Variables.
- *
- * @param lhs Left-hand side.
- * @param rhs Left-hand side.
- */
-template <typename LHS, typename RHS>
-  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
-          (ScalarLike<RHS> || MatrixLike<RHS>) &&
-          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
-InequalityConstraints operator>=(const LHS& lhs, const RHS& rhs) {
-  return InequalityConstraints{lhs, rhs};
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <algorithm>
+#include <concepts>
+#include <vector>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/util/Assert.hpp"
+#include "sleipnir/util/Concepts.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * Make a list of constraints.
+ *
+ * The standard form for equality constraints is c(x) = 0, and the standard form
+ * for inequality constraints is c(x) ≥ 0. This function takes constraints of
+ * the form lhs = rhs or lhs ≥ rhs and converts them to lhs - rhs = 0 or
+ * lhs - rhs ≥ 0.
+ *
+ * @param lhs Left-hand side.
+ * @param rhs Right-hand side.
+ */
+template <typename LHS, typename RHS>
+  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+          (ScalarLike<RHS> || MatrixLike<RHS>) &&
+          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+std::vector<Variable> MakeConstraints(const LHS& lhs, const RHS& rhs) {
+  std::vector<Variable> constraints;
+
+  if constexpr (ScalarLike<LHS> && ScalarLike<RHS>) {
+    constraints.emplace_back(lhs - rhs);
+  } else if constexpr (ScalarLike<LHS> && MatrixLike<RHS>) {
+    int rows;
+    int cols;
+    if constexpr (EigenMatrixLike<RHS>) {
+      rows = rhs.rows();
+      cols = rhs.cols();
+    } else {
+      rows = rhs.Rows();
+      cols = rhs.Cols();
+    }
+
+    constraints.reserve(rows * cols);
+
+    for (int row = 0; row < rows; ++row) {
+      for (int col = 0; col < cols; ++col) {
+        // Make right-hand side zero
+        constraints.emplace_back(lhs - rhs(row, col));
+      }
+    }
+  } else if constexpr (MatrixLike<LHS> && ScalarLike<RHS>) {
+    int rows;
+    int cols;
+    if constexpr (EigenMatrixLike<LHS>) {
+      rows = lhs.rows();
+      cols = lhs.cols();
+    } else {
+      rows = lhs.Rows();
+      cols = lhs.Cols();
+    }
+
+    constraints.reserve(rows * cols);
+
+    for (int row = 0; row < rows; ++row) {
+      for (int col = 0; col < cols; ++col) {
+        // Make right-hand side zero
+        constraints.emplace_back(lhs(row, col) - rhs);
+      }
+    }
+  } else if constexpr (MatrixLike<LHS> && MatrixLike<RHS>) {
+    int lhsRows;
+    int lhsCols;
+    if constexpr (EigenMatrixLike<LHS>) {
+      lhsRows = lhs.rows();
+      lhsCols = lhs.cols();
+    } else {
+      lhsRows = lhs.Rows();
+      lhsCols = lhs.Cols();
+    }
+
+    [[maybe_unused]]
+    int rhsRows;
+    [[maybe_unused]]
+    int rhsCols;
+    if constexpr (EigenMatrixLike<RHS>) {
+      rhsRows = rhs.rows();
+      rhsCols = rhs.cols();
+    } else {
+      rhsRows = rhs.Rows();
+      rhsCols = rhs.Cols();
+    }
+
+    Assert(lhsRows == rhsRows && lhsCols == rhsCols);
+    constraints.reserve(lhsRows * lhsCols);
+
+    for (int row = 0; row < lhsRows; ++row) {
+      for (int col = 0; col < lhsCols; ++col) {
+        // Make right-hand side zero
+        constraints.emplace_back(lhs(row, col) - rhs(row, col));
+      }
+    }
+  }
+
+  return constraints;
+}
+
+/**
+ * A vector of equality constraints of the form cₑ(x) = 0.
+ */
+struct SLEIPNIR_DLLEXPORT EqualityConstraints {
+  /// A vector of scalar equality constraints.
+  std::vector<Variable> constraints;
+
+  /**
+   * Constructs an equality constraint from a left and right side.
+   *
+   * The standard form for equality constraints is c(x) = 0. This function takes
+   * a constraint of the form lhs = rhs and converts it to lhs - rhs = 0.
+   *
+   * @param lhs Left-hand side.
+   * @param rhs Right-hand side.
+   */
+  template <typename LHS, typename RHS>
+    requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+            (ScalarLike<RHS> || MatrixLike<RHS>) &&
+            (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+  EqualityConstraints(const LHS& lhs, const RHS& rhs)
+      : constraints{MakeConstraints(lhs, rhs)} {}
+
+  /**
+   * Implicit conversion operator to bool.
+   */
+  operator bool() const {  // NOLINT
+    return std::all_of(
+        constraints.begin(), constraints.end(),
+        [](const auto& constraint) { return constraint.Value() == 0.0; });
+  }
+};
+
+/**
+ * A vector of inequality constraints of the form cᵢ(x) ≥ 0.
+ */
+struct SLEIPNIR_DLLEXPORT InequalityConstraints {
+  /// A vector of scalar inequality constraints.
+  std::vector<Variable> constraints;
+
+  /**
+   * Constructs an inequality constraint from a left and right side.
+   *
+   * The standard form for inequality constraints is c(x) ≥ 0. This function
+   * takes a constraints of the form lhs ≥ rhs and converts it to lhs - rhs ≥ 0.
+   *
+   * @param lhs Left-hand side.
+   * @param rhs Right-hand side.
+   */
+  template <typename LHS, typename RHS>
+    requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+            (ScalarLike<RHS> || MatrixLike<RHS>) &&
+            (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+  InequalityConstraints(const LHS& lhs, const RHS& rhs)
+      : constraints{MakeConstraints(lhs, rhs)} {}
+
+  /**
+   * Implicit conversion operator to bool.
+   */
+  operator bool() const {  // NOLINT
+    return std::all_of(
+        constraints.begin(), constraints.end(),
+        [](const auto& constraint) { return constraint.Value() >= 0.0; });
+  }
+};
+
+/**
+ * Equality operator that returns an equality constraint for two Variables.
+ *
+ * @param lhs Left-hand side.
+ * @param rhs Left-hand side.
+ */
+template <typename LHS, typename RHS>
+  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+          (ScalarLike<RHS> || MatrixLike<RHS>) &&
+          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+EqualityConstraints operator==(const LHS& lhs, const RHS& rhs) {
+  return EqualityConstraints{lhs, rhs};
+}
+
+/**
+ * Less-than comparison operator that returns an inequality constraint for two
+ * Variables.
+ *
+ * @param lhs Left-hand side.
+ * @param rhs Left-hand side.
+ */
+template <typename LHS, typename RHS>
+  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+          (ScalarLike<RHS> || MatrixLike<RHS>) &&
+          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+InequalityConstraints operator<(const LHS& lhs, const RHS& rhs) {
+  return rhs >= lhs;
+}
+
+/**
+ * Less-than-or-equal-to comparison operator that returns an inequality
+ * constraint for two Variables.
+ *
+ * @param lhs Left-hand side.
+ * @param rhs Left-hand side.
+ */
+template <typename LHS, typename RHS>
+  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+          (ScalarLike<RHS> || MatrixLike<RHS>) &&
+          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+InequalityConstraints operator<=(const LHS& lhs, const RHS& rhs) {
+  return rhs >= lhs;
+}
+
+/**
+ * Greater-than comparison operator that returns an inequality constraint for
+ * two Variables.
+ *
+ * @param lhs Left-hand side.
+ * @param rhs Left-hand side.
+ */
+template <typename LHS, typename RHS>
+  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+          (ScalarLike<RHS> || MatrixLike<RHS>) &&
+          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+InequalityConstraints operator>(const LHS& lhs, const RHS& rhs) {
+  return lhs >= rhs;
+}
+
+/**
+ * Greater-than-or-equal-to comparison operator that returns an inequality
+ * constraint for two Variables.
+ *
+ * @param lhs Left-hand side.
+ * @param rhs Left-hand side.
+ */
+template <typename LHS, typename RHS>
+  requires(ScalarLike<LHS> || MatrixLike<LHS>) &&
+          (ScalarLike<RHS> || MatrixLike<RHS>) &&
+          (!std::same_as<LHS, double> || !std::same_as<RHS, double>)
+InequalityConstraints operator>=(const LHS& lhs, const RHS& rhs) {
+  return InequalityConstraints{lhs, rhs};
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/OptimizationProblem.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/OptimizationProblem.hpp`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,559 +1,559 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <algorithm>
-#include <array>
-#include <concepts>
-#include <functional>
-#include <iterator>
-#include <optional>
-#include <type_traits>
-#include <utility>
-#include <vector>
-
-#include <Eigen/Core>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/autodiff/VariableMatrix.hpp"
-#include "sleipnir/optimization/Constraints.hpp"
-#include "sleipnir/optimization/SolverConfig.hpp"
-#include "sleipnir/optimization/SolverExitCondition.hpp"
-#include "sleipnir/optimization/SolverIterationInfo.hpp"
-#include "sleipnir/optimization/SolverStatus.hpp"
-#include "sleipnir/optimization/solver/InteriorPoint.hpp"
-#include "sleipnir/util/Print.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * This class allows the user to pose a constrained nonlinear optimization
- * problem in natural mathematical notation and solve it.
- *
- * This class supports problems of the form:
-@verbatim
-      minₓ f(x)
-subject to cₑ(x) = 0
-           cᵢ(x) ≥ 0
-@endverbatim
- *
- * where f(x) is the scalar cost function, x is the vector of decision variables
- * (variables the solver can tweak to minimize the cost function), cᵢ(x) are the
- * inequality constraints, and cₑ(x) are the equality constraints. Constraints
- * are equations or inequalities of the decision variables that constrain what
- * values the solver is allowed to use when searching for an optimal solution.
- *
- * The nice thing about this class is users don't have to put their system in
- * the form shown above manually; they can write it in natural mathematical form
- * and it'll be converted for them. We'll cover some examples next.
- *
- * ## Double integrator minimum time
- *
- * A system with position and velocity states and an acceleration input is an
- * example of a double integrator. We want to go from 0 m at rest to 10 m at
- * rest in the minimum time while obeying the velocity limit (-1, 1) and the
- * acceleration limit (-1, 1).
- *
- * The model for our double integrator is ẍ=u where x is the vector [position;
- * velocity] and u is the acceleration. The velocity constraints are -1 ≤ x(1)
- * ≤ 1 and the acceleration constraints are -1 ≤ u ≤ 1.
- *
- * ### Initializing a problem instance
- *
- * First, we need to make a problem instance.
- * @code{.cpp}
- * #include <Eigen/Core>
- * #include <sleipnir/optimization/OptimizationProblem.hpp>
- *
- * int main() {
- *   constexpr auto T = 5s;
- *   constexpr auto dt = 5ms;
- *   constexpr int N = T / dt;
- *
- *   sleipnir::OptimizationProblem problem;
- * @endcode
- *
- * ### Creating decision variables
- *
- * First, we need to make decision variables for our state and input.
- * @code{.cpp}
- *   // 2x1 state vector with N + 1 timesteps (includes last state)
- *   auto X = problem.DecisionVariable(2, N + 1);
- *
- *   // 1x1 input vector with N timesteps (input at last state doesn't matter)
- *   auto U = problem.DecisionVariable(1, N);
- * @endcode
- * By convention, we use capital letters for the variables to designate
- * matrices.
- *
- * ### Applying constraints
- *
- * Now, we need to apply dynamics constraints between timesteps.
- * @code{.cpp}
- * // Kinematics constraint assuming constant acceleration between timesteps
- * for (int k = 0; k < N; ++k) {
- *   constexpr double t = std::chrono::duration<double>(dt).count();
- *   auto p_k1 = X(0, k + 1);
- *   auto v_k1 = X(1, k + 1);
- *   auto p_k = X(0, k);
- *   auto v_k = X(1, k);
- *   auto a_k = U(0, k);
- *
- *   // pₖ₊₁ = pₖ + vₖt
- *   problem.SubjectTo(p_k1 == p_k + v_k * t);
- *
- *   // vₖ₊₁ = vₖ + aₖt
- *   problem.SubjectTo(v_k1 == v_k + a_k * t);
- * }
- * @endcode
- *
- * Next, we'll apply the state and input constraints.
- * @code{.cpp}
- * // Start and end at rest
- * problem.SubjectTo(X.Col(0) == Eigen::Matrix<double, 2, 1>{{0.0}, {0.0}});
- * problem.SubjectTo(
- *   X.Col(N + 1) == Eigen::Matrix<double, 2, 1>{{10.0}, {0.0}});
- *
- * // Limit velocity
- * problem.SubjectTo(-1 <= X.Row(1));
- * problem.SubjectTo(X.Row(1) <= 1);
- *
- * // Limit acceleration
- * problem.SubjectTo(-1 <= U);
- * problem.SubjectTo(U <= 1);
- * @endcode
- *
- * ### Specifying a cost function
- *
- * Next, we'll create a cost function for minimizing position error.
- * @code{.cpp}
- * // Cost function - minimize position error
- * sleipnir::Variable J = 0.0;
- * for (int k = 0; k < N + 1; ++k) {
- *   J += sleipnir::pow(10.0 - X(0, k), 2);
- * }
- * problem.Minimize(J);
- * @endcode
- * The cost function passed to Minimize() should produce a scalar output.
- *
- * ### Solving the problem
- *
- * Now we can solve the problem.
- * @code{.cpp}
- * problem.Solve();
- * @endcode
- *
- * The solver will find the decision variable values that minimize the cost
- * function while satisfying the constraints.
- *
- * ### Accessing the solution
- *
- * You can obtain the solution by querying the values of the variables like so.
- * @code{.cpp}
- * double position = X.Value(0, 0);
- * double velocity = X.Value(1, 0);
- * double acceleration = U.Value(0);
- * @endcode
- *
- * ### Other applications
- *
- * In retrospect, the solution here seems obvious: if you want to reach the
- * desired position in the minimum time, you just apply positive max input to
- * accelerate to the max speed, coast for a while, then apply negative max input
- * to decelerate to a stop at the desired position. Optimization problems can
- * get more complex than this though. In fact, we can use this same framework to
- * design optimal trajectories for a drivetrain while satisfying dynamics
- * constraints, avoiding obstacles, and driving through points of interest.
- *
- * ## Optimizing the problem formulation
- *
- * Cost functions and constraints can have the following orders:
- *
- * <ul>
- *   <li>none (i.e., there is no cost function or are no constraints)</li>
- *   <li>constant</li>
- *   <li>linear</li>
- *   <li>quadratic</li>
- *   <li>nonlinear</li>
- * </ul>
- *
- * For nonlinear problems, the solver calculates the Hessian of the cost
- * function and the Jacobians of the constraints at each iteration. However,
- * problems with lower order cost functions and constraints can be solved
- * faster. For example, the following only need to be computed once because
- * they're constant:
- *
- * <ul>
- *   <li>the Hessian of a quadratic or lower cost function</li>
- *   <li>the Jacobian of linear or lower constraints</li>
- * </ul>
- *
- * A problem is constant if:
- *
- * <ul>
- *   <li>the cost function is constant or lower</li>
- *   <li>the equality constraints are constant or lower</li>
- *   <li>the inequality constraints are constant or lower</li>
- * </ul>
- *
- * A problem is linear if:
- *
- * <ul>
- *   <li>the cost function is linear</li>
- *   <li>the equality constraints are linear or lower</li>
- *   <li>the inequality constraints are linear or lower</li>
- * </ul>
- *
- * A problem is quadratic if:
- *
- * <ul>
- *   <li>the cost function is quadratic</li>
- *   <li>the equality constraints are linear or lower</li>
- *   <li>the inequality constraints are linear or lower</li>
- * </ul>
- *
- * All other problems are nonlinear.
- */
-class SLEIPNIR_DLLEXPORT OptimizationProblem {
- public:
-  /**
-   * Construct the optimization problem.
-   */
-  OptimizationProblem() noexcept {
-    m_decisionVariables.reserve(1024);
-    m_equalityConstraints.reserve(1024);
-    m_inequalityConstraints.reserve(1024);
-  }
-
-  /**
-   * Create a decision variable in the optimization problem.
-   */
-  [[nodiscard]]
-  Variable DecisionVariable() {
-    m_decisionVariables.emplace_back();
-    return m_decisionVariables.back();
-  }
-
-  /**
-   * Create a matrix of decision variables in the optimization problem.
-   *
-   * @param rows Number of matrix rows.
-   * @param cols Number of matrix columns.
-   */
-  [[nodiscard]]
-  VariableMatrix DecisionVariable(int rows, int cols = 1) {
-    m_decisionVariables.reserve(m_decisionVariables.size() + rows * cols);
-
-    VariableMatrix vars{rows, cols};
-
-    for (int row = 0; row < rows; ++row) {
-      for (int col = 0; col < cols; ++col) {
-        m_decisionVariables.emplace_back();
-        vars(row, col) = m_decisionVariables.back();
-      }
-    }
-
-    return vars;
-  }
-
-  /**
-   * Create a symmetric matrix of decision variables in the optimization
-   * problem.
-   *
-   * Variable instances are reused across the diagonal, which helps reduce
-   * problem dimensionality.
-   *
-   * @param rows Number of matrix rows.
-   */
-  [[nodiscard]]
-  VariableMatrix SymmetricDecisionVariable(int rows) {
-    // We only need to store the lower triangle of an n x n symmetric matrix;
-    // the other elements are duplicates. The lower triangle has (n² + n)/2
-    // elements.
-    //
-    //   n
-    //   Σ k = (n² + n)/2
-    //  k=1
-    m_decisionVariables.reserve(m_decisionVariables.size() +
-                                (rows * rows + rows) / 2);
-
-    VariableMatrix vars{rows, rows};
-
-    for (int row = 0; row < rows; ++row) {
-      for (int col = 0; col <= row; ++col) {
-        m_decisionVariables.emplace_back();
-        vars(row, col) = m_decisionVariables.back();
-        vars(col, row) = m_decisionVariables.back();
-      }
-    }
-
-    return vars;
-  }
-
-  /**
-   * Tells the solver to minimize the output of the given cost function.
-   *
-   * Note that this is optional. If only constraints are specified, the solver
-   * will find the closest solution to the initial conditions that's in the
-   * feasible set.
-   *
-   * @param cost The cost function to minimize.
-   */
-  void Minimize(const Variable& cost) {
-    m_f = cost;
-    status.costFunctionType = m_f.value().Type();
-  }
-
-  /**
-   * Tells the solver to minimize the output of the given cost function.
-   *
-   * Note that this is optional. If only constraints are specified, the solver
-   * will find the closest solution to the initial conditions that's in the
-   * feasible set.
-   *
-   * @param cost The cost function to minimize.
-   */
-  void Minimize(Variable&& cost) {
-    m_f = std::move(cost);
-    status.costFunctionType = m_f.value().Type();
-  }
-
-  /**
-   * Tells the solver to maximize the output of the given objective function.
-   *
-   * Note that this is optional. If only constraints are specified, the solver
-   * will find the closest solution to the initial conditions that's in the
-   * feasible set.
-   *
-   * @param objective The objective function to maximize.
-   */
-  void Maximize(const Variable& objective) {
-    // Maximizing a cost function is the same as minimizing its negative
-    m_f = -objective;
-    status.costFunctionType = m_f.value().Type();
-  }
-
-  /**
-   * Tells the solver to maximize the output of the given objective function.
-   *
-   * Note that this is optional. If only constraints are specified, the solver
-   * will find the closest solution to the initial conditions that's in the
-   * feasible set.
-   *
-   * @param objective The objective function to maximize.
-   */
-  void Maximize(Variable&& objective) {
-    // Maximizing a cost function is the same as minimizing its negative
-    m_f = -std::move(objective);
-    status.costFunctionType = m_f.value().Type();
-  }
-
-  /**
-   * Tells the solver to solve the problem while satisfying the given equality
-   * constraint.
-   *
-   * @param constraint The constraint to satisfy.
-   */
-  void SubjectTo(const EqualityConstraints& constraint) {
-    // Get the highest order equality constraint expression type
-    for (const auto& c : constraint.constraints) {
-      status.equalityConstraintType =
-          std::max(status.equalityConstraintType, c.Type());
-    }
-
-    m_equalityConstraints.reserve(m_equalityConstraints.size() +
-                                  constraint.constraints.size());
-    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
-              std::back_inserter(m_equalityConstraints));
-  }
-
-  /**
-   * Tells the solver to solve the problem while satisfying the given equality
-   * constraint.
-   *
-   * @param constraint The constraint to satisfy.
-   */
-  void SubjectTo(EqualityConstraints&& constraint) {
-    // Get the highest order equality constraint expression type
-    for (const auto& c : constraint.constraints) {
-      status.equalityConstraintType =
-          std::max(status.equalityConstraintType, c.Type());
-    }
-
-    m_equalityConstraints.reserve(m_equalityConstraints.size() +
-                                  constraint.constraints.size());
-    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
-              std::back_inserter(m_equalityConstraints));
-  }
-
-  /**
-   * Tells the solver to solve the problem while satisfying the given inequality
-   * constraint.
-   *
-   * @param constraint The constraint to satisfy.
-   */
-  void SubjectTo(const InequalityConstraints& constraint) {
-    // Get the highest order inequality constraint expression type
-    for (const auto& c : constraint.constraints) {
-      status.inequalityConstraintType =
-          std::max(status.inequalityConstraintType, c.Type());
-    }
-
-    m_inequalityConstraints.reserve(m_inequalityConstraints.size() +
-                                    constraint.constraints.size());
-    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
-              std::back_inserter(m_inequalityConstraints));
-  }
-
-  /**
-   * Tells the solver to solve the problem while satisfying the given inequality
-   * constraint.
-   *
-   * @param constraint The constraint to satisfy.
-   */
-  void SubjectTo(InequalityConstraints&& constraint) {
-    // Get the highest order inequality constraint expression type
-    for (const auto& c : constraint.constraints) {
-      status.inequalityConstraintType =
-          std::max(status.inequalityConstraintType, c.Type());
-    }
-
-    m_inequalityConstraints.reserve(m_inequalityConstraints.size() +
-                                    constraint.constraints.size());
-    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
-              std::back_inserter(m_inequalityConstraints));
-  }
-
-  /**
-   * Solve the optimization problem. The solution will be stored in the original
-   * variables used to construct the problem.
-   *
-   * @param config Configuration options for the solver.
-   */
-  SolverStatus Solve(const SolverConfig& config = kDefaultConfig) {
-    // Create the initial value column vector
-    Eigen::VectorXd x{m_decisionVariables.size()};
-    for (size_t i = 0; i < m_decisionVariables.size(); ++i) {
-      x(i) = m_decisionVariables[i].Value();
-    }
-
-    status.exitCondition = SolverExitCondition::kSuccess;
-
-    // If there's no cost function, make it zero and continue
-    if (!m_f.has_value()) {
-      m_f = Variable();
-    }
-
-    if (config.diagnostics) {
-      constexpr std::array kExprTypeToName{"empty", "constant", "linear",
-                                           "quadratic", "nonlinear"};
-
-      // Print cost function and constraint expression types
-      sleipnir::println(
-          "The cost function is {}.",
-          kExprTypeToName[static_cast<int>(status.costFunctionType)]);
-      sleipnir::println(
-          "The equality constraints are {}.",
-          kExprTypeToName[static_cast<int>(status.equalityConstraintType)]);
-      sleipnir::println(
-          "The inequality constraints are {}.",
-          kExprTypeToName[static_cast<int>(status.inequalityConstraintType)]);
-      sleipnir::println("");
-
-      // Print problem dimensionality
-      sleipnir::println("Number of decision variables: {}",
-                        m_decisionVariables.size());
-      sleipnir::println("Number of equality constraints: {}",
-                        m_equalityConstraints.size());
-      sleipnir::println("Number of inequality constraints: {}\n",
-                        m_inequalityConstraints.size());
-    }
-
-    // If the problem is empty or constant, there's nothing to do
-    if (status.costFunctionType <= ExpressionType::kConstant &&
-        status.equalityConstraintType <= ExpressionType::kConstant &&
-        status.inequalityConstraintType <= ExpressionType::kConstant) {
-      return status;
-    }
-
-    // Solve the optimization problem
-    Eigen::VectorXd s = Eigen::VectorXd::Ones(m_inequalityConstraints.size());
-    InteriorPoint(m_decisionVariables, m_equalityConstraints,
-                  m_inequalityConstraints, m_f.value(), m_callback, config,
-                  false, x, s, &status);
-
-    if (config.diagnostics) {
-      sleipnir::println("Exit condition: {}", ToMessage(status.exitCondition));
-    }
-
-    // Assign the solution to the original Variable instances
-    VariableMatrix{m_decisionVariables}.SetValue(x);
-
-    return status;
-  }
-
-  /**
-   * Sets a callback to be called at each solver iteration.
-   *
-   * The callback for this overload should return void.
-   *
-   * @param callback The callback.
-   */
-  template <typename F>
-    requires std::invocable<F, const SolverIterationInfo&> &&
-             std::same_as<std::invoke_result_t<F, const SolverIterationInfo&>,
-                          void>
-  void Callback(F&& callback) {
-    m_callback = [=, callback = std::forward<F>(callback)](
-                     const SolverIterationInfo& info) {
-      callback(info);
-      return false;
-    };
-  }
-
-  /**
-   * Sets a callback to be called at each solver iteration.
-   *
-   * The callback for this overload should return bool.
-   *
-   * @param callback The callback. Returning true from the callback causes the
-   *   solver to exit early with the solution it has so far.
-   */
-  template <typename F>
-    requires std::invocable<F, const SolverIterationInfo&> &&
-             std::same_as<std::invoke_result_t<F, const SolverIterationInfo&>,
-                          bool>
-  void Callback(F&& callback) {
-    m_callback = std::forward<F>(callback);
-  }
-
- private:
-  // GCC incorrectly applies C++14 rules for const static data members, so an
-  // initializer is required here.
-  //
-  // https://stackoverflow.com/a/50639754
-  static constexpr SolverConfig kDefaultConfig{};
-
-  // The list of decision variables, which are the root of the problem's
-  // expression tree
-  std::vector<Variable> m_decisionVariables;
-
-  // The cost function: f(x)
-  std::optional<Variable> m_f;
-
-  // The list of equality constraints: cₑ(x) = 0
-  std::vector<Variable> m_equalityConstraints;
-
-  // The list of inequality constraints: cᵢ(x) ≥ 0
-  std::vector<Variable> m_inequalityConstraints;
-
-  // The user callback
-  std::function<bool(const SolverIterationInfo&)> m_callback =
-      [](const SolverIterationInfo&) { return false; };
-
-  // The solver status
-  SolverStatus status;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <algorithm>
+#include <array>
+#include <concepts>
+#include <functional>
+#include <iterator>
+#include <optional>
+#include <type_traits>
+#include <utility>
+#include <vector>
+
+#include <Eigen/Core>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/autodiff/VariableMatrix.hpp"
+#include "sleipnir/optimization/Constraints.hpp"
+#include "sleipnir/optimization/SolverConfig.hpp"
+#include "sleipnir/optimization/SolverExitCondition.hpp"
+#include "sleipnir/optimization/SolverIterationInfo.hpp"
+#include "sleipnir/optimization/SolverStatus.hpp"
+#include "sleipnir/optimization/solver/InteriorPoint.hpp"
+#include "sleipnir/util/Print.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * This class allows the user to pose a constrained nonlinear optimization
+ * problem in natural mathematical notation and solve it.
+ *
+ * This class supports problems of the form:
+@verbatim
+      minₓ f(x)
+subject to cₑ(x) = 0
+           cᵢ(x) ≥ 0
+@endverbatim
+ *
+ * where f(x) is the scalar cost function, x is the vector of decision variables
+ * (variables the solver can tweak to minimize the cost function), cᵢ(x) are the
+ * inequality constraints, and cₑ(x) are the equality constraints. Constraints
+ * are equations or inequalities of the decision variables that constrain what
+ * values the solver is allowed to use when searching for an optimal solution.
+ *
+ * The nice thing about this class is users don't have to put their system in
+ * the form shown above manually; they can write it in natural mathematical form
+ * and it'll be converted for them. We'll cover some examples next.
+ *
+ * ## Double integrator minimum time
+ *
+ * A system with position and velocity states and an acceleration input is an
+ * example of a double integrator. We want to go from 0 m at rest to 10 m at
+ * rest in the minimum time while obeying the velocity limit (-1, 1) and the
+ * acceleration limit (-1, 1).
+ *
+ * The model for our double integrator is ẍ=u where x is the vector [position;
+ * velocity] and u is the acceleration. The velocity constraints are -1 ≤ x(1)
+ * ≤ 1 and the acceleration constraints are -1 ≤ u ≤ 1.
+ *
+ * ### Initializing a problem instance
+ *
+ * First, we need to make a problem instance.
+ * @code{.cpp}
+ * #include <Eigen/Core>
+ * #include <sleipnir/optimization/OptimizationProblem.hpp>
+ *
+ * int main() {
+ *   constexpr auto T = 5s;
+ *   constexpr auto dt = 5ms;
+ *   constexpr int N = T / dt;
+ *
+ *   sleipnir::OptimizationProblem problem;
+ * @endcode
+ *
+ * ### Creating decision variables
+ *
+ * First, we need to make decision variables for our state and input.
+ * @code{.cpp}
+ *   // 2x1 state vector with N + 1 timesteps (includes last state)
+ *   auto X = problem.DecisionVariable(2, N + 1);
+ *
+ *   // 1x1 input vector with N timesteps (input at last state doesn't matter)
+ *   auto U = problem.DecisionVariable(1, N);
+ * @endcode
+ * By convention, we use capital letters for the variables to designate
+ * matrices.
+ *
+ * ### Applying constraints
+ *
+ * Now, we need to apply dynamics constraints between timesteps.
+ * @code{.cpp}
+ * // Kinematics constraint assuming constant acceleration between timesteps
+ * for (int k = 0; k < N; ++k) {
+ *   constexpr double t = std::chrono::duration<double>(dt).count();
+ *   auto p_k1 = X(0, k + 1);
+ *   auto v_k1 = X(1, k + 1);
+ *   auto p_k = X(0, k);
+ *   auto v_k = X(1, k);
+ *   auto a_k = U(0, k);
+ *
+ *   // pₖ₊₁ = pₖ + vₖt
+ *   problem.SubjectTo(p_k1 == p_k + v_k * t);
+ *
+ *   // vₖ₊₁ = vₖ + aₖt
+ *   problem.SubjectTo(v_k1 == v_k + a_k * t);
+ * }
+ * @endcode
+ *
+ * Next, we'll apply the state and input constraints.
+ * @code{.cpp}
+ * // Start and end at rest
+ * problem.SubjectTo(X.Col(0) == Eigen::Matrix<double, 2, 1>{{0.0}, {0.0}});
+ * problem.SubjectTo(
+ *   X.Col(N + 1) == Eigen::Matrix<double, 2, 1>{{10.0}, {0.0}});
+ *
+ * // Limit velocity
+ * problem.SubjectTo(-1 <= X.Row(1));
+ * problem.SubjectTo(X.Row(1) <= 1);
+ *
+ * // Limit acceleration
+ * problem.SubjectTo(-1 <= U);
+ * problem.SubjectTo(U <= 1);
+ * @endcode
+ *
+ * ### Specifying a cost function
+ *
+ * Next, we'll create a cost function for minimizing position error.
+ * @code{.cpp}
+ * // Cost function - minimize position error
+ * sleipnir::Variable J = 0.0;
+ * for (int k = 0; k < N + 1; ++k) {
+ *   J += sleipnir::pow(10.0 - X(0, k), 2);
+ * }
+ * problem.Minimize(J);
+ * @endcode
+ * The cost function passed to Minimize() should produce a scalar output.
+ *
+ * ### Solving the problem
+ *
+ * Now we can solve the problem.
+ * @code{.cpp}
+ * problem.Solve();
+ * @endcode
+ *
+ * The solver will find the decision variable values that minimize the cost
+ * function while satisfying the constraints.
+ *
+ * ### Accessing the solution
+ *
+ * You can obtain the solution by querying the values of the variables like so.
+ * @code{.cpp}
+ * double position = X.Value(0, 0);
+ * double velocity = X.Value(1, 0);
+ * double acceleration = U.Value(0);
+ * @endcode
+ *
+ * ### Other applications
+ *
+ * In retrospect, the solution here seems obvious: if you want to reach the
+ * desired position in the minimum time, you just apply positive max input to
+ * accelerate to the max speed, coast for a while, then apply negative max input
+ * to decelerate to a stop at the desired position. Optimization problems can
+ * get more complex than this though. In fact, we can use this same framework to
+ * design optimal trajectories for a drivetrain while satisfying dynamics
+ * constraints, avoiding obstacles, and driving through points of interest.
+ *
+ * ## Optimizing the problem formulation
+ *
+ * Cost functions and constraints can have the following orders:
+ *
+ * <ul>
+ *   <li>none (i.e., there is no cost function or are no constraints)</li>
+ *   <li>constant</li>
+ *   <li>linear</li>
+ *   <li>quadratic</li>
+ *   <li>nonlinear</li>
+ * </ul>
+ *
+ * For nonlinear problems, the solver calculates the Hessian of the cost
+ * function and the Jacobians of the constraints at each iteration. However,
+ * problems with lower order cost functions and constraints can be solved
+ * faster. For example, the following only need to be computed once because
+ * they're constant:
+ *
+ * <ul>
+ *   <li>the Hessian of a quadratic or lower cost function</li>
+ *   <li>the Jacobian of linear or lower constraints</li>
+ * </ul>
+ *
+ * A problem is constant if:
+ *
+ * <ul>
+ *   <li>the cost function is constant or lower</li>
+ *   <li>the equality constraints are constant or lower</li>
+ *   <li>the inequality constraints are constant or lower</li>
+ * </ul>
+ *
+ * A problem is linear if:
+ *
+ * <ul>
+ *   <li>the cost function is linear</li>
+ *   <li>the equality constraints are linear or lower</li>
+ *   <li>the inequality constraints are linear or lower</li>
+ * </ul>
+ *
+ * A problem is quadratic if:
+ *
+ * <ul>
+ *   <li>the cost function is quadratic</li>
+ *   <li>the equality constraints are linear or lower</li>
+ *   <li>the inequality constraints are linear or lower</li>
+ * </ul>
+ *
+ * All other problems are nonlinear.
+ */
+class SLEIPNIR_DLLEXPORT OptimizationProblem {
+ public:
+  /**
+   * Construct the optimization problem.
+   */
+  OptimizationProblem() noexcept {
+    m_decisionVariables.reserve(1024);
+    m_equalityConstraints.reserve(1024);
+    m_inequalityConstraints.reserve(1024);
+  }
+
+  /**
+   * Create a decision variable in the optimization problem.
+   */
+  [[nodiscard]]
+  Variable DecisionVariable() {
+    m_decisionVariables.emplace_back();
+    return m_decisionVariables.back();
+  }
+
+  /**
+   * Create a matrix of decision variables in the optimization problem.
+   *
+   * @param rows Number of matrix rows.
+   * @param cols Number of matrix columns.
+   */
+  [[nodiscard]]
+  VariableMatrix DecisionVariable(int rows, int cols = 1) {
+    m_decisionVariables.reserve(m_decisionVariables.size() + rows * cols);
+
+    VariableMatrix vars{rows, cols};
+
+    for (int row = 0; row < rows; ++row) {
+      for (int col = 0; col < cols; ++col) {
+        m_decisionVariables.emplace_back();
+        vars(row, col) = m_decisionVariables.back();
+      }
+    }
+
+    return vars;
+  }
+
+  /**
+   * Create a symmetric matrix of decision variables in the optimization
+   * problem.
+   *
+   * Variable instances are reused across the diagonal, which helps reduce
+   * problem dimensionality.
+   *
+   * @param rows Number of matrix rows.
+   */
+  [[nodiscard]]
+  VariableMatrix SymmetricDecisionVariable(int rows) {
+    // We only need to store the lower triangle of an n x n symmetric matrix;
+    // the other elements are duplicates. The lower triangle has (n² + n)/2
+    // elements.
+    //
+    //   n
+    //   Σ k = (n² + n)/2
+    //  k=1
+    m_decisionVariables.reserve(m_decisionVariables.size() +
+                                (rows * rows + rows) / 2);
+
+    VariableMatrix vars{rows, rows};
+
+    for (int row = 0; row < rows; ++row) {
+      for (int col = 0; col <= row; ++col) {
+        m_decisionVariables.emplace_back();
+        vars(row, col) = m_decisionVariables.back();
+        vars(col, row) = m_decisionVariables.back();
+      }
+    }
+
+    return vars;
+  }
+
+  /**
+   * Tells the solver to minimize the output of the given cost function.
+   *
+   * Note that this is optional. If only constraints are specified, the solver
+   * will find the closest solution to the initial conditions that's in the
+   * feasible set.
+   *
+   * @param cost The cost function to minimize.
+   */
+  void Minimize(const Variable& cost) {
+    m_f = cost;
+    status.costFunctionType = m_f.value().Type();
+  }
+
+  /**
+   * Tells the solver to minimize the output of the given cost function.
+   *
+   * Note that this is optional. If only constraints are specified, the solver
+   * will find the closest solution to the initial conditions that's in the
+   * feasible set.
+   *
+   * @param cost The cost function to minimize.
+   */
+  void Minimize(Variable&& cost) {
+    m_f = std::move(cost);
+    status.costFunctionType = m_f.value().Type();
+  }
+
+  /**
+   * Tells the solver to maximize the output of the given objective function.
+   *
+   * Note that this is optional. If only constraints are specified, the solver
+   * will find the closest solution to the initial conditions that's in the
+   * feasible set.
+   *
+   * @param objective The objective function to maximize.
+   */
+  void Maximize(const Variable& objective) {
+    // Maximizing a cost function is the same as minimizing its negative
+    m_f = -objective;
+    status.costFunctionType = m_f.value().Type();
+  }
+
+  /**
+   * Tells the solver to maximize the output of the given objective function.
+   *
+   * Note that this is optional. If only constraints are specified, the solver
+   * will find the closest solution to the initial conditions that's in the
+   * feasible set.
+   *
+   * @param objective The objective function to maximize.
+   */
+  void Maximize(Variable&& objective) {
+    // Maximizing a cost function is the same as minimizing its negative
+    m_f = -std::move(objective);
+    status.costFunctionType = m_f.value().Type();
+  }
+
+  /**
+   * Tells the solver to solve the problem while satisfying the given equality
+   * constraint.
+   *
+   * @param constraint The constraint to satisfy.
+   */
+  void SubjectTo(const EqualityConstraints& constraint) {
+    // Get the highest order equality constraint expression type
+    for (const auto& c : constraint.constraints) {
+      status.equalityConstraintType =
+          std::max(status.equalityConstraintType, c.Type());
+    }
+
+    m_equalityConstraints.reserve(m_equalityConstraints.size() +
+                                  constraint.constraints.size());
+    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
+              std::back_inserter(m_equalityConstraints));
+  }
+
+  /**
+   * Tells the solver to solve the problem while satisfying the given equality
+   * constraint.
+   *
+   * @param constraint The constraint to satisfy.
+   */
+  void SubjectTo(EqualityConstraints&& constraint) {
+    // Get the highest order equality constraint expression type
+    for (const auto& c : constraint.constraints) {
+      status.equalityConstraintType =
+          std::max(status.equalityConstraintType, c.Type());
+    }
+
+    m_equalityConstraints.reserve(m_equalityConstraints.size() +
+                                  constraint.constraints.size());
+    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
+              std::back_inserter(m_equalityConstraints));
+  }
+
+  /**
+   * Tells the solver to solve the problem while satisfying the given inequality
+   * constraint.
+   *
+   * @param constraint The constraint to satisfy.
+   */
+  void SubjectTo(const InequalityConstraints& constraint) {
+    // Get the highest order inequality constraint expression type
+    for (const auto& c : constraint.constraints) {
+      status.inequalityConstraintType =
+          std::max(status.inequalityConstraintType, c.Type());
+    }
+
+    m_inequalityConstraints.reserve(m_inequalityConstraints.size() +
+                                    constraint.constraints.size());
+    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
+              std::back_inserter(m_inequalityConstraints));
+  }
+
+  /**
+   * Tells the solver to solve the problem while satisfying the given inequality
+   * constraint.
+   *
+   * @param constraint The constraint to satisfy.
+   */
+  void SubjectTo(InequalityConstraints&& constraint) {
+    // Get the highest order inequality constraint expression type
+    for (const auto& c : constraint.constraints) {
+      status.inequalityConstraintType =
+          std::max(status.inequalityConstraintType, c.Type());
+    }
+
+    m_inequalityConstraints.reserve(m_inequalityConstraints.size() +
+                                    constraint.constraints.size());
+    std::copy(constraint.constraints.begin(), constraint.constraints.end(),
+              std::back_inserter(m_inequalityConstraints));
+  }
+
+  /**
+   * Solve the optimization problem. The solution will be stored in the original
+   * variables used to construct the problem.
+   *
+   * @param config Configuration options for the solver.
+   */
+  SolverStatus Solve(const SolverConfig& config = kDefaultConfig) {
+    // Create the initial value column vector
+    Eigen::VectorXd x{m_decisionVariables.size()};
+    for (size_t i = 0; i < m_decisionVariables.size(); ++i) {
+      x(i) = m_decisionVariables[i].Value();
+    }
+
+    status.exitCondition = SolverExitCondition::kSuccess;
+
+    // If there's no cost function, make it zero and continue
+    if (!m_f.has_value()) {
+      m_f = Variable();
+    }
+
+    if (config.diagnostics) {
+      constexpr std::array kExprTypeToName{"empty", "constant", "linear",
+                                           "quadratic", "nonlinear"};
+
+      // Print cost function and constraint expression types
+      sleipnir::println(
+          "The cost function is {}.",
+          kExprTypeToName[static_cast<int>(status.costFunctionType)]);
+      sleipnir::println(
+          "The equality constraints are {}.",
+          kExprTypeToName[static_cast<int>(status.equalityConstraintType)]);
+      sleipnir::println(
+          "The inequality constraints are {}.",
+          kExprTypeToName[static_cast<int>(status.inequalityConstraintType)]);
+      sleipnir::println("");
+
+      // Print problem dimensionality
+      sleipnir::println("Number of decision variables: {}",
+                        m_decisionVariables.size());
+      sleipnir::println("Number of equality constraints: {}",
+                        m_equalityConstraints.size());
+      sleipnir::println("Number of inequality constraints: {}\n",
+                        m_inequalityConstraints.size());
+    }
+
+    // If the problem is empty or constant, there's nothing to do
+    if (status.costFunctionType <= ExpressionType::kConstant &&
+        status.equalityConstraintType <= ExpressionType::kConstant &&
+        status.inequalityConstraintType <= ExpressionType::kConstant) {
+      return status;
+    }
+
+    // Solve the optimization problem
+    Eigen::VectorXd s = Eigen::VectorXd::Ones(m_inequalityConstraints.size());
+    InteriorPoint(m_decisionVariables, m_equalityConstraints,
+                  m_inequalityConstraints, m_f.value(), m_callback, config,
+                  false, x, s, &status);
+
+    if (config.diagnostics) {
+      sleipnir::println("Exit condition: {}", ToMessage(status.exitCondition));
+    }
+
+    // Assign the solution to the original Variable instances
+    VariableMatrix{m_decisionVariables}.SetValue(x);
+
+    return status;
+  }
+
+  /**
+   * Sets a callback to be called at each solver iteration.
+   *
+   * The callback for this overload should return void.
+   *
+   * @param callback The callback.
+   */
+  template <typename F>
+    requires std::invocable<F, const SolverIterationInfo&> &&
+             std::same_as<std::invoke_result_t<F, const SolverIterationInfo&>,
+                          void>
+  void Callback(F&& callback) {
+    m_callback = [=, callback = std::forward<F>(callback)](
+                     const SolverIterationInfo& info) {
+      callback(info);
+      return false;
+    };
+  }
+
+  /**
+   * Sets a callback to be called at each solver iteration.
+   *
+   * The callback for this overload should return bool.
+   *
+   * @param callback The callback. Returning true from the callback causes the
+   *   solver to exit early with the solution it has so far.
+   */
+  template <typename F>
+    requires std::invocable<F, const SolverIterationInfo&> &&
+             std::same_as<std::invoke_result_t<F, const SolverIterationInfo&>,
+                          bool>
+  void Callback(F&& callback) {
+    m_callback = std::forward<F>(callback);
+  }
+
+ private:
+  // GCC incorrectly applies C++14 rules for const static data members, so an
+  // initializer is required here.
+  //
+  // https://stackoverflow.com/a/50639754
+  static constexpr SolverConfig kDefaultConfig{};
+
+  // The list of decision variables, which are the root of the problem's
+  // expression tree
+  std::vector<Variable> m_decisionVariables;
+
+  // The cost function: f(x)
+  std::optional<Variable> m_f;
+
+  // The list of equality constraints: cₑ(x) = 0
+  std::vector<Variable> m_equalityConstraints;
+
+  // The list of inequality constraints: cᵢ(x) ≥ 0
+  std::vector<Variable> m_inequalityConstraints;
+
+  // The user callback
+  std::function<bool(const SolverIterationInfo&)> m_callback =
+      [](const SolverIterationInfo&) { return false; };
+
+  // The solver status
+  SolverStatus status;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/SolverConfig.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/SolverConfig.hpp`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <chrono>
-#include <limits>
-
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * Solver configuration.
- */
-struct SLEIPNIR_DLLEXPORT SolverConfig {
-  /// The solver will stop once the error is below this tolerance.
-  double tolerance = 1e-8;
-
-  /// The maximum number of solver iterations before returning a solution.
-  int maxIterations = 5000;
-
-  /// The solver will stop once the error is below this tolerance for
-  /// `acceptableIterations` iterations. This is useful in cases where the
-  /// solver might not be able to achieve the desired level of accuracy due to
-  /// floating-point round-off.
-  double acceptableTolerance = 1e-6;
-
-  /// The solver will stop once the error is below `acceptableTolerance` for
-  /// this many iterations.
-  int maxAcceptableIterations = 15;
-
-  /// The maximum elapsed wall clock time before returning a solution.
-  std::chrono::duration<double> timeout{
-      std::numeric_limits<double>::infinity()};
-
-  /// Enables the feasible interior-point method. When the inequality
-  /// constraints are all feasible, step sizes are reduced when necessary to
-  /// prevent them becoming infeasible again. This is useful when parts of the
-  /// problem are ill-conditioned in infeasible regions (e.g., square root of a
-  /// negative value). This can slow or prevent progress toward a solution
-  /// though, so only enable it if necessary.
-  bool feasibleIPM = false;
-
-  /// Enables diagnostic prints.
-  bool diagnostics = false;
-
-  /// Enables writing sparsity patterns of H, Aₑ, and Aᵢ to files named H.spy,
-  /// A_e.spy, and A_i.spy respectively during solve.
-  ///
-  /// Use tools/spy.py to plot them.
-  bool spy = false;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <chrono>
+#include <limits>
+
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * Solver configuration.
+ */
+struct SLEIPNIR_DLLEXPORT SolverConfig {
+  /// The solver will stop once the error is below this tolerance.
+  double tolerance = 1e-8;
+
+  /// The maximum number of solver iterations before returning a solution.
+  int maxIterations = 5000;
+
+  /// The solver will stop once the error is below this tolerance for
+  /// `acceptableIterations` iterations. This is useful in cases where the
+  /// solver might not be able to achieve the desired level of accuracy due to
+  /// floating-point round-off.
+  double acceptableTolerance = 1e-6;
+
+  /// The solver will stop once the error is below `acceptableTolerance` for
+  /// this many iterations.
+  int maxAcceptableIterations = 15;
+
+  /// The maximum elapsed wall clock time before returning a solution.
+  std::chrono::duration<double> timeout{
+      std::numeric_limits<double>::infinity()};
+
+  /// Enables the feasible interior-point method. When the inequality
+  /// constraints are all feasible, step sizes are reduced when necessary to
+  /// prevent them becoming infeasible again. This is useful when parts of the
+  /// problem are ill-conditioned in infeasible regions (e.g., square root of a
+  /// negative value). This can slow or prevent progress toward a solution
+  /// though, so only enable it if necessary.
+  bool feasibleIPM = false;
+
+  /// Enables diagnostic prints.
+  bool diagnostics = false;
+
+  /// Enables writing sparsity patterns of H, Aₑ, and Aᵢ to files named H.spy,
+  /// A_e.spy, and A_i.spy respectively during solve.
+  ///
+  /// Use tools/spy.py to plot them.
+  bool spy = false;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/SolverExitCondition.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/SolverExitCondition.hpp`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <string_view>
-
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * Solver exit condition.
- */
-enum class SolverExitCondition {
-  /// Solved the problem to the desired tolerance.
-  kSuccess = 0,
-  /// Solved the problem to an acceptable tolerance, but not the desired one.
-  kSolvedToAcceptableTolerance = 1,
-  /// The solver returned its solution so far after the user requested a stop.
-  kCallbackRequestedStop = 2,
-  /// The solver determined the problem to be overconstrained and gave up.
-  kTooFewDOFs = -1,
-  /// The solver determined the problem to be locally infeasible and gave up.
-  kLocallyInfeasible = -2,
-  /// The solver failed to reach the desired tolerance, and feasibility
-  /// restoration failed to converge.
-  kFeasibilityRestorationFailed = -3,
-  /// The solver encountered nonfinite initial cost or constraints and gave up.
-  kNonfiniteInitialCostOrConstraints = -4,
-  /// The solver encountered diverging primal iterates xₖ and/or sₖ and gave up.
-  kDivergingIterates = -5,
-  /// The solver returned its solution so far after exceeding the maximum number
-  /// of iterations.
-  kMaxIterationsExceeded = -6,
-  /// The solver returned its solution so far after exceeding the maximum
-  /// elapsed wall clock time.
-  kTimeout = -7
-};
-
-/**
- * Returns user-readable message corresponding to the exit condition.
- *
- * @param exitCondition Solver exit condition.
- */
-SLEIPNIR_DLLEXPORT constexpr std::string_view ToMessage(
-    const SolverExitCondition& exitCondition) {
-  using enum SolverExitCondition;
-
-  switch (exitCondition) {
-    case kSuccess:
-      return "solved to desired tolerance";
-    case kSolvedToAcceptableTolerance:
-      return "solved to acceptable tolerance";
-    case kCallbackRequestedStop:
-      return "callback requested stop";
-    case kTooFewDOFs:
-      return "problem has too few degrees of freedom";
-    case kLocallyInfeasible:
-      return "problem is locally infeasible";
-    case kFeasibilityRestorationFailed:
-      return "solver failed to reach the desired tolerance, and feasibility "
-             "restoration failed to converge";
-    case kNonfiniteInitialCostOrConstraints:
-      return "solver encountered nonfinite initial cost or constraints and "
-             "gave up";
-    case kDivergingIterates:
-      return "solver encountered diverging primal iterates xₖ and/or sₖ and "
-             "gave up";
-    case kMaxIterationsExceeded:
-      return "solution returned after maximum iterations exceeded";
-    case kTimeout:
-      return "solution returned after maximum wall clock time exceeded";
-    default:
-      return "unknown";
-  }
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <string_view>
+
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * Solver exit condition.
+ */
+enum class SolverExitCondition {
+  /// Solved the problem to the desired tolerance.
+  kSuccess = 0,
+  /// Solved the problem to an acceptable tolerance, but not the desired one.
+  kSolvedToAcceptableTolerance = 1,
+  /// The solver returned its solution so far after the user requested a stop.
+  kCallbackRequestedStop = 2,
+  /// The solver determined the problem to be overconstrained and gave up.
+  kTooFewDOFs = -1,
+  /// The solver determined the problem to be locally infeasible and gave up.
+  kLocallyInfeasible = -2,
+  /// The solver failed to reach the desired tolerance, and feasibility
+  /// restoration failed to converge.
+  kFeasibilityRestorationFailed = -3,
+  /// The solver encountered nonfinite initial cost or constraints and gave up.
+  kNonfiniteInitialCostOrConstraints = -4,
+  /// The solver encountered diverging primal iterates xₖ and/or sₖ and gave up.
+  kDivergingIterates = -5,
+  /// The solver returned its solution so far after exceeding the maximum number
+  /// of iterations.
+  kMaxIterationsExceeded = -6,
+  /// The solver returned its solution so far after exceeding the maximum
+  /// elapsed wall clock time.
+  kTimeout = -7
+};
+
+/**
+ * Returns user-readable message corresponding to the exit condition.
+ *
+ * @param exitCondition Solver exit condition.
+ */
+SLEIPNIR_DLLEXPORT constexpr std::string_view ToMessage(
+    const SolverExitCondition& exitCondition) {
+  using enum SolverExitCondition;
+
+  switch (exitCondition) {
+    case kSuccess:
+      return "solved to desired tolerance";
+    case kSolvedToAcceptableTolerance:
+      return "solved to acceptable tolerance";
+    case kCallbackRequestedStop:
+      return "callback requested stop";
+    case kTooFewDOFs:
+      return "problem has too few degrees of freedom";
+    case kLocallyInfeasible:
+      return "problem is locally infeasible";
+    case kFeasibilityRestorationFailed:
+      return "solver failed to reach the desired tolerance, and feasibility "
+             "restoration failed to converge";
+    case kNonfiniteInitialCostOrConstraints:
+      return "solver encountered nonfinite initial cost or constraints and "
+             "gave up";
+    case kDivergingIterates:
+      return "solver encountered diverging primal iterates xₖ and/or sₖ and "
+             "gave up";
+    case kMaxIterationsExceeded:
+      return "solution returned after maximum iterations exceeded";
+    case kTimeout:
+      return "solution returned after maximum wall clock time exceeded";
+    default:
+      return "unknown";
+  }
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/SolverStatus.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/SolverStatus.hpp`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include "sleipnir/autodiff/ExpressionType.hpp"
-#include "sleipnir/optimization/SolverExitCondition.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * Return value of OptimizationProblem::Solve() containing the cost function and
- * constraint types and solver's exit condition.
- */
-struct SLEIPNIR_DLLEXPORT SolverStatus {
-  /// The cost function type detected by the solver.
-  ExpressionType costFunctionType = ExpressionType::kNone;
-
-  /// The equality constraint type detected by the solver.
-  ExpressionType equalityConstraintType = ExpressionType::kNone;
-
-  /// The inequality constraint type detected by the solver.
-  ExpressionType inequalityConstraintType = ExpressionType::kNone;
-
-  /// The solver's exit condition.
-  SolverExitCondition exitCondition = SolverExitCondition::kSuccess;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include "sleipnir/autodiff/ExpressionType.hpp"
+#include "sleipnir/optimization/SolverExitCondition.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * Return value of OptimizationProblem::Solve() containing the cost function and
+ * constraint types and solver's exit condition.
+ */
+struct SLEIPNIR_DLLEXPORT SolverStatus {
+  /// The cost function type detected by the solver.
+  ExpressionType costFunctionType = ExpressionType::kNone;
+
+  /// The equality constraint type detected by the solver.
+  ExpressionType equalityConstraintType = ExpressionType::kNone;
+
+  /// The inequality constraint type detected by the solver.
+  ExpressionType inequalityConstraintType = ExpressionType::kNone;
+
+  /// The solver's exit condition.
+  SolverExitCondition exitCondition = SolverExitCondition::kSuccess;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/optimization/solver/InteriorPoint.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/optimization/solver/InteriorPoint.hpp`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <functional>
-#include <span>
-
-#include <Eigen/Core>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/optimization/SolverConfig.hpp"
-#include "sleipnir/optimization/SolverIterationInfo.hpp"
-#include "sleipnir/optimization/SolverStatus.hpp"
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
-Finds the optimal solution to a nonlinear program using the interior-point
-method.
-
-A nonlinear program has the form:
-
-@verbatim
-     min_x f(x)
-subject to cₑ(x) = 0
-           cᵢ(x) ≥ 0
-@endverbatim
-
-where f(x) is the cost function, cₑ(x) are the equality constraints, and cᵢ(x)
-are the inequality constraints.
-
-@param[in] decisionVariables The list of decision variables.
-@param[in] equalityConstraints The list of equality constraints.
-@param[in] inequalityConstraints The list of inequality constraints.
-@param[in] f The cost function.
-@param[in] callback The user callback.
-@param[in] config Configuration options for the solver.
-@param[in] feasibilityRestoration Whether to use feasibility restoration instead
-  of the normal algorithm.
-@param[in,out] x The initial guess and output location for the decision
-  variables.
-@param[in,out] s The initial guess and output location for the inequality
-  constraint slack variables.
-@param[out] status The solver status.
-*/
-SLEIPNIR_DLLEXPORT void InteriorPoint(
-    std::span<Variable> decisionVariables,
-    std::span<Variable> equalityConstraints,
-    std::span<Variable> inequalityConstraints, Variable& f,
-    const std::function<bool(const SolverIterationInfo&)>& callback,
-    const SolverConfig& config, bool feasibilityRestoration, Eigen::VectorXd& x,
-    Eigen::VectorXd& s, SolverStatus* status);
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <functional>
+#include <span>
+
+#include <Eigen/Core>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/optimization/SolverConfig.hpp"
+#include "sleipnir/optimization/SolverIterationInfo.hpp"
+#include "sleipnir/optimization/SolverStatus.hpp"
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+Finds the optimal solution to a nonlinear program using the interior-point
+method.
+
+A nonlinear program has the form:
+
+@verbatim
+     min_x f(x)
+subject to cₑ(x) = 0
+           cᵢ(x) ≥ 0
+@endverbatim
+
+where f(x) is the cost function, cₑ(x) are the equality constraints, and cᵢ(x)
+are the inequality constraints.
+
+@param[in] decisionVariables The list of decision variables.
+@param[in] equalityConstraints The list of equality constraints.
+@param[in] inequalityConstraints The list of inequality constraints.
+@param[in] f The cost function.
+@param[in] callback The user callback.
+@param[in] config Configuration options for the solver.
+@param[in] feasibilityRestoration Whether to use feasibility restoration instead
+  of the normal algorithm.
+@param[in,out] x The initial guess and output location for the decision
+  variables.
+@param[in,out] s The initial guess and output location for the inequality
+  constraint slack variables.
+@param[out] status The solver status.
+*/
+SLEIPNIR_DLLEXPORT void InteriorPoint(
+    std::span<Variable> decisionVariables,
+    std::span<Variable> equalityConstraints,
+    std::span<Variable> inequalityConstraints, Variable& f,
+    const std::function<bool(const SolverIterationInfo&)>& callback,
+    const SolverConfig& config, bool feasibilityRestoration, Eigen::VectorXd& x,
+    Eigen::VectorXd& s, SolverStatus* status);
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Assert.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Assert.hpp`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#ifdef JORMUNGANDR
-#include <stdexcept>
-
-#include <fmt/format.h>
-/**
- * Throw an exception in Python.
- */
-#define Assert(condition)                                                      \
-  do {                                                                         \
-    if (!(condition)) {                                                        \
-      throw std::invalid_argument(                                             \
-          fmt::format("{}:{}: {}: Assertion `{}' failed.", __FILE__, __LINE__, \
-                      __func__, #condition));                                  \
-    }                                                                          \
-  } while (0);
-#else
-#include <cassert>
-/**
- * Abort in C++.
- */
-#define Assert(condition) assert(condition)
-#endif
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#ifdef JORMUNGANDR
+#include <stdexcept>
+
+#include <fmt/format.h>
+/**
+ * Throw an exception in Python.
+ */
+#define Assert(condition)                                                      \
+  do {                                                                         \
+    if (!(condition)) {                                                        \
+      throw std::invalid_argument(                                             \
+          fmt::format("{}:{}: {}: Assertion `{}' failed.", __FILE__, __LINE__, \
+                      __func__, #condition));                                  \
+    }                                                                          \
+  } while (0);
+#else
+#include <cassert>
+/**
+ * Abort in C++.
+ */
+#define Assert(condition) assert(condition)
+#endif
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Concepts.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Concepts.hpp`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <concepts>
-
-#include <Eigen/Core>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/autodiff/VariableMatrix.hpp"
-
-namespace sleipnir {
-
-template <typename T>
-concept ScalarLike = std::same_as<T, double> || std::same_as<T, int> ||
-                     std::same_as<T, Variable>;
-
-template <typename Derived>
-concept EigenMatrixLike =
-    std::derived_from<Derived, Eigen::MatrixBase<Derived>>;
-
-template <typename T>
-concept EigenSolver = requires(T t) { t.solve(Eigen::VectorXd{}); };
-
-template <typename T>
-concept MatrixLike =
-    std::same_as<T, VariableMatrix> ||
-    std::same_as<T, VariableBlock<VariableMatrix>> || EigenMatrixLike<T>;
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <concepts>
+
+#include <Eigen/Core>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/autodiff/VariableMatrix.hpp"
+
+namespace sleipnir {
+
+template <typename T>
+concept ScalarLike = std::same_as<T, double> || std::same_as<T, int> ||
+                     std::same_as<T, Variable>;
+
+template <typename Derived>
+concept EigenMatrixLike =
+    std::derived_from<Derived, Eigen::MatrixBase<Derived>>;
+
+template <typename T>
+concept EigenSolver = requires(T t) { t.solve(Eigen::VectorXd{}); };
+
+template <typename T>
+concept MatrixLike =
+    std::same_as<T, VariableMatrix> ||
+    std::same_as<T, VariableBlock<VariableMatrix>> || EigenMatrixLike<T>;
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Formatters.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Formatters.hpp`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <concepts>
-
-#include <Eigen/Core>
-#include <Eigen/SparseCore>
-#include <fmt/format.h>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/autodiff/VariableBlock.hpp"
-#include "sleipnir/autodiff/VariableMatrix.hpp"
-
-// FIXME: Doxygen gives internal inconsistency errors:
-//   scope for class sleipnir::fmt::formatter< Derived, CharT > not found!
-//   scope for class sleipnir::fmt::formatter< sleipnir::Variable > not found!
-//   scope for class sleipnir::fmt::formatter< T > not found!
-
-//! @cond Doxygen_Suppress
-
-/**
- * Formatter for classes derived from Eigen::DenseBase<Derived> or
- * Eigen::SparseCompressedBase<Derived>.
- */
-template <typename Derived, typename CharT>
-  requires std::derived_from<Derived, Eigen::DenseBase<Derived>> ||
-           std::derived_from<Derived, Eigen::SparseCompressedBase<Derived>>
-struct fmt::formatter<Derived, CharT> {
-  constexpr auto parse(fmt::format_parse_context& ctx) {
-    return m_underlying.parse(ctx);
-  }
-
-  auto format(const Derived& mat, fmt::format_context& ctx) const {
-    auto out = ctx.out();
-
-    for (int row = 0; row < mat.rows(); ++row) {
-      for (int col = 0; col < mat.cols(); ++col) {
-        out = fmt::format_to(out, "  ");
-        out = m_underlying.format(mat.coeff(row, col), ctx);
-      }
-
-      if (row < mat.rows() - 1) {
-        out = fmt::format_to(out, "\n");
-      }
-    }
-
-    return out;
-  }
-
- private:
-  fmt::formatter<typename Derived::Scalar, CharT> m_underlying;
-};
-
-/**
- * Formatter for sleipnir::Variable.
- */
-template <>
-struct fmt::formatter<sleipnir::Variable> {
-  constexpr auto parse(fmt::format_parse_context& ctx) {
-    return m_underlying.parse(ctx);
-  }
-
-  auto format(const sleipnir::Variable& variable,
-              fmt::format_context& ctx) const {
-    return m_underlying.format(variable.Value(), ctx);
-  }
-
- private:
-  fmt::formatter<double> m_underlying;
-};
-
-/**
- * Formatter for sleipnir::VariableBlock or sleipnir::VariableMatrix.
- */
-template <typename T>
-  requires std::same_as<T, sleipnir::VariableBlock<sleipnir::VariableMatrix>> ||
-           std::same_as<T, sleipnir::VariableMatrix>
-struct fmt::formatter<T> {
-  constexpr auto parse(fmt::format_parse_context& ctx) {
-    return m_underlying.parse(ctx);
-  }
-
-  auto format(const T& mat, fmt::format_context& ctx) const {
-    auto out = ctx.out();
-
-    for (int row = 0; row < mat.Rows(); ++row) {
-      for (int col = 0; col < mat.Cols(); ++col) {
-        out = fmt::format_to(out, "  ");
-        out = m_underlying.format(mat(row, col).Value(), ctx);
-      }
-
-      if (row < mat.Rows() - 1) {
-        out = fmt::format_to(out, "\n");
-      }
-    }
-
-    return out;
-  }
-
- private:
-  fmt::formatter<double> m_underlying;
-};
-
-//! @endcond
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <concepts>
+
+#include <Eigen/Core>
+#include <Eigen/SparseCore>
+#include <fmt/format.h>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/autodiff/VariableBlock.hpp"
+#include "sleipnir/autodiff/VariableMatrix.hpp"
+
+// FIXME: Doxygen gives internal inconsistency errors:
+//   scope for class sleipnir::fmt::formatter< Derived, CharT > not found!
+//   scope for class sleipnir::fmt::formatter< sleipnir::Variable > not found!
+//   scope for class sleipnir::fmt::formatter< T > not found!
+
+//! @cond Doxygen_Suppress
+
+/**
+ * Formatter for classes derived from Eigen::DenseBase<Derived> or
+ * Eigen::SparseCompressedBase<Derived>.
+ */
+template <typename Derived, typename CharT>
+  requires std::derived_from<Derived, Eigen::DenseBase<Derived>> ||
+           std::derived_from<Derived, Eigen::SparseCompressedBase<Derived>>
+struct fmt::formatter<Derived, CharT> {
+  constexpr auto parse(fmt::format_parse_context& ctx) {
+    return m_underlying.parse(ctx);
+  }
+
+  auto format(const Derived& mat, fmt::format_context& ctx) const {
+    auto out = ctx.out();
+
+    for (int row = 0; row < mat.rows(); ++row) {
+      for (int col = 0; col < mat.cols(); ++col) {
+        out = fmt::format_to(out, "  ");
+        out = m_underlying.format(mat.coeff(row, col), ctx);
+      }
+
+      if (row < mat.rows() - 1) {
+        out = fmt::format_to(out, "\n");
+      }
+    }
+
+    return out;
+  }
+
+ private:
+  fmt::formatter<typename Derived::Scalar, CharT> m_underlying;
+};
+
+/**
+ * Formatter for sleipnir::Variable.
+ */
+template <>
+struct fmt::formatter<sleipnir::Variable> {
+  constexpr auto parse(fmt::format_parse_context& ctx) {
+    return m_underlying.parse(ctx);
+  }
+
+  auto format(const sleipnir::Variable& variable,
+              fmt::format_context& ctx) const {
+    return m_underlying.format(variable.Value(), ctx);
+  }
+
+ private:
+  fmt::formatter<double> m_underlying;
+};
+
+/**
+ * Formatter for sleipnir::VariableBlock or sleipnir::VariableMatrix.
+ */
+template <typename T>
+  requires std::same_as<T, sleipnir::VariableBlock<sleipnir::VariableMatrix>> ||
+           std::same_as<T, sleipnir::VariableMatrix>
+struct fmt::formatter<T> {
+  constexpr auto parse(fmt::format_parse_context& ctx) {
+    return m_underlying.parse(ctx);
+  }
+
+  auto format(const T& mat, fmt::format_context& ctx) const {
+    auto out = ctx.out();
+
+    for (int row = 0; row < mat.Rows(); ++row) {
+      for (int col = 0; col < mat.Cols(); ++col) {
+        out = fmt::format_to(out, "  ");
+        out = m_underlying.format(mat(row, col).Value(), ctx);
+      }
+
+      if (row < mat.Rows() - 1) {
+        out = fmt::format_to(out, "\n");
+      }
+    }
+
+    return out;
+  }
+
+ private:
+  fmt::formatter<double> m_underlying;
+};
+
+//! @endcond
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/IntrusiveSharedPtr.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/IntrusiveSharedPtr.hpp`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <cstddef>
-#include <memory>
-#include <utility>
-
-namespace sleipnir {
-
-/**
- * A custom intrusive shared pointer implementation without thread
- * synchronization overhead.
- *
- * Types used with this class should have three things:
- *
- * 1. A zero-initialized public counter variable that serves as the shared
- *    pointer's reference count.
- * 2. A free function `void IntrusiveSharedPtrIncRefCount(T*)` that increments
- *    the reference count.
- * 3. A free function `void IntrusiveSharedPtrDecRefCount(T*)` that decrements
- *    the reference count and deallocates the pointed to object if the reference
- *    count reaches zero.
- *
- * @tparam T The type of the object to be reference counted.
- */
-template <typename T>
-class IntrusiveSharedPtr {
- public:
-  /**
-   * Constructs an empty intrusive shared pointer.
-   */
-  constexpr IntrusiveSharedPtr() noexcept = default;
-
-  /**
-   * Constructs an empty intrusive shared pointer.
-   */
-  constexpr IntrusiveSharedPtr(std::nullptr_t) noexcept {}  // NOLINT
-
-  /**
-   * Constructs an intrusive shared pointer from the given pointer and takes
-   * ownership.
-   */
-  explicit constexpr IntrusiveSharedPtr(T* ptr) noexcept : m_ptr{ptr} {
-    if (m_ptr != nullptr) {
-      IntrusiveSharedPtrIncRefCount(m_ptr);
-    }
-  }
-
-  constexpr ~IntrusiveSharedPtr() {
-    if (m_ptr != nullptr) {
-      IntrusiveSharedPtrDecRefCount(m_ptr);
-    }
-  }
-
-  /**
-   * Copy constructs from the given intrusive shared pointer.
-   */
-  constexpr IntrusiveSharedPtr(const IntrusiveSharedPtr<T>& rhs) noexcept
-      : m_ptr{rhs.m_ptr} {
-    if (m_ptr != nullptr) {
-      IntrusiveSharedPtrIncRefCount(m_ptr);
-    }
-  }
-
-  /**
-   * Makes a copy of the given intrusive shared pointer.
-   */
-  constexpr IntrusiveSharedPtr<T>& operator=(  // NOLINT
-      const IntrusiveSharedPtr<T>& rhs) noexcept {
-    if (m_ptr == rhs.m_ptr) {
-      return *this;
-    }
-
-    if (m_ptr != nullptr) {
-      IntrusiveSharedPtrDecRefCount(m_ptr);
-    }
-
-    m_ptr = rhs.m_ptr;
-
-    if (m_ptr != nullptr) {
-      IntrusiveSharedPtrIncRefCount(m_ptr);
-    }
-
-    return *this;
-  }
-
-  /**
-   * Move constructs from the given intrusive shared pointer.
-   */
-  constexpr IntrusiveSharedPtr(IntrusiveSharedPtr<T>&& rhs) noexcept
-      : m_ptr{std::exchange(rhs.m_ptr, nullptr)} {}
-
-  /**
-   * Move assigns from the given intrusive shared pointer.
-   */
-  constexpr IntrusiveSharedPtr<T>& operator=(
-      IntrusiveSharedPtr<T>&& rhs) noexcept {
-    if (m_ptr == rhs.m_ptr) {
-      return *this;
-    }
-
-    std::swap(m_ptr, rhs.m_ptr);
-
-    return *this;
-  }
-
-  /**
-   * Returns the internal pointer.
-   */
-  constexpr T* Get() const noexcept { return m_ptr; }
-
-  /**
-   * Returns the object pointed to by the internal pointer.
-   */
-  constexpr T& operator*() const noexcept { return *m_ptr; }
-
-  /**
-   * Returns the internal pointer.
-   */
-  constexpr T* operator->() const noexcept { return m_ptr; }
-
-  /**
-   * Returns true if the internal pointer isn't nullptr.
-   */
-  explicit constexpr operator bool() const noexcept { return m_ptr != nullptr; }
-
-  /**
-   * Returns true if the given intrusive shared pointers point to the same
-   * object.
-   */
-  friend constexpr bool operator==(const IntrusiveSharedPtr<T>& lhs,
-                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
-    return lhs.m_ptr == rhs.m_ptr;
-  }
-
-  /**
-   * Returns true if the given intrusive shared pointers point to different
-   * objects.
-   */
-  friend constexpr bool operator!=(const IntrusiveSharedPtr<T>& lhs,
-                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
-    return lhs.m_ptr != rhs.m_ptr;
-  }
-
-  /**
-   * Returns true if the left-hand intrusive shared pointer points to nullptr.
-   */
-  friend constexpr bool operator==(const IntrusiveSharedPtr<T>& lhs,
-                                   std::nullptr_t) noexcept {
-    return lhs.m_ptr == nullptr;
-  }
-
-  /**
-   * Returns true if the right-hand intrusive shared pointer points to nullptr.
-   */
-  friend constexpr bool operator==(std::nullptr_t,
-                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
-    return nullptr == rhs.m_ptr;
-  }
-
-  /**
-   * Returns true if the left-hand intrusive shared pointer doesn't point to
-   * nullptr.
-   */
-  friend constexpr bool operator!=(const IntrusiveSharedPtr<T>& lhs,
-                                   std::nullptr_t) noexcept {
-    return lhs.m_ptr != nullptr;
-  }
-
-  /**
-   * Returns true if the right-hand intrusive shared pointer doesn't point to
-   * nullptr.
-   */
-  friend constexpr bool operator!=(std::nullptr_t,
-                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
-    return nullptr != rhs.m_ptr;
-  }
-
- private:
-  T* m_ptr = nullptr;
-};
-
-/**
- * Constructs an object of type T and wraps it in an intrusive shared pointer
- * using args as the parameter list for the constructor of T.
- *
- * @tparam T Type of object for intrusive shared pointer.
- * @tparam Args Types of constructor arguments.
- * @param args Constructor arguments for T.
- */
-template <typename T, typename... Args>
-IntrusiveSharedPtr<T> MakeIntrusiveShared(Args&&... args) {
-  return IntrusiveSharedPtr<T>{new T(std::forward<Args>(args)...)};
-}
-
-/**
- * Constructs an object of type T and wraps it in an intrusive shared pointer
- * using alloc as the storage allocator of T and args as the parameter list for
- * the constructor of T.
- *
- * @tparam T Type of object for intrusive shared pointer.
- * @tparam Alloc Type of allocator for T.
- * @tparam Args Types of constructor arguments.
- * @param alloc The allocator for T.
- * @param args Constructor arguments for T.
- */
-template <typename T, typename Alloc, typename... Args>
-IntrusiveSharedPtr<T> AllocateIntrusiveShared(Alloc alloc, Args&&... args) {
-  auto ptr = std::allocator_traits<Alloc>::allocate(alloc, sizeof(T));
-  std::allocator_traits<Alloc>::construct(alloc, ptr,
-                                          std::forward<Args>(args)...);
-  return IntrusiveSharedPtr<T>{ptr};
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <cstddef>
+#include <memory>
+#include <utility>
+
+namespace sleipnir {
+
+/**
+ * A custom intrusive shared pointer implementation without thread
+ * synchronization overhead.
+ *
+ * Types used with this class should have three things:
+ *
+ * 1. A zero-initialized public counter variable that serves as the shared
+ *    pointer's reference count.
+ * 2. A free function `void IntrusiveSharedPtrIncRefCount(T*)` that increments
+ *    the reference count.
+ * 3. A free function `void IntrusiveSharedPtrDecRefCount(T*)` that decrements
+ *    the reference count and deallocates the pointed to object if the reference
+ *    count reaches zero.
+ *
+ * @tparam T The type of the object to be reference counted.
+ */
+template <typename T>
+class IntrusiveSharedPtr {
+ public:
+  /**
+   * Constructs an empty intrusive shared pointer.
+   */
+  constexpr IntrusiveSharedPtr() noexcept = default;
+
+  /**
+   * Constructs an empty intrusive shared pointer.
+   */
+  constexpr IntrusiveSharedPtr(std::nullptr_t) noexcept {}  // NOLINT
+
+  /**
+   * Constructs an intrusive shared pointer from the given pointer and takes
+   * ownership.
+   */
+  explicit constexpr IntrusiveSharedPtr(T* ptr) noexcept : m_ptr{ptr} {
+    if (m_ptr != nullptr) {
+      IntrusiveSharedPtrIncRefCount(m_ptr);
+    }
+  }
+
+  constexpr ~IntrusiveSharedPtr() {
+    if (m_ptr != nullptr) {
+      IntrusiveSharedPtrDecRefCount(m_ptr);
+    }
+  }
+
+  /**
+   * Copy constructs from the given intrusive shared pointer.
+   */
+  constexpr IntrusiveSharedPtr(const IntrusiveSharedPtr<T>& rhs) noexcept
+      : m_ptr{rhs.m_ptr} {
+    if (m_ptr != nullptr) {
+      IntrusiveSharedPtrIncRefCount(m_ptr);
+    }
+  }
+
+  /**
+   * Makes a copy of the given intrusive shared pointer.
+   */
+  constexpr IntrusiveSharedPtr<T>& operator=(  // NOLINT
+      const IntrusiveSharedPtr<T>& rhs) noexcept {
+    if (m_ptr == rhs.m_ptr) {
+      return *this;
+    }
+
+    if (m_ptr != nullptr) {
+      IntrusiveSharedPtrDecRefCount(m_ptr);
+    }
+
+    m_ptr = rhs.m_ptr;
+
+    if (m_ptr != nullptr) {
+      IntrusiveSharedPtrIncRefCount(m_ptr);
+    }
+
+    return *this;
+  }
+
+  /**
+   * Move constructs from the given intrusive shared pointer.
+   */
+  constexpr IntrusiveSharedPtr(IntrusiveSharedPtr<T>&& rhs) noexcept
+      : m_ptr{std::exchange(rhs.m_ptr, nullptr)} {}
+
+  /**
+   * Move assigns from the given intrusive shared pointer.
+   */
+  constexpr IntrusiveSharedPtr<T>& operator=(
+      IntrusiveSharedPtr<T>&& rhs) noexcept {
+    if (m_ptr == rhs.m_ptr) {
+      return *this;
+    }
+
+    std::swap(m_ptr, rhs.m_ptr);
+
+    return *this;
+  }
+
+  /**
+   * Returns the internal pointer.
+   */
+  constexpr T* Get() const noexcept { return m_ptr; }
+
+  /**
+   * Returns the object pointed to by the internal pointer.
+   */
+  constexpr T& operator*() const noexcept { return *m_ptr; }
+
+  /**
+   * Returns the internal pointer.
+   */
+  constexpr T* operator->() const noexcept { return m_ptr; }
+
+  /**
+   * Returns true if the internal pointer isn't nullptr.
+   */
+  explicit constexpr operator bool() const noexcept { return m_ptr != nullptr; }
+
+  /**
+   * Returns true if the given intrusive shared pointers point to the same
+   * object.
+   */
+  friend constexpr bool operator==(const IntrusiveSharedPtr<T>& lhs,
+                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
+    return lhs.m_ptr == rhs.m_ptr;
+  }
+
+  /**
+   * Returns true if the given intrusive shared pointers point to different
+   * objects.
+   */
+  friend constexpr bool operator!=(const IntrusiveSharedPtr<T>& lhs,
+                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
+    return lhs.m_ptr != rhs.m_ptr;
+  }
+
+  /**
+   * Returns true if the left-hand intrusive shared pointer points to nullptr.
+   */
+  friend constexpr bool operator==(const IntrusiveSharedPtr<T>& lhs,
+                                   std::nullptr_t) noexcept {
+    return lhs.m_ptr == nullptr;
+  }
+
+  /**
+   * Returns true if the right-hand intrusive shared pointer points to nullptr.
+   */
+  friend constexpr bool operator==(std::nullptr_t,
+                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
+    return nullptr == rhs.m_ptr;
+  }
+
+  /**
+   * Returns true if the left-hand intrusive shared pointer doesn't point to
+   * nullptr.
+   */
+  friend constexpr bool operator!=(const IntrusiveSharedPtr<T>& lhs,
+                                   std::nullptr_t) noexcept {
+    return lhs.m_ptr != nullptr;
+  }
+
+  /**
+   * Returns true if the right-hand intrusive shared pointer doesn't point to
+   * nullptr.
+   */
+  friend constexpr bool operator!=(std::nullptr_t,
+                                   const IntrusiveSharedPtr<T>& rhs) noexcept {
+    return nullptr != rhs.m_ptr;
+  }
+
+ private:
+  T* m_ptr = nullptr;
+};
+
+/**
+ * Constructs an object of type T and wraps it in an intrusive shared pointer
+ * using args as the parameter list for the constructor of T.
+ *
+ * @tparam T Type of object for intrusive shared pointer.
+ * @tparam Args Types of constructor arguments.
+ * @param args Constructor arguments for T.
+ */
+template <typename T, typename... Args>
+IntrusiveSharedPtr<T> MakeIntrusiveShared(Args&&... args) {
+  return IntrusiveSharedPtr<T>{new T(std::forward<Args>(args)...)};
+}
+
+/**
+ * Constructs an object of type T and wraps it in an intrusive shared pointer
+ * using alloc as the storage allocator of T and args as the parameter list for
+ * the constructor of T.
+ *
+ * @tparam T Type of object for intrusive shared pointer.
+ * @tparam Alloc Type of allocator for T.
+ * @tparam Args Types of constructor arguments.
+ * @param alloc The allocator for T.
+ * @param args Constructor arguments for T.
+ */
+template <typename T, typename Alloc, typename... Args>
+IntrusiveSharedPtr<T> AllocateIntrusiveShared(Alloc alloc, Args&&... args) {
+  auto ptr = std::allocator_traits<Alloc>::allocate(alloc, sizeof(T));
+  std::allocator_traits<Alloc>::construct(alloc, ptr,
+                                          std::forward<Args>(args)...);
+  return IntrusiveSharedPtr<T>{ptr};
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Print.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Print.hpp`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <system_error>
-#include <utility>
-
-#include <fmt/core.h>
-
-namespace sleipnir {
-
-/**
- * Wrapper around fmt::print() that squelches write failure exceptions.
- */
-template <typename... T>
-inline void print(fmt::format_string<T...> fmt, T&&... args) {
-  try {
-    fmt::print(fmt, std::forward<T>(args)...);
-  } catch (const std::system_error&) {
-  }
-}
-
-/**
- * Wrapper around fmt::print() that squelches write failure exceptions.
- */
-template <typename... T>
-inline void print(std::FILE* f, fmt::format_string<T...> fmt, T&&... args) {
-  try {
-    fmt::print(f, fmt, std::forward<T>(args)...);
-  } catch (const std::system_error&) {
-  }
-}
-
-/**
- * Wrapper around fmt::println() that squelches write failure exceptions.
- */
-template <typename... T>
-inline void println(fmt::format_string<T...> fmt, T&&... args) {
-  try {
-    fmt::println(fmt, std::forward<T>(args)...);
-  } catch (const std::system_error&) {
-  }
-}
-
-/**
- * Wrapper around fmt::println() that squelches write failure exceptions.
- */
-template <typename... T>
-inline void println(std::FILE* f, fmt::format_string<T...> fmt, T&&... args) {
-  try {
-    fmt::println(f, fmt, std::forward<T>(args)...);
-  } catch (const std::system_error&) {
-  }
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <system_error>
+#include <utility>
+
+#include <fmt/core.h>
+
+namespace sleipnir {
+
+/**
+ * Wrapper around fmt::print() that squelches write failure exceptions.
+ */
+template <typename... T>
+inline void print(fmt::format_string<T...> fmt, T&&... args) {
+  try {
+    fmt::print(fmt, std::forward<T>(args)...);
+  } catch (const std::system_error&) {
+  }
+}
+
+/**
+ * Wrapper around fmt::print() that squelches write failure exceptions.
+ */
+template <typename... T>
+inline void print(std::FILE* f, fmt::format_string<T...> fmt, T&&... args) {
+  try {
+    fmt::print(f, fmt, std::forward<T>(args)...);
+  } catch (const std::system_error&) {
+  }
+}
+
+/**
+ * Wrapper around fmt::println() that squelches write failure exceptions.
+ */
+template <typename... T>
+inline void println(fmt::format_string<T...> fmt, T&&... args) {
+  try {
+    fmt::println(fmt, std::forward<T>(args)...);
+  } catch (const std::system_error&) {
+  }
+}
+
+/**
+ * Wrapper around fmt::println() that squelches write failure exceptions.
+ */
+template <typename... T>
+inline void println(std::FILE* f, fmt::format_string<T...> fmt, T&&... args) {
+  try {
+    fmt::println(f, fmt, std::forward<T>(args)...);
+  } catch (const std::system_error&) {
+  }
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/Spy.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/Spy.hpp`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <fstream>
-#include <string>
-#include <string_view>
-#include <vector>
-
-#include <Eigen/SparseCore>
-
-#include "sleipnir/util/SymbolExports.hpp"
-
-namespace sleipnir {
-
-/**
- * Write the sparsity pattern of a sparse matrix to a file.
- *
- * Each character represents an element with '.' representing zero, '+'
- * representing positive, and '-' representing negative. Here's an example for a
- * 3x3 identity matrix.
- *
- * "+.."
- * ".+."
- * "..+"
- *
- * @param[out] file A file stream.
- * @param[in] mat The sparse matrix.
- */
-SLEIPNIR_DLLEXPORT inline void Spy(std::ostream& file,
-                                   const Eigen::SparseMatrix<double>& mat) {
-  const int cells_width = mat.cols() + 1;
-  const int cells_height = mat.rows();
-
-  std::vector<uint8_t> cells;
-
-  // Allocate space for matrix of characters plus trailing newlines
-  cells.reserve(cells_width * cells_height);
-
-  // Initialize cell array
-  for (int row = 0; row < mat.rows(); ++row) {
-    for (int col = 0; col < mat.cols(); ++col) {
-      cells.emplace_back('.');
-    }
-    cells.emplace_back('\n');
-  }
-
-  // Fill in non-sparse entries
-  for (int k = 0; k < mat.outerSize(); ++k) {
-    for (Eigen::SparseMatrix<double>::InnerIterator it{mat, k}; it; ++it) {
-      if (it.value() < 0.0) {
-        cells[it.row() * cells_width + it.col()] = '-';
-      } else if (it.value() > 0.0) {
-        cells[it.row() * cells_width + it.col()] = '+';
-      }
-    }
-  }
-
-  // Write cell array to file
-  for (const auto& c : cells) {
-    file << c;
-  }
-}
-
-/**
- * Write the sparsity pattern of a sparse matrix to a file.
- *
- * Each character represents an element with "." representing zero, "+"
- * representing positive, and "-" representing negative. Here's an example for a
- * 3x3 identity matrix.
- *
- * "+.."
- * ".+."
- * "..+"
- *
- * @param[in] filename The filename.
- * @param[in] mat The sparse matrix.
- */
-SLEIPNIR_DLLEXPORT inline void Spy(std::string_view filename,
-                                   const Eigen::SparseMatrix<double>& mat) {
-  std::ofstream file{std::string{filename}};
-  if (!file.is_open()) {
-    return;
-  }
-
-  Spy(file, mat);
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <fstream>
+#include <string>
+#include <string_view>
+#include <vector>
+
+#include <Eigen/SparseCore>
+
+#include "sleipnir/util/SymbolExports.hpp"
+
+namespace sleipnir {
+
+/**
+ * Write the sparsity pattern of a sparse matrix to a file.
+ *
+ * Each character represents an element with '.' representing zero, '+'
+ * representing positive, and '-' representing negative. Here's an example for a
+ * 3x3 identity matrix.
+ *
+ * "+.."
+ * ".+."
+ * "..+"
+ *
+ * @param[out] file A file stream.
+ * @param[in] mat The sparse matrix.
+ */
+SLEIPNIR_DLLEXPORT inline void Spy(std::ostream& file,
+                                   const Eigen::SparseMatrix<double>& mat) {
+  const int cells_width = mat.cols() + 1;
+  const int cells_height = mat.rows();
+
+  std::vector<uint8_t> cells;
+
+  // Allocate space for matrix of characters plus trailing newlines
+  cells.reserve(cells_width * cells_height);
+
+  // Initialize cell array
+  for (int row = 0; row < mat.rows(); ++row) {
+    for (int col = 0; col < mat.cols(); ++col) {
+      cells.emplace_back('.');
+    }
+    cells.emplace_back('\n');
+  }
+
+  // Fill in non-sparse entries
+  for (int k = 0; k < mat.outerSize(); ++k) {
+    for (Eigen::SparseMatrix<double>::InnerIterator it{mat, k}; it; ++it) {
+      if (it.value() < 0.0) {
+        cells[it.row() * cells_width + it.col()] = '-';
+      } else if (it.value() > 0.0) {
+        cells[it.row() * cells_width + it.col()] = '+';
+      }
+    }
+  }
+
+  // Write cell array to file
+  for (const auto& c : cells) {
+    file << c;
+  }
+}
+
+/**
+ * Write the sparsity pattern of a sparse matrix to a file.
+ *
+ * Each character represents an element with "." representing zero, "+"
+ * representing positive, and "-" representing negative. Here's an example for a
+ * 3x3 identity matrix.
+ *
+ * "+.."
+ * ".+."
+ * "..+"
+ *
+ * @param[in] filename The filename.
+ * @param[in] mat The sparse matrix.
+ */
+SLEIPNIR_DLLEXPORT inline void Spy(std::string_view filename,
+                                   const Eigen::SparseMatrix<double>& mat) {
+  std::ofstream file{std::string{filename}};
+  if (!file.is_open()) {
+    return;
+  }
+
+  Spy(file, mat);
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/include/sleipnir/util/SymbolExports.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/include/sleipnir/util/SymbolExports.hpp`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#ifdef _WIN32
-#ifdef _MSC_VER
-#pragma warning(disable : 4251)
-#endif
-
-#ifdef SLEIPNIR_EXPORTS
-#ifdef __GNUC__
-#define SLEIPNIR_DLLEXPORT __attribute__((dllexport))
-#else
-#define SLEIPNIR_DLLEXPORT __declspec(dllexport)
-#endif
-
-#elif defined(SLEIPNIR_IMPORTS)
-
-#ifdef __GNUC__
-#define SLEIPNIR_DLLEXPORT __attribute__((dllimport))
-#else
-#define SLEIPNIR_DLLEXPORT __declspec(dllimport)
-#endif
-
-#else
-#define SLEIPNIR_DLLEXPORT
-#endif
-
-#else  // _WIN32
-
-#ifdef SLEIPNIR_EXPORTS
-#define SLEIPNIR_DLLEXPORT __attribute__((visibility("default")))
-#else
-#define SLEIPNIR_DLLEXPORT
-#endif
-
-#endif  // _WIN32
-
-// Synopsis
-//
-// This header provides macros for using FOO_EXPORT macros with explicit
-// template instantiation declarations and definitions.
-// Generally, the FOO_EXPORT macros are used at declarations,
-// and GCC requires them to be used at explicit instantiation declarations,
-// but MSVC requires __declspec(dllexport) to be used at the explicit
-// instantiation definitions instead.
-
-// Usage
-//
-// In a header file, write:
-//
-//   extern template class EXPORT_TEMPLATE_DECLARE(FOO_EXPORT) foo<bar>;
-//
-// In a source file, write:
-//
-//   template class EXPORT_TEMPLATE_DEFINE(FOO_EXPORT) foo<bar>;
-
-// Implementation notes
-//
-// The implementation of this header uses some subtle macro semantics to
-// detect what the provided FOO_EXPORT value was defined as and then
-// to dispatch to appropriate macro definitions.  Unfortunately,
-// MSVC's C preprocessor is rather non-compliant and requires special
-// care to make it work.
-//
-// Issue 1.
-//
-//   #define F(x)
-//   F()
-//
-// MSVC emits warning C4003 ("not enough actual parameters for macro
-// 'F'), even though it's a valid macro invocation.  This affects the
-// macros below that take just an "export" parameter, because export
-// may be empty.
-//
-// As a workaround, we can add a dummy parameter and arguments:
-//
-//   #define F(x,_)
-//   F(,)
-//
-// Issue 2.
-//
-//   #define F(x) G##x
-//   #define Gj() ok
-//   F(j())
-//
-// The correct replacement for "F(j())" is "ok", but MSVC replaces it
-// with "Gj()".  As a workaround, we can pass the result to an
-// identity macro to force MSVC to look for replacements again.  (This
-// is why EXPORT_TEMPLATE_STYLE_3 exists.)
-
-#define EXPORT_TEMPLATE_DECLARE(export) \
-  EXPORT_TEMPLATE_INVOKE(DECLARE, EXPORT_TEMPLATE_STYLE(export, ), export)
-#define EXPORT_TEMPLATE_DEFINE(export) \
-  EXPORT_TEMPLATE_INVOKE(DEFINE, EXPORT_TEMPLATE_STYLE(export, ), export)
-
-// INVOKE is an internal helper macro to perform parameter replacements
-// and token pasting to chain invoke another macro.  E.g.,
-//     EXPORT_TEMPLATE_INVOKE(DECLARE, DEFAULT, FOO_EXPORT)
-// will export to call
-//     EXPORT_TEMPLATE_DECLARE_DEFAULT(FOO_EXPORT, )
-// (but with FOO_EXPORT expanded too).
-#define EXPORT_TEMPLATE_INVOKE(which, style, export) \
-  EXPORT_TEMPLATE_INVOKE_2(which, style, export)
-#define EXPORT_TEMPLATE_INVOKE_2(which, style, export) \
-  EXPORT_TEMPLATE_##which##_##style(export, )
-
-// Default style is to apply the FOO_EXPORT macro at declaration sites.
-#define EXPORT_TEMPLATE_DECLARE_DEFAULT(export, _) export
-#define EXPORT_TEMPLATE_DEFINE_DEFAULT(export, _)
-
-// The "MSVC hack" style is used when FOO_EXPORT is defined
-// as __declspec(dllexport), which MSVC requires to be used at
-// definition sites instead.
-#define EXPORT_TEMPLATE_DECLARE_MSVC_HACK(export, _)
-#define EXPORT_TEMPLATE_DEFINE_MSVC_HACK(export, _) export
-
-// EXPORT_TEMPLATE_STYLE is an internal helper macro that identifies which
-// export style needs to be used for the provided FOO_EXPORT macro definition.
-// "", "__attribute__(...)", and "__declspec(dllimport)" are mapped
-// to "DEFAULT"; while "__declspec(dllexport)" is mapped to "MSVC_HACK".
-//
-// It's implemented with token pasting to transform the __attribute__ and
-// __declspec annotations into macro invocations.  E.g., if FOO_EXPORT is
-// defined as "__declspec(dllimport)", it undergoes the following sequence of
-// macro substitutions:
-//     EXPORT_TEMPLATE_STYLE(FOO_EXPORT, )
-//     EXPORT_TEMPLATE_STYLE_2(__declspec(dllimport), )
-//     EXPORT_TEMPLATE_STYLE_3(EXPORT_TEMPLATE_STYLE_MATCH__declspec(dllimport))
-//     EXPORT_TEMPLATE_STYLE_MATCH__declspec(dllimport)
-//     EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_dllimport
-//     DEFAULT
-#define EXPORT_TEMPLATE_STYLE(export, _) EXPORT_TEMPLATE_STYLE_2(export, )
-#define EXPORT_TEMPLATE_STYLE_2(export, _) \
-  EXPORT_TEMPLATE_STYLE_3(                 \
-      EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA##export)
-#define EXPORT_TEMPLATE_STYLE_3(style) style
-
-// Internal helper macros for EXPORT_TEMPLATE_STYLE.
-//
-// XXX: C++ reserves all identifiers containing "__" for the implementation,
-// but "__attribute__" and "__declspec" already contain "__" and the token-paste
-// operator can only add characters; not remove them.  To minimize the risk of
-// conflict with implementations, we include "foj3FJo5StF0OvIzl7oMxA" (a random
-// 128-bit string, encoded in Base64) in the macro name.
-#define EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA DEFAULT
-#define EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA__attribute__(...) \
-  DEFAULT
-#define EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA__declspec(arg) \
-  EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_##arg
-
-// Internal helper macros for EXPORT_TEMPLATE_STYLE.
-#define EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_dllexport MSVC_HACK
-#define EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_dllimport DEFAULT
-
-// Sanity checks.
-//
-// EXPORT_TEMPLATE_TEST uses the same macro invocation pattern as
-// EXPORT_TEMPLATE_DECLARE and EXPORT_TEMPLATE_DEFINE do to check that they're
-// working correctly.  When they're working correctly, the sequence of macro
-// replacements should go something like:
-//
-//     EXPORT_TEMPLATE_TEST(DEFAULT, __declspec(dllimport));
-//
-//     static_assert(EXPORT_TEMPLATE_INVOKE(TEST_DEFAULT,
-//         EXPORT_TEMPLATE_STYLE(__declspec(dllimport), ),
-//         __declspec(dllimport)), "__declspec(dllimport)");
-//
-//     static_assert(EXPORT_TEMPLATE_INVOKE(TEST_DEFAULT,
-//         DEFAULT, __declspec(dllimport)), "__declspec(dllimport)");
-//
-//     static_assert(EXPORT_TEMPLATE_TEST_DEFAULT_DEFAULT(
-//         __declspec(dllimport)), "__declspec(dllimport)");
-//
-//     static_assert(true, "__declspec(dllimport)");
-//
-// When they're not working correctly, a syntax error should occur instead.
-#define EXPORT_TEMPLATE_TEST(want, export)                                 \
-  static_assert(EXPORT_TEMPLATE_INVOKE(                                    \
-                    TEST_##want, EXPORT_TEMPLATE_STYLE(export, ), export), \
-                #export)
-#define EXPORT_TEMPLATE_TEST_DEFAULT_DEFAULT(...) true
-#define EXPORT_TEMPLATE_TEST_MSVC_HACK_MSVC_HACK(...) true
-
-EXPORT_TEMPLATE_TEST(DEFAULT, );
-EXPORT_TEMPLATE_TEST(DEFAULT, __attribute__((visibility("default"))));
-EXPORT_TEMPLATE_TEST(MSVC_HACK, __declspec(dllexport));
-EXPORT_TEMPLATE_TEST(DEFAULT, __declspec(dllimport));
-
-#undef EXPORT_TEMPLATE_TEST
-#undef EXPORT_TEMPLATE_TEST_DEFAULT_DEFAULT
-#undef EXPORT_TEMPLATE_TEST_MSVC_HACK_MSVC_HACK
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#ifdef _WIN32
+#ifdef _MSC_VER
+#pragma warning(disable : 4251)
+#endif
+
+#ifdef SLEIPNIR_EXPORTS
+#ifdef __GNUC__
+#define SLEIPNIR_DLLEXPORT __attribute__((dllexport))
+#else
+#define SLEIPNIR_DLLEXPORT __declspec(dllexport)
+#endif
+
+#elif defined(SLEIPNIR_IMPORTS)
+
+#ifdef __GNUC__
+#define SLEIPNIR_DLLEXPORT __attribute__((dllimport))
+#else
+#define SLEIPNIR_DLLEXPORT __declspec(dllimport)
+#endif
+
+#else
+#define SLEIPNIR_DLLEXPORT
+#endif
+
+#else  // _WIN32
+
+#ifdef SLEIPNIR_EXPORTS
+#define SLEIPNIR_DLLEXPORT __attribute__((visibility("default")))
+#else
+#define SLEIPNIR_DLLEXPORT
+#endif
+
+#endif  // _WIN32
+
+// Synopsis
+//
+// This header provides macros for using FOO_EXPORT macros with explicit
+// template instantiation declarations and definitions.
+// Generally, the FOO_EXPORT macros are used at declarations,
+// and GCC requires them to be used at explicit instantiation declarations,
+// but MSVC requires __declspec(dllexport) to be used at the explicit
+// instantiation definitions instead.
+
+// Usage
+//
+// In a header file, write:
+//
+//   extern template class EXPORT_TEMPLATE_DECLARE(FOO_EXPORT) foo<bar>;
+//
+// In a source file, write:
+//
+//   template class EXPORT_TEMPLATE_DEFINE(FOO_EXPORT) foo<bar>;
+
+// Implementation notes
+//
+// The implementation of this header uses some subtle macro semantics to
+// detect what the provided FOO_EXPORT value was defined as and then
+// to dispatch to appropriate macro definitions.  Unfortunately,
+// MSVC's C preprocessor is rather non-compliant and requires special
+// care to make it work.
+//
+// Issue 1.
+//
+//   #define F(x)
+//   F()
+//
+// MSVC emits warning C4003 ("not enough actual parameters for macro
+// 'F'), even though it's a valid macro invocation.  This affects the
+// macros below that take just an "export" parameter, because export
+// may be empty.
+//
+// As a workaround, we can add a dummy parameter and arguments:
+//
+//   #define F(x,_)
+//   F(,)
+//
+// Issue 2.
+//
+//   #define F(x) G##x
+//   #define Gj() ok
+//   F(j())
+//
+// The correct replacement for "F(j())" is "ok", but MSVC replaces it
+// with "Gj()".  As a workaround, we can pass the result to an
+// identity macro to force MSVC to look for replacements again.  (This
+// is why EXPORT_TEMPLATE_STYLE_3 exists.)
+
+#define EXPORT_TEMPLATE_DECLARE(export) \
+  EXPORT_TEMPLATE_INVOKE(DECLARE, EXPORT_TEMPLATE_STYLE(export, ), export)
+#define EXPORT_TEMPLATE_DEFINE(export) \
+  EXPORT_TEMPLATE_INVOKE(DEFINE, EXPORT_TEMPLATE_STYLE(export, ), export)
+
+// INVOKE is an internal helper macro to perform parameter replacements
+// and token pasting to chain invoke another macro.  E.g.,
+//     EXPORT_TEMPLATE_INVOKE(DECLARE, DEFAULT, FOO_EXPORT)
+// will export to call
+//     EXPORT_TEMPLATE_DECLARE_DEFAULT(FOO_EXPORT, )
+// (but with FOO_EXPORT expanded too).
+#define EXPORT_TEMPLATE_INVOKE(which, style, export) \
+  EXPORT_TEMPLATE_INVOKE_2(which, style, export)
+#define EXPORT_TEMPLATE_INVOKE_2(which, style, export) \
+  EXPORT_TEMPLATE_##which##_##style(export, )
+
+// Default style is to apply the FOO_EXPORT macro at declaration sites.
+#define EXPORT_TEMPLATE_DECLARE_DEFAULT(export, _) export
+#define EXPORT_TEMPLATE_DEFINE_DEFAULT(export, _)
+
+// The "MSVC hack" style is used when FOO_EXPORT is defined
+// as __declspec(dllexport), which MSVC requires to be used at
+// definition sites instead.
+#define EXPORT_TEMPLATE_DECLARE_MSVC_HACK(export, _)
+#define EXPORT_TEMPLATE_DEFINE_MSVC_HACK(export, _) export
+
+// EXPORT_TEMPLATE_STYLE is an internal helper macro that identifies which
+// export style needs to be used for the provided FOO_EXPORT macro definition.
+// "", "__attribute__(...)", and "__declspec(dllimport)" are mapped
+// to "DEFAULT"; while "__declspec(dllexport)" is mapped to "MSVC_HACK".
+//
+// It's implemented with token pasting to transform the __attribute__ and
+// __declspec annotations into macro invocations.  E.g., if FOO_EXPORT is
+// defined as "__declspec(dllimport)", it undergoes the following sequence of
+// macro substitutions:
+//     EXPORT_TEMPLATE_STYLE(FOO_EXPORT, )
+//     EXPORT_TEMPLATE_STYLE_2(__declspec(dllimport), )
+//     EXPORT_TEMPLATE_STYLE_3(EXPORT_TEMPLATE_STYLE_MATCH__declspec(dllimport))
+//     EXPORT_TEMPLATE_STYLE_MATCH__declspec(dllimport)
+//     EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_dllimport
+//     DEFAULT
+#define EXPORT_TEMPLATE_STYLE(export, _) EXPORT_TEMPLATE_STYLE_2(export, )
+#define EXPORT_TEMPLATE_STYLE_2(export, _) \
+  EXPORT_TEMPLATE_STYLE_3(                 \
+      EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA##export)
+#define EXPORT_TEMPLATE_STYLE_3(style) style
+
+// Internal helper macros for EXPORT_TEMPLATE_STYLE.
+//
+// XXX: C++ reserves all identifiers containing "__" for the implementation,
+// but "__attribute__" and "__declspec" already contain "__" and the token-paste
+// operator can only add characters; not remove them.  To minimize the risk of
+// conflict with implementations, we include "foj3FJo5StF0OvIzl7oMxA" (a random
+// 128-bit string, encoded in Base64) in the macro name.
+#define EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA DEFAULT
+#define EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA__attribute__(...) \
+  DEFAULT
+#define EXPORT_TEMPLATE_STYLE_MATCH_foj3FJo5StF0OvIzl7oMxA__declspec(arg) \
+  EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_##arg
+
+// Internal helper macros for EXPORT_TEMPLATE_STYLE.
+#define EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_dllexport MSVC_HACK
+#define EXPORT_TEMPLATE_STYLE_MATCH_DECLSPEC_dllimport DEFAULT
+
+// Sanity checks.
+//
+// EXPORT_TEMPLATE_TEST uses the same macro invocation pattern as
+// EXPORT_TEMPLATE_DECLARE and EXPORT_TEMPLATE_DEFINE do to check that they're
+// working correctly.  When they're working correctly, the sequence of macro
+// replacements should go something like:
+//
+//     EXPORT_TEMPLATE_TEST(DEFAULT, __declspec(dllimport));
+//
+//     static_assert(EXPORT_TEMPLATE_INVOKE(TEST_DEFAULT,
+//         EXPORT_TEMPLATE_STYLE(__declspec(dllimport), ),
+//         __declspec(dllimport)), "__declspec(dllimport)");
+//
+//     static_assert(EXPORT_TEMPLATE_INVOKE(TEST_DEFAULT,
+//         DEFAULT, __declspec(dllimport)), "__declspec(dllimport)");
+//
+//     static_assert(EXPORT_TEMPLATE_TEST_DEFAULT_DEFAULT(
+//         __declspec(dllimport)), "__declspec(dllimport)");
+//
+//     static_assert(true, "__declspec(dllimport)");
+//
+// When they're not working correctly, a syntax error should occur instead.
+#define EXPORT_TEMPLATE_TEST(want, export)                                 \
+  static_assert(EXPORT_TEMPLATE_INVOKE(                                    \
+                    TEST_##want, EXPORT_TEMPLATE_STYLE(export, ), export), \
+                #export)
+#define EXPORT_TEMPLATE_TEST_DEFAULT_DEFAULT(...) true
+#define EXPORT_TEMPLATE_TEST_MSVC_HACK_MSVC_HACK(...) true
+
+EXPORT_TEMPLATE_TEST(DEFAULT, );
+EXPORT_TEMPLATE_TEST(DEFAULT, __attribute__((visibility("default"))));
+EXPORT_TEMPLATE_TEST(MSVC_HACK, __declspec(dllexport));
+EXPORT_TEMPLATE_TEST(DEFAULT, __declspec(dllimport));
+
+#undef EXPORT_TEMPLATE_TEST
+#undef EXPORT_TEMPLATE_TEST_DEFAULT_DEFAULT
+#undef EXPORT_TEMPLATE_TEST_MSVC_HACK_MSVC_HACK
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/autodiff/__init__.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/autodiff/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from .._jormungandr.autodiff import *
-
-import scipy.sparse
-
-
-def spy(mat: scipy.sparse.csc_matrix):
-    """
-    Plot the sparsity pattern of a sparse matrix.
-
-    Green points represent positive values and red points represent negative
-    values.
-
-    Parameter ``mat``:
-        The sparse matrix.
-    """
-    from matplotlib.colors import ListedColormap
-    import matplotlib.pyplot as plt
-    import matplotlib.ticker as mticker
-
-    xs = []
-    ys = []
-    vs = []
-
-    cmat = mat.tocoo()
-    for row, col, value in zip(cmat.row, cmat.col, cmat.data):
-        xs.append(col)
-        ys.append(row)
-        if value > 0.0:
-            vs.append(1.0)
-        elif value < 0.0:
-            vs.append(-1.0)
-        else:
-            vs.append(0.0)
-
-    fig = plt.figure()
-    ax = fig.add_subplot()
-
-    # Display scatter plot
-    cmap = ListedColormap(["red", "green"])
-    sc = ax.scatter(xs, ys, s=1, c=vs, marker=".", cmap=cmap, vmin=-1, vmax=1)
-
-    # Display colorbar
-    colorbar = fig.colorbar(sc)
-    ticklabels = ["Negative", "Positive"]
-    colorbar.ax.yaxis.set_major_locator(mticker.FixedLocator(ticklabels))
-    colorbar.ax.set_yticks([-1, 1])
-    colorbar.ax.set_yticklabels(ticklabels)
-
-    ax.set_title("Sparsity")
-    ax.set_xlabel("Cols")
-    ax.set_ylabel("Rows")
-
-    ax.set_xlim([0, mat.shape[1]])
-    ax.set_ylim([0, mat.shape[0]])
-    ax.invert_yaxis()
-    ax.set_aspect(1.0)
-
-    plt.show()
+from .._jormungandr.autodiff import *
+
+import scipy.sparse
+
+
+def spy(mat: scipy.sparse.csc_matrix):
+    """
+    Plot the sparsity pattern of a sparse matrix.
+
+    Green points represent positive values and red points represent negative
+    values.
+
+    Parameter ``mat``:
+        The sparse matrix.
+    """
+    from matplotlib.colors import ListedColormap
+    import matplotlib.pyplot as plt
+    import matplotlib.ticker as mticker
+
+    xs = []
+    ys = []
+    vs = []
+
+    cmat = mat.tocoo()
+    for row, col, value in zip(cmat.row, cmat.col, cmat.data):
+        xs.append(col)
+        ys.append(row)
+        if value > 0.0:
+            vs.append(1.0)
+        elif value < 0.0:
+            vs.append(-1.0)
+        else:
+            vs.append(0.0)
+
+    fig = plt.figure()
+    ax = fig.add_subplot()
+
+    # Display scatter plot
+    cmap = ListedColormap(["red", "green"])
+    sc = ax.scatter(xs, ys, s=1, c=vs, marker=".", cmap=cmap, vmin=-1, vmax=1)
+
+    # Display colorbar
+    colorbar = fig.colorbar(sc)
+    ticklabels = ["Negative", "Positive"]
+    colorbar.ax.yaxis.set_major_locator(mticker.FixedLocator(ticklabels))
+    colorbar.ax.set_yticks([-1, 1])
+    colorbar.ax.set_yticklabels(ticklabels)
+
+    ax.set_title("Sparsity")
+    ax.set_xlabel("Cols")
+    ax.set_ylabel("Rows")
+
+    ax.set_xlim([0, mat.shape[1]])
+    ax.set_ylim([0, mat.shape[0]])
+    ax.invert_yaxis()
+    ax.set_aspect(1.0)
+
+    plt.show()
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/Binders.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/Binders.hpp`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <pybind11/pybind11.h>
-
-namespace py = pybind11;
-
-namespace sleipnir {
-
-void BindExpressionType(py::module_& autodiff);
-void BindGradient(py::module_& autodiff);
-void BindHessian(py::module_& autodiff);
-void BindJacobian(py::module_& autodiff);
-void BindVariable(py::module_& autodiff);
-void BindVariableBlock(py::module_& autodiff);
-void BindVariableMatrix(py::module_& autodiff);
-
-void BindConstraints(py::module_& optimization);
-void BindOptimizationProblem(py::module_& optimization);
-void BindSolverExitCondition(py::module_& optimization);
-void BindSolverIterationInfo(py::module_& optimization);
-void BindSolverStatus(py::module_& optimization);
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <pybind11/pybind11.h>
+
+namespace py = pybind11;
+
+namespace sleipnir {
+
+void BindExpressionType(py::module_& autodiff);
+void BindGradient(py::module_& autodiff);
+void BindHessian(py::module_& autodiff);
+void BindJacobian(py::module_& autodiff);
+void BindVariable(py::module_& autodiff);
+void BindVariableBlock(py::module_& autodiff);
+void BindVariableMatrix(py::module_& autodiff);
+
+void BindConstraints(py::module_& optimization);
+void BindOptimizationProblem(py::module_& optimization);
+void BindSolverExitCondition(py::module_& optimization);
+void BindSolverIterationInfo(py::module_& optimization);
+void BindSolverStatus(py::module_& optimization);
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/Main.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/Main.cpp`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-// Copyright (c) Sleipnir contributors
-
-#include <pybind11/pybind11.h>
-
-#include "Binders.hpp"
-
-namespace py = pybind11;
-
-namespace sleipnir {
-
-PYBIND11_MODULE(_jormungandr, m) {
-  m.doc() =
-      "A linearity-exploiting sparse nonlinear constrained optimization "
-      "problem solver that uses the interior-point method.";
-
-  py::module_ autodiff = m.def_submodule("autodiff");
-  BindExpressionType(autodiff);
-  BindGradient(autodiff);
-  BindHessian(autodiff);
-  BindJacobian(autodiff);
-  BindVariable(autodiff);
-  BindVariableMatrix(autodiff);
-  BindVariableBlock(autodiff);  // Must be bound after VariableMatrix
-
-  py::module_ optimization = m.def_submodule("optimization");
-  BindConstraints(optimization);
-  BindSolverExitCondition(optimization);
-  BindSolverIterationInfo(optimization);
-  BindSolverStatus(optimization);
-  BindOptimizationProblem(optimization);
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include <pybind11/pybind11.h>
+
+#include "Binders.hpp"
+
+namespace py = pybind11;
+
+namespace sleipnir {
+
+PYBIND11_MODULE(_jormungandr, m) {
+  m.doc() =
+      "A linearity-exploiting sparse nonlinear constrained optimization "
+      "problem solver that uses the interior-point method.";
+
+  py::module_ autodiff = m.def_submodule("autodiff");
+  BindExpressionType(autodiff);
+  BindGradient(autodiff);
+  BindHessian(autodiff);
+  BindJacobian(autodiff);
+  BindVariable(autodiff);
+  BindVariableMatrix(autodiff);
+  BindVariableBlock(autodiff);  // Must be bound after VariableMatrix
+
+  py::module_ optimization = m.def_submodule("optimization");
+  BindConstraints(optimization);
+  BindSolverExitCondition(optimization);
+  BindSolverIterationInfo(optimization);
+  BindSolverStatus(optimization);
+  BindOptimizationProblem(optimization);
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindExpressionType.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindExpressionType.cpp`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-// Copyright (c) Sleipnir contributors
-
-#include <pybind11/pybind11.h>
-#include <sleipnir/autodiff/ExpressionType.hpp>
-
-#include "Docstrings.hpp"
-
-namespace py = pybind11;
-
-namespace sleipnir {
-
-void BindExpressionType(py::module_& autodiff) {
-  py::enum_<ExpressionType> expressionType{autodiff, "ExpressionType",
-                                           DOC(sleipnir, ExpressionType)};
-  expressionType
-      .value("NONE", ExpressionType::kNone,
-             DOC(sleipnir, ExpressionType, kNone))
-      .value("CONSTANT", ExpressionType::kConstant,
-             DOC(sleipnir, ExpressionType, kConstant))
-      .value("LINEAR", ExpressionType::kLinear,
-             DOC(sleipnir, ExpressionType, kLinear))
-      .value("QUADRATIC", ExpressionType::kQuadratic,
-             DOC(sleipnir, ExpressionType, kQuadratic))
-      .value("NONLINEAR", ExpressionType::kNonlinear,
-             DOC(sleipnir, ExpressionType, kNonlinear));
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include <pybind11/pybind11.h>
+#include <sleipnir/autodiff/ExpressionType.hpp>
+
+#include "Docstrings.hpp"
+
+namespace py = pybind11;
+
+namespace sleipnir {
+
+void BindExpressionType(py::module_& autodiff) {
+  py::enum_<ExpressionType> expressionType{autodiff, "ExpressionType",
+                                           DOC(sleipnir, ExpressionType)};
+  expressionType
+      .value("NONE", ExpressionType::kNone,
+             DOC(sleipnir, ExpressionType, kNone))
+      .value("CONSTANT", ExpressionType::kConstant,
+             DOC(sleipnir, ExpressionType, kConstant))
+      .value("LINEAR", ExpressionType::kLinear,
+             DOC(sleipnir, ExpressionType, kLinear))
+      .value("QUADRATIC", ExpressionType::kQuadratic,
+             DOC(sleipnir, ExpressionType, kQuadratic))
+      .value("NONLINEAR", ExpressionType::kNonlinear,
+             DOC(sleipnir, ExpressionType, kNonlinear));
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindGradient.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindGradient.cpp`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-// Copyright (c) Sleipnir contributors
-
-#include <pybind11/eigen.h>
-#include <pybind11/pybind11.h>
-#include <sleipnir/autodiff/Gradient.hpp>
-
-#include "Docstrings.hpp"
-
-namespace py = pybind11;
-
-namespace sleipnir {
-
-void BindGradient(py::module_& autodiff) {
-  py::class_<Gradient> cls{autodiff, "Gradient", DOC(sleipnir, Gradient)};
-  cls.def(py::init<Variable, Variable>(), DOC(sleipnir, Gradient, Gradient))
-      .def(py::init<Variable, VariableMatrix>(),
-           DOC(sleipnir, Gradient, Gradient, 2))
-      .def("get", &Gradient::Get, DOC(sleipnir, Gradient, Get))
-      .def(
-          "value",
-          [](Gradient& self) {
-            return Eigen::SparseMatrix<double>{self.Value()};
-          },
-          DOC(sleipnir, Gradient, Value))
-      .def("update", &Gradient::Update, DOC(sleipnir, Gradient, Update));
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include <pybind11/eigen.h>
+#include <pybind11/pybind11.h>
+#include <sleipnir/autodiff/Gradient.hpp>
+
+#include "Docstrings.hpp"
+
+namespace py = pybind11;
+
+namespace sleipnir {
+
+void BindGradient(py::module_& autodiff) {
+  py::class_<Gradient> cls{autodiff, "Gradient", DOC(sleipnir, Gradient)};
+  cls.def(py::init<Variable, Variable>(), DOC(sleipnir, Gradient, Gradient))
+      .def(py::init<Variable, VariableMatrix>(),
+           DOC(sleipnir, Gradient, Gradient, 2))
+      .def("get", &Gradient::Get, DOC(sleipnir, Gradient, Get))
+      .def(
+          "value",
+          [](Gradient& self) {
+            return Eigen::SparseMatrix<double>{self.Value()};
+          },
+          DOC(sleipnir, Gradient, Value))
+      .def("update", &Gradient::Update, DOC(sleipnir, Gradient, Update));
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindHessian.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindHessian.cpp`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-// Copyright (c) Sleipnir contributors
-
-#include <pybind11/eigen.h>
-#include <pybind11/pybind11.h>
-#include <sleipnir/autodiff/Hessian.hpp>
-
-#include "Docstrings.hpp"
-
-namespace py = pybind11;
-
-namespace sleipnir {
-
-void BindHessian(py::module_& autodiff) {
-  py::class_<Hessian> cls{autodiff, "Hessian", DOC(sleipnir, Hessian)};
-  cls.def(py::init<Variable, VariableMatrix>(), DOC(sleipnir, Hessian, Hessian))
-      .def("get", &Hessian::Get, DOC(sleipnir, Hessian, Get))
-      .def("value", &Hessian::Value, DOC(sleipnir, Hessian, Value))
-      .def("update", &Hessian::Update, DOC(sleipnir, Hessian, Update));
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include <pybind11/eigen.h>
+#include <pybind11/pybind11.h>
+#include <sleipnir/autodiff/Hessian.hpp>
+
+#include "Docstrings.hpp"
+
+namespace py = pybind11;
+
+namespace sleipnir {
+
+void BindHessian(py::module_& autodiff) {
+  py::class_<Hessian> cls{autodiff, "Hessian", DOC(sleipnir, Hessian)};
+  cls.def(py::init<Variable, VariableMatrix>(), DOC(sleipnir, Hessian, Hessian))
+      .def("get", &Hessian::Get, DOC(sleipnir, Hessian, Get))
+      .def("value", &Hessian::Value, DOC(sleipnir, Hessian, Value))
+      .def("update", &Hessian::Update, DOC(sleipnir, Hessian, Update));
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindVariable.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindVariable.cpp`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-// Copyright (c) Sleipnir contributors
-
-#include <pybind11/eigen.h>
-#include <pybind11/operators.h>
-#include <pybind11/pybind11.h>
-#include <sleipnir/autodiff/Variable.hpp>
-#include <sleipnir/optimization/Constraints.hpp>
-
-#include "Docstrings.hpp"
-
-namespace py = pybind11;
-
-#if defined(__APPLE__) && defined(__clang__)
-#if (__clang_major__ >= 10)
-PYBIND11_WARNING_DISABLE_CLANG("-Wself-assign-overloaded")
-#endif
-#elif defined(__clang__)
-#if (__clang_major__ >= 7)
-PYBIND11_WARNING_DISABLE_CLANG("-Wself-assign-overloaded")
-#endif
-#endif
-
-namespace sleipnir {
-
-void BindVariable(py::module_& autodiff) {
-  py::class_<Variable> variable{autodiff, "Variable", DOC(sleipnir, Variable)};
-  variable.def(py::init<>(), DOC(sleipnir, Variable, Variable));
-  variable.def(py::init<double>(), DOC(sleipnir, Variable, Variable, 2));
-  variable.def(py::init<int>(), DOC(sleipnir, Variable, Variable, 3));
-  variable.def("set", py::overload_cast<double>(&Variable::operator=),
-               DOC(sleipnir, Variable, operator, assign));
-  variable.def("set", py::overload_cast<int>(&Variable::operator=),
-               DOC(sleipnir, Variable, operator, assign, 2));
-  variable.def("set_value", py::overload_cast<double>(&Variable::SetValue),
-               DOC(sleipnir, Variable, SetValue));
-  variable.def("set_value", py::overload_cast<int>(&Variable::SetValue),
-               DOC(sleipnir, Variable, SetValue, 2));
-  variable.def(double() * py::self);
-  variable.def(py::self * double());
-  variable.def(py::self * py::self);
-  variable.def(py::self *= double(), DOC(sleipnir, Variable, operator, imul));
-  variable.def(py::self *= py::self, DOC(sleipnir, Variable, operator, imul));
-  variable.def(double() / py::self);
-  variable.def(py::self / double());
-  variable.def(py::self / py::self);
-  variable.def(py::self /= double(), DOC(sleipnir, Variable, operator, idiv));
-  variable.def(py::self /= py::self, DOC(sleipnir, Variable, operator, idiv));
-  variable.def(double() + py::self);
-  variable.def(py::self + double());
-  variable.def(py::self + py::self);
-  variable.def(py::self += double(), DOC(sleipnir, Variable, operator, iadd));
-  variable.def(py::self += py::self, DOC(sleipnir, Variable, operator, iadd));
-  variable.def(double() - py::self);
-  variable.def(py::self - double());
-  variable.def(py::self - py::self);
-  variable.def(py::self -= double(), DOC(sleipnir, Variable, operator, isub));
-  variable.def(py::self -= py::self, DOC(sleipnir, Variable, operator, isub));
-  variable.def(
-      "__pow__",
-      [](const Variable& self, int power) {
-        return sleipnir::pow(self, power);
-      },
-      py::is_operator());
-  variable.def(-py::self);
-  variable.def(+py::self);
-  variable.def("value", &Variable::Value, DOC(sleipnir, Variable, Value));
-  variable.def("type", &Variable::Type, DOC(sleipnir, Variable, Type));
-  variable.def("update", &Variable::Update, DOC(sleipnir, Variable, Update));
-  variable.def(py::self == py::self, DOC(sleipnir, operator, eq));
-  variable.def(py::self < py::self, DOC(sleipnir, operator, lt));
-  variable.def(py::self <= py::self, DOC(sleipnir, operator, le));
-  variable.def(py::self > py::self, DOC(sleipnir, operator, gt));
-  variable.def(py::self >= py::self, DOC(sleipnir, operator, ge));
-  variable.def(py::self == double(), DOC(sleipnir, operator, eq));
-  variable.def(py::self < double(), DOC(sleipnir, operator, lt));
-  variable.def(py::self <= double(), DOC(sleipnir, operator, le));
-  variable.def(py::self > double(), DOC(sleipnir, operator, gt));
-  variable.def(py::self >= double(), DOC(sleipnir, operator, ge));
-  variable.def(double() == py::self, DOC(sleipnir, operator, eq));
-  variable.def(double() < py::self, DOC(sleipnir, operator, lt));
-  variable.def(double() <= py::self, DOC(sleipnir, operator, le));
-  variable.def(double() > py::self, DOC(sleipnir, operator, gt));
-  variable.def(double() >= py::self, DOC(sleipnir, operator, ge));
-
-  autodiff.def(
-      "abs", [](double x) { return sleipnir::abs(Variable{x}); },
-      DOC(sleipnir, abs));
-  autodiff.def("abs", static_cast<Variable (*)(const Variable&)>(&abs),
-               DOC(sleipnir, abs));
-  autodiff.def(
-      "acos", [](double x) { return sleipnir::acos(Variable{x}); },
-      DOC(sleipnir, acos));
-  autodiff.def("acos", static_cast<Variable (*)(const Variable&)>(&acos),
-               DOC(sleipnir, acos));
-  autodiff.def(
-      "asin", [](double x) { return sleipnir::asin(Variable{x}); },
-      DOC(sleipnir, asin));
-  autodiff.def("asin", static_cast<Variable (*)(const Variable&)>(&asin),
-               DOC(sleipnir, asin));
-  autodiff.def(
-      "atan", [](double x) { return sleipnir::atan(Variable{x}); },
-      DOC(sleipnir, atan));
-  autodiff.def("atan", static_cast<Variable (*)(const Variable&)>(&atan),
-               DOC(sleipnir, atan));
-  autodiff.def(
-      "atan2",
-      [](double y, const Variable& x) { return sleipnir::atan2(y, x); },
-      DOC(sleipnir, atan2));
-  autodiff.def(
-      "atan2",
-      [](const Variable& y, double x) { return sleipnir::atan2(y, x); },
-      DOC(sleipnir, atan2));
-  autodiff.def(
-      "atan2",
-      [](const Variable& y, const Variable& x) {
-        return sleipnir::atan2(y, x);
-      },
-      DOC(sleipnir, atan2));
-  autodiff.def(
-      "cos", [](double x) { return sleipnir::cos(Variable{x}); },
-      DOC(sleipnir, cos));
-  autodiff.def("cos", static_cast<Variable (*)(const Variable&)>(&cos),
-               DOC(sleipnir, cos));
-  autodiff.def(
-      "cosh", [](double x) { return sleipnir::cosh(Variable{x}); },
-      DOC(sleipnir, cosh));
-  autodiff.def("cosh", static_cast<Variable (*)(const Variable&)>(&cosh),
-               DOC(sleipnir, cosh));
-  autodiff.def(
-      "erf", [](double x) { return sleipnir::erf(Variable{x}); },
-      DOC(sleipnir, erf));
-  autodiff.def("erf", static_cast<Variable (*)(const Variable&)>(&erf),
-               DOC(sleipnir, erf));
-  autodiff.def(
-      "exp", [](double x) { return sleipnir::exp(Variable{x}); },
-      DOC(sleipnir, exp));
-  autodiff.def("exp", static_cast<Variable (*)(const Variable&)>(&exp),
-               DOC(sleipnir, exp));
-  autodiff.def(
-      "hypot",
-      [](double x, const Variable& y) { return sleipnir::hypot(x, y); },
-      DOC(sleipnir, hypot));
-  autodiff.def(
-      "hypot",
-      [](const Variable& x, double y) { return sleipnir::hypot(x, y); },
-      DOC(sleipnir, hypot));
-  autodiff.def(
-      "hypot",
-      static_cast<Variable (*)(const Variable&, const Variable&)>(&hypot),
-      DOC(sleipnir, hypot));
-  autodiff.def("hypot",
-               static_cast<Variable (*)(const Variable&, const Variable&,
-                                        const Variable&)>(&hypot),
-               DOC(sleipnir, hypot, 2));
-  autodiff.def(
-      "log", [](double x) { return sleipnir::log(Variable{x}); },
-      DOC(sleipnir, log));
-  autodiff.def("log", static_cast<Variable (*)(const Variable&)>(&log),
-               DOC(sleipnir, log));
-  autodiff.def(
-      "log10", [](double x) { return sleipnir::log10(Variable{x}); },
-      DOC(sleipnir, log10));
-  autodiff.def("log10", static_cast<Variable (*)(const Variable&)>(&log10),
-               DOC(sleipnir, log10));
-  autodiff.def(
-      "pow",
-      [](double base, const Variable& power) {
-        return sleipnir::pow(base, power);
-      },
-      DOC(sleipnir, pow));
-  autodiff.def(
-      "pow",
-      [](const Variable& base, double power) {
-        return sleipnir::pow(base, power);
-      },
-      DOC(sleipnir, pow));
-  autodiff.def(
-      "pow", static_cast<Variable (*)(const Variable&, const Variable&)>(&pow),
-      DOC(sleipnir, pow));
-  autodiff.def(
-      "sign", [](double x) { return sleipnir::sign(Variable{x}); },
-      DOC(sleipnir, sign));
-  autodiff.def("sign", static_cast<Variable (*)(const Variable&)>(&sign),
-               DOC(sleipnir, sign));
-  autodiff.def(
-      "sin", [](double x) { return sleipnir::sin(Variable{x}); },
-      DOC(sleipnir, sin));
-  autodiff.def("sin", static_cast<Variable (*)(const Variable&)>(&sin),
-               DOC(sleipnir, sin));
-  autodiff.def(
-      "sinh", [](double x) { return sleipnir::sinh(Variable{x}); },
-      DOC(sleipnir, sinh));
-  autodiff.def("sinh", static_cast<Variable (*)(const Variable&)>(&sinh),
-               DOC(sleipnir, sinh));
-  autodiff.def(
-      "sqrt", [](double x) { return sleipnir::sqrt(Variable{x}); },
-      DOC(sleipnir, sqrt));
-  autodiff.def("sqrt", static_cast<Variable (*)(const Variable&)>(&sqrt),
-               DOC(sleipnir, sqrt));
-  autodiff.def(
-      "tan", [](double x) { return sleipnir::tan(Variable{x}); },
-      DOC(sleipnir, tan));
-  autodiff.def("tan", static_cast<Variable (*)(const Variable&)>(&tan),
-               DOC(sleipnir, tan));
-  autodiff.def(
-      "tanh", [](double x) { return sleipnir::tanh(Variable{x}); },
-      DOC(sleipnir, tanh));
-  autodiff.def("tanh", static_cast<Variable (*)(const Variable&)>(&tanh),
-               DOC(sleipnir, tanh));
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include <pybind11/eigen.h>
+#include <pybind11/operators.h>
+#include <pybind11/pybind11.h>
+#include <sleipnir/autodiff/Variable.hpp>
+#include <sleipnir/optimization/Constraints.hpp>
+
+#include "Docstrings.hpp"
+
+namespace py = pybind11;
+
+#if defined(__APPLE__) && defined(__clang__)
+#if (__clang_major__ >= 10)
+PYBIND11_WARNING_DISABLE_CLANG("-Wself-assign-overloaded")
+#endif
+#elif defined(__clang__)
+#if (__clang_major__ >= 7)
+PYBIND11_WARNING_DISABLE_CLANG("-Wself-assign-overloaded")
+#endif
+#endif
+
+namespace sleipnir {
+
+void BindVariable(py::module_& autodiff) {
+  py::class_<Variable> variable{autodiff, "Variable", DOC(sleipnir, Variable)};
+  variable.def(py::init<>(), DOC(sleipnir, Variable, Variable));
+  variable.def(py::init<double>(), DOC(sleipnir, Variable, Variable, 2));
+  variable.def(py::init<int>(), DOC(sleipnir, Variable, Variable, 3));
+  variable.def("set", py::overload_cast<double>(&Variable::operator=),
+               DOC(sleipnir, Variable, operator, assign));
+  variable.def("set", py::overload_cast<int>(&Variable::operator=),
+               DOC(sleipnir, Variable, operator, assign, 2));
+  variable.def("set_value", py::overload_cast<double>(&Variable::SetValue),
+               DOC(sleipnir, Variable, SetValue));
+  variable.def("set_value", py::overload_cast<int>(&Variable::SetValue),
+               DOC(sleipnir, Variable, SetValue, 2));
+  variable.def(double() * py::self);
+  variable.def(py::self * double());
+  variable.def(py::self * py::self);
+  variable.def(py::self *= double(), DOC(sleipnir, Variable, operator, imul));
+  variable.def(py::self *= py::self, DOC(sleipnir, Variable, operator, imul));
+  variable.def(double() / py::self);
+  variable.def(py::self / double());
+  variable.def(py::self / py::self);
+  variable.def(py::self /= double(), DOC(sleipnir, Variable, operator, idiv));
+  variable.def(py::self /= py::self, DOC(sleipnir, Variable, operator, idiv));
+  variable.def(double() + py::self);
+  variable.def(py::self + double());
+  variable.def(py::self + py::self);
+  variable.def(py::self += double(), DOC(sleipnir, Variable, operator, iadd));
+  variable.def(py::self += py::self, DOC(sleipnir, Variable, operator, iadd));
+  variable.def(double() - py::self);
+  variable.def(py::self - double());
+  variable.def(py::self - py::self);
+  variable.def(py::self -= double(), DOC(sleipnir, Variable, operator, isub));
+  variable.def(py::self -= py::self, DOC(sleipnir, Variable, operator, isub));
+  variable.def(
+      "__pow__",
+      [](const Variable& self, int power) {
+        return sleipnir::pow(self, power);
+      },
+      py::is_operator());
+  variable.def(-py::self);
+  variable.def(+py::self);
+  variable.def("value", &Variable::Value, DOC(sleipnir, Variable, Value));
+  variable.def("type", &Variable::Type, DOC(sleipnir, Variable, Type));
+  variable.def("update", &Variable::Update, DOC(sleipnir, Variable, Update));
+  variable.def(py::self == py::self, DOC(sleipnir, operator, eq));
+  variable.def(py::self < py::self, DOC(sleipnir, operator, lt));
+  variable.def(py::self <= py::self, DOC(sleipnir, operator, le));
+  variable.def(py::self > py::self, DOC(sleipnir, operator, gt));
+  variable.def(py::self >= py::self, DOC(sleipnir, operator, ge));
+  variable.def(py::self == double(), DOC(sleipnir, operator, eq));
+  variable.def(py::self < double(), DOC(sleipnir, operator, lt));
+  variable.def(py::self <= double(), DOC(sleipnir, operator, le));
+  variable.def(py::self > double(), DOC(sleipnir, operator, gt));
+  variable.def(py::self >= double(), DOC(sleipnir, operator, ge));
+  variable.def(double() == py::self, DOC(sleipnir, operator, eq));
+  variable.def(double() < py::self, DOC(sleipnir, operator, lt));
+  variable.def(double() <= py::self, DOC(sleipnir, operator, le));
+  variable.def(double() > py::self, DOC(sleipnir, operator, gt));
+  variable.def(double() >= py::self, DOC(sleipnir, operator, ge));
+
+  autodiff.def(
+      "abs", [](double x) { return sleipnir::abs(Variable{x}); },
+      DOC(sleipnir, abs));
+  autodiff.def("abs", static_cast<Variable (*)(const Variable&)>(&abs),
+               DOC(sleipnir, abs));
+  autodiff.def(
+      "acos", [](double x) { return sleipnir::acos(Variable{x}); },
+      DOC(sleipnir, acos));
+  autodiff.def("acos", static_cast<Variable (*)(const Variable&)>(&acos),
+               DOC(sleipnir, acos));
+  autodiff.def(
+      "asin", [](double x) { return sleipnir::asin(Variable{x}); },
+      DOC(sleipnir, asin));
+  autodiff.def("asin", static_cast<Variable (*)(const Variable&)>(&asin),
+               DOC(sleipnir, asin));
+  autodiff.def(
+      "atan", [](double x) { return sleipnir::atan(Variable{x}); },
+      DOC(sleipnir, atan));
+  autodiff.def("atan", static_cast<Variable (*)(const Variable&)>(&atan),
+               DOC(sleipnir, atan));
+  autodiff.def(
+      "atan2",
+      [](double y, const Variable& x) { return sleipnir::atan2(y, x); },
+      DOC(sleipnir, atan2));
+  autodiff.def(
+      "atan2",
+      [](const Variable& y, double x) { return sleipnir::atan2(y, x); },
+      DOC(sleipnir, atan2));
+  autodiff.def(
+      "atan2",
+      [](const Variable& y, const Variable& x) {
+        return sleipnir::atan2(y, x);
+      },
+      DOC(sleipnir, atan2));
+  autodiff.def(
+      "cos", [](double x) { return sleipnir::cos(Variable{x}); },
+      DOC(sleipnir, cos));
+  autodiff.def("cos", static_cast<Variable (*)(const Variable&)>(&cos),
+               DOC(sleipnir, cos));
+  autodiff.def(
+      "cosh", [](double x) { return sleipnir::cosh(Variable{x}); },
+      DOC(sleipnir, cosh));
+  autodiff.def("cosh", static_cast<Variable (*)(const Variable&)>(&cosh),
+               DOC(sleipnir, cosh));
+  autodiff.def(
+      "erf", [](double x) { return sleipnir::erf(Variable{x}); },
+      DOC(sleipnir, erf));
+  autodiff.def("erf", static_cast<Variable (*)(const Variable&)>(&erf),
+               DOC(sleipnir, erf));
+  autodiff.def(
+      "exp", [](double x) { return sleipnir::exp(Variable{x}); },
+      DOC(sleipnir, exp));
+  autodiff.def("exp", static_cast<Variable (*)(const Variable&)>(&exp),
+               DOC(sleipnir, exp));
+  autodiff.def(
+      "hypot",
+      [](double x, const Variable& y) { return sleipnir::hypot(x, y); },
+      DOC(sleipnir, hypot));
+  autodiff.def(
+      "hypot",
+      [](const Variable& x, double y) { return sleipnir::hypot(x, y); },
+      DOC(sleipnir, hypot));
+  autodiff.def(
+      "hypot",
+      static_cast<Variable (*)(const Variable&, const Variable&)>(&hypot),
+      DOC(sleipnir, hypot));
+  autodiff.def("hypot",
+               static_cast<Variable (*)(const Variable&, const Variable&,
+                                        const Variable&)>(&hypot),
+               DOC(sleipnir, hypot, 2));
+  autodiff.def(
+      "log", [](double x) { return sleipnir::log(Variable{x}); },
+      DOC(sleipnir, log));
+  autodiff.def("log", static_cast<Variable (*)(const Variable&)>(&log),
+               DOC(sleipnir, log));
+  autodiff.def(
+      "log10", [](double x) { return sleipnir::log10(Variable{x}); },
+      DOC(sleipnir, log10));
+  autodiff.def("log10", static_cast<Variable (*)(const Variable&)>(&log10),
+               DOC(sleipnir, log10));
+  autodiff.def(
+      "pow",
+      [](double base, const Variable& power) {
+        return sleipnir::pow(base, power);
+      },
+      DOC(sleipnir, pow));
+  autodiff.def(
+      "pow",
+      [](const Variable& base, double power) {
+        return sleipnir::pow(base, power);
+      },
+      DOC(sleipnir, pow));
+  autodiff.def(
+      "pow", static_cast<Variable (*)(const Variable&, const Variable&)>(&pow),
+      DOC(sleipnir, pow));
+  autodiff.def(
+      "sign", [](double x) { return sleipnir::sign(Variable{x}); },
+      DOC(sleipnir, sign));
+  autodiff.def("sign", static_cast<Variable (*)(const Variable&)>(&sign),
+               DOC(sleipnir, sign));
+  autodiff.def(
+      "sin", [](double x) { return sleipnir::sin(Variable{x}); },
+      DOC(sleipnir, sin));
+  autodiff.def("sin", static_cast<Variable (*)(const Variable&)>(&sin),
+               DOC(sleipnir, sin));
+  autodiff.def(
+      "sinh", [](double x) { return sleipnir::sinh(Variable{x}); },
+      DOC(sleipnir, sinh));
+  autodiff.def("sinh", static_cast<Variable (*)(const Variable&)>(&sinh),
+               DOC(sleipnir, sinh));
+  autodiff.def(
+      "sqrt", [](double x) { return sleipnir::sqrt(Variable{x}); },
+      DOC(sleipnir, sqrt));
+  autodiff.def("sqrt", static_cast<Variable (*)(const Variable&)>(&sqrt),
+               DOC(sleipnir, sqrt));
+  autodiff.def(
+      "tan", [](double x) { return sleipnir::tan(Variable{x}); },
+      DOC(sleipnir, tan));
+  autodiff.def("tan", static_cast<Variable (*)(const Variable&)>(&tan),
+               DOC(sleipnir, tan));
+  autodiff.def(
+      "tanh", [](double x) { return sleipnir::tanh(Variable{x}); },
+      DOC(sleipnir, tanh));
+  autodiff.def("tanh", static_cast<Variable (*)(const Variable&)>(&tanh),
+               DOC(sleipnir, tanh));
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindVariableBlock.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindVariableBlock.cpp`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,477 +1,477 @@
-// Copyright (c) Sleipnir contributors
-
-#include <fmt/format.h>
-#include <pybind11/eigen.h>
-#include <pybind11/functional.h>
-#include <pybind11/operators.h>
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
-#include <sleipnir/autodiff/VariableBlock.hpp>
-#include <sleipnir/optimization/Constraints.hpp>
-
-#include "Docstrings.hpp"
-#include "NumPy.hpp"
-
-namespace py = pybind11;
-
-namespace sleipnir {
-
-void BindVariableBlock(py::module_& autodiff) {
-  py::class_<VariableBlock<VariableMatrix>> variable_block{
-      autodiff, "VariableBlock", DOC(sleipnir, VariableBlock)};
-
-  // VariableBlock-VariableMatrix overloads
-  variable_block.def(py::self * VariableMatrix());
-  variable_block.def(py::self + VariableMatrix());
-  variable_block.def(py::self - VariableMatrix());
-  variable_block.def(py::self == VariableMatrix(), DOC(sleipnir, operator, eq));
-  variable_block.def(py::self < VariableMatrix(), DOC(sleipnir, operator, lt));
-  variable_block.def(py::self <= VariableMatrix(), DOC(sleipnir, operator, le));
-  variable_block.def(py::self > VariableMatrix(), DOC(sleipnir, operator, gt));
-  variable_block.def(py::self >= VariableMatrix(), DOC(sleipnir, operator, ge));
-
-  variable_block.def(py::init<VariableMatrix&>(),
-                     DOC(sleipnir, VariableBlock, VariableBlock, 3));
-  variable_block.def(py::init<VariableMatrix&, int, int, int, int>(),
-                     DOC(sleipnir, VariableBlock, VariableBlock, 4));
-  variable_block.def(
-      "set",
-      [](VariableBlock<VariableMatrix>& self, double value) { self = value; },
-      DOC(sleipnir, VariableBlock, operator, assign, 3));
-  variable_block.def(
-      "set_value",
-      [](VariableBlock<VariableMatrix>& self, double value) {
-        self.SetValue(value);
-      },
-      DOC(sleipnir, VariableBlock, SetValue));
-  variable_block.def(
-      "set",
-      [](VariableBlock<VariableMatrix>& self, const Eigen::MatrixXd& values) {
-        self = values;
-      },
-      DOC(sleipnir, VariableBlock, operator, assign, 4));
-  variable_block.def(
-      "set_value",
-      [](VariableBlock<VariableMatrix>& self, const Eigen::MatrixXd& values) {
-        self.SetValue(values);
-      },
-      DOC(sleipnir, VariableBlock, SetValue, 2));
-  variable_block.def("__setitem__",
-                     [](VariableBlock<VariableMatrix>& self, int row,
-                        const Variable& value) { return self(row) = value; });
-  // TODO: Support slice stride other than 1
-  variable_block.def("__setitem__", [](VariableBlock<VariableMatrix>& self,
-                                       py::tuple slices, py::object value) {
-    if (slices.size() != 2) {
-      throw py::index_error(
-          fmt::format("Expected 2 slices, got {}.", slices.size()));
-    }
-
-    int rowOffset = 0;
-    int colOffset = 0;
-    int blockRows = self.Rows();
-    int blockCols = self.Cols();
-
-    size_t start;
-    size_t stop;
-    size_t step;
-    size_t sliceLength;
-
-    // Row slice
-    const auto& rowElem = slices[0];
-    if (py::isinstance<py::slice>(rowElem)) {
-      const auto& rowSlice = rowElem.cast<py::slice>();
-      if (!rowSlice.compute(self.Rows(), &start, &stop, &step, &sliceLength)) {
-        throw py::error_already_set();
-      }
-      rowOffset = start;
-      blockRows = stop - start;
-    } else {
-      rowOffset = rowElem.cast<int>();
-      blockRows = 1;
-    }
-
-    // Column slice
-    const auto& colElem = slices[1];
-    if (py::isinstance<py::slice>(colElem)) {
-      const auto& colSlice = colElem.cast<py::slice>();
-      if (!colSlice.compute(self.Cols(), &start, &stop, &step, &sliceLength)) {
-        throw py::error_already_set();
-      }
-      colOffset = start;
-      blockCols = stop - start;
-    } else {
-      colOffset = colElem.cast<int>();
-      blockCols = 1;
-    }
-
-    if (py::isinstance<VariableMatrix>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<VariableMatrix>();
-    } else if (py::isinstance<VariableBlock<VariableMatrix>>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<VariableBlock<VariableMatrix>>();
-    } else if (IsNumPyArithmeticArray(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<Eigen::MatrixXd>();
-    } else if (py::isinstance<Variable>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<Variable>();
-    } else if (py::isinstance<py::float_>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<double>();
-    } else if (py::isinstance<py::int_>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<int>();
-    } else {
-      throw py::value_error(
-          "VariableBlock.__setitem__ not implemented for value");
-    }
-  });
-  variable_block.def(
-      "__getitem__",
-      [](VariableBlock<VariableMatrix>& self, int row) -> Variable& {
-        if (row < 0) {
-          row = self.size() + row;
-        }
-        return self(row);
-      },
-      py::keep_alive<0, 1>(), DOC(sleipnir, VariableBlock, operator, call, 3));
-  // TODO: Support slice stride other than 1
-  variable_block.def(
-      "__getitem__",
-      [](VariableBlock<VariableMatrix>& self, py::tuple slices) -> py::object {
-        if (slices.size() != 2) {
-          throw py::index_error(
-              fmt::format("Expected 2 slices, got {}.", slices.size()));
-        }
-
-        // If both indices are integers instead of slices, return Variable
-        // instead of VariableBlock
-        if (py::isinstance<py::int_>(slices[0]) &&
-            py::isinstance<py::int_>(slices[1])) {
-          int row = slices[0].cast<int>();
-          int col = slices[1].cast<int>();
-
-          if (row >= self.Rows() || col >= self.Cols()) {
-            throw std::out_of_range("Index out of bounds");
-          }
-
-          if (row < 0) {
-            row = self.Rows() + row;
-          }
-          if (col < 0) {
-            col = self.Cols() + col;
-          }
-          return py::cast(self(row, col));
-        }
-
-        int rowOffset = 0;
-        int colOffset = 0;
-        int blockRows = self.Rows();
-        int blockCols = self.Cols();
-
-        size_t start;
-        size_t stop;
-        size_t step;
-        size_t sliceLength;
-
-        // Row slice
-        const auto& rowElem = slices[0];
-        if (py::isinstance<py::slice>(rowElem)) {
-          const auto& rowSlice = rowElem.cast<py::slice>();
-          if (!rowSlice.compute(self.Rows(), &start, &stop, &step,
-                                &sliceLength)) {
-            throw py::error_already_set();
-          }
-          rowOffset = start;
-          blockRows = stop - start;
-        } else {
-          rowOffset = rowElem.cast<int>();
-          if (rowOffset < 0) {
-            rowOffset = self.Rows() + rowOffset;
-          }
-          blockRows = 1;
-        }
-
-        // Column slice
-        const auto& colElem = slices[1];
-        if (py::isinstance<py::slice>(colElem)) {
-          const auto& colSlice = colElem.cast<py::slice>();
-          if (!colSlice.compute(self.Cols(), &start, &stop, &step,
-                                &sliceLength)) {
-            throw py::error_already_set();
-          }
-          colOffset = start;
-          blockCols = stop - start;
-        } else {
-          colOffset = colElem.cast<int>();
-          if (colOffset < 0) {
-            colOffset = self.Cols() + colOffset;
-          }
-          blockCols = 1;
-        }
-
-        return py::cast(self.Block(rowOffset, colOffset, blockRows, blockCols));
-      },
-      py::keep_alive<0, 1>(), DOC(sleipnir, VariableBlock, operator, call));
-  variable_block.def(
-      "row", py::overload_cast<int>(&VariableBlock<VariableMatrix>::Row),
-      DOC(sleipnir, VariableBlock, Row));
-  variable_block.def(
-      "col", py::overload_cast<int>(&VariableBlock<VariableMatrix>::Col),
-      DOC(sleipnir, VariableBlock, Col));
-  variable_block.def(
-      "__mul__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const VariableBlock<VariableMatrix>& rhs) { return lhs * rhs; },
-      py::is_operator());
-  variable_block.def(
-      "__rmul__",
-      [](const VariableBlock<VariableMatrix>& rhs,
-         const VariableBlock<VariableMatrix>& lhs) { return lhs * rhs; },
-      py::is_operator());
-  variable_block.def(
-      "__matmul__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const VariableBlock<VariableMatrix>& rhs) { return lhs * rhs; },
-      py::is_operator());
-
-  // https://numpy.org/doc/stable/user/basics.dispatch.html
-  variable_block.def(
-      "__array_ufunc__",
-      [](VariableBlock<VariableMatrix>& self, py::object ufunc, py::str method,
-         py::args inputs, const py::kwargs& kwargs) -> py::object {
-        std::string method_name = method;
-        std::string ufunc_name = ufunc.attr("__repr__")().cast<py::str>();
-
-        if (method_name == "__call__") {
-          if (ufunc_name == "<ufunc 'matmul'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() * self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self * inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'add'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() + self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self + inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'subtract'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() - self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self - inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'equal'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() == self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self == inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'less'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() < self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self < inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'less_equal'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() <= self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self <= inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'greater'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() > self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self > inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'greater_equal'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() >= self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self >= inputs[1].cast<Eigen::MatrixXd>());
-            }
-          }
-        }
-
-        std::string input1_name = inputs[0].attr("__repr__")().cast<py::str>();
-        std::string input2_name = inputs[1].attr("__repr__")().cast<py::str>();
-        throw py::value_error(
-            fmt::format("VariableBlock: numpy method {}, ufunc {} not "
-                        "implemented for ({}, {})",
-                        method_name, ufunc_name, input1_name, input2_name));
-        return py::cast(VariableMatrix{self});
-      });
-
-  variable_block.def(py::self * Variable());
-  variable_block.def(py::self * double());
-  variable_block.def(Variable() * py::self);
-  variable_block.def(double() * py::self);
-  variable_block.def(py::self / Variable());
-  variable_block.def(py::self / double());
-  variable_block.def(py::self + py::self);
-  variable_block.def(
-      "__add__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
-        return lhs + rhs;
-      },
-      py::is_operator());
-  variable_block.def(
-      "__add__",
-      [](const Eigen::Ref<const Eigen::MatrixXd>& lhs,
-         const VariableBlock<VariableMatrix>& rhs) -> VariableMatrix {
-        return lhs + rhs;
-      },
-      py::is_operator());
-  variable_block.def(py::self - py::self);
-  variable_block.def(
-      "__sub__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
-        return lhs - rhs;
-      },
-      py::is_operator());
-  variable_block.def(
-      "__sub__",
-      [](const Eigen::Ref<const Eigen::MatrixXd>& lhs,
-         const VariableBlock<VariableMatrix>& rhs) -> VariableMatrix {
-        return lhs - rhs;
-      },
-      py::is_operator());
-  variable_block.def(-py::self);
-  variable_block.def(
-      "__pow__",
-      [](const VariableBlock<VariableMatrix>& self, int power) {
-        return sleipnir::pow(VariableMatrix{self}, power);
-      },
-      py::is_operator());
-  variable_block.def_property_readonly("T", &VariableBlock<VariableMatrix>::T,
-                                       DOC(sleipnir, VariableBlock, T));
-  variable_block.def("rows", &VariableBlock<VariableMatrix>::Rows,
-                     DOC(sleipnir, VariableBlock, Rows));
-  variable_block.def("cols", &VariableBlock<VariableMatrix>::Cols,
-                     DOC(sleipnir, VariableBlock, Cols));
-  variable_block.def_property_readonly(
-      "shape", [](const VariableBlock<VariableMatrix>& self) {
-        return py::make_tuple(self.Rows(), self.Cols());
-      });
-  variable_block.def(
-      "value",
-      static_cast<double (VariableBlock<VariableMatrix>::*)(int, int) const>(
-          &VariableBlock<VariableMatrix>::Value),
-      DOC(sleipnir, VariableBlock, Value));
-  variable_block.def(
-      "value",
-      static_cast<double (VariableBlock<VariableMatrix>::*)(int) const>(
-          &VariableBlock<VariableMatrix>::Value),
-      DOC(sleipnir, VariableBlock, Value, 2));
-  variable_block.def(
-      "value",
-      static_cast<Eigen::MatrixXd (VariableBlock<VariableMatrix>::*)() const>(
-          &VariableBlock<VariableMatrix>::Value),
-      DOC(sleipnir, VariableBlock, Value, 3));
-  variable_block.def(
-      "cwise_transform",
-      [](const VariableBlock<VariableMatrix>& self,
-         const std::function<Variable(const Variable&)>& func) {
-        return self.CwiseTransform(func);
-      },
-      DOC(sleipnir, VariableBlock, CwiseTransform));
-  variable_block.def(py::self == py::self, DOC(sleipnir, operator, eq));
-  variable_block.def(py::self == Variable(), DOC(sleipnir, operator, eq));
-  variable_block.def(py::self == double(), DOC(sleipnir, operator, eq));
-  variable_block.def(py::self == int(), DOC(sleipnir, operator, eq));
-  variable_block.def(Variable() == py::self, DOC(sleipnir, operator, eq));
-  variable_block.def(double() == py::self, DOC(sleipnir, operator, eq));
-  variable_block.def(int() == py::self, DOC(sleipnir, operator, eq));
-  variable_block.def(py::self < py::self, DOC(sleipnir, operator, lt));
-  variable_block.def(py::self < Variable(), DOC(sleipnir, operator, lt));
-  variable_block.def(py::self < double(), DOC(sleipnir, operator, lt));
-  variable_block.def(py::self < int(), DOC(sleipnir, operator, lt));
-  variable_block.def(Variable() < py::self, DOC(sleipnir, operator, lt));
-  variable_block.def(double() < py::self, DOC(sleipnir, operator, lt));
-  variable_block.def(int() < py::self, DOC(sleipnir, operator, lt));
-  variable_block.def(py::self <= py::self, DOC(sleipnir, operator, le));
-  variable_block.def(py::self <= Variable(), DOC(sleipnir, operator, le));
-  variable_block.def(py::self <= double(), DOC(sleipnir, operator, le));
-  variable_block.def(py::self <= int(), DOC(sleipnir, operator, le));
-  variable_block.def(Variable() <= py::self, DOC(sleipnir, operator, le));
-  variable_block.def(double() <= py::self, DOC(sleipnir, operator, le));
-  variable_block.def(int() <= py::self, DOC(sleipnir, operator, le));
-  variable_block.def(py::self > py::self, DOC(sleipnir, operator, gt));
-  variable_block.def(py::self > Variable(), DOC(sleipnir, operator, gt));
-  variable_block.def(py::self > double(), DOC(sleipnir, operator, gt));
-  variable_block.def(py::self > int(), DOC(sleipnir, operator, gt));
-  variable_block.def(Variable() > py::self, DOC(sleipnir, operator, gt));
-  variable_block.def(double() > py::self, DOC(sleipnir, operator, gt));
-  variable_block.def(int() > py::self, DOC(sleipnir, operator, gt));
-  variable_block.def(py::self >= py::self, DOC(sleipnir, operator, ge));
-  variable_block.def(py::self >= Variable(), DOC(sleipnir, operator, ge));
-  variable_block.def(py::self >= double(), DOC(sleipnir, operator, ge));
-  variable_block.def(py::self >= int(), DOC(sleipnir, operator, ge));
-  variable_block.def(Variable() >= py::self, DOC(sleipnir, operator, ge));
-  variable_block.def(double() >= py::self, DOC(sleipnir, operator, ge));
-  variable_block.def(int() >= py::self, DOC(sleipnir, operator, ge));
-  variable_block.def(
-      "__eq__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const py::array_t<double>& rhs) {
-        return lhs == rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, eq));
-  variable_block.def(
-      "__lt__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const py::array_t<double>& rhs) {
-        return lhs < rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, lt));
-  variable_block.def(
-      "__le__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const py::array_t<double>& rhs) {
-        return lhs <= rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, le));
-  variable_block.def(
-      "__gt__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const py::array_t<double>& rhs) {
-        return lhs > rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, gt));
-  variable_block.def(
-      "__ge__",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const py::array_t<double>& rhs) {
-        return lhs >= rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, ge));
-
-  variable_block.def("__len__", &VariableBlock<VariableMatrix>::Rows,
-                     DOC(sleipnir, VariableBlock, Rows));
-
-  variable_block.def(
-      "__iter__",
-      [](const VariableBlock<VariableMatrix>& self) {
-        return py::make_iterator(self.begin(), self.end());
-      },
-      py::keep_alive<0, 1>());
-
-  py::implicitly_convertible<VariableBlock<VariableMatrix>, VariableMatrix>();
-
-  autodiff.def(
-      "cwise_reduce",
-      [](const VariableBlock<VariableMatrix>& lhs,
-         const VariableBlock<VariableMatrix>& rhs,
-         const std::function<Variable(const Variable&, const Variable&)> func) {
-        return CwiseReduce(lhs, rhs, func);
-      },
-      DOC(sleipnir, CwiseReduce));
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include <fmt/format.h>
+#include <pybind11/eigen.h>
+#include <pybind11/functional.h>
+#include <pybind11/operators.h>
+#include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
+#include <sleipnir/autodiff/VariableBlock.hpp>
+#include <sleipnir/optimization/Constraints.hpp>
+
+#include "Docstrings.hpp"
+#include "NumPy.hpp"
+
+namespace py = pybind11;
+
+namespace sleipnir {
+
+void BindVariableBlock(py::module_& autodiff) {
+  py::class_<VariableBlock<VariableMatrix>> variable_block{
+      autodiff, "VariableBlock", DOC(sleipnir, VariableBlock)};
+
+  // VariableBlock-VariableMatrix overloads
+  variable_block.def(py::self * VariableMatrix());
+  variable_block.def(py::self + VariableMatrix());
+  variable_block.def(py::self - VariableMatrix());
+  variable_block.def(py::self == VariableMatrix(), DOC(sleipnir, operator, eq));
+  variable_block.def(py::self < VariableMatrix(), DOC(sleipnir, operator, lt));
+  variable_block.def(py::self <= VariableMatrix(), DOC(sleipnir, operator, le));
+  variable_block.def(py::self > VariableMatrix(), DOC(sleipnir, operator, gt));
+  variable_block.def(py::self >= VariableMatrix(), DOC(sleipnir, operator, ge));
+
+  variable_block.def(py::init<VariableMatrix&>(),
+                     DOC(sleipnir, VariableBlock, VariableBlock, 3));
+  variable_block.def(py::init<VariableMatrix&, int, int, int, int>(),
+                     DOC(sleipnir, VariableBlock, VariableBlock, 4));
+  variable_block.def(
+      "set",
+      [](VariableBlock<VariableMatrix>& self, double value) { self = value; },
+      DOC(sleipnir, VariableBlock, operator, assign, 3));
+  variable_block.def(
+      "set_value",
+      [](VariableBlock<VariableMatrix>& self, double value) {
+        self.SetValue(value);
+      },
+      DOC(sleipnir, VariableBlock, SetValue));
+  variable_block.def(
+      "set",
+      [](VariableBlock<VariableMatrix>& self, const Eigen::MatrixXd& values) {
+        self = values;
+      },
+      DOC(sleipnir, VariableBlock, operator, assign, 4));
+  variable_block.def(
+      "set_value",
+      [](VariableBlock<VariableMatrix>& self, const Eigen::MatrixXd& values) {
+        self.SetValue(values);
+      },
+      DOC(sleipnir, VariableBlock, SetValue, 2));
+  variable_block.def("__setitem__",
+                     [](VariableBlock<VariableMatrix>& self, int row,
+                        const Variable& value) { return self(row) = value; });
+  // TODO: Support slice stride other than 1
+  variable_block.def("__setitem__", [](VariableBlock<VariableMatrix>& self,
+                                       py::tuple slices, py::object value) {
+    if (slices.size() != 2) {
+      throw py::index_error(
+          fmt::format("Expected 2 slices, got {}.", slices.size()));
+    }
+
+    int rowOffset = 0;
+    int colOffset = 0;
+    int blockRows = self.Rows();
+    int blockCols = self.Cols();
+
+    size_t start;
+    size_t stop;
+    size_t step;
+    size_t sliceLength;
+
+    // Row slice
+    const auto& rowElem = slices[0];
+    if (py::isinstance<py::slice>(rowElem)) {
+      const auto& rowSlice = rowElem.cast<py::slice>();
+      if (!rowSlice.compute(self.Rows(), &start, &stop, &step, &sliceLength)) {
+        throw py::error_already_set();
+      }
+      rowOffset = start;
+      blockRows = stop - start;
+    } else {
+      rowOffset = rowElem.cast<int>();
+      blockRows = 1;
+    }
+
+    // Column slice
+    const auto& colElem = slices[1];
+    if (py::isinstance<py::slice>(colElem)) {
+      const auto& colSlice = colElem.cast<py::slice>();
+      if (!colSlice.compute(self.Cols(), &start, &stop, &step, &sliceLength)) {
+        throw py::error_already_set();
+      }
+      colOffset = start;
+      blockCols = stop - start;
+    } else {
+      colOffset = colElem.cast<int>();
+      blockCols = 1;
+    }
+
+    if (py::isinstance<VariableMatrix>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<VariableMatrix>();
+    } else if (py::isinstance<VariableBlock<VariableMatrix>>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<VariableBlock<VariableMatrix>>();
+    } else if (IsNumPyArithmeticArray(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<Eigen::MatrixXd>();
+    } else if (py::isinstance<Variable>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<Variable>();
+    } else if (py::isinstance<py::float_>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<double>();
+    } else if (py::isinstance<py::int_>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<int>();
+    } else {
+      throw py::value_error(
+          "VariableBlock.__setitem__ not implemented for value");
+    }
+  });
+  variable_block.def(
+      "__getitem__",
+      [](VariableBlock<VariableMatrix>& self, int row) -> Variable& {
+        if (row < 0) {
+          row = self.size() + row;
+        }
+        return self(row);
+      },
+      py::keep_alive<0, 1>(), DOC(sleipnir, VariableBlock, operator, call, 3));
+  // TODO: Support slice stride other than 1
+  variable_block.def(
+      "__getitem__",
+      [](VariableBlock<VariableMatrix>& self, py::tuple slices) -> py::object {
+        if (slices.size() != 2) {
+          throw py::index_error(
+              fmt::format("Expected 2 slices, got {}.", slices.size()));
+        }
+
+        // If both indices are integers instead of slices, return Variable
+        // instead of VariableBlock
+        if (py::isinstance<py::int_>(slices[0]) &&
+            py::isinstance<py::int_>(slices[1])) {
+          int row = slices[0].cast<int>();
+          int col = slices[1].cast<int>();
+
+          if (row >= self.Rows() || col >= self.Cols()) {
+            throw std::out_of_range("Index out of bounds");
+          }
+
+          if (row < 0) {
+            row = self.Rows() + row;
+          }
+          if (col < 0) {
+            col = self.Cols() + col;
+          }
+          return py::cast(self(row, col));
+        }
+
+        int rowOffset = 0;
+        int colOffset = 0;
+        int blockRows = self.Rows();
+        int blockCols = self.Cols();
+
+        size_t start;
+        size_t stop;
+        size_t step;
+        size_t sliceLength;
+
+        // Row slice
+        const auto& rowElem = slices[0];
+        if (py::isinstance<py::slice>(rowElem)) {
+          const auto& rowSlice = rowElem.cast<py::slice>();
+          if (!rowSlice.compute(self.Rows(), &start, &stop, &step,
+                                &sliceLength)) {
+            throw py::error_already_set();
+          }
+          rowOffset = start;
+          blockRows = stop - start;
+        } else {
+          rowOffset = rowElem.cast<int>();
+          if (rowOffset < 0) {
+            rowOffset = self.Rows() + rowOffset;
+          }
+          blockRows = 1;
+        }
+
+        // Column slice
+        const auto& colElem = slices[1];
+        if (py::isinstance<py::slice>(colElem)) {
+          const auto& colSlice = colElem.cast<py::slice>();
+          if (!colSlice.compute(self.Cols(), &start, &stop, &step,
+                                &sliceLength)) {
+            throw py::error_already_set();
+          }
+          colOffset = start;
+          blockCols = stop - start;
+        } else {
+          colOffset = colElem.cast<int>();
+          if (colOffset < 0) {
+            colOffset = self.Cols() + colOffset;
+          }
+          blockCols = 1;
+        }
+
+        return py::cast(self.Block(rowOffset, colOffset, blockRows, blockCols));
+      },
+      py::keep_alive<0, 1>(), DOC(sleipnir, VariableBlock, operator, call));
+  variable_block.def(
+      "row", py::overload_cast<int>(&VariableBlock<VariableMatrix>::Row),
+      DOC(sleipnir, VariableBlock, Row));
+  variable_block.def(
+      "col", py::overload_cast<int>(&VariableBlock<VariableMatrix>::Col),
+      DOC(sleipnir, VariableBlock, Col));
+  variable_block.def(
+      "__mul__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const VariableBlock<VariableMatrix>& rhs) { return lhs * rhs; },
+      py::is_operator());
+  variable_block.def(
+      "__rmul__",
+      [](const VariableBlock<VariableMatrix>& rhs,
+         const VariableBlock<VariableMatrix>& lhs) { return lhs * rhs; },
+      py::is_operator());
+  variable_block.def(
+      "__matmul__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const VariableBlock<VariableMatrix>& rhs) { return lhs * rhs; },
+      py::is_operator());
+
+  // https://numpy.org/doc/stable/user/basics.dispatch.html
+  variable_block.def(
+      "__array_ufunc__",
+      [](VariableBlock<VariableMatrix>& self, py::object ufunc, py::str method,
+         py::args inputs, const py::kwargs& kwargs) -> py::object {
+        std::string method_name = method;
+        std::string ufunc_name = ufunc.attr("__repr__")().cast<py::str>();
+
+        if (method_name == "__call__") {
+          if (ufunc_name == "<ufunc 'matmul'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() * self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self * inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'add'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() + self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self + inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'subtract'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() - self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self - inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'equal'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() == self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self == inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'less'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() < self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self < inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'less_equal'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() <= self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self <= inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'greater'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() > self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self > inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'greater_equal'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() >= self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self >= inputs[1].cast<Eigen::MatrixXd>());
+            }
+          }
+        }
+
+        std::string input1_name = inputs[0].attr("__repr__")().cast<py::str>();
+        std::string input2_name = inputs[1].attr("__repr__")().cast<py::str>();
+        throw py::value_error(
+            fmt::format("VariableBlock: numpy method {}, ufunc {} not "
+                        "implemented for ({}, {})",
+                        method_name, ufunc_name, input1_name, input2_name));
+        return py::cast(VariableMatrix{self});
+      });
+
+  variable_block.def(py::self * Variable());
+  variable_block.def(py::self * double());
+  variable_block.def(Variable() * py::self);
+  variable_block.def(double() * py::self);
+  variable_block.def(py::self / Variable());
+  variable_block.def(py::self / double());
+  variable_block.def(py::self + py::self);
+  variable_block.def(
+      "__add__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
+        return lhs + rhs;
+      },
+      py::is_operator());
+  variable_block.def(
+      "__add__",
+      [](const Eigen::Ref<const Eigen::MatrixXd>& lhs,
+         const VariableBlock<VariableMatrix>& rhs) -> VariableMatrix {
+        return lhs + rhs;
+      },
+      py::is_operator());
+  variable_block.def(py::self - py::self);
+  variable_block.def(
+      "__sub__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
+        return lhs - rhs;
+      },
+      py::is_operator());
+  variable_block.def(
+      "__sub__",
+      [](const Eigen::Ref<const Eigen::MatrixXd>& lhs,
+         const VariableBlock<VariableMatrix>& rhs) -> VariableMatrix {
+        return lhs - rhs;
+      },
+      py::is_operator());
+  variable_block.def(-py::self);
+  variable_block.def(
+      "__pow__",
+      [](const VariableBlock<VariableMatrix>& self, int power) {
+        return sleipnir::pow(VariableMatrix{self}, power);
+      },
+      py::is_operator());
+  variable_block.def_property_readonly("T", &VariableBlock<VariableMatrix>::T,
+                                       DOC(sleipnir, VariableBlock, T));
+  variable_block.def("rows", &VariableBlock<VariableMatrix>::Rows,
+                     DOC(sleipnir, VariableBlock, Rows));
+  variable_block.def("cols", &VariableBlock<VariableMatrix>::Cols,
+                     DOC(sleipnir, VariableBlock, Cols));
+  variable_block.def_property_readonly(
+      "shape", [](const VariableBlock<VariableMatrix>& self) {
+        return py::make_tuple(self.Rows(), self.Cols());
+      });
+  variable_block.def(
+      "value",
+      static_cast<double (VariableBlock<VariableMatrix>::*)(int, int) const>(
+          &VariableBlock<VariableMatrix>::Value),
+      DOC(sleipnir, VariableBlock, Value));
+  variable_block.def(
+      "value",
+      static_cast<double (VariableBlock<VariableMatrix>::*)(int) const>(
+          &VariableBlock<VariableMatrix>::Value),
+      DOC(sleipnir, VariableBlock, Value, 2));
+  variable_block.def(
+      "value",
+      static_cast<Eigen::MatrixXd (VariableBlock<VariableMatrix>::*)() const>(
+          &VariableBlock<VariableMatrix>::Value),
+      DOC(sleipnir, VariableBlock, Value, 3));
+  variable_block.def(
+      "cwise_transform",
+      [](const VariableBlock<VariableMatrix>& self,
+         const std::function<Variable(const Variable&)>& func) {
+        return self.CwiseTransform(func);
+      },
+      DOC(sleipnir, VariableBlock, CwiseTransform));
+  variable_block.def(py::self == py::self, DOC(sleipnir, operator, eq));
+  variable_block.def(py::self == Variable(), DOC(sleipnir, operator, eq));
+  variable_block.def(py::self == double(), DOC(sleipnir, operator, eq));
+  variable_block.def(py::self == int(), DOC(sleipnir, operator, eq));
+  variable_block.def(Variable() == py::self, DOC(sleipnir, operator, eq));
+  variable_block.def(double() == py::self, DOC(sleipnir, operator, eq));
+  variable_block.def(int() == py::self, DOC(sleipnir, operator, eq));
+  variable_block.def(py::self < py::self, DOC(sleipnir, operator, lt));
+  variable_block.def(py::self < Variable(), DOC(sleipnir, operator, lt));
+  variable_block.def(py::self < double(), DOC(sleipnir, operator, lt));
+  variable_block.def(py::self < int(), DOC(sleipnir, operator, lt));
+  variable_block.def(Variable() < py::self, DOC(sleipnir, operator, lt));
+  variable_block.def(double() < py::self, DOC(sleipnir, operator, lt));
+  variable_block.def(int() < py::self, DOC(sleipnir, operator, lt));
+  variable_block.def(py::self <= py::self, DOC(sleipnir, operator, le));
+  variable_block.def(py::self <= Variable(), DOC(sleipnir, operator, le));
+  variable_block.def(py::self <= double(), DOC(sleipnir, operator, le));
+  variable_block.def(py::self <= int(), DOC(sleipnir, operator, le));
+  variable_block.def(Variable() <= py::self, DOC(sleipnir, operator, le));
+  variable_block.def(double() <= py::self, DOC(sleipnir, operator, le));
+  variable_block.def(int() <= py::self, DOC(sleipnir, operator, le));
+  variable_block.def(py::self > py::self, DOC(sleipnir, operator, gt));
+  variable_block.def(py::self > Variable(), DOC(sleipnir, operator, gt));
+  variable_block.def(py::self > double(), DOC(sleipnir, operator, gt));
+  variable_block.def(py::self > int(), DOC(sleipnir, operator, gt));
+  variable_block.def(Variable() > py::self, DOC(sleipnir, operator, gt));
+  variable_block.def(double() > py::self, DOC(sleipnir, operator, gt));
+  variable_block.def(int() > py::self, DOC(sleipnir, operator, gt));
+  variable_block.def(py::self >= py::self, DOC(sleipnir, operator, ge));
+  variable_block.def(py::self >= Variable(), DOC(sleipnir, operator, ge));
+  variable_block.def(py::self >= double(), DOC(sleipnir, operator, ge));
+  variable_block.def(py::self >= int(), DOC(sleipnir, operator, ge));
+  variable_block.def(Variable() >= py::self, DOC(sleipnir, operator, ge));
+  variable_block.def(double() >= py::self, DOC(sleipnir, operator, ge));
+  variable_block.def(int() >= py::self, DOC(sleipnir, operator, ge));
+  variable_block.def(
+      "__eq__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const py::array_t<double>& rhs) {
+        return lhs == rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, eq));
+  variable_block.def(
+      "__lt__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const py::array_t<double>& rhs) {
+        return lhs < rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, lt));
+  variable_block.def(
+      "__le__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const py::array_t<double>& rhs) {
+        return lhs <= rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, le));
+  variable_block.def(
+      "__gt__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const py::array_t<double>& rhs) {
+        return lhs > rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, gt));
+  variable_block.def(
+      "__ge__",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const py::array_t<double>& rhs) {
+        return lhs >= rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, ge));
+
+  variable_block.def("__len__", &VariableBlock<VariableMatrix>::Rows,
+                     DOC(sleipnir, VariableBlock, Rows));
+
+  variable_block.def(
+      "__iter__",
+      [](const VariableBlock<VariableMatrix>& self) {
+        return py::make_iterator(self.begin(), self.end());
+      },
+      py::keep_alive<0, 1>());
+
+  py::implicitly_convertible<VariableBlock<VariableMatrix>, VariableMatrix>();
+
+  autodiff.def(
+      "cwise_reduce",
+      [](const VariableBlock<VariableMatrix>& lhs,
+         const VariableBlock<VariableMatrix>& rhs,
+         const std::function<Variable(const Variable&, const Variable&)> func) {
+        return CwiseReduce(lhs, rhs, func);
+      },
+      DOC(sleipnir, CwiseReduce));
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/cpp/autodiff/BindVariableMatrix.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/cpp/autodiff/BindVariableMatrix.cpp`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,575 +1,575 @@
-// Copyright (c) Sleipnir contributors
-
-#include <fmt/format.h>
-#include <pybind11/eigen.h>
-#include <pybind11/functional.h>
-#include <pybind11/operators.h>
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
-#include <sleipnir/autodiff/VariableMatrix.hpp>
-#include <sleipnir/optimization/Constraints.hpp>
-
-#include "Docstrings.hpp"
-#include "NumPy.hpp"
-
-namespace py = pybind11;
-
-namespace sleipnir {
-
-void BindVariableMatrix(py::module_& autodiff) {
-  py::class_<VariableMatrix> variable_matrix{autodiff, "VariableMatrix",
-                                             DOC(sleipnir, VariableMatrix)};
-
-  variable_matrix.def(py::init<>(),
-                      DOC(sleipnir, VariableMatrix, VariableMatrix));
-  variable_matrix.def(py::init<int>(),
-                      DOC(sleipnir, VariableMatrix, VariableMatrix, 2));
-  variable_matrix.def(py::init<int, int>(),
-                      DOC(sleipnir, VariableMatrix, VariableMatrix, 3));
-  variable_matrix.def(py::init<std::vector<std::vector<double>>>(),
-                      DOC(sleipnir, VariableMatrix, VariableMatrix, 5));
-  variable_matrix.def(py::init<std::vector<std::vector<Variable>>>(),
-                      DOC(sleipnir, VariableMatrix, VariableMatrix, 6));
-  variable_matrix.def(py::init<const Variable&>(),
-                      DOC(sleipnir, VariableMatrix, VariableMatrix, 9));
-  variable_matrix.def(py::init<const VariableBlock<VariableMatrix>&>(),
-                      DOC(sleipnir, VariableMatrix, VariableMatrix, 11));
-  variable_matrix.def(
-      "set",
-      [](VariableMatrix& self, const Eigen::MatrixXd& values) {
-        self = values;
-      },
-      DOC(sleipnir, VariableMatrix, operator, assign));
-  variable_matrix.def(
-      "set_value",
-      [](VariableMatrix& self, const Eigen::MatrixXd& values) {
-        self.SetValue(values);
-      },
-      DOC(sleipnir, VariableMatrix, SetValue));
-  variable_matrix.def("__setitem__",
-                      [](VariableMatrix& self, int row, const Variable& value) {
-                        return self(row) = value;
-                      });
-  // TODO: Support slice stride other than 1
-  variable_matrix.def("__setitem__", [](VariableMatrix& self, py::tuple slices,
-                                        py::object value) {
-    if (slices.size() != 2) {
-      throw py::index_error(
-          fmt::format("Expected 2 slices, got {}.", slices.size()));
-    }
-
-    int rowOffset = 0;
-    int colOffset = 0;
-    int blockRows = self.Rows();
-    int blockCols = self.Cols();
-
-    size_t start;
-    size_t stop;
-    size_t step;
-    size_t sliceLength;
-
-    // Row slice
-    const auto& rowElem = slices[0];
-    if (py::isinstance<py::slice>(rowElem)) {
-      const auto& rowSlice = rowElem.cast<py::slice>();
-      if (!rowSlice.compute(self.Rows(), &start, &stop, &step, &sliceLength)) {
-        throw py::error_already_set();
-      }
-      rowOffset = start;
-      blockRows = stop - start;
-    } else {
-      rowOffset = rowElem.cast<int>();
-      blockRows = 1;
-    }
-
-    // Column slice
-    const auto& colElem = slices[1];
-    if (py::isinstance<py::slice>(colElem)) {
-      const auto& colSlice = colElem.cast<py::slice>();
-      if (!colSlice.compute(self.Cols(), &start, &stop, &step, &sliceLength)) {
-        throw py::error_already_set();
-      }
-      colOffset = start;
-      blockCols = stop - start;
-    } else {
-      colOffset = colElem.cast<int>();
-      blockCols = 1;
-    }
-
-    if (py::isinstance<VariableMatrix>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<VariableMatrix>();
-    } else if (py::isinstance<VariableBlock<VariableMatrix>>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<VariableBlock<VariableMatrix>>();
-    } else if (IsNumPyArithmeticArray(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<Eigen::MatrixXd>();
-    } else if (py::isinstance<Variable>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<Variable>();
-    } else if (py::isinstance<py::float_>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<double>();
-    } else if (py::isinstance<py::int_>(value)) {
-      self.Block(rowOffset, colOffset, blockRows, blockCols) =
-          value.cast<int>();
-    } else {
-      throw py::value_error(
-          "VariableMatrix.__setitem__ not implemented for value");
-    }
-  });
-  variable_matrix.def(
-      "__getitem__",
-      [](VariableMatrix& self, int row) -> Variable& {
-        if (row < 0) {
-          row = self.size() + row;
-        }
-        return self(row);
-      },
-      py::keep_alive<0, 1>(), DOC(sleipnir, VariableMatrix, operator, call, 3));
-  // TODO: Support slice stride other than 1
-  variable_matrix.def(
-      "__getitem__",
-      [](VariableMatrix& self, py::tuple slices) -> py::object {
-        if (slices.size() != 2) {
-          throw py::index_error(
-              fmt::format("Expected 2 slices, got {}.", slices.size()));
-        }
-
-        // If both indices are integers instead of slices, return Variable
-        // instead of VariableBlock
-        if (py::isinstance<py::int_>(slices[0]) &&
-            py::isinstance<py::int_>(slices[1])) {
-          int row = slices[0].cast<int>();
-          int col = slices[1].cast<int>();
-
-          if (row >= self.Rows() || col >= self.Cols()) {
-            throw std::out_of_range("Index out of bounds");
-          }
-
-          if (row < 0) {
-            row = self.Rows() + row;
-          }
-          if (col < 0) {
-            col = self.Cols() + col;
-          }
-          return py::cast(self(row, col));
-        }
-
-        int rowOffset = 0;
-        int colOffset = 0;
-        int blockRows = self.Rows();
-        int blockCols = self.Cols();
-
-        size_t start;
-        size_t stop;
-        size_t step;
-        size_t sliceLength;
-
-        // Row slice
-        const auto& rowElem = slices[0];
-        if (py::isinstance<py::slice>(rowElem)) {
-          const auto& rowSlice = rowElem.cast<py::slice>();
-          if (!rowSlice.compute(self.Rows(), &start, &stop, &step,
-                                &sliceLength)) {
-            throw py::error_already_set();
-          }
-          rowOffset = start;
-          blockRows = stop - start;
-        } else {
-          rowOffset = rowElem.cast<int>();
-          if (rowOffset < 0) {
-            rowOffset = self.Rows() + rowOffset;
-          }
-          blockRows = 1;
-        }
-
-        // Column slice
-        const auto& colElem = slices[1];
-        if (py::isinstance<py::slice>(colElem)) {
-          const auto& colSlice = colElem.cast<py::slice>();
-          if (!colSlice.compute(self.Cols(), &start, &stop, &step,
-                                &sliceLength)) {
-            throw py::error_already_set();
-          }
-          colOffset = start;
-          blockCols = stop - start;
-        } else {
-          colOffset = colElem.cast<int>();
-          if (colOffset < 0) {
-            colOffset = self.Cols() + colOffset;
-          }
-          blockCols = 1;
-        }
-
-        return py::cast(self.Block(rowOffset, colOffset, blockRows, blockCols));
-      },
-      py::keep_alive<0, 1>(), DOC(sleipnir, VariableMatrix, operator, call));
-  variable_matrix.def("row", py::overload_cast<int>(&VariableMatrix::Row),
-                      DOC(sleipnir, VariableMatrix, Row));
-  variable_matrix.def("col", py::overload_cast<int>(&VariableMatrix::Col),
-                      DOC(sleipnir, VariableMatrix, Col));
-  variable_matrix.def(
-      "__mul__",
-      [](const VariableMatrix& lhs, const VariableMatrix& rhs) {
-        return lhs * rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__rmul__",
-      [](const VariableMatrix& rhs, const VariableMatrix& lhs) {
-        return lhs * rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__matmul__",
-      [](const VariableMatrix& lhs, const VariableMatrix& rhs) {
-        return lhs * rhs;
-      },
-      py::is_operator());
-
-  // https://numpy.org/doc/stable/user/basics.dispatch.html
-  variable_matrix.def(
-      "__array_ufunc__",
-      [](VariableMatrix& self, py::object ufunc, py::str method,
-         py::args inputs, const py::kwargs& kwargs) -> py::object {
-        std::string method_name = method;
-        std::string ufunc_name = ufunc.attr("__repr__")().cast<py::str>();
-
-        if (method_name == "__call__") {
-          if (ufunc_name == "<ufunc 'matmul'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() * self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self * inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'add'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() + self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self + inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'subtract'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() - self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self - inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'equal'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() == self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self == inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'less'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() < self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self < inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'less_equal'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() <= self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self <= inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'greater'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() > self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self > inputs[1].cast<Eigen::MatrixXd>());
-            }
-          } else if (ufunc_name == "<ufunc 'greater_equal'>") {
-            if (IsNumPyArithmeticArray(inputs[0])) {
-              return py::cast(inputs[0].cast<Eigen::MatrixXd>() >= self);
-            } else if (IsNumPyArithmeticArray(inputs[1])) {
-              return py::cast(self >= inputs[1].cast<Eigen::MatrixXd>());
-            }
-          }
-        }
-
-        std::string input1_name = inputs[0].attr("__repr__")().cast<py::str>();
-        std::string input2_name = inputs[1].attr("__repr__")().cast<py::str>();
-        throw py::value_error(
-            fmt::format("VariableMatrix: numpy method {}, ufunc {} not "
-                        "implemented for ({}, {})",
-                        method_name, ufunc_name, input1_name, input2_name));
-        return py::cast(VariableMatrix{self});
-      });
-
-  variable_matrix.def(py::self * Variable());
-  variable_matrix.def(py::self * double());
-  variable_matrix.def(Variable() * py::self);
-  variable_matrix.def(double() * py::self);
-
-  variable_matrix.def(py::self / Variable());
-  variable_matrix.def(py::self / double());
-  variable_matrix.def(py::self /= Variable(),
-                      DOC(sleipnir, VariableMatrix, operator, idiv));
-  variable_matrix.def(py::self /= double(),
-                      DOC(sleipnir, VariableMatrix, operator, idiv));
-
-  variable_matrix.def(py::self + py::self);
-  variable_matrix.def(
-      "__add__",
-      [](const VariableMatrix& lhs, const Variable& rhs) {
-        return lhs + VariableMatrix{rhs};
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__radd__",
-      [](const VariableMatrix& rhs, const Variable& lhs) {
-        return VariableMatrix{lhs} + rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__add__",
-      [](double lhs, const VariableMatrix& rhs) {
-        return VariableMatrix{Variable{lhs}} + rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__radd__",
-      [](const VariableMatrix& rhs, double lhs) {
-        return VariableMatrix{Variable{lhs}} + rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__add__",
-      [](const VariableMatrix& lhs,
-         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
-        return lhs + rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__radd__",
-      [](const VariableMatrix& rhs,
-         const Eigen::Ref<const Eigen::MatrixXd>& lhs) -> VariableMatrix {
-        return lhs + rhs;
-      },
-      py::is_operator());
-
-  variable_matrix.def(py::self - py::self);
-  variable_matrix.def(
-      "__sub__",
-      [](const VariableMatrix& lhs, const Variable& rhs) {
-        return lhs - VariableMatrix{rhs};
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__rsub__",
-      [](const VariableMatrix& rhs, const Variable& lhs) {
-        return VariableMatrix{lhs} - rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__sub__",
-      [](const VariableMatrix& lhs,
-         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
-        return lhs - rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__rsub__",
-      [](const VariableMatrix& rhs,
-         const Eigen::Ref<const Eigen::MatrixXd>& lhs) -> VariableMatrix {
-        return lhs - rhs;
-      },
-      py::is_operator());
-
-  variable_matrix.def(-py::self);
-  variable_matrix.def(
-      "__pow__",
-      [](const VariableMatrix& self, int power) {
-        return sleipnir::pow(self, power);
-      },
-      py::is_operator());
-  variable_matrix.def_property_readonly("T", &VariableMatrix::T,
-                                        DOC(sleipnir, VariableMatrix, T));
-  variable_matrix.def("rows", &VariableMatrix::Rows,
-                      DOC(sleipnir, VariableMatrix, Rows));
-  variable_matrix.def("cols", &VariableMatrix::Cols,
-                      DOC(sleipnir, VariableMatrix, Cols));
-  variable_matrix.def_property_readonly(
-      "shape", [](const VariableMatrix& self) {
-        return py::make_tuple(self.Rows(), self.Cols());
-      });
-  variable_matrix.def("value",
-                      static_cast<double (VariableMatrix::*)(int, int) const>(
-                          &VariableMatrix::Value),
-                      DOC(sleipnir, VariableMatrix, Value));
-  variable_matrix.def("value",
-                      static_cast<double (VariableMatrix::*)(int) const>(
-                          &VariableMatrix::Value),
-                      DOC(sleipnir, VariableMatrix, Value, 2));
-  variable_matrix.def("value",
-                      static_cast<Eigen::MatrixXd (VariableMatrix::*)() const>(
-                          &VariableMatrix::Value),
-                      DOC(sleipnir, VariableMatrix, Value, 3));
-  variable_matrix.def(
-      "cwise_transform",
-      [](const VariableMatrix& self,
-         const std::function<Variable(const Variable&)>& func) {
-        return self.CwiseTransform(func);
-      },
-      DOC(sleipnir, VariableMatrix, CwiseTransform));
-  variable_matrix.def_static("zero", &VariableMatrix::Zero,
-                             DOC(sleipnir, VariableMatrix, Zero));
-  variable_matrix.def_static("ones", &VariableMatrix::Ones,
-                             DOC(sleipnir, VariableMatrix, Ones));
-  variable_matrix.def(py::self == py::self, DOC(sleipnir, operator, eq));
-  variable_matrix.def(py::self == Variable(), DOC(sleipnir, operator, eq));
-  variable_matrix.def(py::self == double(), DOC(sleipnir, operator, eq));
-  variable_matrix.def(py::self == int(), DOC(sleipnir, operator, eq));
-  variable_matrix.def(Variable() == py::self, DOC(sleipnir, operator, eq));
-  variable_matrix.def(double() == py::self, DOC(sleipnir, operator, eq));
-  variable_matrix.def(int() == py::self, DOC(sleipnir, operator, eq));
-  variable_matrix.def(py::self < py::self, DOC(sleipnir, operator, lt));
-  variable_matrix.def(py::self < Variable(), DOC(sleipnir, operator, lt));
-  variable_matrix.def(py::self < double(), DOC(sleipnir, operator, lt));
-  variable_matrix.def(py::self < int(), DOC(sleipnir, operator, lt));
-  variable_matrix.def(Variable() < py::self, DOC(sleipnir, operator, lt));
-  variable_matrix.def(double() < py::self, DOC(sleipnir, operator, lt));
-  variable_matrix.def(int() < py::self, DOC(sleipnir, operator, lt));
-  variable_matrix.def(py::self <= py::self, DOC(sleipnir, operator, le));
-  variable_matrix.def(py::self <= Variable(), DOC(sleipnir, operator, le));
-  variable_matrix.def(py::self <= double(), DOC(sleipnir, operator, le));
-  variable_matrix.def(py::self <= int(), DOC(sleipnir, operator, le));
-  variable_matrix.def(Variable() <= py::self, DOC(sleipnir, operator, le));
-  variable_matrix.def(double() <= py::self, DOC(sleipnir, operator, le));
-  variable_matrix.def(int() <= py::self, DOC(sleipnir, operator, le));
-  variable_matrix.def(py::self > py::self, DOC(sleipnir, operator, gt));
-  variable_matrix.def(py::self > Variable(), DOC(sleipnir, operator, gt));
-  variable_matrix.def(py::self > double(), DOC(sleipnir, operator, gt));
-  variable_matrix.def(py::self > int(), DOC(sleipnir, operator, gt));
-  variable_matrix.def(Variable() > py::self, DOC(sleipnir, operator, gt));
-  variable_matrix.def(double() > py::self, DOC(sleipnir, operator, gt));
-  variable_matrix.def(int() > py::self, DOC(sleipnir, operator, gt));
-  variable_matrix.def(py::self >= py::self, DOC(sleipnir, operator, ge));
-  variable_matrix.def(py::self >= Variable(), DOC(sleipnir, operator, ge));
-  variable_matrix.def(py::self >= double(), DOC(sleipnir, operator, ge));
-  variable_matrix.def(py::self >= int(), DOC(sleipnir, operator, ge));
-  variable_matrix.def(Variable() >= py::self, DOC(sleipnir, operator, ge));
-  variable_matrix.def(double() >= py::self, DOC(sleipnir, operator, ge));
-  variable_matrix.def(int() >= py::self, DOC(sleipnir, operator, ge));
-  py::implicitly_convertible<VariableMatrix, Variable>();
-
-  // VariableMatrix-VariableBlock overloads
-  variable_matrix.def(
-      "__mul__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs * rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__rmul__",
-      [](const VariableMatrix& rhs, const VariableBlock<VariableMatrix>& lhs) {
-        return lhs * rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__matmul__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs * rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__add__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs + rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__sub__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs - rhs;
-      },
-      py::is_operator());
-  variable_matrix.def(
-      "__eq__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs == rhs;
-      },
-      py::is_operator(), DOC(sleipnir, operator, eq));
-  variable_matrix.def(
-      "__lt__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs < rhs;
-      },
-      py::is_operator(), DOC(sleipnir, operator, lt));
-  variable_matrix.def(
-      "__le__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs <= rhs;
-      },
-      py::is_operator(), DOC(sleipnir, operator, le));
-  variable_matrix.def(
-      "__gt__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs > rhs;
-      },
-      py::is_operator(), DOC(sleipnir, operator, gt));
-  variable_matrix.def(
-      "__ge__",
-      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
-        return lhs >= rhs;
-      },
-      py::is_operator(), DOC(sleipnir, operator, ge));
-  variable_matrix.def(
-      "__eq__",
-      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
-        return lhs == rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, eq));
-  variable_matrix.def(
-      "__lt__",
-      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
-        return lhs < rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, lt));
-  variable_matrix.def(
-      "__le__",
-      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
-        return lhs <= rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, le));
-  variable_matrix.def(
-      "__gt__",
-      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
-        return lhs > rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, gt));
-  variable_matrix.def(
-      "__ge__",
-      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
-        return lhs >= rhs.cast<Eigen::MatrixXd>();
-      },
-      py::is_operator(), DOC(sleipnir, operator, ge));
-
-  variable_matrix.def("__len__", &VariableMatrix::Rows,
-                      DOC(sleipnir, VariableMatrix, Rows));
-
-  variable_matrix.def(
-      "__iter__",
-      [](const VariableMatrix& self) {
-        return py::make_iterator(self.begin(), self.end());
-      },
-      py::keep_alive<0, 1>());
-
-  autodiff.def(
-      "cwise_reduce",
-      [](const VariableMatrix& lhs, const VariableMatrix& rhs,
-         const std::function<Variable(const Variable&, const Variable&)> func) {
-        return CwiseReduce(lhs, rhs, func);
-      },
-      DOC(sleipnir, CwiseReduce));
-
-  autodiff.def(
-      "block",
-      static_cast<VariableMatrix (*)(std::vector<std::vector<VariableMatrix>>)>(
-          &Block),
-      DOC(sleipnir, Block));
-}  // NOLINT(readability/fn_size)
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include <fmt/format.h>
+#include <pybind11/eigen.h>
+#include <pybind11/functional.h>
+#include <pybind11/operators.h>
+#include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
+#include <sleipnir/autodiff/VariableMatrix.hpp>
+#include <sleipnir/optimization/Constraints.hpp>
+
+#include "Docstrings.hpp"
+#include "NumPy.hpp"
+
+namespace py = pybind11;
+
+namespace sleipnir {
+
+void BindVariableMatrix(py::module_& autodiff) {
+  py::class_<VariableMatrix> variable_matrix{autodiff, "VariableMatrix",
+                                             DOC(sleipnir, VariableMatrix)};
+
+  variable_matrix.def(py::init<>(),
+                      DOC(sleipnir, VariableMatrix, VariableMatrix));
+  variable_matrix.def(py::init<int>(),
+                      DOC(sleipnir, VariableMatrix, VariableMatrix, 2));
+  variable_matrix.def(py::init<int, int>(),
+                      DOC(sleipnir, VariableMatrix, VariableMatrix, 3));
+  variable_matrix.def(py::init<std::vector<std::vector<double>>>(),
+                      DOC(sleipnir, VariableMatrix, VariableMatrix, 5));
+  variable_matrix.def(py::init<std::vector<std::vector<Variable>>>(),
+                      DOC(sleipnir, VariableMatrix, VariableMatrix, 6));
+  variable_matrix.def(py::init<const Variable&>(),
+                      DOC(sleipnir, VariableMatrix, VariableMatrix, 9));
+  variable_matrix.def(py::init<const VariableBlock<VariableMatrix>&>(),
+                      DOC(sleipnir, VariableMatrix, VariableMatrix, 11));
+  variable_matrix.def(
+      "set",
+      [](VariableMatrix& self, const Eigen::MatrixXd& values) {
+        self = values;
+      },
+      DOC(sleipnir, VariableMatrix, operator, assign));
+  variable_matrix.def(
+      "set_value",
+      [](VariableMatrix& self, const Eigen::MatrixXd& values) {
+        self.SetValue(values);
+      },
+      DOC(sleipnir, VariableMatrix, SetValue));
+  variable_matrix.def("__setitem__",
+                      [](VariableMatrix& self, int row, const Variable& value) {
+                        return self(row) = value;
+                      });
+  // TODO: Support slice stride other than 1
+  variable_matrix.def("__setitem__", [](VariableMatrix& self, py::tuple slices,
+                                        py::object value) {
+    if (slices.size() != 2) {
+      throw py::index_error(
+          fmt::format("Expected 2 slices, got {}.", slices.size()));
+    }
+
+    int rowOffset = 0;
+    int colOffset = 0;
+    int blockRows = self.Rows();
+    int blockCols = self.Cols();
+
+    size_t start;
+    size_t stop;
+    size_t step;
+    size_t sliceLength;
+
+    // Row slice
+    const auto& rowElem = slices[0];
+    if (py::isinstance<py::slice>(rowElem)) {
+      const auto& rowSlice = rowElem.cast<py::slice>();
+      if (!rowSlice.compute(self.Rows(), &start, &stop, &step, &sliceLength)) {
+        throw py::error_already_set();
+      }
+      rowOffset = start;
+      blockRows = stop - start;
+    } else {
+      rowOffset = rowElem.cast<int>();
+      blockRows = 1;
+    }
+
+    // Column slice
+    const auto& colElem = slices[1];
+    if (py::isinstance<py::slice>(colElem)) {
+      const auto& colSlice = colElem.cast<py::slice>();
+      if (!colSlice.compute(self.Cols(), &start, &stop, &step, &sliceLength)) {
+        throw py::error_already_set();
+      }
+      colOffset = start;
+      blockCols = stop - start;
+    } else {
+      colOffset = colElem.cast<int>();
+      blockCols = 1;
+    }
+
+    if (py::isinstance<VariableMatrix>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<VariableMatrix>();
+    } else if (py::isinstance<VariableBlock<VariableMatrix>>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<VariableBlock<VariableMatrix>>();
+    } else if (IsNumPyArithmeticArray(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<Eigen::MatrixXd>();
+    } else if (py::isinstance<Variable>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<Variable>();
+    } else if (py::isinstance<py::float_>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<double>();
+    } else if (py::isinstance<py::int_>(value)) {
+      self.Block(rowOffset, colOffset, blockRows, blockCols) =
+          value.cast<int>();
+    } else {
+      throw py::value_error(
+          "VariableMatrix.__setitem__ not implemented for value");
+    }
+  });
+  variable_matrix.def(
+      "__getitem__",
+      [](VariableMatrix& self, int row) -> Variable& {
+        if (row < 0) {
+          row = self.size() + row;
+        }
+        return self(row);
+      },
+      py::keep_alive<0, 1>(), DOC(sleipnir, VariableMatrix, operator, call, 3));
+  // TODO: Support slice stride other than 1
+  variable_matrix.def(
+      "__getitem__",
+      [](VariableMatrix& self, py::tuple slices) -> py::object {
+        if (slices.size() != 2) {
+          throw py::index_error(
+              fmt::format("Expected 2 slices, got {}.", slices.size()));
+        }
+
+        // If both indices are integers instead of slices, return Variable
+        // instead of VariableBlock
+        if (py::isinstance<py::int_>(slices[0]) &&
+            py::isinstance<py::int_>(slices[1])) {
+          int row = slices[0].cast<int>();
+          int col = slices[1].cast<int>();
+
+          if (row >= self.Rows() || col >= self.Cols()) {
+            throw std::out_of_range("Index out of bounds");
+          }
+
+          if (row < 0) {
+            row = self.Rows() + row;
+          }
+          if (col < 0) {
+            col = self.Cols() + col;
+          }
+          return py::cast(self(row, col));
+        }
+
+        int rowOffset = 0;
+        int colOffset = 0;
+        int blockRows = self.Rows();
+        int blockCols = self.Cols();
+
+        size_t start;
+        size_t stop;
+        size_t step;
+        size_t sliceLength;
+
+        // Row slice
+        const auto& rowElem = slices[0];
+        if (py::isinstance<py::slice>(rowElem)) {
+          const auto& rowSlice = rowElem.cast<py::slice>();
+          if (!rowSlice.compute(self.Rows(), &start, &stop, &step,
+                                &sliceLength)) {
+            throw py::error_already_set();
+          }
+          rowOffset = start;
+          blockRows = stop - start;
+        } else {
+          rowOffset = rowElem.cast<int>();
+          if (rowOffset < 0) {
+            rowOffset = self.Rows() + rowOffset;
+          }
+          blockRows = 1;
+        }
+
+        // Column slice
+        const auto& colElem = slices[1];
+        if (py::isinstance<py::slice>(colElem)) {
+          const auto& colSlice = colElem.cast<py::slice>();
+          if (!colSlice.compute(self.Cols(), &start, &stop, &step,
+                                &sliceLength)) {
+            throw py::error_already_set();
+          }
+          colOffset = start;
+          blockCols = stop - start;
+        } else {
+          colOffset = colElem.cast<int>();
+          if (colOffset < 0) {
+            colOffset = self.Cols() + colOffset;
+          }
+          blockCols = 1;
+        }
+
+        return py::cast(self.Block(rowOffset, colOffset, blockRows, blockCols));
+      },
+      py::keep_alive<0, 1>(), DOC(sleipnir, VariableMatrix, operator, call));
+  variable_matrix.def("row", py::overload_cast<int>(&VariableMatrix::Row),
+                      DOC(sleipnir, VariableMatrix, Row));
+  variable_matrix.def("col", py::overload_cast<int>(&VariableMatrix::Col),
+                      DOC(sleipnir, VariableMatrix, Col));
+  variable_matrix.def(
+      "__mul__",
+      [](const VariableMatrix& lhs, const VariableMatrix& rhs) {
+        return lhs * rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__rmul__",
+      [](const VariableMatrix& rhs, const VariableMatrix& lhs) {
+        return lhs * rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__matmul__",
+      [](const VariableMatrix& lhs, const VariableMatrix& rhs) {
+        return lhs * rhs;
+      },
+      py::is_operator());
+
+  // https://numpy.org/doc/stable/user/basics.dispatch.html
+  variable_matrix.def(
+      "__array_ufunc__",
+      [](VariableMatrix& self, py::object ufunc, py::str method,
+         py::args inputs, const py::kwargs& kwargs) -> py::object {
+        std::string method_name = method;
+        std::string ufunc_name = ufunc.attr("__repr__")().cast<py::str>();
+
+        if (method_name == "__call__") {
+          if (ufunc_name == "<ufunc 'matmul'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() * self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self * inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'add'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() + self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self + inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'subtract'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() - self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self - inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'equal'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() == self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self == inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'less'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() < self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self < inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'less_equal'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() <= self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self <= inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'greater'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() > self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self > inputs[1].cast<Eigen::MatrixXd>());
+            }
+          } else if (ufunc_name == "<ufunc 'greater_equal'>") {
+            if (IsNumPyArithmeticArray(inputs[0])) {
+              return py::cast(inputs[0].cast<Eigen::MatrixXd>() >= self);
+            } else if (IsNumPyArithmeticArray(inputs[1])) {
+              return py::cast(self >= inputs[1].cast<Eigen::MatrixXd>());
+            }
+          }
+        }
+
+        std::string input1_name = inputs[0].attr("__repr__")().cast<py::str>();
+        std::string input2_name = inputs[1].attr("__repr__")().cast<py::str>();
+        throw py::value_error(
+            fmt::format("VariableMatrix: numpy method {}, ufunc {} not "
+                        "implemented for ({}, {})",
+                        method_name, ufunc_name, input1_name, input2_name));
+        return py::cast(VariableMatrix{self});
+      });
+
+  variable_matrix.def(py::self * Variable());
+  variable_matrix.def(py::self * double());
+  variable_matrix.def(Variable() * py::self);
+  variable_matrix.def(double() * py::self);
+
+  variable_matrix.def(py::self / Variable());
+  variable_matrix.def(py::self / double());
+  variable_matrix.def(py::self /= Variable(),
+                      DOC(sleipnir, VariableMatrix, operator, idiv));
+  variable_matrix.def(py::self /= double(),
+                      DOC(sleipnir, VariableMatrix, operator, idiv));
+
+  variable_matrix.def(py::self + py::self);
+  variable_matrix.def(
+      "__add__",
+      [](const VariableMatrix& lhs, const Variable& rhs) {
+        return lhs + VariableMatrix{rhs};
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__radd__",
+      [](const VariableMatrix& rhs, const Variable& lhs) {
+        return VariableMatrix{lhs} + rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__add__",
+      [](double lhs, const VariableMatrix& rhs) {
+        return VariableMatrix{Variable{lhs}} + rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__radd__",
+      [](const VariableMatrix& rhs, double lhs) {
+        return VariableMatrix{Variable{lhs}} + rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__add__",
+      [](const VariableMatrix& lhs,
+         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
+        return lhs + rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__radd__",
+      [](const VariableMatrix& rhs,
+         const Eigen::Ref<const Eigen::MatrixXd>& lhs) -> VariableMatrix {
+        return lhs + rhs;
+      },
+      py::is_operator());
+
+  variable_matrix.def(py::self - py::self);
+  variable_matrix.def(
+      "__sub__",
+      [](const VariableMatrix& lhs, const Variable& rhs) {
+        return lhs - VariableMatrix{rhs};
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__rsub__",
+      [](const VariableMatrix& rhs, const Variable& lhs) {
+        return VariableMatrix{lhs} - rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__sub__",
+      [](const VariableMatrix& lhs,
+         const Eigen::Ref<const Eigen::MatrixXd>& rhs) -> VariableMatrix {
+        return lhs - rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__rsub__",
+      [](const VariableMatrix& rhs,
+         const Eigen::Ref<const Eigen::MatrixXd>& lhs) -> VariableMatrix {
+        return lhs - rhs;
+      },
+      py::is_operator());
+
+  variable_matrix.def(-py::self);
+  variable_matrix.def(
+      "__pow__",
+      [](const VariableMatrix& self, int power) {
+        return sleipnir::pow(self, power);
+      },
+      py::is_operator());
+  variable_matrix.def_property_readonly("T", &VariableMatrix::T,
+                                        DOC(sleipnir, VariableMatrix, T));
+  variable_matrix.def("rows", &VariableMatrix::Rows,
+                      DOC(sleipnir, VariableMatrix, Rows));
+  variable_matrix.def("cols", &VariableMatrix::Cols,
+                      DOC(sleipnir, VariableMatrix, Cols));
+  variable_matrix.def_property_readonly(
+      "shape", [](const VariableMatrix& self) {
+        return py::make_tuple(self.Rows(), self.Cols());
+      });
+  variable_matrix.def("value",
+                      static_cast<double (VariableMatrix::*)(int, int) const>(
+                          &VariableMatrix::Value),
+                      DOC(sleipnir, VariableMatrix, Value));
+  variable_matrix.def("value",
+                      static_cast<double (VariableMatrix::*)(int) const>(
+                          &VariableMatrix::Value),
+                      DOC(sleipnir, VariableMatrix, Value, 2));
+  variable_matrix.def("value",
+                      static_cast<Eigen::MatrixXd (VariableMatrix::*)() const>(
+                          &VariableMatrix::Value),
+                      DOC(sleipnir, VariableMatrix, Value, 3));
+  variable_matrix.def(
+      "cwise_transform",
+      [](const VariableMatrix& self,
+         const std::function<Variable(const Variable&)>& func) {
+        return self.CwiseTransform(func);
+      },
+      DOC(sleipnir, VariableMatrix, CwiseTransform));
+  variable_matrix.def_static("zero", &VariableMatrix::Zero,
+                             DOC(sleipnir, VariableMatrix, Zero));
+  variable_matrix.def_static("ones", &VariableMatrix::Ones,
+                             DOC(sleipnir, VariableMatrix, Ones));
+  variable_matrix.def(py::self == py::self, DOC(sleipnir, operator, eq));
+  variable_matrix.def(py::self == Variable(), DOC(sleipnir, operator, eq));
+  variable_matrix.def(py::self == double(), DOC(sleipnir, operator, eq));
+  variable_matrix.def(py::self == int(), DOC(sleipnir, operator, eq));
+  variable_matrix.def(Variable() == py::self, DOC(sleipnir, operator, eq));
+  variable_matrix.def(double() == py::self, DOC(sleipnir, operator, eq));
+  variable_matrix.def(int() == py::self, DOC(sleipnir, operator, eq));
+  variable_matrix.def(py::self < py::self, DOC(sleipnir, operator, lt));
+  variable_matrix.def(py::self < Variable(), DOC(sleipnir, operator, lt));
+  variable_matrix.def(py::self < double(), DOC(sleipnir, operator, lt));
+  variable_matrix.def(py::self < int(), DOC(sleipnir, operator, lt));
+  variable_matrix.def(Variable() < py::self, DOC(sleipnir, operator, lt));
+  variable_matrix.def(double() < py::self, DOC(sleipnir, operator, lt));
+  variable_matrix.def(int() < py::self, DOC(sleipnir, operator, lt));
+  variable_matrix.def(py::self <= py::self, DOC(sleipnir, operator, le));
+  variable_matrix.def(py::self <= Variable(), DOC(sleipnir, operator, le));
+  variable_matrix.def(py::self <= double(), DOC(sleipnir, operator, le));
+  variable_matrix.def(py::self <= int(), DOC(sleipnir, operator, le));
+  variable_matrix.def(Variable() <= py::self, DOC(sleipnir, operator, le));
+  variable_matrix.def(double() <= py::self, DOC(sleipnir, operator, le));
+  variable_matrix.def(int() <= py::self, DOC(sleipnir, operator, le));
+  variable_matrix.def(py::self > py::self, DOC(sleipnir, operator, gt));
+  variable_matrix.def(py::self > Variable(), DOC(sleipnir, operator, gt));
+  variable_matrix.def(py::self > double(), DOC(sleipnir, operator, gt));
+  variable_matrix.def(py::self > int(), DOC(sleipnir, operator, gt));
+  variable_matrix.def(Variable() > py::self, DOC(sleipnir, operator, gt));
+  variable_matrix.def(double() > py::self, DOC(sleipnir, operator, gt));
+  variable_matrix.def(int() > py::self, DOC(sleipnir, operator, gt));
+  variable_matrix.def(py::self >= py::self, DOC(sleipnir, operator, ge));
+  variable_matrix.def(py::self >= Variable(), DOC(sleipnir, operator, ge));
+  variable_matrix.def(py::self >= double(), DOC(sleipnir, operator, ge));
+  variable_matrix.def(py::self >= int(), DOC(sleipnir, operator, ge));
+  variable_matrix.def(Variable() >= py::self, DOC(sleipnir, operator, ge));
+  variable_matrix.def(double() >= py::self, DOC(sleipnir, operator, ge));
+  variable_matrix.def(int() >= py::self, DOC(sleipnir, operator, ge));
+  py::implicitly_convertible<VariableMatrix, Variable>();
+
+  // VariableMatrix-VariableBlock overloads
+  variable_matrix.def(
+      "__mul__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs * rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__rmul__",
+      [](const VariableMatrix& rhs, const VariableBlock<VariableMatrix>& lhs) {
+        return lhs * rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__matmul__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs * rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__add__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs + rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__sub__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs - rhs;
+      },
+      py::is_operator());
+  variable_matrix.def(
+      "__eq__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs == rhs;
+      },
+      py::is_operator(), DOC(sleipnir, operator, eq));
+  variable_matrix.def(
+      "__lt__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs < rhs;
+      },
+      py::is_operator(), DOC(sleipnir, operator, lt));
+  variable_matrix.def(
+      "__le__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs <= rhs;
+      },
+      py::is_operator(), DOC(sleipnir, operator, le));
+  variable_matrix.def(
+      "__gt__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs > rhs;
+      },
+      py::is_operator(), DOC(sleipnir, operator, gt));
+  variable_matrix.def(
+      "__ge__",
+      [](const VariableMatrix& lhs, const VariableBlock<VariableMatrix>& rhs) {
+        return lhs >= rhs;
+      },
+      py::is_operator(), DOC(sleipnir, operator, ge));
+  variable_matrix.def(
+      "__eq__",
+      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
+        return lhs == rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, eq));
+  variable_matrix.def(
+      "__lt__",
+      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
+        return lhs < rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, lt));
+  variable_matrix.def(
+      "__le__",
+      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
+        return lhs <= rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, le));
+  variable_matrix.def(
+      "__gt__",
+      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
+        return lhs > rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, gt));
+  variable_matrix.def(
+      "__ge__",
+      [](const VariableMatrix& lhs, const py::array_t<double>& rhs) {
+        return lhs >= rhs.cast<Eigen::MatrixXd>();
+      },
+      py::is_operator(), DOC(sleipnir, operator, ge));
+
+  variable_matrix.def("__len__", &VariableMatrix::Rows,
+                      DOC(sleipnir, VariableMatrix, Rows));
+
+  variable_matrix.def(
+      "__iter__",
+      [](const VariableMatrix& self) {
+        return py::make_iterator(self.begin(), self.end());
+      },
+      py::keep_alive<0, 1>());
+
+  autodiff.def(
+      "cwise_reduce",
+      [](const VariableMatrix& lhs, const VariableMatrix& rhs,
+         const std::function<Variable(const Variable&, const Variable&)> func) {
+        return CwiseReduce(lhs, rhs, func);
+      },
+      DOC(sleipnir, CwiseReduce));
+
+  autodiff.def(
+      "block",
+      static_cast<VariableMatrix (*)(std::vector<std::vector<VariableMatrix>>)>(
+          &Block),
+      DOC(sleipnir, Block));
+}  // NOLINT(readability/fn_size)
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/autodiff/gradient_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/autodiff/gradient_test.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,511 +1,511 @@
-import math
-
-from jormungandr.autodiff import Gradient, Variable
-import jormungandr.autodiff as autodiff
-import numpy as np
-import pytest
-
-
-def test_trivial_case():
-    a = Variable()
-    a.set_value(10)
-    b = Variable()
-    b.set_value(20)
-    c = a
-
-    assert Gradient(a, a).value()[0, 0] == 1.0
-    assert Gradient(a, b).value()[0, 0] == 0.0
-    assert Gradient(c, a).value()[0, 0] == 1.0
-    assert Gradient(c, b).value()[0, 0] == 0.0
-
-
-def test_unary_plus():
-    a = Variable()
-    a.set_value(10)
-    c = +a
-
-    assert c.value() == a.value()
-    assert Gradient(c, a).value()[0, 0] == 1.0
-
-
-def test_unary_minus():
-    a = Variable()
-    a.set_value(10)
-    c = -a
-
-    assert c.value() == -a.value()
-    assert Gradient(c, a).value()[0, 0] == -1.0
-
-
-def test_identical_variables():
-    a = Variable()
-    a.set_value(10)
-    x = a
-    c = a * a + x
-
-    assert c.value() == a.value() * a.value() + x.value()
-    assert Gradient(c, a).value()[0, 0] == 2 * a.value() + Gradient(x, a).value()[0, 0]
-    assert (
-        Gradient(c, a).value()[0, 0] == 2 * a.value() * Gradient(x, a).value()[0, 0] + 1
-    )
-
-
-def test_elementary():
-    a = Variable()
-    a.set_value(1.0)
-    b = Variable()
-    b.set_value(2.0)
-    c = Variable()
-    c.set_value(3.0)
-
-    c = -2 * a
-    assert Gradient(c, a).value()[0, 0] == -2.0
-
-    c = a / 3.0
-    assert Gradient(c, a).value()[0, 0] == 1.0 / 3.0
-
-    a.set_value(100.0)
-    b.set_value(200.0)
-
-    c = a + b
-    assert Gradient(c, a).value()[0, 0] == 1.0
-    assert Gradient(c, b).value()[0, 0] == 1.0
-
-    c = a - b
-    assert Gradient(c, a).value()[0, 0] == 1.0
-    assert Gradient(c, b).value()[0, 0] == -1.0
-
-    c = -a + b
-    assert Gradient(c, a).value()[0, 0] == -1.0
-    assert Gradient(c, b).value()[0, 0] == 1.0
-
-    c = a + 1
-    assert Gradient(c, a).value()[0, 0] == 1.0
-
-
-def test_comparison():
-    x = Variable()
-    x.set_value(10.0)
-    a = Variable()
-    a.set_value(10.0)
-    b = Variable()
-    b.set_value(200.0)
-
-    assert a.value() == a.value()
-    assert a.value() == x.value()
-    assert a.value() == 10.0
-    assert 10.0 == a.value()
-
-    assert a.value() != b.value()
-    assert a.value() != 20.0
-    assert 20.0 != a.value()
-
-    assert a.value() < b.value()
-    assert a.value() < 20.0
-
-    assert b.value() > a.value()
-    assert 20.0 > a.value()
-
-    assert a.value() <= a.value()
-    assert a.value() <= x.value()
-    assert a.value() <= b.value()
-    assert a.value() <= 10.0
-    assert a.value() <= 20.0
-
-    assert a.value() >= a.value()
-    assert x.value() >= a.value()
-    assert b.value() >= a.value()
-    assert 10.0 >= a.value()
-    assert 20.0 >= a.value()
-
-    # Comparison between variables and expressions
-    assert a.value() == a.value() / a.value() * a.value()
-    assert a.value() / a.value() * a.value() == a.value()
-
-    assert a.value() != (a - a).value()
-    assert (a - a).value() != a.value()
-
-    assert (a - a).value() < a.value()
-    assert a.value() < (a + a).value()
-
-    assert (a + a).value() > a.value()
-    assert a.value() > (a - a).value()
-
-    assert a.value() <= (a - a + a).value()
-    assert (a - a + a).value() <= a.value()
-
-    assert a.value() <= (a + a).value()
-    assert (a - a).value() <= a.value()
-
-    assert a.value() >= (a - a + a).value()
-    assert (a - a + a).value() >= a.value()
-
-    assert (a + a).value() >= a.value()
-    assert a.value() >= (a - a).value()
-
-
-def test_trigonometry():
-    x = Variable()
-    x.set_value(0.5)
-
-    # sin(x)
-    assert autodiff.sin(x).value() == math.sin(x.value())
-    g = Gradient(autodiff.sin(x), x)
-    assert g.get().value()[0, 0] == math.cos(x.value())
-    assert g.value()[0, 0] == math.cos(x.value())
-
-    # cos(x)
-    assert autodiff.cos(x).value() == math.cos(x.value())
-    g = Gradient(autodiff.cos(x), x)
-    assert g.get().value()[0, 0] == -math.sin(x.value())
-    assert g.value()[0, 0] == -math.sin(x.value())
-
-    # tan(x)
-    assert autodiff.tan(x).value() == math.tan(x.value())
-    g = Gradient(autodiff.tan(x), x)
-    assert g.get().value()[0, 0] == 1.0 / (math.cos(x.value()) * math.cos(x.value()))
-    assert g.value()[0, 0] == 1.0 / (math.cos(x.value()) * math.cos(x.value()))
-
-    # asin(x)
-    assert autodiff.asin(x).value() == math.asin(x.value())
-    g = Gradient(autodiff.asin(x), x)
-    assert g.get().value()[0, 0] == 1.0 / math.sqrt(1 - x.value() * x.value())
-    assert g.value()[0, 0] == 1.0 / math.sqrt(1 - x.value() * x.value())
-
-    # acos(x)
-    assert autodiff.acos(x).value() == math.acos(x.value())
-    g = Gradient(autodiff.acos(x), x)
-    assert g.get().value()[0, 0] == -1.0 / math.sqrt(1 - x.value() * x.value())
-    assert g.value()[0, 0] == -1.0 / math.sqrt(1 - x.value() * x.value())
-
-    # atan(x)
-    assert autodiff.atan(x).value() == math.atan(x.value())
-    g = Gradient(autodiff.atan(x), x)
-    assert g.get().value()[0, 0] == 1.0 / (1 + x.value() * x.value())
-    assert g.value()[0, 0] == 1.0 / (1 + x.value() * x.value())
-
-
-def test_hyperbolic():
-    x = Variable()
-    x.set_value(1.0)
-
-    # sinh(x)
-    assert autodiff.sinh(x).value() == math.sinh(x.value())
-    g = Gradient(autodiff.sinh(x), x)
-    assert g.get().value()[0, 0] == math.cosh(x.value())
-    assert g.value()[0, 0] == math.cosh(x.value())
-
-    # cosh(x)
-    assert autodiff.cosh(x).value() == math.cosh(x.value())
-    g = Gradient(autodiff.cosh(x), x)
-    assert g.get().value()[0, 0] == math.sinh(x.value())
-    assert g.value()[0, 0] == math.sinh(x.value())
-
-    # tanh(x)
-    assert autodiff.tanh(x).value() == math.tanh(x.value())
-    g = Gradient(autodiff.tanh(x), x)
-    assert g.get().value()[0, 0] == 1.0 / (math.cosh(x.value()) * math.cosh(x.value()))
-    assert g.value()[0, 0] == 1.0 / (math.cosh(x.value()) * math.cosh(x.value()))
-
-
-def test_exponential():
-    x = Variable()
-    x.set_value(1.0)
-
-    # log(x)
-    assert autodiff.log(x).value() == math.log(x.value())
-    g = Gradient(autodiff.log(x), x)
-    assert g.get().value()[0, 0] == 1.0 / x.value()
-    assert g.value()[0, 0] == 1.0 / x.value()
-
-    # log10(x)
-    assert autodiff.log10(x).value() == math.log10(x.value())
-    g = Gradient(autodiff.log10(x), x)
-    assert g.get().value()[0, 0] == 1.0 / (math.log(10.0) * x.value())
-    assert g.value()[0, 0] == 1.0 / (math.log(10.0) * x.value())
-
-    # exp(x)
-    assert autodiff.exp(x).value() == math.exp(x.value())
-    g = Gradient(autodiff.exp(x), x)
-    assert g.get().value()[0, 0] == math.exp(x.value())
-    assert g.value()[0, 0] == math.exp(x.value())
-
-
-def test_power():
-    x = Variable()
-    x.set_value(1.0)
-    a = Variable()
-    a.set_value(2.0)
-    y = 2 * a
-
-    # sqrt(x)
-    g = Gradient(autodiff.sqrt(x), x)
-    assert autodiff.sqrt(x).value() == math.sqrt(x.value())
-    assert g.get().value()[0, 0] == 0.5 / math.sqrt(x.value())
-    assert g.value()[0, 0] == 0.5 / math.sqrt(x.value())
-
-    # x²
-    g = Gradient(autodiff.pow(x, 2.0), x)
-    assert autodiff.pow(x, 2.0).value() == math.pow(x.value(), 2.0)
-    assert g.get().value()[0, 0] == 2.0 * x.value()
-    assert g.value()[0, 0] == 2.0 * x.value()
-
-    # 2ˣ
-    assert autodiff.pow(2.0, x).value() == math.pow(2.0, x.value())
-    assert Gradient(autodiff.pow(2.0, x), x).value()[0, 0] == math.log(2.0) * math.pow(
-        2.0, x.value()
-    )
-
-    # xˣ
-    assert autodiff.pow(x, x).value() == math.pow(x.value(), x.value())
-    g = Gradient(autodiff.pow(x, x), x)
-    assert g.get().value()[0, 0] == ((autodiff.log(x) + 1) * autodiff.pow(x, x)).value()
-    assert g.value()[0, 0] == ((autodiff.log(x) + 1) * autodiff.pow(x, x)).value()
-
-    # y(a)
-    assert y.value() == 2 * a.value()
-    g = Gradient(y, a)
-    assert g.get().value()[0, 0] == 2.0
-    assert g.value()[0, 0] == 2.0
-
-    # xʸ(x)
-    assert autodiff.pow(x, y).value() == math.pow(x.value(), y.value())
-    g = Gradient(autodiff.pow(x, y), x)
-    assert g.get().value()[0, 0] == y.value() / x.value() * math.pow(
-        x.value(), y.value()
-    )
-    assert g.value()[0, 0] == y.value() / x.value() * math.pow(x.value(), y.value())
-
-    # xʸ(a)
-    assert autodiff.pow(x, y).value() == math.pow(x.value(), y.value())
-    g = Gradient(autodiff.pow(x, y), a)
-    assert g.get().value()[0, 0] == math.pow(x.value(), y.value()) * (
-        y.value() / x.value() * Gradient(x, a).value()[0, 0]
-        + math.log(x.value()) * Gradient(y, a).value()[0, 0]
-    )
-    assert g.value()[0, 0] == math.pow(x.value(), y.value()) * (
-        y.value() / x.value() * Gradient(x, a).value()[0, 0]
-        + math.log(x.value()) * Gradient(y, a).value()[0, 0]
-    )
-
-    # xʸ(y)
-    assert autodiff.pow(x, y).value() == math.pow(x.value(), y.value())
-    g = Gradient(autodiff.pow(x, y), y)
-    assert g.get().value()[0, 0] == math.log(x.value()) * math.pow(x.value(), y.value())
-    assert g.value()[0, 0] == math.log(x.value()) * math.pow(x.value(), y.value())
-
-
-def test_abs():
-    x = Variable()
-    g = Gradient(autodiff.abs(x), x)
-
-    x.set_value(1.0)
-    assert autodiff.abs(x).value() == abs(x.value())
-    assert g.get().value()[0, 0] == 1.0
-    assert g.value()[0, 0] == 1.0
-
-    x.set_value(-1.0)
-    assert autodiff.abs(x).value() == abs(x.value())
-    assert g.get().value()[0, 0] == -1.0
-    assert g.value()[0, 0] == -1.0
-
-    x.set_value(0.0)
-    assert autodiff.abs(x).value() == abs(x.value())
-    assert g.get().value()[0, 0] == 0.0
-    assert g.value()[0, 0] == 0.0
-
-
-def test_atan2():
-    # Testing atan2 function on (double, var)
-    x = Variable()
-    x.set_value(1.0)
-    y = Variable()
-    y.set_value(0.9)
-    assert autodiff.atan2(2.0, x).value() == math.atan2(2.0, x.value())
-    assert Gradient(autodiff.atan2(2.0, x), x).value()[0, 0] == pytest.approx(
-        (-2.0 / (2 * 2 + x * x)).value(), abs=1e-15
-    )
-
-    # Testing atan2 function on (var, double)
-    x.set_value(1.0)
-    assert autodiff.atan2(x, 2.0).value() == math.atan2(x.value(), 2.0)
-    assert Gradient(autodiff.atan2(x, 2.0), x).value()[0, 0] == pytest.approx(
-        (2.0 / (2 * 2 + x * x)).value(), abs=1e-15
-    )
-
-    # Testing atan2 function on (var, var)
-    x.set_value(1.1)
-    assert autodiff.atan2(y, x).value() == math.atan2(y.value(), x.value())
-    assert Gradient(autodiff.atan2(y, x), y).value()[0, 0] == pytest.approx(
-        (x / (x * x + y * y)).value(), abs=1e-15
-    )
-    assert Gradient(autodiff.atan2(y, x), x).value()[0, 0] == pytest.approx(
-        (-y / (x * x + y * y)).value(), abs=1e-15
-    )
-
-    # Testing atan2 function on (expr, expr)
-    assert 3 * autodiff.atan2(autodiff.sin(y), 2 * x + 1).value() == 3 * math.atan2(
-        autodiff.sin(y).value(), 2 * x.value() + 1
-    )
-    assert Gradient(3 * autodiff.atan2(autodiff.sin(y), 2 * x + 1), y).value()[
-        0, 0
-    ] == pytest.approx(
-        (
-            3
-            * (2 * x + 1)
-            * autodiff.cos(y)
-            / ((2 * x + 1) * (2 * x + 1) + autodiff.sin(y) * autodiff.sin(y))
-        ).value(),
-        abs=1e-15,
-    )
-    assert Gradient(3 * autodiff.atan2(autodiff.sin(y), 2 * x + 1), x).value()[
-        0, 0
-    ] == pytest.approx(
-        (
-            3
-            * -2
-            * autodiff.sin(y)
-            / ((2 * x + 1) * (2 * x + 1) + autodiff.sin(y) * autodiff.sin(y))
-        ).value(),
-        abs=1e-15,
-    )
-
-
-def test_hypot():
-    # Testing hypot function on (var, double)
-    x = Variable()
-    x.set_value(1.8)
-    y = Variable()
-    y.set_value(1.5)
-    assert autodiff.hypot(x, 2.0).value() == math.hypot(x.value(), 2.0)
-    assert (
-        Gradient(autodiff.hypot(x, 2.0), x).value()[0, 0]
-        == (x / math.hypot(x.value(), 2.0)).value()
-    )
-
-    # Testing hypot function on (double, var)
-    assert autodiff.hypot(2.0, y).value() == math.hypot(2.0, y.value())
-    assert (
-        Gradient(autodiff.hypot(2.0, y), y).value()[0, 0]
-        == (y / math.hypot(2.0, y.value())).value()
-    )
-
-    # Testing hypot function on (var, var)
-    x.set_value(1.3)
-    y.set_value(2.3)
-    assert autodiff.hypot(x, y).value() == math.hypot(x.value(), y.value())
-    assert (
-        Gradient(autodiff.hypot(x, y), x).value()[0, 0]
-        == (x / math.hypot(x.value(), y.value())).value()
-    )
-    assert (
-        Gradient(autodiff.hypot(x, y), y).value()[0, 0]
-        == (y / math.hypot(x.value(), y.value())).value()
-    )
-
-    # Testing hypot function on (expr, expr)
-    x.set_value(1.3)
-    y.set_value(2.3)
-    assert autodiff.hypot(2.0 * x, 3.0 * y).value() == math.hypot(
-        2.0 * x.value(), 3.0 * y.value()
-    )
-    assert (
-        Gradient(autodiff.hypot(2.0 * x, 3.0 * y), x).value()[0, 0]
-        == (4.0 * x / math.hypot(2.0 * x.value(), 3.0 * y.value())).value()
-    )
-    assert (
-        Gradient(autodiff.hypot(2.0 * x, 3.0 * y), y).value()[0, 0]
-        == (9.0 * y / math.hypot(2.0 * x.value(), 3.0 * y.value())).value()
-    )
-
-    # Testing hypot function on (var, var, var)
-    x.set_value(1.3)
-    y.set_value(2.3)
-    z = Variable()
-    z.set_value(3.3)
-    assert autodiff.hypot(x, y, z).value() == math.hypot(
-        x.value(), y.value(), z.value()
-    )
-    assert (
-        Gradient(autodiff.hypot(x, y, z), x).value()[0, 0]
-        == (x / math.hypot(x.value(), y.value(), z.value())).value()
-    )
-    assert (
-        Gradient(autodiff.hypot(x, y, z), y).value()[0, 0]
-        == (y / math.hypot(x.value(), y.value(), z.value())).value()
-    )
-    assert (
-        Gradient(autodiff.hypot(x, y, z), z).value()[0, 0]
-        == (z / math.hypot(x.value(), y.value(), z.value())).value()
-    )
-
-
-def test_miscellaneous():
-    x = Variable()
-
-    # dx/dx
-    x.set_value(3.0)
-    g = Gradient(x, x)
-    assert autodiff.abs(x).value() == abs(x.value())
-    assert g.get().value()[0, 0] == 1.0
-    assert g.value()[0, 0] == 1.0
-
-    # erf(x)
-    x.set_value(0.5)
-    g = Gradient(autodiff.erf(x), x)
-    assert autodiff.erf(x).value() == math.erf(x.value())
-    assert g.get().value()[0, 0] == 2.0 / math.sqrt(math.pi) * math.exp(
-        -x.value() * x.value()
-    )
-    assert g.value()[0, 0] == 2.0 / math.sqrt(math.pi) * math.exp(
-        -x.value() * x.value()
-    )
-
-
-def test_reuse():
-    a = Variable()
-    a.set_value(10)
-
-    b = Variable()
-    b.set_value(20)
-
-    x = a * b
-
-    g = Gradient(x, a)
-
-    assert g.get().value()[0] == 20.0
-    assert g.value()[0] == 20.0
-
-    b.set_value(10)
-    assert g.get().value()[0] == 10.0
-    assert g.value()[0] == 10.0
-
-
-def test_sign():
-    def sign(x):
-        if x < 0.0:
-            return -1.0
-        elif x == 0.0:
-            return 0.0
-        else:
-            return 1.0
-
-    x = Variable()
-
-    x.set_value(1.0)
-    g = Gradient(autodiff.sign(x), x)
-    assert sign(x.value()) == autodiff.sign(x).value()
-    assert g.get().value()[0, 0] == 0.0
-    assert g.value()[0, 0] == 0.0
-
-    x.set_value(-1.0)
-    g = Gradient(autodiff.sign(x), x)
-    assert sign(x.value()) == autodiff.sign(x).value()
-    assert g.get().value()[0, 0] == 0.0
-    assert g.value()[0, 0] == 0.0
-
-    x.set_value(0.0)
-    g = Gradient(autodiff.sign(x), x)
-    assert sign(x.value()) == autodiff.sign(x).value()
-    assert g.get().value()[0, 0] == 0.0
-    assert g.value()[0, 0] == 0.0
+import math
+
+from jormungandr.autodiff import Gradient, Variable
+import jormungandr.autodiff as autodiff
+import numpy as np
+import pytest
+
+
+def test_trivial_case():
+    a = Variable()
+    a.set_value(10)
+    b = Variable()
+    b.set_value(20)
+    c = a
+
+    assert Gradient(a, a).value()[0, 0] == 1.0
+    assert Gradient(a, b).value()[0, 0] == 0.0
+    assert Gradient(c, a).value()[0, 0] == 1.0
+    assert Gradient(c, b).value()[0, 0] == 0.0
+
+
+def test_unary_plus():
+    a = Variable()
+    a.set_value(10)
+    c = +a
+
+    assert c.value() == a.value()
+    assert Gradient(c, a).value()[0, 0] == 1.0
+
+
+def test_unary_minus():
+    a = Variable()
+    a.set_value(10)
+    c = -a
+
+    assert c.value() == -a.value()
+    assert Gradient(c, a).value()[0, 0] == -1.0
+
+
+def test_identical_variables():
+    a = Variable()
+    a.set_value(10)
+    x = a
+    c = a * a + x
+
+    assert c.value() == a.value() * a.value() + x.value()
+    assert Gradient(c, a).value()[0, 0] == 2 * a.value() + Gradient(x, a).value()[0, 0]
+    assert (
+        Gradient(c, a).value()[0, 0] == 2 * a.value() * Gradient(x, a).value()[0, 0] + 1
+    )
+
+
+def test_elementary():
+    a = Variable()
+    a.set_value(1.0)
+    b = Variable()
+    b.set_value(2.0)
+    c = Variable()
+    c.set_value(3.0)
+
+    c = -2 * a
+    assert Gradient(c, a).value()[0, 0] == -2.0
+
+    c = a / 3.0
+    assert Gradient(c, a).value()[0, 0] == 1.0 / 3.0
+
+    a.set_value(100.0)
+    b.set_value(200.0)
+
+    c = a + b
+    assert Gradient(c, a).value()[0, 0] == 1.0
+    assert Gradient(c, b).value()[0, 0] == 1.0
+
+    c = a - b
+    assert Gradient(c, a).value()[0, 0] == 1.0
+    assert Gradient(c, b).value()[0, 0] == -1.0
+
+    c = -a + b
+    assert Gradient(c, a).value()[0, 0] == -1.0
+    assert Gradient(c, b).value()[0, 0] == 1.0
+
+    c = a + 1
+    assert Gradient(c, a).value()[0, 0] == 1.0
+
+
+def test_comparison():
+    x = Variable()
+    x.set_value(10.0)
+    a = Variable()
+    a.set_value(10.0)
+    b = Variable()
+    b.set_value(200.0)
+
+    assert a.value() == a.value()
+    assert a.value() == x.value()
+    assert a.value() == 10.0
+    assert 10.0 == a.value()
+
+    assert a.value() != b.value()
+    assert a.value() != 20.0
+    assert 20.0 != a.value()
+
+    assert a.value() < b.value()
+    assert a.value() < 20.0
+
+    assert b.value() > a.value()
+    assert 20.0 > a.value()
+
+    assert a.value() <= a.value()
+    assert a.value() <= x.value()
+    assert a.value() <= b.value()
+    assert a.value() <= 10.0
+    assert a.value() <= 20.0
+
+    assert a.value() >= a.value()
+    assert x.value() >= a.value()
+    assert b.value() >= a.value()
+    assert 10.0 >= a.value()
+    assert 20.0 >= a.value()
+
+    # Comparison between variables and expressions
+    assert a.value() == a.value() / a.value() * a.value()
+    assert a.value() / a.value() * a.value() == a.value()
+
+    assert a.value() != (a - a).value()
+    assert (a - a).value() != a.value()
+
+    assert (a - a).value() < a.value()
+    assert a.value() < (a + a).value()
+
+    assert (a + a).value() > a.value()
+    assert a.value() > (a - a).value()
+
+    assert a.value() <= (a - a + a).value()
+    assert (a - a + a).value() <= a.value()
+
+    assert a.value() <= (a + a).value()
+    assert (a - a).value() <= a.value()
+
+    assert a.value() >= (a - a + a).value()
+    assert (a - a + a).value() >= a.value()
+
+    assert (a + a).value() >= a.value()
+    assert a.value() >= (a - a).value()
+
+
+def test_trigonometry():
+    x = Variable()
+    x.set_value(0.5)
+
+    # sin(x)
+    assert autodiff.sin(x).value() == math.sin(x.value())
+    g = Gradient(autodiff.sin(x), x)
+    assert g.get().value()[0, 0] == math.cos(x.value())
+    assert g.value()[0, 0] == math.cos(x.value())
+
+    # cos(x)
+    assert autodiff.cos(x).value() == math.cos(x.value())
+    g = Gradient(autodiff.cos(x), x)
+    assert g.get().value()[0, 0] == -math.sin(x.value())
+    assert g.value()[0, 0] == -math.sin(x.value())
+
+    # tan(x)
+    assert autodiff.tan(x).value() == math.tan(x.value())
+    g = Gradient(autodiff.tan(x), x)
+    assert g.get().value()[0, 0] == 1.0 / (math.cos(x.value()) * math.cos(x.value()))
+    assert g.value()[0, 0] == 1.0 / (math.cos(x.value()) * math.cos(x.value()))
+
+    # asin(x)
+    assert autodiff.asin(x).value() == math.asin(x.value())
+    g = Gradient(autodiff.asin(x), x)
+    assert g.get().value()[0, 0] == 1.0 / math.sqrt(1 - x.value() * x.value())
+    assert g.value()[0, 0] == 1.0 / math.sqrt(1 - x.value() * x.value())
+
+    # acos(x)
+    assert autodiff.acos(x).value() == math.acos(x.value())
+    g = Gradient(autodiff.acos(x), x)
+    assert g.get().value()[0, 0] == -1.0 / math.sqrt(1 - x.value() * x.value())
+    assert g.value()[0, 0] == -1.0 / math.sqrt(1 - x.value() * x.value())
+
+    # atan(x)
+    assert autodiff.atan(x).value() == math.atan(x.value())
+    g = Gradient(autodiff.atan(x), x)
+    assert g.get().value()[0, 0] == 1.0 / (1 + x.value() * x.value())
+    assert g.value()[0, 0] == 1.0 / (1 + x.value() * x.value())
+
+
+def test_hyperbolic():
+    x = Variable()
+    x.set_value(1.0)
+
+    # sinh(x)
+    assert autodiff.sinh(x).value() == math.sinh(x.value())
+    g = Gradient(autodiff.sinh(x), x)
+    assert g.get().value()[0, 0] == math.cosh(x.value())
+    assert g.value()[0, 0] == math.cosh(x.value())
+
+    # cosh(x)
+    assert autodiff.cosh(x).value() == math.cosh(x.value())
+    g = Gradient(autodiff.cosh(x), x)
+    assert g.get().value()[0, 0] == math.sinh(x.value())
+    assert g.value()[0, 0] == math.sinh(x.value())
+
+    # tanh(x)
+    assert autodiff.tanh(x).value() == math.tanh(x.value())
+    g = Gradient(autodiff.tanh(x), x)
+    assert g.get().value()[0, 0] == 1.0 / (math.cosh(x.value()) * math.cosh(x.value()))
+    assert g.value()[0, 0] == 1.0 / (math.cosh(x.value()) * math.cosh(x.value()))
+
+
+def test_exponential():
+    x = Variable()
+    x.set_value(1.0)
+
+    # log(x)
+    assert autodiff.log(x).value() == math.log(x.value())
+    g = Gradient(autodiff.log(x), x)
+    assert g.get().value()[0, 0] == 1.0 / x.value()
+    assert g.value()[0, 0] == 1.0 / x.value()
+
+    # log10(x)
+    assert autodiff.log10(x).value() == math.log10(x.value())
+    g = Gradient(autodiff.log10(x), x)
+    assert g.get().value()[0, 0] == 1.0 / (math.log(10.0) * x.value())
+    assert g.value()[0, 0] == 1.0 / (math.log(10.0) * x.value())
+
+    # exp(x)
+    assert autodiff.exp(x).value() == math.exp(x.value())
+    g = Gradient(autodiff.exp(x), x)
+    assert g.get().value()[0, 0] == math.exp(x.value())
+    assert g.value()[0, 0] == math.exp(x.value())
+
+
+def test_power():
+    x = Variable()
+    x.set_value(1.0)
+    a = Variable()
+    a.set_value(2.0)
+    y = 2 * a
+
+    # sqrt(x)
+    g = Gradient(autodiff.sqrt(x), x)
+    assert autodiff.sqrt(x).value() == math.sqrt(x.value())
+    assert g.get().value()[0, 0] == 0.5 / math.sqrt(x.value())
+    assert g.value()[0, 0] == 0.5 / math.sqrt(x.value())
+
+    # x²
+    g = Gradient(autodiff.pow(x, 2.0), x)
+    assert autodiff.pow(x, 2.0).value() == math.pow(x.value(), 2.0)
+    assert g.get().value()[0, 0] == 2.0 * x.value()
+    assert g.value()[0, 0] == 2.0 * x.value()
+
+    # 2ˣ
+    assert autodiff.pow(2.0, x).value() == math.pow(2.0, x.value())
+    assert Gradient(autodiff.pow(2.0, x), x).value()[0, 0] == math.log(2.0) * math.pow(
+        2.0, x.value()
+    )
+
+    # xˣ
+    assert autodiff.pow(x, x).value() == math.pow(x.value(), x.value())
+    g = Gradient(autodiff.pow(x, x), x)
+    assert g.get().value()[0, 0] == ((autodiff.log(x) + 1) * autodiff.pow(x, x)).value()
+    assert g.value()[0, 0] == ((autodiff.log(x) + 1) * autodiff.pow(x, x)).value()
+
+    # y(a)
+    assert y.value() == 2 * a.value()
+    g = Gradient(y, a)
+    assert g.get().value()[0, 0] == 2.0
+    assert g.value()[0, 0] == 2.0
+
+    # xʸ(x)
+    assert autodiff.pow(x, y).value() == math.pow(x.value(), y.value())
+    g = Gradient(autodiff.pow(x, y), x)
+    assert g.get().value()[0, 0] == y.value() / x.value() * math.pow(
+        x.value(), y.value()
+    )
+    assert g.value()[0, 0] == y.value() / x.value() * math.pow(x.value(), y.value())
+
+    # xʸ(a)
+    assert autodiff.pow(x, y).value() == math.pow(x.value(), y.value())
+    g = Gradient(autodiff.pow(x, y), a)
+    assert g.get().value()[0, 0] == math.pow(x.value(), y.value()) * (
+        y.value() / x.value() * Gradient(x, a).value()[0, 0]
+        + math.log(x.value()) * Gradient(y, a).value()[0, 0]
+    )
+    assert g.value()[0, 0] == math.pow(x.value(), y.value()) * (
+        y.value() / x.value() * Gradient(x, a).value()[0, 0]
+        + math.log(x.value()) * Gradient(y, a).value()[0, 0]
+    )
+
+    # xʸ(y)
+    assert autodiff.pow(x, y).value() == math.pow(x.value(), y.value())
+    g = Gradient(autodiff.pow(x, y), y)
+    assert g.get().value()[0, 0] == math.log(x.value()) * math.pow(x.value(), y.value())
+    assert g.value()[0, 0] == math.log(x.value()) * math.pow(x.value(), y.value())
+
+
+def test_abs():
+    x = Variable()
+    g = Gradient(autodiff.abs(x), x)
+
+    x.set_value(1.0)
+    assert autodiff.abs(x).value() == abs(x.value())
+    assert g.get().value()[0, 0] == 1.0
+    assert g.value()[0, 0] == 1.0
+
+    x.set_value(-1.0)
+    assert autodiff.abs(x).value() == abs(x.value())
+    assert g.get().value()[0, 0] == -1.0
+    assert g.value()[0, 0] == -1.0
+
+    x.set_value(0.0)
+    assert autodiff.abs(x).value() == abs(x.value())
+    assert g.get().value()[0, 0] == 0.0
+    assert g.value()[0, 0] == 0.0
+
+
+def test_atan2():
+    # Testing atan2 function on (double, var)
+    x = Variable()
+    x.set_value(1.0)
+    y = Variable()
+    y.set_value(0.9)
+    assert autodiff.atan2(2.0, x).value() == math.atan2(2.0, x.value())
+    assert Gradient(autodiff.atan2(2.0, x), x).value()[0, 0] == pytest.approx(
+        (-2.0 / (2 * 2 + x * x)).value(), abs=1e-15
+    )
+
+    # Testing atan2 function on (var, double)
+    x.set_value(1.0)
+    assert autodiff.atan2(x, 2.0).value() == math.atan2(x.value(), 2.0)
+    assert Gradient(autodiff.atan2(x, 2.0), x).value()[0, 0] == pytest.approx(
+        (2.0 / (2 * 2 + x * x)).value(), abs=1e-15
+    )
+
+    # Testing atan2 function on (var, var)
+    x.set_value(1.1)
+    assert autodiff.atan2(y, x).value() == math.atan2(y.value(), x.value())
+    assert Gradient(autodiff.atan2(y, x), y).value()[0, 0] == pytest.approx(
+        (x / (x * x + y * y)).value(), abs=1e-15
+    )
+    assert Gradient(autodiff.atan2(y, x), x).value()[0, 0] == pytest.approx(
+        (-y / (x * x + y * y)).value(), abs=1e-15
+    )
+
+    # Testing atan2 function on (expr, expr)
+    assert 3 * autodiff.atan2(autodiff.sin(y), 2 * x + 1).value() == 3 * math.atan2(
+        autodiff.sin(y).value(), 2 * x.value() + 1
+    )
+    assert Gradient(3 * autodiff.atan2(autodiff.sin(y), 2 * x + 1), y).value()[
+        0, 0
+    ] == pytest.approx(
+        (
+            3
+            * (2 * x + 1)
+            * autodiff.cos(y)
+            / ((2 * x + 1) * (2 * x + 1) + autodiff.sin(y) * autodiff.sin(y))
+        ).value(),
+        abs=1e-15,
+    )
+    assert Gradient(3 * autodiff.atan2(autodiff.sin(y), 2 * x + 1), x).value()[
+        0, 0
+    ] == pytest.approx(
+        (
+            3
+            * -2
+            * autodiff.sin(y)
+            / ((2 * x + 1) * (2 * x + 1) + autodiff.sin(y) * autodiff.sin(y))
+        ).value(),
+        abs=1e-15,
+    )
+
+
+def test_hypot():
+    # Testing hypot function on (var, double)
+    x = Variable()
+    x.set_value(1.8)
+    y = Variable()
+    y.set_value(1.5)
+    assert autodiff.hypot(x, 2.0).value() == math.hypot(x.value(), 2.0)
+    assert (
+        Gradient(autodiff.hypot(x, 2.0), x).value()[0, 0]
+        == (x / math.hypot(x.value(), 2.0)).value()
+    )
+
+    # Testing hypot function on (double, var)
+    assert autodiff.hypot(2.0, y).value() == math.hypot(2.0, y.value())
+    assert (
+        Gradient(autodiff.hypot(2.0, y), y).value()[0, 0]
+        == (y / math.hypot(2.0, y.value())).value()
+    )
+
+    # Testing hypot function on (var, var)
+    x.set_value(1.3)
+    y.set_value(2.3)
+    assert autodiff.hypot(x, y).value() == math.hypot(x.value(), y.value())
+    assert (
+        Gradient(autodiff.hypot(x, y), x).value()[0, 0]
+        == (x / math.hypot(x.value(), y.value())).value()
+    )
+    assert (
+        Gradient(autodiff.hypot(x, y), y).value()[0, 0]
+        == (y / math.hypot(x.value(), y.value())).value()
+    )
+
+    # Testing hypot function on (expr, expr)
+    x.set_value(1.3)
+    y.set_value(2.3)
+    assert autodiff.hypot(2.0 * x, 3.0 * y).value() == math.hypot(
+        2.0 * x.value(), 3.0 * y.value()
+    )
+    assert (
+        Gradient(autodiff.hypot(2.0 * x, 3.0 * y), x).value()[0, 0]
+        == (4.0 * x / math.hypot(2.0 * x.value(), 3.0 * y.value())).value()
+    )
+    assert (
+        Gradient(autodiff.hypot(2.0 * x, 3.0 * y), y).value()[0, 0]
+        == (9.0 * y / math.hypot(2.0 * x.value(), 3.0 * y.value())).value()
+    )
+
+    # Testing hypot function on (var, var, var)
+    x.set_value(1.3)
+    y.set_value(2.3)
+    z = Variable()
+    z.set_value(3.3)
+    assert autodiff.hypot(x, y, z).value() == math.hypot(
+        x.value(), y.value(), z.value()
+    )
+    assert (
+        Gradient(autodiff.hypot(x, y, z), x).value()[0, 0]
+        == (x / math.hypot(x.value(), y.value(), z.value())).value()
+    )
+    assert (
+        Gradient(autodiff.hypot(x, y, z), y).value()[0, 0]
+        == (y / math.hypot(x.value(), y.value(), z.value())).value()
+    )
+    assert (
+        Gradient(autodiff.hypot(x, y, z), z).value()[0, 0]
+        == (z / math.hypot(x.value(), y.value(), z.value())).value()
+    )
+
+
+def test_miscellaneous():
+    x = Variable()
+
+    # dx/dx
+    x.set_value(3.0)
+    g = Gradient(x, x)
+    assert autodiff.abs(x).value() == abs(x.value())
+    assert g.get().value()[0, 0] == 1.0
+    assert g.value()[0, 0] == 1.0
+
+    # erf(x)
+    x.set_value(0.5)
+    g = Gradient(autodiff.erf(x), x)
+    assert autodiff.erf(x).value() == math.erf(x.value())
+    assert g.get().value()[0, 0] == 2.0 / math.sqrt(math.pi) * math.exp(
+        -x.value() * x.value()
+    )
+    assert g.value()[0, 0] == 2.0 / math.sqrt(math.pi) * math.exp(
+        -x.value() * x.value()
+    )
+
+
+def test_reuse():
+    a = Variable()
+    a.set_value(10)
+
+    b = Variable()
+    b.set_value(20)
+
+    x = a * b
+
+    g = Gradient(x, a)
+
+    assert g.get().value()[0] == 20.0
+    assert g.value()[0] == 20.0
+
+    b.set_value(10)
+    assert g.get().value()[0] == 10.0
+    assert g.value()[0] == 10.0
+
+
+def test_sign():
+    def sign(x):
+        if x < 0.0:
+            return -1.0
+        elif x == 0.0:
+            return 0.0
+        else:
+            return 1.0
+
+    x = Variable()
+
+    x.set_value(1.0)
+    g = Gradient(autodiff.sign(x), x)
+    assert sign(x.value()) == autodiff.sign(x).value()
+    assert g.get().value()[0, 0] == 0.0
+    assert g.value()[0, 0] == 0.0
+
+    x.set_value(-1.0)
+    g = Gradient(autodiff.sign(x), x)
+    assert sign(x.value()) == autodiff.sign(x).value()
+    assert g.get().value()[0, 0] == 0.0
+    assert g.value()[0, 0] == 0.0
+
+    x.set_value(0.0)
+    g = Gradient(autodiff.sign(x), x)
+    assert sign(x.value()) == autodiff.sign(x).value()
+    assert g.get().value()[0, 0] == 0.0
+    assert g.value()[0, 0] == 0.0
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/autodiff/hessian_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/autodiff/hessian_test.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-from functools import reduce
-import math
-import operator
-
-from jormungandr.autodiff import Gradient, Hessian, Variable, VariableMatrix
-import jormungandr.autodiff as autodiff
-import numpy as np
-import pytest
-
-
-def prod(iterable):
-    return reduce(operator.mul, iterable, 1)
-
-
-def test_linear():
-    # y = x
-    x = VariableMatrix(1)
-    x[0].set_value(3)
-    y = x[0]
-
-    # dy/dx = 1
-    g = Gradient(y, x[0]).value()[0, 0]
-    assert g == 1.0
-
-    # d²y/dx² = 0
-    H = Hessian(y, x)
-    assert H.get().value()[0, 0] == 0.0
-    assert H.value()[0, 0] == 0.0
-
-
-def test_quartic():
-    # y = x²
-    # y = x * x
-    x = VariableMatrix(1)
-    x[0].set_value(3)
-    y = x[0] * x[0]
-
-    # dy/dx = x (rhs) + x (lhs)
-    #       = (3) + (3)
-    #       = 6
-    g = Gradient(y, x[0]).value()[0, 0]
-    assert g == 6.0
-
-    # d²y/dx² = d/dx(x (rhs) + x (lhs))
-    #         = 1 + 1
-    #         = 2
-    H = Hessian(y, x)
-    assert H.get().value()[0, 0] == 2.0
-    assert H.value()[0, 0] == 2.0
-
-
-def test_sum():
-    y = Variable()
-    x = VariableMatrix(5)
-    x[0].set_value(1)
-    x[1].set_value(2)
-    x[2].set_value(3)
-    x[3].set_value(4)
-    x[4].set_value(5)
-
-    y = sum(x)
-    assert y.value() == 15.0
-
-    g = Gradient(y, x)
-    assert (g.get().value() == np.full((5, 1), 1.0)).all()
-    assert (g.value() == np.full((5, 1), 1.0)).all()
-
-    H = Hessian(y, x)
-    assert (H.get().value() == np.zeros((5, 5))).all()
-    assert (H.value() == np.zeros((5, 5))).all()
-
-
-def test_sum_of_products():
-    x = VariableMatrix(5)
-    x[0].set_value(1)
-    x[1].set_value(2)
-    x[2].set_value(3)
-    x[3].set_value(4)
-    x[4].set_value(5)
-
-    # y = ||x||²
-    y = (x.T @ x)[0, 0]
-    assert y.value() == 1 + 2 * 2 + 3 * 3 + 4 * 4 + 5 * 5
-
-    g = Gradient(y, x)
-    assert (g.get().value() == 2 * x.value()).all()
-    assert (g.value() == 2 * x.value()).all()
-
-    H = Hessian(y, x)
-
-    expected_H = np.diag([2.0] * 5)
-    assert (H.get().value() == expected_H).all()
-    assert (H.value() == expected_H).all()
-
-
-def test_product_of_sines():
-    x = VariableMatrix(5)
-    x[0].set_value(1)
-    x[1].set_value(2)
-    x[2].set_value(3)
-    x[3].set_value(4)
-    x[4].set_value(5)
-
-    # y = prod(sin(x))
-    y = prod(x.cwise_transform(autodiff.sin))
-    assert y.value() == math.sin(1) * math.sin(2) * math.sin(3) * math.sin(
-        4
-    ) * math.sin(5)
-
-    g = Gradient(y, x)
-    for i in range(x.rows()):
-        assert g.get().value()[i, 0] == pytest.approx(
-            (y / autodiff.tan(x[i])).value(), abs=1e-15
-        )
-        assert g.value()[i, 0] == pytest.approx(
-            (y / autodiff.tan(x[i])).value(), abs=1e-15
-        )
-
-    H = Hessian(y, x)
-
-    expected_H = np.empty((5, 5))
-    for i in range(x.rows()):
-        for j in range(x.rows()):
-            if i == j:
-                expected_H[i, j] = (g.value()[i, 0] / autodiff.tan(x[i])).value() * (
-                    1.0 - 1.0 / (autodiff.cos(x[i]) * autodiff.cos(x[i]))
-                ).value()
-            else:
-                expected_H[i, j] = (g.value()[j, 0] / autodiff.tan(x[i])).value()
-
-    actual_H = H.get().value()
-    for i in range(x.rows()):
-        for j in range(x.rows()):
-            assert actual_H[i, j] == pytest.approx(expected_H[i, j], abs=1e-15)
-
-    actual_H = H.value()
-    for i in range(x.rows()):
-        for j in range(x.rows()):
-            assert actual_H[i, j] == pytest.approx(expected_H[i, j], abs=1e-15)
-
-
-def test_sum_of_squared_residuals():
-    y = Variable()
-    x = VariableMatrix(5)
-    x[0].set_value(1)
-    x[1].set_value(1)
-    x[2].set_value(1)
-    x[3].set_value(1)
-    x[4].set_value(1)
-
-    # y = sum(diff(x).^2)
-    y = sum((x[:4, :1] - x[1:5, :1]).cwise_transform(lambda x: x**2))
-    g = Gradient(y, x).value()
-
-    assert y.value() == 0.0
-    assert g[0, 0] == (2 * x[0] - 2 * x[1]).value()
-    assert g[1, 0] == (-2 * x[0] + 4 * x[1] - 2 * x[2]).value()
-    assert g[2, 0] == (-2 * x[1] + 4 * x[2] - 2 * x[3]).value()
-    assert g[3, 0] == (-2 * x[2] + 4 * x[3] - 2 * x[4]).value()
-    assert g[4, 0] == (-2 * x[3] + 2 * x[4]).value()
-
-    H = Hessian(y, x)
-
-    expected_H = np.array(
-        [
-            [2.0, -2.0, 0.0, 0.0, 0.0],
-            [-2.0, 4.0, -2.0, 0.0, 0.0],
-            [0.0, -2.0, 4.0, -2.0, 0.0],
-            [0.0, 0.0, -2.0, 4.0, -2.0],
-            [0.0, 0.0, 0.0, -2.0, 2.0],
-        ]
-    )
-
-    actual_H = H.get().value()
-    for i in range(x.rows()):
-        for j in range(x.rows()):
-            assert actual_H[i, j] == expected_H[i, j]
-
-    actual_H = H.value()
-    for i in range(x.rows()):
-        for j in range(x.rows()):
-            assert actual_H[i, j] == expected_H[i, j]
-
-
-def test_sum_of_squares():
-    r = VariableMatrix(4)
-    r[0].set_value(25.0)
-    r[1].set_value(10.0)
-    r[2].set_value(5.0)
-    r[3].set_value(0.0)
-    x = VariableMatrix(4)
-    x[0].set_value(0.0)
-    x[1].set_value(0.0)
-    x[2].set_value(0.0)
-    x[3].set_value(0.0)
-
-    J = 0.0
-    for i in range(4):
-        J += (r[i] - x[i]) * (r[i] - x[i])
-
-    H = Hessian(J, x)
-
-    expected_H = np.diag([2.0] * 4)
-    assert (H.get().value() == expected_H).all()
-    assert (H.value() == expected_H).all()
-
-
-def test_rosenbrock():
-    input = VariableMatrix(2)
-    x = input[0]
-    y = input[1]
-
-    for x0 in np.arange(-2.5, 2.5, 0.1):
-        for y0 in np.arange(-2.5, 2.5, 0.1):
-            x.set_value(x0)
-            y.set_value(y0)
-            z = (1 - x) ** 2 + 100 * (y - x**2) ** 2
-
-            H = Hessian(z, input).value()
-            assert H[0, 0] == pytest.approx(
-                -400 * (y0 - x0 * x0) + 800 * x0 * x0 + 2, abs=1e-12
-            )
-            assert H[0, 1] == -400 * x0
-            assert H[1, 0] == -400 * x0
-            assert H[1, 1] == 200
-
-
-def test_variable_reuse():
-    y = Variable()
-    x = VariableMatrix(1)
-
-    # y = x³
-    x[0].set_value(1)
-    y = x[0] * x[0] * x[0]
-
-    hessian = Hessian(y, x)
-
-    # d²y/dx² = 6x
-    # H = 6
-    H = hessian.value()
-
-    assert H.shape == (1, 1)
-    assert H[0, 0] == 6.0
-
-    x[0].set_value(2)
-    # d²y/dx² = 6x
-    # H = 12
-    H = hessian.value()
-
-    assert H.shape == (1, 1)
-    assert H[0, 0] == 12.0
+from functools import reduce
+import math
+import operator
+
+from jormungandr.autodiff import Gradient, Hessian, Variable, VariableMatrix
+import jormungandr.autodiff as autodiff
+import numpy as np
+import pytest
+
+
+def prod(iterable):
+    return reduce(operator.mul, iterable, 1)
+
+
+def test_linear():
+    # y = x
+    x = VariableMatrix(1)
+    x[0].set_value(3)
+    y = x[0]
+
+    # dy/dx = 1
+    g = Gradient(y, x[0]).value()[0, 0]
+    assert g == 1.0
+
+    # d²y/dx² = 0
+    H = Hessian(y, x)
+    assert H.get().value()[0, 0] == 0.0
+    assert H.value()[0, 0] == 0.0
+
+
+def test_quartic():
+    # y = x²
+    # y = x * x
+    x = VariableMatrix(1)
+    x[0].set_value(3)
+    y = x[0] * x[0]
+
+    # dy/dx = x (rhs) + x (lhs)
+    #       = (3) + (3)
+    #       = 6
+    g = Gradient(y, x[0]).value()[0, 0]
+    assert g == 6.0
+
+    # d²y/dx² = d/dx(x (rhs) + x (lhs))
+    #         = 1 + 1
+    #         = 2
+    H = Hessian(y, x)
+    assert H.get().value()[0, 0] == 2.0
+    assert H.value()[0, 0] == 2.0
+
+
+def test_sum():
+    y = Variable()
+    x = VariableMatrix(5)
+    x[0].set_value(1)
+    x[1].set_value(2)
+    x[2].set_value(3)
+    x[3].set_value(4)
+    x[4].set_value(5)
+
+    y = sum(x)
+    assert y.value() == 15.0
+
+    g = Gradient(y, x)
+    assert (g.get().value() == np.full((5, 1), 1.0)).all()
+    assert (g.value() == np.full((5, 1), 1.0)).all()
+
+    H = Hessian(y, x)
+    assert (H.get().value() == np.zeros((5, 5))).all()
+    assert (H.value() == np.zeros((5, 5))).all()
+
+
+def test_sum_of_products():
+    x = VariableMatrix(5)
+    x[0].set_value(1)
+    x[1].set_value(2)
+    x[2].set_value(3)
+    x[3].set_value(4)
+    x[4].set_value(5)
+
+    # y = ||x||²
+    y = (x.T @ x)[0, 0]
+    assert y.value() == 1 + 2 * 2 + 3 * 3 + 4 * 4 + 5 * 5
+
+    g = Gradient(y, x)
+    assert (g.get().value() == 2 * x.value()).all()
+    assert (g.value() == 2 * x.value()).all()
+
+    H = Hessian(y, x)
+
+    expected_H = np.diag([2.0] * 5)
+    assert (H.get().value() == expected_H).all()
+    assert (H.value() == expected_H).all()
+
+
+def test_product_of_sines():
+    x = VariableMatrix(5)
+    x[0].set_value(1)
+    x[1].set_value(2)
+    x[2].set_value(3)
+    x[3].set_value(4)
+    x[4].set_value(5)
+
+    # y = prod(sin(x))
+    y = prod(x.cwise_transform(autodiff.sin))
+    assert y.value() == math.sin(1) * math.sin(2) * math.sin(3) * math.sin(
+        4
+    ) * math.sin(5)
+
+    g = Gradient(y, x)
+    for i in range(x.rows()):
+        assert g.get().value()[i, 0] == pytest.approx(
+            (y / autodiff.tan(x[i])).value(), abs=1e-15
+        )
+        assert g.value()[i, 0] == pytest.approx(
+            (y / autodiff.tan(x[i])).value(), abs=1e-15
+        )
+
+    H = Hessian(y, x)
+
+    expected_H = np.empty((5, 5))
+    for i in range(x.rows()):
+        for j in range(x.rows()):
+            if i == j:
+                expected_H[i, j] = (g.value()[i, 0] / autodiff.tan(x[i])).value() * (
+                    1.0 - 1.0 / (autodiff.cos(x[i]) * autodiff.cos(x[i]))
+                ).value()
+            else:
+                expected_H[i, j] = (g.value()[j, 0] / autodiff.tan(x[i])).value()
+
+    actual_H = H.get().value()
+    for i in range(x.rows()):
+        for j in range(x.rows()):
+            assert actual_H[i, j] == pytest.approx(expected_H[i, j], abs=1e-15)
+
+    actual_H = H.value()
+    for i in range(x.rows()):
+        for j in range(x.rows()):
+            assert actual_H[i, j] == pytest.approx(expected_H[i, j], abs=1e-15)
+
+
+def test_sum_of_squared_residuals():
+    y = Variable()
+    x = VariableMatrix(5)
+    x[0].set_value(1)
+    x[1].set_value(1)
+    x[2].set_value(1)
+    x[3].set_value(1)
+    x[4].set_value(1)
+
+    # y = sum(diff(x).^2)
+    y = sum((x[:4, :1] - x[1:5, :1]).cwise_transform(lambda x: x**2))
+    g = Gradient(y, x).value()
+
+    assert y.value() == 0.0
+    assert g[0, 0] == (2 * x[0] - 2 * x[1]).value()
+    assert g[1, 0] == (-2 * x[0] + 4 * x[1] - 2 * x[2]).value()
+    assert g[2, 0] == (-2 * x[1] + 4 * x[2] - 2 * x[3]).value()
+    assert g[3, 0] == (-2 * x[2] + 4 * x[3] - 2 * x[4]).value()
+    assert g[4, 0] == (-2 * x[3] + 2 * x[4]).value()
+
+    H = Hessian(y, x)
+
+    expected_H = np.array(
+        [
+            [2.0, -2.0, 0.0, 0.0, 0.0],
+            [-2.0, 4.0, -2.0, 0.0, 0.0],
+            [0.0, -2.0, 4.0, -2.0, 0.0],
+            [0.0, 0.0, -2.0, 4.0, -2.0],
+            [0.0, 0.0, 0.0, -2.0, 2.0],
+        ]
+    )
+
+    actual_H = H.get().value()
+    for i in range(x.rows()):
+        for j in range(x.rows()):
+            assert actual_H[i, j] == expected_H[i, j]
+
+    actual_H = H.value()
+    for i in range(x.rows()):
+        for j in range(x.rows()):
+            assert actual_H[i, j] == expected_H[i, j]
+
+
+def test_sum_of_squares():
+    r = VariableMatrix(4)
+    r[0].set_value(25.0)
+    r[1].set_value(10.0)
+    r[2].set_value(5.0)
+    r[3].set_value(0.0)
+    x = VariableMatrix(4)
+    x[0].set_value(0.0)
+    x[1].set_value(0.0)
+    x[2].set_value(0.0)
+    x[3].set_value(0.0)
+
+    J = 0.0
+    for i in range(4):
+        J += (r[i] - x[i]) * (r[i] - x[i])
+
+    H = Hessian(J, x)
+
+    expected_H = np.diag([2.0] * 4)
+    assert (H.get().value() == expected_H).all()
+    assert (H.value() == expected_H).all()
+
+
+def test_rosenbrock():
+    input = VariableMatrix(2)
+    x = input[0]
+    y = input[1]
+
+    for x0 in np.arange(-2.5, 2.5, 0.1):
+        for y0 in np.arange(-2.5, 2.5, 0.1):
+            x.set_value(x0)
+            y.set_value(y0)
+            z = (1 - x) ** 2 + 100 * (y - x**2) ** 2
+
+            H = Hessian(z, input).value()
+            assert H[0, 0] == pytest.approx(
+                -400 * (y0 - x0 * x0) + 800 * x0 * x0 + 2, abs=1e-12
+            )
+            assert H[0, 1] == -400 * x0
+            assert H[1, 0] == -400 * x0
+            assert H[1, 1] == 200
+
+
+def test_variable_reuse():
+    y = Variable()
+    x = VariableMatrix(1)
+
+    # y = x³
+    x[0].set_value(1)
+    y = x[0] * x[0] * x[0]
+
+    hessian = Hessian(y, x)
+
+    # d²y/dx² = 6x
+    # H = 6
+    H = hessian.value()
+
+    assert H.shape == (1, 1)
+    assert H[0, 0] == 6.0
+
+    x[0].set_value(2)
+    # d²y/dx² = 6x
+    # H = 12
+    H = hessian.value()
+
+    assert H.shape == (1, 1)
+    assert H[0, 0] == 12.0
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/constraints_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/constraints_test.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-from jormungandr.autodiff import Variable, VariableMatrix
-
-import numpy as np
-
-
-def test_equality_constraint_boolean_comparisons():
-    args = [(1.0, 1.0), (1.0, 2.0), (2.0, 1.0)]
-
-    # double-Variable
-    for lhs, rhs in args:
-        assert bool(float(lhs) == Variable(rhs)) == (lhs == rhs)
-
-    # double-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(float(lhs) == VariableMatrix([[rhs]])) == (lhs == rhs)
-
-    # Variable-double
-    for lhs, rhs in args:
-        assert bool(Variable(lhs) == float(rhs)) == (lhs == rhs)
-
-    # Variable-Variable
-    for lhs, rhs in args:
-        assert bool(Variable(lhs) == Variable(rhs)) == (lhs == rhs)
-
-    # Variable-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(Variable(lhs) == VariableMatrix([[rhs]])) == (lhs == rhs)
-
-    # VariableMatrix-double
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) == float(rhs)) == (lhs == rhs)
-
-    # VariableMatrix-Variable
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) == Variable(rhs)) == (lhs == rhs)
-
-    # VariableMatrix-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) == VariableMatrix([[rhs]])) == (lhs == rhs)
-
-    # np.array-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(np.array([[lhs]]) == VariableMatrix([[rhs]])) == (lhs == rhs)
-
-    # np.array-VariableBlock
-    for lhs, rhs in args:
-        assert bool(np.array([[lhs]]) == VariableMatrix([[rhs]])[:, :]) == (lhs == rhs)
-
-    # VariableMatrix-np.array
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) == np.array([[rhs]])) == (lhs == rhs)
-
-    # VariableBlock-np.array
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]])[:, :] == np.array([[rhs]])) == (lhs == rhs)
-
-
-# For the purposes of optimization, a < constraint is treated the same as a <=
-# constraint
-def test_inequality_constraint_boolean_comparisons():
-    args = [(1.0, 1.0), (1.0, 2.0), (2.0, 1.0)]
-
-    # double-Variable
-    for lhs, rhs in args:
-        assert bool(float(lhs) < Variable(rhs)) == (lhs <= rhs)
-        assert bool(float(lhs) <= Variable(rhs)) == (lhs <= rhs)
-        assert bool(float(lhs) > Variable(rhs)) == (lhs >= rhs)
-        assert bool(float(lhs) >= Variable(rhs)) == (lhs >= rhs)
-
-    # double-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(float(lhs) < VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(float(lhs) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(float(lhs) > VariableMatrix([[rhs]])) == (lhs >= rhs)
-        assert bool(float(lhs) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
-
-    # Variable-Variable
-    for lhs, rhs in args:
-        assert bool(Variable(lhs) < Variable(rhs)) == (lhs <= rhs)
-        assert bool(Variable(lhs) <= Variable(rhs)) == (lhs <= rhs)
-        assert bool(Variable(lhs) > Variable(rhs)) == (lhs >= rhs)
-        assert bool(Variable(lhs) >= Variable(rhs)) == (lhs >= rhs)
-
-    # Variable-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(Variable(lhs) < VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(Variable(lhs) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(Variable(lhs) > VariableMatrix([[rhs]])) == (lhs >= rhs)
-        assert bool(Variable(lhs) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
-
-    # VariableMatrix-double
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) < float(rhs)) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) <= float(rhs)) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) > float(rhs)) == (lhs >= rhs)
-        assert bool(VariableMatrix([[lhs]]) >= float(rhs)) == (lhs >= rhs)
-
-    # VariableMatrix-Variable
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) < Variable(rhs)) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) <= Variable(rhs)) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) > Variable(rhs)) == (lhs >= rhs)
-        assert bool(VariableMatrix([[lhs]]) >= Variable(rhs)) == (lhs >= rhs)
-
-    # VariableMatrix-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) < VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) > VariableMatrix([[rhs]])) == (lhs >= rhs)
-        assert bool(VariableMatrix([[lhs]]) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
-
-    # np.array-VariableMatrix
-    for lhs, rhs in args:
-        assert bool(np.array([[lhs]]) < VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(np.array([[lhs]]) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
-        assert bool(np.array([[lhs]]) > VariableMatrix([[rhs]])) == (lhs >= rhs)
-        assert bool(np.array([[lhs]]) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
-
-    # np.array-VariableBlock
-    for lhs, rhs in args:
-        assert bool(np.array([[lhs]]) < VariableMatrix([[rhs]])[:, :]) == (lhs <= rhs)
-        assert bool(np.array([[lhs]]) <= VariableMatrix([[rhs]])[:, :]) == (lhs <= rhs)
-        assert bool(np.array([[lhs]]) > VariableMatrix([[rhs]])[:, :]) == (lhs >= rhs)
-        assert bool(np.array([[lhs]]) >= VariableMatrix([[rhs]])[:, :]) == (lhs >= rhs)
-
-    # VariableMatrix-np.array
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]]) < np.array([[rhs]])) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) <= np.array([[rhs]])) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]]) > np.array([[rhs]])) == (lhs >= rhs)
-        assert bool(VariableMatrix([[lhs]]) >= np.array([[rhs]])) == (lhs >= rhs)
-
-    # VariableBlock-np.array
-    for lhs, rhs in args:
-        assert bool(VariableMatrix([[lhs]])[:, :] < np.array([[rhs]])) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]])[:, :] <= np.array([[rhs]])) == (lhs <= rhs)
-        assert bool(VariableMatrix([[lhs]])[:, :] > np.array([[rhs]])) == (lhs >= rhs)
-        assert bool(VariableMatrix([[lhs]])[:, :] >= np.array([[rhs]])) == (lhs >= rhs)
+from jormungandr.autodiff import Variable, VariableMatrix
+
+import numpy as np
+
+
+def test_equality_constraint_boolean_comparisons():
+    args = [(1.0, 1.0), (1.0, 2.0), (2.0, 1.0)]
+
+    # double-Variable
+    for lhs, rhs in args:
+        assert bool(float(lhs) == Variable(rhs)) == (lhs == rhs)
+
+    # double-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(float(lhs) == VariableMatrix([[rhs]])) == (lhs == rhs)
+
+    # Variable-double
+    for lhs, rhs in args:
+        assert bool(Variable(lhs) == float(rhs)) == (lhs == rhs)
+
+    # Variable-Variable
+    for lhs, rhs in args:
+        assert bool(Variable(lhs) == Variable(rhs)) == (lhs == rhs)
+
+    # Variable-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(Variable(lhs) == VariableMatrix([[rhs]])) == (lhs == rhs)
+
+    # VariableMatrix-double
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) == float(rhs)) == (lhs == rhs)
+
+    # VariableMatrix-Variable
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) == Variable(rhs)) == (lhs == rhs)
+
+    # VariableMatrix-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) == VariableMatrix([[rhs]])) == (lhs == rhs)
+
+    # np.array-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(np.array([[lhs]]) == VariableMatrix([[rhs]])) == (lhs == rhs)
+
+    # np.array-VariableBlock
+    for lhs, rhs in args:
+        assert bool(np.array([[lhs]]) == VariableMatrix([[rhs]])[:, :]) == (lhs == rhs)
+
+    # VariableMatrix-np.array
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) == np.array([[rhs]])) == (lhs == rhs)
+
+    # VariableBlock-np.array
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]])[:, :] == np.array([[rhs]])) == (lhs == rhs)
+
+
+# For the purposes of optimization, a < constraint is treated the same as a <=
+# constraint
+def test_inequality_constraint_boolean_comparisons():
+    args = [(1.0, 1.0), (1.0, 2.0), (2.0, 1.0)]
+
+    # double-Variable
+    for lhs, rhs in args:
+        assert bool(float(lhs) < Variable(rhs)) == (lhs <= rhs)
+        assert bool(float(lhs) <= Variable(rhs)) == (lhs <= rhs)
+        assert bool(float(lhs) > Variable(rhs)) == (lhs >= rhs)
+        assert bool(float(lhs) >= Variable(rhs)) == (lhs >= rhs)
+
+    # double-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(float(lhs) < VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(float(lhs) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(float(lhs) > VariableMatrix([[rhs]])) == (lhs >= rhs)
+        assert bool(float(lhs) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
+
+    # Variable-Variable
+    for lhs, rhs in args:
+        assert bool(Variable(lhs) < Variable(rhs)) == (lhs <= rhs)
+        assert bool(Variable(lhs) <= Variable(rhs)) == (lhs <= rhs)
+        assert bool(Variable(lhs) > Variable(rhs)) == (lhs >= rhs)
+        assert bool(Variable(lhs) >= Variable(rhs)) == (lhs >= rhs)
+
+    # Variable-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(Variable(lhs) < VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(Variable(lhs) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(Variable(lhs) > VariableMatrix([[rhs]])) == (lhs >= rhs)
+        assert bool(Variable(lhs) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
+
+    # VariableMatrix-double
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) < float(rhs)) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) <= float(rhs)) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) > float(rhs)) == (lhs >= rhs)
+        assert bool(VariableMatrix([[lhs]]) >= float(rhs)) == (lhs >= rhs)
+
+    # VariableMatrix-Variable
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) < Variable(rhs)) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) <= Variable(rhs)) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) > Variable(rhs)) == (lhs >= rhs)
+        assert bool(VariableMatrix([[lhs]]) >= Variable(rhs)) == (lhs >= rhs)
+
+    # VariableMatrix-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) < VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) > VariableMatrix([[rhs]])) == (lhs >= rhs)
+        assert bool(VariableMatrix([[lhs]]) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
+
+    # np.array-VariableMatrix
+    for lhs, rhs in args:
+        assert bool(np.array([[lhs]]) < VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(np.array([[lhs]]) <= VariableMatrix([[rhs]])) == (lhs <= rhs)
+        assert bool(np.array([[lhs]]) > VariableMatrix([[rhs]])) == (lhs >= rhs)
+        assert bool(np.array([[lhs]]) >= VariableMatrix([[rhs]])) == (lhs >= rhs)
+
+    # np.array-VariableBlock
+    for lhs, rhs in args:
+        assert bool(np.array([[lhs]]) < VariableMatrix([[rhs]])[:, :]) == (lhs <= rhs)
+        assert bool(np.array([[lhs]]) <= VariableMatrix([[rhs]])[:, :]) == (lhs <= rhs)
+        assert bool(np.array([[lhs]]) > VariableMatrix([[rhs]])[:, :]) == (lhs >= rhs)
+        assert bool(np.array([[lhs]]) >= VariableMatrix([[rhs]])[:, :]) == (lhs >= rhs)
+
+    # VariableMatrix-np.array
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]]) < np.array([[rhs]])) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) <= np.array([[rhs]])) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]]) > np.array([[rhs]])) == (lhs >= rhs)
+        assert bool(VariableMatrix([[lhs]]) >= np.array([[rhs]])) == (lhs >= rhs)
+
+    # VariableBlock-np.array
+    for lhs, rhs in args:
+        assert bool(VariableMatrix([[lhs]])[:, :] < np.array([[rhs]])) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]])[:, :] <= np.array([[rhs]])) == (lhs <= rhs)
+        assert bool(VariableMatrix([[lhs]])[:, :] > np.array([[rhs]])) == (lhs >= rhs)
+        assert bool(VariableMatrix([[lhs]])[:, :] >= np.array([[rhs]])) == (lhs >= rhs)
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/linear_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/linear_problem_test.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-
-import pytest
-
-
-def test_maximize():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    x.set_value(1.0)
-
-    y = problem.decision_variable()
-    y.set_value(1.0)
-
-    problem.maximize(50 * x + 40 * y)
-
-    problem.subject_to(x + 1.5 * y <= 750)
-    problem.subject_to(2 * x + 3 * y <= 1500)
-    problem.subject_to(2 * x + y <= 1000)
-    problem.subject_to(x >= 0)
-    problem.subject_to(y >= 0)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.LINEAR
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.LINEAR
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value() == pytest.approx(375.0, abs=1e-6)
-    assert y.value() == pytest.approx(250.0, abs=1e-6)
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+
+import pytest
+
+
+def test_maximize():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    x.set_value(1.0)
+
+    y = problem.decision_variable()
+    y.set_value(1.0)
+
+    problem.maximize(50 * x + 40 * y)
+
+    problem.subject_to(x + 1.5 * y <= 750)
+    problem.subject_to(2 * x + 3 * y <= 1500)
+    problem.subject_to(2 * x + y <= 1000)
+    problem.subject_to(x >= 0)
+    problem.subject_to(y >= 0)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.LINEAR
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.LINEAR
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value() == pytest.approx(375.0, abs=1e-6)
+    assert y.value() == pytest.approx(250.0, abs=1e-6)
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/nonlinear_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/quadratic_problem_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,144 @@
-import platform
-
-import jormungandr.autodiff as autodiff
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-
-import numpy as np
-import pytest
-
-
-def test_quartic():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    x.set_value(20.0)
-
-    problem.minimize(autodiff.pow(x, 4))
-
-    problem.subject_to(x >= 1)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONLINEAR
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.LINEAR
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value() == pytest.approx(1.0, abs=1e-6)
-
-
-def test_rosenbrock_with_cubic_and_line_constraint():
-    # https://en.wikipedia.org/wiki/Test_functions_for_optimization#Test_functions_for_constrained_optimization
-    for x0 in np.arange(-1.5, 1.5, 0.1):
-        for y0 in np.arange(-0.5, 2.5, 0.1):
-            problem = OptimizationProblem()
-
-            x = problem.decision_variable()
-            x.set_value(x0)
-            y = problem.decision_variable()
-            y.set_value(y0)
-
-            problem.minimize(
-                autodiff.pow(1 - x, 2) + 100 * autodiff.pow(y - autodiff.pow(x, 2), 2)
-            )
-
-            problem.subject_to(autodiff.pow(x - 1, 3) - y + 1 <= 0)
-            problem.subject_to(x + y - 2 <= 0)
-
-            status = problem.solve()
-
-            assert status.cost_function_type == ExpressionType.NONLINEAR
-            assert status.equality_constraint_type == ExpressionType.NONE
-            assert status.inequality_constraint_type == ExpressionType.NONLINEAR
-            assert status.exit_condition == SolverExitCondition.SUCCESS
-
-            # Local minimum at (0.0, 0.0)
-            # Global minimum at (1.0, 1.0)
-            assert x.value() == pytest.approx(
-                0.0, abs=1e-2
-            ) or x.value() == pytest.approx(1.0, abs=1e-2)
-            assert y.value() == pytest.approx(
-                0.0, abs=1e-2
-            ) or y.value() == pytest.approx(1.0, abs=1e-2)
-
-
-def test_rosenbrock_with_disk_constraint():
-    # https://en.wikipedia.org/wiki/Test_functions_for_optimization#Test_functions_for_constrained_optimization
-    for x0 in np.arange(-1.5, 1.5, 0.1):
-        for y0 in np.arange(-1.5, 1.5, 0.1):
-            problem = OptimizationProblem()
-
-            x = problem.decision_variable()
-            x.set_value(x0)
-            y = problem.decision_variable()
-            y.set_value(y0)
-
-            problem.minimize(
-                autodiff.pow(1 - x, 2) + 100 * autodiff.pow(y - autodiff.pow(x, 2), 2)
-            )
-
-            problem.subject_to(autodiff.pow(x, 2) + autodiff.pow(y, 2) <= 2)
-
-            status = problem.solve()
-
-            assert status.cost_function_type == ExpressionType.NONLINEAR
-            assert status.equality_constraint_type == ExpressionType.NONE
-            assert status.inequality_constraint_type == ExpressionType.QUADRATIC
-            assert status.exit_condition == SolverExitCondition.SUCCESS
-
-            assert x.value() == pytest.approx(1.0, abs=1e-1)
-            assert y.value() == pytest.approx(1.0, abs=1e-1)
-
-
-def test_narrow_feasible_region():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    x.set_value(20.0)
-
-    y = problem.decision_variable()
-    y.set_value(50.0)
-
-    problem.minimize(autodiff.sqrt(x * x + y * y))
-
-    problem.subject_to(y == -x + 5.0)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONLINEAR
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.NONE
-
-    if platform.system() == "Darwin" and platform.machine() == "arm64":
-        # FIXME: Fails on macOS arm64 with "diverging iterates"
-        assert status.exit_condition == SolverExitCondition.DIVERGING_ITERATES
-        return
-    else:
-        assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value() == pytest.approx(2.5, abs=1e-2)
-    assert y.value() == pytest.approx(2.5, abs=1e-2)
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+import numpy as np
+import pytest
+
+
+def test_unconstrained1d():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    x.set_value(2.0)
+
+    problem.minimize(x * x - 6.0 * x)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value() == pytest.approx(3.0, abs=1e-6)
+
+
+def test_unconstrained2d_1():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    x.set_value(1.0)
+    y = problem.decision_variable()
+    y.set_value(2.0)
+
+    problem.minimize(x * x + y * y)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value() == pytest.approx(0.0, abs=1e-6)
+    assert y.value() == pytest.approx(0.0, abs=1e-6)
+
+
+def test_unconstrained2d_2():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable(2)
+    x[0].set_value(1.0)
+    x[1].set_value(2.0)
+
+    problem.minimize(x.T @ x)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value(0) == pytest.approx(0.0, abs=1e-6)
+    assert x.value(1) == pytest.approx(0.0, abs=1e-6)
+
+
+# Maximize xy subject to x + 3y = 36.
+#
+# Maximize f(x,y) = xy
+# subject to g(x,y) = x + 3y - 36 = 0
+#
+#         value func  constraint
+#              |          |
+#              v          v
+# L(x,y,λ) = f(x,y) - λg(x,y)
+# L(x,y,λ) = xy - λ(x + 3y - 36)
+# L(x,y,λ) = xy - xλ - 3yλ + 36λ
+#
+# ∇_x,y,λ L(x,y,λ) = 0
+#
+# ∂L/∂x = y - λ
+# ∂L/∂y = x - 3λ
+# ∂L/∂λ = -x - 3y + 36
+#
+#  0x + 1y - 1λ = 0
+#  1x + 0y - 3λ = 0
+# -1x - 3y + 0λ + 36 = 0
+#
+# [ 0  1 -1][x]   [  0]
+# [ 1  0 -3][y] = [  0]
+# [-1 -3  0][λ]   [-36]
+#
+# Solve with:
+# ```python
+#   np.linalg.solve(
+#     np.array([[0,1,-1],
+#               [1,0,-3],
+#               [-1,-3,0]]),
+#     np.array([[0], [0], [-36]]))
+# ```
+#
+# [x]   [18]
+# [y] = [ 6]
+# [λ]   [ 6]
+def test_equality_constrained_1():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    y = problem.decision_variable()
+
+    problem.maximize(x * y)
+
+    problem.subject_to(x + 3 * y == 36)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value() == pytest.approx(18.0, abs=1e-5)
+    assert y.value() == pytest.approx(6.0, abs=1e-5)
+
+
+def test_equality_constrained_2():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable(2)
+    x[0].set_value(1.0)
+    x[1].set_value(2.0)
+
+    problem.minimize(x.T @ x)
+
+    problem.subject_to(x == np.array([[3.0], [3.0]]))
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value(0) == pytest.approx(3.0, abs=1e-5)
+    assert x.value(1) == pytest.approx(3.0, abs=1e-5)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-"""This problem tests the case where regularization fails"""
-
-import math
-
-import jormungandr.autodiff as autodiff
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-import numpy as np
-
-
-def test_optimization_problem_arm_on_elevator():
-    N = 800
-
-    ELEVATOR_START_HEIGHT = 1.0  # m
-    ELEVATOR_END_HEIGHT = 1.25  # m
-    ELEVATOR_MAX_VELOCITY = 1  # m/s
-    ELEVATOR_MAX_ACCELERATION = 2.0  # m/s²
-
-    ARM_LENGTH = 1.0  # m
-    ARM_START_ANGLE = 0.0  # rad
-    ARM_END_ANGLE = math.pi  # rad
-    ARM_MAX_VELOCITY = 2.0 * math.pi  # rad/s
-    ARM_MAX_ACCELERATION = 4.0 * math.pi  # rad/s²
-
-    END_EFFECTOR_MAX_HEIGHT = 1.8  # m
-
-    TOTAL_TIME = 4.0  # s
-    dt = TOTAL_TIME / N
-
-    problem = OptimizationProblem()
-
-    elevator = problem.decision_variable(2, N + 1)
-    elevator_accel = problem.decision_variable(1, N)
-
-    arm = problem.decision_variable(2, N + 1)
-    arm_accel = problem.decision_variable(1, N)
-
-    for k in range(N):
-        # Elevator dynamics constraints
-        problem.subject_to(elevator[0, k + 1] == elevator[0, k] + elevator[1, k] * dt)
-        problem.subject_to(
-            elevator[1, k + 1] == elevator[1, k] + elevator_accel[0, k] * dt
-        )
-
-        # Arm dynamics constraints
-        problem.subject_to(arm[0, k + 1] == arm[0, k] + arm[1, k] * dt)
-        problem.subject_to(arm[1, k + 1] == arm[1, k] + arm_accel[0, k] * dt)
-
-    # Elevator start and end conditions
-    problem.subject_to(elevator[:, :1] == np.array([[ELEVATOR_START_HEIGHT], [0.0]]))
-    problem.subject_to(
-        elevator[:, N : N + 1] == np.array([[ELEVATOR_END_HEIGHT], [0.0]])
-    )
-
-    # Arm start and end conditions
-    problem.subject_to(arm[:, :1] == np.array([[ARM_START_ANGLE], [0.0]]))
-    problem.subject_to(arm[:, N : N + 1] == np.array([[ARM_END_ANGLE], [0.0]]))
-
-    # Elevator velocity limits
-    problem.subject_to(-ELEVATOR_MAX_VELOCITY <= elevator[1:2, :])
-    problem.subject_to(elevator[1:2, :] <= ELEVATOR_MAX_VELOCITY)
-
-    # Elevator acceleration limits
-    problem.subject_to(-ELEVATOR_MAX_ACCELERATION <= elevator_accel)
-    problem.subject_to(elevator_accel <= ELEVATOR_MAX_ACCELERATION)
-
-    # Arm velocity limits
-    problem.subject_to(-ARM_MAX_VELOCITY <= arm[1:2, :])
-    problem.subject_to(arm[1:2, :] <= ARM_MAX_VELOCITY)
-
-    # Arm acceleration limits
-    problem.subject_to(-ARM_MAX_ACCELERATION <= arm_accel)
-    problem.subject_to(arm_accel <= ARM_MAX_ACCELERATION)
-
-    # Height limit
-    problem.subject_to(
-        elevator[:1, :] + ARM_LENGTH * arm[:1, :].cwise_transform(autodiff.sin)
-        <= END_EFFECTOR_MAX_HEIGHT
-    )
-
-    # Cost function
-    J = 0.0
-    for k in range(N + 1):
-        J += (ELEVATOR_END_HEIGHT - elevator[0, k]) ** 2 + (
-            ARM_END_ANGLE - arm[0, k]
-        ) ** 2
-    problem.minimize(J)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.NONLINEAR
-    assert status.exit_condition == SolverExitCondition.SUCCESS
+"""This problem tests the case where regularization fails"""
+
+import math
+
+import jormungandr.autodiff as autodiff
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+import numpy as np
+
+
+def test_optimization_problem_arm_on_elevator():
+    N = 800
+
+    ELEVATOR_START_HEIGHT = 1.0  # m
+    ELEVATOR_END_HEIGHT = 1.25  # m
+    ELEVATOR_MAX_VELOCITY = 1  # m/s
+    ELEVATOR_MAX_ACCELERATION = 2.0  # m/s²
+
+    ARM_LENGTH = 1.0  # m
+    ARM_START_ANGLE = 0.0  # rad
+    ARM_END_ANGLE = math.pi  # rad
+    ARM_MAX_VELOCITY = 2.0 * math.pi  # rad/s
+    ARM_MAX_ACCELERATION = 4.0 * math.pi  # rad/s²
+
+    END_EFFECTOR_MAX_HEIGHT = 1.8  # m
+
+    TOTAL_TIME = 4.0  # s
+    dt = TOTAL_TIME / N
+
+    problem = OptimizationProblem()
+
+    elevator = problem.decision_variable(2, N + 1)
+    elevator_accel = problem.decision_variable(1, N)
+
+    arm = problem.decision_variable(2, N + 1)
+    arm_accel = problem.decision_variable(1, N)
+
+    for k in range(N):
+        # Elevator dynamics constraints
+        problem.subject_to(elevator[0, k + 1] == elevator[0, k] + elevator[1, k] * dt)
+        problem.subject_to(
+            elevator[1, k + 1] == elevator[1, k] + elevator_accel[0, k] * dt
+        )
+
+        # Arm dynamics constraints
+        problem.subject_to(arm[0, k + 1] == arm[0, k] + arm[1, k] * dt)
+        problem.subject_to(arm[1, k + 1] == arm[1, k] + arm_accel[0, k] * dt)
+
+    # Elevator start and end conditions
+    problem.subject_to(elevator[:, :1] == np.array([[ELEVATOR_START_HEIGHT], [0.0]]))
+    problem.subject_to(
+        elevator[:, N : N + 1] == np.array([[ELEVATOR_END_HEIGHT], [0.0]])
+    )
+
+    # Arm start and end conditions
+    problem.subject_to(arm[:, :1] == np.array([[ARM_START_ANGLE], [0.0]]))
+    problem.subject_to(arm[:, N : N + 1] == np.array([[ARM_END_ANGLE], [0.0]]))
+
+    # Elevator velocity limits
+    problem.subject_to(-ELEVATOR_MAX_VELOCITY <= elevator[1:2, :])
+    problem.subject_to(elevator[1:2, :] <= ELEVATOR_MAX_VELOCITY)
+
+    # Elevator acceleration limits
+    problem.subject_to(-ELEVATOR_MAX_ACCELERATION <= elevator_accel)
+    problem.subject_to(elevator_accel <= ELEVATOR_MAX_ACCELERATION)
+
+    # Arm velocity limits
+    problem.subject_to(-ARM_MAX_VELOCITY <= arm[1:2, :])
+    problem.subject_to(arm[1:2, :] <= ARM_MAX_VELOCITY)
+
+    # Arm acceleration limits
+    problem.subject_to(-ARM_MAX_ACCELERATION <= arm_accel)
+    problem.subject_to(arm_accel <= ARM_MAX_ACCELERATION)
+
+    # Height limit
+    problem.subject_to(
+        elevator[:1, :] + ARM_LENGTH * arm[:1, :].cwise_transform(autodiff.sin)
+        <= END_EFFECTOR_MAX_HEIGHT
+    )
+
+    # Cost function
+    J = 0.0
+    for k in range(N + 1):
+        J += (ELEVATOR_END_HEIGHT - elevator[0, k]) ** 2 + (
+            ARM_END_ANGLE - arm[0, k]
+        ) ** 2
+    problem.minimize(J)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.NONLINEAR
+    assert status.exit_condition == SolverExitCondition.SUCCESS
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_cart_pole_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_cart_pole_test.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-import math
-
-import jormungandr.autodiff as autodiff
-from jormungandr.autodiff import ExpressionType, VariableMatrix, Variable
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-import numpy as np
-import pytest
-
-
-def rk4(f, x, u, dt):
-    h = dt
-
-    k1 = f(x, u)
-    k2 = f(x + h * 0.5 * k1, u)
-    k3 = f(x + h * 0.5 * k2, u)
-    k4 = f(x + h * k3, u)
-
-    return x + h / 6.0 * (k1 + 2.0 * k2 + 2.0 * k3 + k4)
-
-
-# https://underactuated.mit.edu/acrobot.html#cart_pole
-#
-# θ is CCW+ measured from negative y-axis.
-#
-# q = [x, θ]ᵀ
-# q̇ = [ẋ, θ̇]ᵀ
-# u = f_x
-#
-# M(q)q̈ + C(q, q̇)q̇ = τ_g(q) + Bu
-# M(q)q̈ = τ_g(q) − C(q, q̇)q̇ + Bu
-# q̈ = M⁻¹(q)(τ_g(q) − C(q, q̇)q̇ + Bu)
-#
-#        [ m_c + m_p  m_p l cosθ]
-# M(q) = [m_p l cosθ    m_p l²  ]
-#
-#           [0  −m_p lθ̇ sinθ]
-# C(q, q̇) = [0       0      ]
-#
-#          [     0      ]
-# τ_g(q) = [-m_p gl sinθ]
-#
-#     [1]
-# B = [0]
-
-m_c = 5.0  # Cart mass (kg)
-m_p = 0.5  # Pole mass (kg)
-l = 0.5  # Pole length (m)
-g = 9.806  # Acceleration due to gravity (m/s²)
-
-
-def cart_pole_dynamics_double(x, u):
-    q = x[:2, :]
-    qdot = x[2:, :]
-    theta = q[1, 0]
-    thetadot = qdot[1, 0]
-
-    #        [ m_c + m_p  m_p l cosθ]
-    # M(q) = [m_p l cosθ    m_p l²  ]
-    M = np.array(
-        [
-            [m_c + m_p, m_p * l * math.cos(theta)],
-            [m_p * l * math.cos(theta), m_p * l**2],
-        ]
-    )
-
-    detM = M[0, 0] * M[1, 1] - M[0, 1] * M[1, 0]
-    Minv = np.array(
-        [[M[1, 1] / detM, -M[0, 1] / detM], [-M[1, 0] / detM, M[0, 0] / detM]]
-    )
-
-    #           [0  −m_p lθ̇ sinθ]
-    # C(q, q̇) = [0       0      ]
-    C = np.array([[0.0, -m_p * l * thetadot * math.sin(theta)], [0.0, 0.0]])
-
-    #          [     0      ]
-    # τ_g(q) = [-m_p gl sinθ]
-    tau_g = np.array([[0.0], [-m_p * g * l * math.sin(theta)]])
-
-    #     [1]
-    # B = [0]
-    B = np.array([[1], [0]])
-
-    # q̈ = M⁻¹(q)(τ_g(q) − C(q, q̇)q̇ + Bu)
-    qddot = np.empty((4, 1))
-    qddot[:2, :] = qdot
-    qddot[2:, :] = Minv @ (tau_g - C @ qdot + B @ u)
-    return qddot
-
-
-def cart_pole_dynamics(x, u):
-    q = x[:2, :]
-    qdot = x[2:, :]
-    theta = q[1, 0]
-    thetadot = qdot[1, 0]
-
-    #        [ m_c + m_p  m_p l cosθ]
-    # M(q) = [m_p l cosθ    m_p l²  ]
-    M = VariableMatrix(
-        [
-            [Variable(m_c + m_p), m_p * l * autodiff.cos(theta)],
-            [m_p * l * autodiff.cos(theta), Variable(m_p * l**2)],
-        ]
-    )
-
-    detM = M[0, 0] * M[1, 1] - M[0, 1] * M[1, 0]
-    Minv = VariableMatrix(
-        [[M[1, 1] / detM, -M[0, 1] / detM], [-M[1, 0] / detM, M[0, 0] / detM]]
-    )
-
-    #           [0  −m_p lθ̇ sinθ]
-    # C(q, q̇) = [0       0      ]
-    C = VariableMatrix(
-        [
-            [Variable(0.0), -m_p * l * thetadot * autodiff.sin(theta)],
-            [Variable(0.0), Variable(0.0)],
-        ]
-    )
-
-    #          [     0      ]
-    # τ_g(q) = [-m_p gl sinθ]
-    tau_g = VariableMatrix([[Variable(0.0)], [-m_p * g * l * autodiff.sin(theta)]])
-
-    #     [1]
-    # B = [0]
-    B = np.array([[1], [0]])
-
-    # q̈ = M⁻¹(q)(τ_g(q) − C(q, q̇)q̇ + Bu)
-    qddot = VariableMatrix(4, 1)
-    qddot[:2, :] = qdot
-    qddot[2:, :] = Minv @ (tau_g - C @ qdot + B @ u)
-    return qddot
-
-
-def lerp(a, b, t):
-    return a + t * (b - a)
-
-
-def test_optimization_problem_cart_pole():
-    T = 5.0  # s
-    dt = 0.05  # s
-    N = int(T / dt)
-
-    u_max = 20.0  # N
-    d_max = 2.0  # m
-
-    x_initial = np.zeros((4, 1))
-    x_final = np.array([[1.0], [math.pi], [0.0], [0.0]])
-
-    problem = OptimizationProblem()
-
-    # x = [q, q̇]ᵀ = [x, θ, ẋ, θ̇]ᵀ
-    X = problem.decision_variable(4, N + 1)
-
-    # Initial guess
-    for k in range(N + 1):
-        X[0, k].set_value(lerp(x_initial[0, 0], x_final[0, 0], k / N))
-        X[1, k].set_value(lerp(x_initial[1, 0], x_final[1, 0], k / N))
-
-    # u = f_x
-    U = problem.decision_variable(1, N)
-
-    # Initial conditions
-    problem.subject_to(X[:, :1] == x_initial)
-
-    # Final conditions
-    problem.subject_to(X[:, N : N + 1] == x_final)
-
-    # Cart position constraints
-    problem.subject_to(X[:1, :] >= 0.0)
-    problem.subject_to(X[:1, :] <= d_max)
-
-    # Input constraints
-    problem.subject_to(U >= -u_max)
-    problem.subject_to(U <= u_max)
-
-    # Dynamics constraints - RK4 integration
-    for k in range(N):
-        problem.subject_to(
-            X[:, k + 1 : k + 2]
-            == rk4(cart_pole_dynamics, X[:, k : k + 1], U[:, k : k + 1], dt)
-        )
-
-    # Minimize sum squared inputs
-    J = 0.0
-    for k in range(N):
-        J += U[:, k : k + 1].T @ U[:, k : k + 1]
-    problem.minimize(J)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONLINEAR
-    assert status.inequality_constraint_type == ExpressionType.LINEAR
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    # Verify initial state
-    assert X.value(0, 0) == pytest.approx(x_initial[0, 0], abs=1e-8)
-    assert X.value(1, 0) == pytest.approx(x_initial[1, 0], abs=1e-8)
-    assert X.value(2, 0) == pytest.approx(x_initial[2, 0], abs=1e-8)
-    assert X.value(3, 0) == pytest.approx(x_initial[3, 0], abs=1e-8)
-
-    # Verify solution
-    for k in range(N):
-        # Cart position constraints
-        assert X[0, k] >= 0.0
-        assert X[0, k] <= d_max
-
-        # Input constraints
-        assert U[0, k] >= -u_max
-        assert U[0, k] <= u_max
-
-        # Dynamics constraints
-        expected_x_k1 = rk4(
-            cart_pole_dynamics_double,
-            X[:, k : k + 1].value(),
-            U[:, k : k + 1].value(),
-            dt,
-        )
-        actual_x_k1 = X[:, k + 1 : k + 2].value()
-        for row in range(actual_x_k1.shape[0]):
-            assert actual_x_k1[row, 0] == pytest.approx(expected_x_k1[row, 0], abs=1e-8)
-
-    # Verify final state
-    assert X.value(0, N) == pytest.approx(x_final[0, 0], abs=1e-8)
-    assert X.value(1, N) == pytest.approx(x_final[1, 0], abs=1e-8)
-    assert X.value(2, N) == pytest.approx(x_final[2, 0], abs=1e-8)
-    assert X.value(3, N) == pytest.approx(x_final[3, 0], abs=1e-8)
-
-    # Log states for offline viewing
-    with open("Cart-pole states.csv", "w") as f:
-        f.write(
-            "Time (s),Cart position (m),Pole angle (rad),Cart velocity (m/s),Pole angular velocity (rad/s)\n"
-        )
-
-        for k in range(N + 1):
-            f.write(
-                f"{k * dt},{X.value(0, k)},{X.value(1, k)},{X.value(2, k)},{X.value(3, k)}\n"
-            )
-
-    # Log inputs for offline viewing
-    with open("Cart-pole inputs.csv", "w") as f:
-        f.write("Time (s),Cart force (N)\n")
-
-        for k in range(N + 1):
-            if k < N:
-                f.write(f"{k * dt},{U.value(0, k)}\n")
-            else:
-                f.write(f"{k * dt},0.0\n")
+import math
+
+import jormungandr.autodiff as autodiff
+from jormungandr.autodiff import ExpressionType, VariableMatrix, Variable
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+import numpy as np
+import pytest
+
+
+def rk4(f, x, u, dt):
+    h = dt
+
+    k1 = f(x, u)
+    k2 = f(x + h * 0.5 * k1, u)
+    k3 = f(x + h * 0.5 * k2, u)
+    k4 = f(x + h * k3, u)
+
+    return x + h / 6.0 * (k1 + 2.0 * k2 + 2.0 * k3 + k4)
+
+
+# https://underactuated.mit.edu/acrobot.html#cart_pole
+#
+# θ is CCW+ measured from negative y-axis.
+#
+# q = [x, θ]ᵀ
+# q̇ = [ẋ, θ̇]ᵀ
+# u = f_x
+#
+# M(q)q̈ + C(q, q̇)q̇ = τ_g(q) + Bu
+# M(q)q̈ = τ_g(q) − C(q, q̇)q̇ + Bu
+# q̈ = M⁻¹(q)(τ_g(q) − C(q, q̇)q̇ + Bu)
+#
+#        [ m_c + m_p  m_p l cosθ]
+# M(q) = [m_p l cosθ    m_p l²  ]
+#
+#           [0  −m_p lθ̇ sinθ]
+# C(q, q̇) = [0       0      ]
+#
+#          [     0      ]
+# τ_g(q) = [-m_p gl sinθ]
+#
+#     [1]
+# B = [0]
+
+m_c = 5.0  # Cart mass (kg)
+m_p = 0.5  # Pole mass (kg)
+l = 0.5  # Pole length (m)
+g = 9.806  # Acceleration due to gravity (m/s²)
+
+
+def cart_pole_dynamics_double(x, u):
+    q = x[:2, :]
+    qdot = x[2:, :]
+    theta = q[1, 0]
+    thetadot = qdot[1, 0]
+
+    #        [ m_c + m_p  m_p l cosθ]
+    # M(q) = [m_p l cosθ    m_p l²  ]
+    M = np.array(
+        [
+            [m_c + m_p, m_p * l * math.cos(theta)],
+            [m_p * l * math.cos(theta), m_p * l**2],
+        ]
+    )
+
+    detM = M[0, 0] * M[1, 1] - M[0, 1] * M[1, 0]
+    Minv = np.array(
+        [[M[1, 1] / detM, -M[0, 1] / detM], [-M[1, 0] / detM, M[0, 0] / detM]]
+    )
+
+    #           [0  −m_p lθ̇ sinθ]
+    # C(q, q̇) = [0       0      ]
+    C = np.array([[0.0, -m_p * l * thetadot * math.sin(theta)], [0.0, 0.0]])
+
+    #          [     0      ]
+    # τ_g(q) = [-m_p gl sinθ]
+    tau_g = np.array([[0.0], [-m_p * g * l * math.sin(theta)]])
+
+    #     [1]
+    # B = [0]
+    B = np.array([[1], [0]])
+
+    # q̈ = M⁻¹(q)(τ_g(q) − C(q, q̇)q̇ + Bu)
+    qddot = np.empty((4, 1))
+    qddot[:2, :] = qdot
+    qddot[2:, :] = Minv @ (tau_g - C @ qdot + B @ u)
+    return qddot
+
+
+def cart_pole_dynamics(x, u):
+    q = x[:2, :]
+    qdot = x[2:, :]
+    theta = q[1, 0]
+    thetadot = qdot[1, 0]
+
+    #        [ m_c + m_p  m_p l cosθ]
+    # M(q) = [m_p l cosθ    m_p l²  ]
+    M = VariableMatrix(
+        [
+            [Variable(m_c + m_p), m_p * l * autodiff.cos(theta)],
+            [m_p * l * autodiff.cos(theta), Variable(m_p * l**2)],
+        ]
+    )
+
+    detM = M[0, 0] * M[1, 1] - M[0, 1] * M[1, 0]
+    Minv = VariableMatrix(
+        [[M[1, 1] / detM, -M[0, 1] / detM], [-M[1, 0] / detM, M[0, 0] / detM]]
+    )
+
+    #           [0  −m_p lθ̇ sinθ]
+    # C(q, q̇) = [0       0      ]
+    C = VariableMatrix(
+        [
+            [Variable(0.0), -m_p * l * thetadot * autodiff.sin(theta)],
+            [Variable(0.0), Variable(0.0)],
+        ]
+    )
+
+    #          [     0      ]
+    # τ_g(q) = [-m_p gl sinθ]
+    tau_g = VariableMatrix([[Variable(0.0)], [-m_p * g * l * autodiff.sin(theta)]])
+
+    #     [1]
+    # B = [0]
+    B = np.array([[1], [0]])
+
+    # q̈ = M⁻¹(q)(τ_g(q) − C(q, q̇)q̇ + Bu)
+    qddot = VariableMatrix(4, 1)
+    qddot[:2, :] = qdot
+    qddot[2:, :] = Minv @ (tau_g - C @ qdot + B @ u)
+    return qddot
+
+
+def lerp(a, b, t):
+    return a + t * (b - a)
+
+
+def test_optimization_problem_cart_pole():
+    T = 5.0  # s
+    dt = 0.05  # s
+    N = int(T / dt)
+
+    u_max = 20.0  # N
+    d_max = 2.0  # m
+
+    x_initial = np.zeros((4, 1))
+    x_final = np.array([[1.0], [math.pi], [0.0], [0.0]])
+
+    problem = OptimizationProblem()
+
+    # x = [q, q̇]ᵀ = [x, θ, ẋ, θ̇]ᵀ
+    X = problem.decision_variable(4, N + 1)
+
+    # Initial guess
+    for k in range(N + 1):
+        X[0, k].set_value(lerp(x_initial[0, 0], x_final[0, 0], k / N))
+        X[1, k].set_value(lerp(x_initial[1, 0], x_final[1, 0], k / N))
+
+    # u = f_x
+    U = problem.decision_variable(1, N)
+
+    # Initial conditions
+    problem.subject_to(X[:, :1] == x_initial)
+
+    # Final conditions
+    problem.subject_to(X[:, N : N + 1] == x_final)
+
+    # Cart position constraints
+    problem.subject_to(X[:1, :] >= 0.0)
+    problem.subject_to(X[:1, :] <= d_max)
+
+    # Input constraints
+    problem.subject_to(U >= -u_max)
+    problem.subject_to(U <= u_max)
+
+    # Dynamics constraints - RK4 integration
+    for k in range(N):
+        problem.subject_to(
+            X[:, k + 1 : k + 2]
+            == rk4(cart_pole_dynamics, X[:, k : k + 1], U[:, k : k + 1], dt)
+        )
+
+    # Minimize sum squared inputs
+    J = 0.0
+    for k in range(N):
+        J += U[:, k : k + 1].T @ U[:, k : k + 1]
+    problem.minimize(J)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONLINEAR
+    assert status.inequality_constraint_type == ExpressionType.LINEAR
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    # Verify initial state
+    assert X.value(0, 0) == pytest.approx(x_initial[0, 0], abs=1e-8)
+    assert X.value(1, 0) == pytest.approx(x_initial[1, 0], abs=1e-8)
+    assert X.value(2, 0) == pytest.approx(x_initial[2, 0], abs=1e-8)
+    assert X.value(3, 0) == pytest.approx(x_initial[3, 0], abs=1e-8)
+
+    # Verify solution
+    for k in range(N):
+        # Cart position constraints
+        assert X[0, k] >= 0.0
+        assert X[0, k] <= d_max
+
+        # Input constraints
+        assert U[0, k] >= -u_max
+        assert U[0, k] <= u_max
+
+        # Dynamics constraints
+        expected_x_k1 = rk4(
+            cart_pole_dynamics_double,
+            X[:, k : k + 1].value(),
+            U[:, k : k + 1].value(),
+            dt,
+        )
+        actual_x_k1 = X[:, k + 1 : k + 2].value()
+        for row in range(actual_x_k1.shape[0]):
+            assert actual_x_k1[row, 0] == pytest.approx(expected_x_k1[row, 0], abs=1e-8)
+
+    # Verify final state
+    assert X.value(0, N) == pytest.approx(x_final[0, 0], abs=1e-8)
+    assert X.value(1, N) == pytest.approx(x_final[1, 0], abs=1e-8)
+    assert X.value(2, N) == pytest.approx(x_final[2, 0], abs=1e-8)
+    assert X.value(3, N) == pytest.approx(x_final[3, 0], abs=1e-8)
+
+    # Log states for offline viewing
+    with open("Cart-pole states.csv", "w") as f:
+        f.write(
+            "Time (s),Cart position (m),Pole angle (rad),Cart velocity (m/s),Pole angular velocity (rad/s)\n"
+        )
+
+        for k in range(N + 1):
+            f.write(
+                f"{k * dt},{X.value(0, k)},{X.value(1, k)},{X.value(2, k)},{X.value(3, k)}\n"
+            )
+
+    # Log inputs for offline viewing
+    with open("Cart-pole inputs.csv", "w") as f:
+        f.write("Time (s),Cart force (N)\n")
+
+        for k in range(N + 1):
+            if k < N:
+                f.write(f"{k * dt},{U.value(0, k)}\n")
+            else:
+                f.write(f"{k * dt},0.0\n")
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_differential_drive_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_differential_drive_test.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-import math
-
-import jormungandr.autodiff as autodiff
-from jormungandr.autodiff import ExpressionType, VariableMatrix
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-import numpy as np
-import pytest
-
-
-def rk4(f, x, u, dt):
-    h = dt
-
-    k1 = f(x, u)
-    k2 = f(x + h * 0.5 * k1, u)
-    k3 = f(x + h * 0.5 * k2, u)
-    k4 = f(x + h * k3, u)
-
-    return x + h / 6.0 * (k1 + 2.0 * k2 + 2.0 * k3 + k4)
-
-
-# x = [x, y, heading, left velocity, right velocity]ᵀ
-# u = [left voltage, right voltage]ᵀ
-trackwidth = 0.699  # m
-Kv_linear = 3.02  # V/(m/s)
-Ka_linear = 0.642  # V/(m/s²)
-Kv_angular = 1.382  # V/(m/s)
-Ka_angular = 0.08495  # V/(m/s²)
-
-A1 = -(Kv_linear / Ka_linear + Kv_angular / Ka_angular) / 2.0
-A2 = -(Kv_linear / Ka_linear - Kv_angular / Ka_angular) / 2.0
-B1 = 0.5 / Ka_linear + 0.5 / Ka_angular
-B2 = 0.5 / Ka_linear - 0.5 / Ka_angular
-A = np.array([[A1, A2], [A2, A1]])
-B = np.array([[B1, B2], [B2, B1]])
-
-
-def differential_drive_dynamics_double(x, u):
-    xdot = np.empty((5, 1))
-
-    v = (x[3, 0] + x[4, 0]) / 2.0
-    xdot[0, :] = v * math.cos(x[2, 0])
-    xdot[1, :] = v * math.sin(x[2, 0])
-    xdot[2, :] = (x[4, 0] - x[3, 0]) / trackwidth
-    xdot[3:5, :] = A @ x[3:5, :] + B @ u
-
-    return xdot
-
-
-def differential_drive_dynamics(x, u):
-    xdot = VariableMatrix(5, 1)
-
-    v = (x[3, 0] + x[4, 0]) / 2.0
-    xdot[0, :] = v * autodiff.cos(x[2, 0])
-    xdot[1, :] = v * autodiff.sin(x[2, 0])
-    xdot[2, :] = (x[4, 0] - x[3, 0]) / trackwidth
-    xdot[3:5, :] = A @ x[3:5, :] + B @ u
-
-    return xdot
-
-
-def lerp(a, b, t):
-    return a + t * (b - a)
-
-
-def test_optimization_problem_differential_drive():
-    T = 5.0  # s
-    dt = 0.05  # s
-    N = int(T / dt)
-
-    u_max = 12.0  # V
-
-    x_initial = np.zeros((5, 1))
-    x_final = np.array([[1.0], [1.0], [0.0], [0.0], [0.0]])
-
-    problem = OptimizationProblem()
-
-    # x = [x, y, heading, left velocity, right velocity]ᵀ
-    X = problem.decision_variable(5, N + 1)
-
-    # Initial guess
-    for k in range(N + 1):
-        X[0, k].set_value(lerp(x_initial[0, 0], x_final[0, 0], k / N))
-        X[1, k].set_value(lerp(x_initial[1, 0], x_final[1, 0], k / N))
-
-    # u = [left voltage, right voltage]ᵀ
-    U = problem.decision_variable(2, N)
-
-    # Initial conditions
-    problem.subject_to(X[:, :1] == x_initial)
-
-    # Final conditions
-    problem.subject_to(X[:, N : N + 1] == x_final)
-
-    # Input constraints
-    problem.subject_to(U >= -u_max)
-    problem.subject_to(U <= u_max)
-
-    # Dynamics constraints - RK4 integration
-    for k in range(N):
-        problem.subject_to(
-            X[:, k + 1 : k + 2]
-            == rk4(differential_drive_dynamics, X[:, k : k + 1], U[:, k : k + 1], dt)
-        )
-
-    # Minimize sum squared states and inputs
-    J = 0.0
-    for k in range(N):
-        J += X[:, k : k + 1].T @ X[:, k : k + 1] + U[:, k : k + 1].T @ U[:, k : k + 1]
-    problem.minimize(J)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONLINEAR
-    assert status.inequality_constraint_type == ExpressionType.LINEAR
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    # Verify initial state
-    assert X.value(0, 0) == pytest.approx(x_initial[0, 0], abs=1e-8)
-    assert X.value(1, 0) == pytest.approx(x_initial[1, 0], abs=1e-8)
-    assert X.value(2, 0) == pytest.approx(x_initial[2, 0], abs=1e-8)
-    assert X.value(3, 0) == pytest.approx(x_initial[3, 0], abs=1e-8)
-    assert X.value(4, 0) == pytest.approx(x_initial[4, 0], abs=1e-8)
-
-    # Verify solution
-    x = np.zeros((5, 1))
-    for k in range(N):
-        u = U[:, k : k + 1].value()
-
-        # Input constraints
-        assert U[0, k].value() >= -u_max
-        assert U[0, k].value() <= u_max
-        assert U[1, k].value() >= -u_max
-        assert U[1, k].value() <= u_max
-
-        # Verify state
-        assert X.value(0, k) == pytest.approx(x[0, 0], abs=1e-8)
-        assert X.value(1, k) == pytest.approx(x[1, 0], abs=1e-8)
-        assert X.value(2, k) == pytest.approx(x[2, 0], abs=1e-8)
-        assert X.value(3, k) == pytest.approx(x[3, 0], abs=1e-8)
-        assert X.value(4, k) == pytest.approx(x[4, 0], abs=1e-8)
-
-        # Project state forward
-        x = rk4(differential_drive_dynamics_double, x, u, dt)
-
-    # Verify final state
-    assert X.value(0, N) == pytest.approx(x_final[0, 0], abs=1e-8)
-    assert X.value(1, N) == pytest.approx(x_final[1, 0], abs=1e-8)
-    assert X.value(2, N) == pytest.approx(x_final[2, 0], abs=1e-8)
-    assert X.value(3, N) == pytest.approx(x_final[3, 0], abs=1e-8)
-    assert X.value(4, N) == pytest.approx(x_final[4, 0], abs=1e-8)
-
-    # Log states for offline viewing
-    with open("Differential drive states.csv", "w") as f:
-        f.write(
-            "Time (s),X position (m),Y position (m),Heading (rad),Left velocity (m/s),Right velocity (m/s)\n"
-        )
-
-        for k in range(N + 1):
-            f.write(
-                f"{k * dt},{X.value(0, k)},{X.value(1, k)},{X.value(2, k)},{X.value(3, k)},{X.value(4, k)}\n"
-            )
-
-    # Log inputs for offline viewing
-    with open("Differential drive inputs.csv", "w") as f:
-        f.write("Time (s),Left voltage (V),Right voltage (V)\n")
-
-        for k in range(N + 1):
-            if k < N:
-                f.write(f"{k * dt},{U.value(0, k)},{U.value(1, k)}\n")
-            else:
-                f.write(f"{k * dt},0.0,0.0\n")
+import math
+
+import jormungandr.autodiff as autodiff
+from jormungandr.autodiff import ExpressionType, VariableMatrix
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+import numpy as np
+import pytest
+
+
+def rk4(f, x, u, dt):
+    h = dt
+
+    k1 = f(x, u)
+    k2 = f(x + h * 0.5 * k1, u)
+    k3 = f(x + h * 0.5 * k2, u)
+    k4 = f(x + h * k3, u)
+
+    return x + h / 6.0 * (k1 + 2.0 * k2 + 2.0 * k3 + k4)
+
+
+# x = [x, y, heading, left velocity, right velocity]ᵀ
+# u = [left voltage, right voltage]ᵀ
+trackwidth = 0.699  # m
+Kv_linear = 3.02  # V/(m/s)
+Ka_linear = 0.642  # V/(m/s²)
+Kv_angular = 1.382  # V/(m/s)
+Ka_angular = 0.08495  # V/(m/s²)
+
+A1 = -(Kv_linear / Ka_linear + Kv_angular / Ka_angular) / 2.0
+A2 = -(Kv_linear / Ka_linear - Kv_angular / Ka_angular) / 2.0
+B1 = 0.5 / Ka_linear + 0.5 / Ka_angular
+B2 = 0.5 / Ka_linear - 0.5 / Ka_angular
+A = np.array([[A1, A2], [A2, A1]])
+B = np.array([[B1, B2], [B2, B1]])
+
+
+def differential_drive_dynamics_double(x, u):
+    xdot = np.empty((5, 1))
+
+    v = (x[3, 0] + x[4, 0]) / 2.0
+    xdot[0, :] = v * math.cos(x[2, 0])
+    xdot[1, :] = v * math.sin(x[2, 0])
+    xdot[2, :] = (x[4, 0] - x[3, 0]) / trackwidth
+    xdot[3:5, :] = A @ x[3:5, :] + B @ u
+
+    return xdot
+
+
+def differential_drive_dynamics(x, u):
+    xdot = VariableMatrix(5, 1)
+
+    v = (x[3, 0] + x[4, 0]) / 2.0
+    xdot[0, :] = v * autodiff.cos(x[2, 0])
+    xdot[1, :] = v * autodiff.sin(x[2, 0])
+    xdot[2, :] = (x[4, 0] - x[3, 0]) / trackwidth
+    xdot[3:5, :] = A @ x[3:5, :] + B @ u
+
+    return xdot
+
+
+def lerp(a, b, t):
+    return a + t * (b - a)
+
+
+def test_optimization_problem_differential_drive():
+    T = 5.0  # s
+    dt = 0.05  # s
+    N = int(T / dt)
+
+    u_max = 12.0  # V
+
+    x_initial = np.zeros((5, 1))
+    x_final = np.array([[1.0], [1.0], [0.0], [0.0], [0.0]])
+
+    problem = OptimizationProblem()
+
+    # x = [x, y, heading, left velocity, right velocity]ᵀ
+    X = problem.decision_variable(5, N + 1)
+
+    # Initial guess
+    for k in range(N + 1):
+        X[0, k].set_value(lerp(x_initial[0, 0], x_final[0, 0], k / N))
+        X[1, k].set_value(lerp(x_initial[1, 0], x_final[1, 0], k / N))
+
+    # u = [left voltage, right voltage]ᵀ
+    U = problem.decision_variable(2, N)
+
+    # Initial conditions
+    problem.subject_to(X[:, :1] == x_initial)
+
+    # Final conditions
+    problem.subject_to(X[:, N : N + 1] == x_final)
+
+    # Input constraints
+    problem.subject_to(U >= -u_max)
+    problem.subject_to(U <= u_max)
+
+    # Dynamics constraints - RK4 integration
+    for k in range(N):
+        problem.subject_to(
+            X[:, k + 1 : k + 2]
+            == rk4(differential_drive_dynamics, X[:, k : k + 1], U[:, k : k + 1], dt)
+        )
+
+    # Minimize sum squared states and inputs
+    J = 0.0
+    for k in range(N):
+        J += X[:, k : k + 1].T @ X[:, k : k + 1] + U[:, k : k + 1].T @ U[:, k : k + 1]
+    problem.minimize(J)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONLINEAR
+    assert status.inequality_constraint_type == ExpressionType.LINEAR
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    # Verify initial state
+    assert X.value(0, 0) == pytest.approx(x_initial[0, 0], abs=1e-8)
+    assert X.value(1, 0) == pytest.approx(x_initial[1, 0], abs=1e-8)
+    assert X.value(2, 0) == pytest.approx(x_initial[2, 0], abs=1e-8)
+    assert X.value(3, 0) == pytest.approx(x_initial[3, 0], abs=1e-8)
+    assert X.value(4, 0) == pytest.approx(x_initial[4, 0], abs=1e-8)
+
+    # Verify solution
+    x = np.zeros((5, 1))
+    for k in range(N):
+        u = U[:, k : k + 1].value()
+
+        # Input constraints
+        assert U[0, k].value() >= -u_max
+        assert U[0, k].value() <= u_max
+        assert U[1, k].value() >= -u_max
+        assert U[1, k].value() <= u_max
+
+        # Verify state
+        assert X.value(0, k) == pytest.approx(x[0, 0], abs=1e-8)
+        assert X.value(1, k) == pytest.approx(x[1, 0], abs=1e-8)
+        assert X.value(2, k) == pytest.approx(x[2, 0], abs=1e-8)
+        assert X.value(3, k) == pytest.approx(x[3, 0], abs=1e-8)
+        assert X.value(4, k) == pytest.approx(x[4, 0], abs=1e-8)
+
+        # Project state forward
+        x = rk4(differential_drive_dynamics_double, x, u, dt)
+
+    # Verify final state
+    assert X.value(0, N) == pytest.approx(x_final[0, 0], abs=1e-8)
+    assert X.value(1, N) == pytest.approx(x_final[1, 0], abs=1e-8)
+    assert X.value(2, N) == pytest.approx(x_final[2, 0], abs=1e-8)
+    assert X.value(3, N) == pytest.approx(x_final[3, 0], abs=1e-8)
+    assert X.value(4, N) == pytest.approx(x_final[4, 0], abs=1e-8)
+
+    # Log states for offline viewing
+    with open("Differential drive states.csv", "w") as f:
+        f.write(
+            "Time (s),X position (m),Y position (m),Heading (rad),Left velocity (m/s),Right velocity (m/s)\n"
+        )
+
+        for k in range(N + 1):
+            f.write(
+                f"{k * dt},{X.value(0, k)},{X.value(1, k)},{X.value(2, k)},{X.value(3, k)},{X.value(4, k)}\n"
+            )
+
+    # Log inputs for offline viewing
+    with open("Differential drive inputs.csv", "w") as f:
+        f.write("Time (s),Left voltage (V),Right voltage (V)\n")
+
+        for k in range(N + 1):
+            if k < N:
+                f.write(f"{k * dt},{U.value(0, k)},{U.value(1, k)}\n")
+            else:
+                f.write(f"{k * dt},0.0,0.0\n")
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_double_integrator_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_double_integrator_test.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-import numpy as np
-import pytest
-
-
-def test_optimization_problem_double_integrator():
-    T = 3.5
-    dt = 0.005
-    N = int(T / dt)
-
-    r = 2.0
-
-    problem = OptimizationProblem()
-
-    # 2x1 state vector with N + 1 timesteps (includes last state)
-    X = problem.decision_variable(2, N + 1)
-
-    # 1x1 input vector with N timesteps (input at last state doesn't matter)
-    U = problem.decision_variable(1, N)
-
-    # Kinematics constraint assuming constant acceleration between timesteps
-    for k in range(N):
-        t = dt
-        p_k1 = X[0, k + 1]
-        v_k1 = X[1, k + 1]
-        p_k = X[0, k]
-        v_k = X[1, k]
-        a_k = U[0, k]
-
-        # pₖ₊₁ = pₖ + vₖt
-        problem.subject_to(p_k1 == p_k + v_k * t)
-
-        # vₖ₊₁ = vₖ + aₖt
-        problem.subject_to(v_k1 == v_k + a_k * t)
-
-    # Start and end at rest
-    problem.subject_to(X[:, :1] == np.array([[0.0], [0.0]]))
-    problem.subject_to(X[:, N : N + 1] == np.array([[r], [0.0]]))
-
-    # Limit velocity
-    problem.subject_to(-1 <= X[1:2, :])
-    problem.subject_to(X[1:2, :] <= 1)
-
-    # Limit acceleration
-    problem.subject_to(-1 <= U)
-    problem.subject_to(U <= 1)
-
-    # Cost function - minimize position error
-    J = 0.0
-    for k in range(N + 1):
-        J += (r - X[0, k]) ** 2
-    problem.minimize(J)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.LINEAR
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    A = np.array([[1.0, dt], [0.0, 1.0]])
-    B = np.array([[0.5 * dt * dt], [dt]])
-
-    # Verify initial state
-    assert X.value(0, 0) == pytest.approx(0.0, abs=1e-8)
-    assert X.value(1, 0) == pytest.approx(0.0, abs=1e-8)
-
-    # Verify solution
-    x = np.zeros((2, 1))
-    u = np.zeros((1, 1))
-    for k in range(N):
-        # Verify state
-        assert X.value(0, k) == pytest.approx(x[0, 0], abs=1e-2)
-        assert X.value(1, k) == pytest.approx(x[1, 0], abs=1e-2)
-
-        # Determine expected input for this timestep
-        if k * dt < 1.0:
-            # Accelerate
-            u[0, 0] = 1.0
-        elif k * dt < 2.05:
-            # Maintain speed
-            u[0, 0] = 0.0
-        elif k * dt < 3.275:
-            # Decelerate
-            u[0, 0] = -1.0
-        else:
-            # Accelerate
-            u[0, 0] = 1.0
-
-        # Verify input
-        if (
-            k > 0
-            and k < N - 1
-            and abs(U.value(0, k - 1) - U.value(0, k + 1)) >= 1.0 - 1e-2
-        ):
-            # If control input is transitioning between -1, 0, or 1, ensure it's
-            # within (-1, 1)
-            assert U.value(0, k) >= -1.0
-            assert U.value(0, k) <= 1.0
-        else:
-            assert U.value(0, k) == pytest.approx(u[0, 0], abs=1e-4)
-
-        # Project state forward
-        x = A @ x + B @ u
-
-    # Verify final state
-    assert X.value(0, N) == pytest.approx(r, abs=1e-8)
-    assert X.value(1, N) == pytest.approx(0.0, abs=1e-8)
-
-    # Log states for offline viewing
-    with open("Double integrator states.csv", "w") as f:
-        f.write("Time (s),Position (m),Velocity (rad/s)\n")
-
-        for k in range(N + 1):
-            f.write(f"{k * dt},{X.value(0, k)},{X.value(1, k)}\n")
-
-    # Log inputs for offline viewing
-    with open("Double integrator inputs.csv", "w") as f:
-        f.write("Time (s),Acceleration (m/s²)\n")
-
-        for k in range(N + 1):
-            if k < N:
-                f.write(f"{k * dt},{U.value(0, k)}\n")
-            else:
-                f.write(f"{k * dt},0.0\n")
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+import numpy as np
+import pytest
+
+
+def test_optimization_problem_double_integrator():
+    T = 3.5
+    dt = 0.005
+    N = int(T / dt)
+
+    r = 2.0
+
+    problem = OptimizationProblem()
+
+    # 2x1 state vector with N + 1 timesteps (includes last state)
+    X = problem.decision_variable(2, N + 1)
+
+    # 1x1 input vector with N timesteps (input at last state doesn't matter)
+    U = problem.decision_variable(1, N)
+
+    # Kinematics constraint assuming constant acceleration between timesteps
+    for k in range(N):
+        t = dt
+        p_k1 = X[0, k + 1]
+        v_k1 = X[1, k + 1]
+        p_k = X[0, k]
+        v_k = X[1, k]
+        a_k = U[0, k]
+
+        # pₖ₊₁ = pₖ + vₖt
+        problem.subject_to(p_k1 == p_k + v_k * t)
+
+        # vₖ₊₁ = vₖ + aₖt
+        problem.subject_to(v_k1 == v_k + a_k * t)
+
+    # Start and end at rest
+    problem.subject_to(X[:, :1] == np.array([[0.0], [0.0]]))
+    problem.subject_to(X[:, N : N + 1] == np.array([[r], [0.0]]))
+
+    # Limit velocity
+    problem.subject_to(-1 <= X[1:2, :])
+    problem.subject_to(X[1:2, :] <= 1)
+
+    # Limit acceleration
+    problem.subject_to(-1 <= U)
+    problem.subject_to(U <= 1)
+
+    # Cost function - minimize position error
+    J = 0.0
+    for k in range(N + 1):
+        J += (r - X[0, k]) ** 2
+    problem.minimize(J)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.LINEAR
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    A = np.array([[1.0, dt], [0.0, 1.0]])
+    B = np.array([[0.5 * dt * dt], [dt]])
+
+    # Verify initial state
+    assert X.value(0, 0) == pytest.approx(0.0, abs=1e-8)
+    assert X.value(1, 0) == pytest.approx(0.0, abs=1e-8)
+
+    # Verify solution
+    x = np.zeros((2, 1))
+    u = np.zeros((1, 1))
+    for k in range(N):
+        # Verify state
+        assert X.value(0, k) == pytest.approx(x[0, 0], abs=1e-2)
+        assert X.value(1, k) == pytest.approx(x[1, 0], abs=1e-2)
+
+        # Determine expected input for this timestep
+        if k * dt < 1.0:
+            # Accelerate
+            u[0, 0] = 1.0
+        elif k * dt < 2.05:
+            # Maintain speed
+            u[0, 0] = 0.0
+        elif k * dt < 3.275:
+            # Decelerate
+            u[0, 0] = -1.0
+        else:
+            # Accelerate
+            u[0, 0] = 1.0
+
+        # Verify input
+        if (
+            k > 0
+            and k < N - 1
+            and abs(U.value(0, k - 1) - U.value(0, k + 1)) >= 1.0 - 1e-2
+        ):
+            # If control input is transitioning between -1, 0, or 1, ensure it's
+            # within (-1, 1)
+            assert U.value(0, k) >= -1.0
+            assert U.value(0, k) <= 1.0
+        else:
+            assert U.value(0, k) == pytest.approx(u[0, 0], abs=1e-4)
+
+        # Project state forward
+        x = A @ x + B @ u
+
+    # Verify final state
+    assert X.value(0, N) == pytest.approx(r, abs=1e-8)
+    assert X.value(1, N) == pytest.approx(0.0, abs=1e-8)
+
+    # Log states for offline viewing
+    with open("Double integrator states.csv", "w") as f:
+        f.write("Time (s),Position (m),Velocity (rad/s)\n")
+
+        for k in range(N + 1):
+            f.write(f"{k * dt},{X.value(0, k)},{X.value(1, k)}\n")
+
+    # Log inputs for offline viewing
+    with open("Double integrator inputs.csv", "w") as f:
+        f.write("Time (s),Acceleration (m/s²)\n")
+
+        for k in range(N + 1):
+            if k < N:
+                f.write(f"{k * dt},{U.value(0, k)}\n")
+            else:
+                f.write(f"{k * dt},0.0\n")
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/optimization_problem_flywheel_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/optimization_problem_flywheel_test.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import math
-
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-import numpy as np
-import pytest
-
-
-def near(expected, actual, tolerance):
-    return abs(expected - actual) < tolerance
-
-
-def test_optimization_problem_flywheel():
-    T = 5.0
-    dt = 0.005
-    N = int(T / dt)
-
-    # Flywheel model:
-    # States: [velocity]
-    # Inputs: [voltage]
-    A = math.exp(-dt)
-    B = 1.0 - math.exp(-dt)
-
-    problem = OptimizationProblem()
-    X = problem.decision_variable(1, N + 1)
-    U = problem.decision_variable(1, N)
-
-    # Dynamics constraint
-    for k in range(N):
-        problem.subject_to(
-            X[:, k + 1 : k + 2] == A * X[:, k : k + 1] + B * U[:, k : k + 1]
-        )
-
-    # State and input constraints
-    problem.subject_to(X[0, 0] == 0.0)
-    problem.subject_to(-12 <= U)
-    problem.subject_to(U <= 12)
-
-    # Cost function - minimize error
-    r = np.array([[10.0]])
-    J = 0.0
-    for k in range(N + 1):
-        J += (r - X[:, k : k + 1]).T @ (r - X[:, k : k + 1])
-    problem.minimize(J)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.LINEAR
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    # Voltage for steady-state velocity:
-    #
-    # rₖ₊₁ = Arₖ + Buₖ
-    # uₖ = B⁺(rₖ₊₁ − Arₖ)
-    # uₖ = B⁺(rₖ − Arₖ)
-    # uₖ = B⁺(I − A)rₖ
-    u_ss = 1.0 / B * (1.0 - A) * r[0, 0]
-
-    # Verify initial state
-    assert X.value(0, 0) == pytest.approx(0.0, abs=1e-8)
-
-    # Verify solution
-    x = 0.0
-    u = 0.0
-    for k in range(N):
-        # Verify state
-        assert X.value(0, k) == pytest.approx(x, abs=1e-2)
-
-        # Determine expected input for this timestep
-        error = r[0, 0] - x
-        if error > 1e-2:
-            # Max control input until the reference is reached
-            u = 12.0
-        else:
-            # Maintain speed
-            u = u_ss
-
-        # Verify input
-        if (
-            k > 0
-            and k < N - 1
-            and near(12.0, U.value(0, k - 1), 1e-2)
-            and near(u_ss, U.value(0, k + 1), 1e-2)
-        ):
-            # If control input is transitioning between 12 and u_ss, ensure it's
-            # within (u_ss, 12)
-            assert U.value(0, k) >= u_ss
-            assert U.value(0, k) <= 12.0
-        else:
-            assert U.value(0, k) == pytest.approx(u, abs=1e-4)
-
-        # Project state forward
-        x = A * x + B * u
-
-    # Verify final state
-    assert X.value(0, N) == pytest.approx(r[0, 0], abs=1e-7)
-
-    # Log states for offline viewing
-    with open("Flywheel states.csv", "w") as f:
-        f.write("Time (s),Velocity (rad/s)\n")
-
-        for k in range(N + 1):
-            f.write(f"{k * dt},{X.value(0, k)}\n")
-
-    # Log inputs for offline viewing
-    with open("Flywheel inputs.csv", "w") as f:
-        f.write("Time (s),Voltage (V)\n")
-
-        for k in range(N + 1):
-            if k < N:
-                f.write(f"{k * dt},{U.value(0, k)}\n")
-            else:
-                f.write(f"{k * dt},0.0\n")
+import math
+
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+import numpy as np
+import pytest
+
+
+def near(expected, actual, tolerance):
+    return abs(expected - actual) < tolerance
+
+
+def test_optimization_problem_flywheel():
+    T = 5.0
+    dt = 0.005
+    N = int(T / dt)
+
+    # Flywheel model:
+    # States: [velocity]
+    # Inputs: [voltage]
+    A = math.exp(-dt)
+    B = 1.0 - math.exp(-dt)
+
+    problem = OptimizationProblem()
+    X = problem.decision_variable(1, N + 1)
+    U = problem.decision_variable(1, N)
+
+    # Dynamics constraint
+    for k in range(N):
+        problem.subject_to(
+            X[:, k + 1 : k + 2] == A * X[:, k : k + 1] + B * U[:, k : k + 1]
+        )
+
+    # State and input constraints
+    problem.subject_to(X[0, 0] == 0.0)
+    problem.subject_to(-12 <= U)
+    problem.subject_to(U <= 12)
+
+    # Cost function - minimize error
+    r = np.array([[10.0]])
+    J = 0.0
+    for k in range(N + 1):
+        J += (r - X[:, k : k + 1]).T @ (r - X[:, k : k + 1])
+    problem.minimize(J)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.LINEAR
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    # Voltage for steady-state velocity:
+    #
+    # rₖ₊₁ = Arₖ + Buₖ
+    # uₖ = B⁺(rₖ₊₁ − Arₖ)
+    # uₖ = B⁺(rₖ − Arₖ)
+    # uₖ = B⁺(I − A)rₖ
+    u_ss = 1.0 / B * (1.0 - A) * r[0, 0]
+
+    # Verify initial state
+    assert X.value(0, 0) == pytest.approx(0.0, abs=1e-8)
+
+    # Verify solution
+    x = 0.0
+    u = 0.0
+    for k in range(N):
+        # Verify state
+        assert X.value(0, k) == pytest.approx(x, abs=1e-2)
+
+        # Determine expected input for this timestep
+        error = r[0, 0] - x
+        if error > 1e-2:
+            # Max control input until the reference is reached
+            u = 12.0
+        else:
+            # Maintain speed
+            u = u_ss
+
+        # Verify input
+        if (
+            k > 0
+            and k < N - 1
+            and near(12.0, U.value(0, k - 1), 1e-2)
+            and near(u_ss, U.value(0, k + 1), 1e-2)
+        ):
+            # If control input is transitioning between 12 and u_ss, ensure it's
+            # within (u_ss, 12)
+            assert U.value(0, k) >= u_ss
+            assert U.value(0, k) <= 12.0
+        else:
+            assert U.value(0, k) == pytest.approx(u, abs=1e-4)
+
+        # Project state forward
+        x = A * x + B * u
+
+    # Verify final state
+    assert X.value(0, N) == pytest.approx(r[0, 0], abs=1e-7)
+
+    # Log states for offline viewing
+    with open("Flywheel states.csv", "w") as f:
+        f.write("Time (s),Velocity (rad/s)\n")
+
+        for k in range(N + 1):
+            f.write(f"{k * dt},{X.value(0, k)}\n")
+
+    # Log inputs for offline viewing
+    with open("Flywheel inputs.csv", "w") as f:
+        f.write("Time (s),Voltage (V)\n")
+
+        for k in range(N + 1):
+            if k < N:
+                f.write(f"{k * dt},{U.value(0, k)}\n")
+            else:
+                f.write(f"{k * dt},0.0\n")
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/quadratic_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/nonlinear_problem_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,144 +1,121 @@
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-import numpy as np
-import pytest
-
-
-def test_unconstrained1d():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    x.set_value(2.0)
-
-    problem.minimize(x * x - 6.0 * x)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value() == pytest.approx(3.0, abs=1e-6)
-
-
-def test_unconstrained2d_1():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    x.set_value(1.0)
-    y = problem.decision_variable()
-    y.set_value(2.0)
-
-    problem.minimize(x * x + y * y)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value() == pytest.approx(0.0, abs=1e-6)
-    assert y.value() == pytest.approx(0.0, abs=1e-6)
-
-
-def test_unconstrained2d_2():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable(2)
-    x[0].set_value(1.0)
-    x[1].set_value(2.0)
-
-    problem.minimize(x.T @ x)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value(0) == pytest.approx(0.0, abs=1e-6)
-    assert x.value(1) == pytest.approx(0.0, abs=1e-6)
-
-
-# Maximize xy subject to x + 3y = 36.
-#
-# Maximize f(x,y) = xy
-# subject to g(x,y) = x + 3y - 36 = 0
-#
-#         value func  constraint
-#              |          |
-#              v          v
-# L(x,y,λ) = f(x,y) - λg(x,y)
-# L(x,y,λ) = xy - λ(x + 3y - 36)
-# L(x,y,λ) = xy - xλ - 3yλ + 36λ
-#
-# ∇_x,y,λ L(x,y,λ) = 0
-#
-# ∂L/∂x = y - λ
-# ∂L/∂y = x - 3λ
-# ∂L/∂λ = -x - 3y + 36
-#
-#  0x + 1y - 1λ = 0
-#  1x + 0y - 3λ = 0
-# -1x - 3y + 0λ + 36 = 0
-#
-# [ 0  1 -1][x]   [  0]
-# [ 1  0 -3][y] = [  0]
-# [-1 -3  0][λ]   [-36]
-#
-# Solve with:
-# ```python
-#   np.linalg.solve(
-#     np.array([[0,1,-1],
-#               [1,0,-3],
-#               [-1,-3,0]]),
-#     np.array([[0], [0], [-36]]))
-# ```
-#
-# [x]   [18]
-# [y] = [ 6]
-# [λ]   [ 6]
-def test_equality_constrained_1():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    y = problem.decision_variable()
-
-    problem.maximize(x * y)
-
-    problem.subject_to(x + 3 * y == 36)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value() == pytest.approx(18.0, abs=1e-5)
-    assert y.value() == pytest.approx(6.0, abs=1e-5)
-
-
-def test_equality_constrained_2():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable(2)
-    x[0].set_value(1.0)
-    x[1].set_value(2.0)
-
-    problem.minimize(x.T @ x)
-
-    problem.subject_to(x == np.array([[3.0], [3.0]]))
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    assert x.value(0) == pytest.approx(3.0, abs=1e-5)
-    assert x.value(1) == pytest.approx(3.0, abs=1e-5)
+import platform
+
+import jormungandr.autodiff as autodiff
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+
+import numpy as np
+import pytest
+
+
+def test_quartic():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    x.set_value(20.0)
+
+    problem.minimize(autodiff.pow(x, 4))
+
+    problem.subject_to(x >= 1)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONLINEAR
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.LINEAR
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value() == pytest.approx(1.0, abs=1e-6)
+
+
+def test_rosenbrock_with_cubic_and_line_constraint():
+    # https://en.wikipedia.org/wiki/Test_functions_for_optimization#Test_functions_for_constrained_optimization
+    for x0 in np.arange(-1.5, 1.5, 0.1):
+        for y0 in np.arange(-0.5, 2.5, 0.1):
+            problem = OptimizationProblem()
+
+            x = problem.decision_variable()
+            x.set_value(x0)
+            y = problem.decision_variable()
+            y.set_value(y0)
+
+            problem.minimize(
+                autodiff.pow(1 - x, 2) + 100 * autodiff.pow(y - autodiff.pow(x, 2), 2)
+            )
+
+            problem.subject_to(autodiff.pow(x - 1, 3) - y + 1 <= 0)
+            problem.subject_to(x + y - 2 <= 0)
+
+            status = problem.solve()
+
+            assert status.cost_function_type == ExpressionType.NONLINEAR
+            assert status.equality_constraint_type == ExpressionType.NONE
+            assert status.inequality_constraint_type == ExpressionType.NONLINEAR
+            assert status.exit_condition == SolverExitCondition.SUCCESS
+
+            # Local minimum at (0.0, 0.0)
+            # Global minimum at (1.0, 1.0)
+            assert x.value() == pytest.approx(
+                0.0, abs=1e-2
+            ) or x.value() == pytest.approx(1.0, abs=1e-2)
+            assert y.value() == pytest.approx(
+                0.0, abs=1e-2
+            ) or y.value() == pytest.approx(1.0, abs=1e-2)
+
+
+def test_rosenbrock_with_disk_constraint():
+    # https://en.wikipedia.org/wiki/Test_functions_for_optimization#Test_functions_for_constrained_optimization
+    for x0 in np.arange(-1.5, 1.5, 0.1):
+        for y0 in np.arange(-1.5, 1.5, 0.1):
+            problem = OptimizationProblem()
+
+            x = problem.decision_variable()
+            x.set_value(x0)
+            y = problem.decision_variable()
+            y.set_value(y0)
+
+            problem.minimize(
+                autodiff.pow(1 - x, 2) + 100 * autodiff.pow(y - autodiff.pow(x, 2), 2)
+            )
+
+            problem.subject_to(autodiff.pow(x, 2) + autodiff.pow(y, 2) <= 2)
+
+            status = problem.solve()
+
+            assert status.cost_function_type == ExpressionType.NONLINEAR
+            assert status.equality_constraint_type == ExpressionType.NONE
+            assert status.inequality_constraint_type == ExpressionType.QUADRATIC
+            assert status.exit_condition == SolverExitCondition.SUCCESS
+
+            assert x.value() == pytest.approx(1.0, abs=1e-1)
+            assert y.value() == pytest.approx(1.0, abs=1e-1)
+
+
+def test_narrow_feasible_region():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    x.set_value(20.0)
+
+    y = problem.decision_variable()
+    y.set_value(50.0)
+
+    problem.minimize(autodiff.sqrt(x * x + y * y))
+
+    problem.subject_to(y == -x + 5.0)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONLINEAR
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.NONE
+
+    if platform.system() == "Darwin" and platform.machine() == "arm64":
+        # FIXME: Fails on macOS arm64 with "diverging iterates"
+        assert status.exit_condition == SolverExitCondition.DIVERGING_ITERATES
+        return
+    else:
+        assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    assert x.value() == pytest.approx(2.5, abs=1e-2)
+    assert y.value() == pytest.approx(2.5, abs=1e-2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/solver_exit_condition_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/solver_exit_condition_test.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-"""These tests ensure coverage of the off-nominal solver exit conditions"""
-
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-
-
-def test_callback_requested_stop():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    problem.minimize(x * x)
-
-    problem.callback(lambda info: None)
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    problem.callback(lambda info: False)
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    problem.callback(lambda info: True)
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.CALLBACK_REQUESTED_STOP
-
-
-def test_too_few_dofs():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    y = problem.decision_variable()
-    z = problem.decision_variable()
-
-    problem.subject_to(x == 1)
-    problem.subject_to(x == 2)
-    problem.subject_to(y == 1)
-    problem.subject_to(z == 1)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONE
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.TOO_FEW_DOFS
-
-
-def test_locally_infeasible_equality_constraints():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    y = problem.decision_variable()
-    z = problem.decision_variable()
-
-    problem.subject_to(x == y + 1)
-    problem.subject_to(y == z + 1)
-    problem.subject_to(z == x + 1)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONE
-    assert status.equality_constraint_type == ExpressionType.LINEAR
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.LOCALLY_INFEASIBLE
-
-
-def test_locally_infeasible_inequality_constraints():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    y = problem.decision_variable()
-    z = problem.decision_variable()
-
-    problem.subject_to(x >= y + 1)
-    problem.subject_to(y >= z + 1)
-    problem.subject_to(z >= x + 1)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONE
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.LINEAR
-    assert status.exit_condition == SolverExitCondition.LOCALLY_INFEASIBLE
-
-
-def test_diverging_iterates():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    problem.minimize(x)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.LINEAR
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.DIVERGING_ITERATES
-
-
-def test_max_iterations_exceeded():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    problem.minimize(x * x)
-
-    status = problem.solve(max_iterations=0, diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.MAX_ITERATIONS_EXCEEDED
-
-
-def test_timeout():
-    problem = OptimizationProblem()
-
-    x = problem.decision_variable()
-    problem.minimize(x * x)
-
-    status = problem.solve(timeout=0.0, diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.QUADRATIC
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.TIMEOUT
+"""These tests ensure coverage of the off-nominal solver exit conditions"""
+
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+
+
+def test_callback_requested_stop():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    problem.minimize(x * x)
+
+    problem.callback(lambda info: None)
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    problem.callback(lambda info: False)
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    problem.callback(lambda info: True)
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.CALLBACK_REQUESTED_STOP
+
+
+def test_too_few_dofs():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    y = problem.decision_variable()
+    z = problem.decision_variable()
+
+    problem.subject_to(x == 1)
+    problem.subject_to(x == 2)
+    problem.subject_to(y == 1)
+    problem.subject_to(z == 1)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONE
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.TOO_FEW_DOFS
+
+
+def test_locally_infeasible_equality_constraints():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    y = problem.decision_variable()
+    z = problem.decision_variable()
+
+    problem.subject_to(x == y + 1)
+    problem.subject_to(y == z + 1)
+    problem.subject_to(z == x + 1)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONE
+    assert status.equality_constraint_type == ExpressionType.LINEAR
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.LOCALLY_INFEASIBLE
+
+
+def test_locally_infeasible_inequality_constraints():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    y = problem.decision_variable()
+    z = problem.decision_variable()
+
+    problem.subject_to(x >= y + 1)
+    problem.subject_to(y >= z + 1)
+    problem.subject_to(z >= x + 1)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONE
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.LINEAR
+    assert status.exit_condition == SolverExitCondition.LOCALLY_INFEASIBLE
+
+
+def test_diverging_iterates():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    problem.minimize(x)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.LINEAR
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.DIVERGING_ITERATES
+
+
+def test_max_iterations_exceeded():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    problem.minimize(x * x)
+
+    status = problem.solve(max_iterations=0, diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.MAX_ITERATIONS_EXCEEDED
+
+
+def test_timeout():
+    problem = OptimizationProblem()
+
+    x = problem.decision_variable()
+    problem.minimize(x * x)
+
+    status = problem.solve(timeout=0.0, diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.QUADRATIC
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.TIMEOUT
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/jormungandr/test/optimization/trivial_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev96/jormungandr/test/optimization/trivial_problem_test.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from jormungandr.autodiff import ExpressionType
-from jormungandr.optimization import OptimizationProblem, SolverExitCondition
-import numpy as np
-
-
-def test_empty():
-    problem = OptimizationProblem()
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONE
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-
-def test_no_cost_unconstrained_1():
-    problem = OptimizationProblem()
-
-    X = problem.decision_variable(2, 3)
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONE
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    for row in range(X.rows()):
-        for col in range(X.cols()):
-            assert X.value(row, col) == 0.0
-
-
-def test_no_cost_unconstrained_2():
-    problem = OptimizationProblem()
-
-    X = problem.decision_variable(2, 3)
-    X.set_value([[1.0, 1.0, 1.0], [1.0, 1.0, 1.0]])
-
-    status = problem.solve(diagnostics=True)
-
-    assert status.cost_function_type == ExpressionType.NONE
-    assert status.equality_constraint_type == ExpressionType.NONE
-    assert status.inequality_constraint_type == ExpressionType.NONE
-    assert status.exit_condition == SolverExitCondition.SUCCESS
-
-    for row in range(X.rows()):
-        for col in range(X.cols()):
-            assert X.value(row, col) == 1.0
+from jormungandr.autodiff import ExpressionType
+from jormungandr.optimization import OptimizationProblem, SolverExitCondition
+import numpy as np
+
+
+def test_empty():
+    problem = OptimizationProblem()
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONE
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+
+def test_no_cost_unconstrained_1():
+    problem = OptimizationProblem()
+
+    X = problem.decision_variable(2, 3)
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONE
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    for row in range(X.rows()):
+        for col in range(X.cols()):
+            assert X.value(row, col) == 0.0
+
+
+def test_no_cost_unconstrained_2():
+    problem = OptimizationProblem()
+
+    X = problem.decision_variable(2, 3)
+    X.set_value([[1.0, 1.0, 1.0], [1.0, 1.0, 1.0]])
+
+    status = problem.solve(diagnostics=True)
+
+    assert status.cost_function_type == ExpressionType.NONE
+    assert status.equality_constraint_type == ExpressionType.NONE
+    assert status.inequality_constraint_type == ExpressionType.NONE
+    assert status.exit_condition == SolverExitCondition.SUCCESS
+
+    for row in range(X.rows()):
+        for col in range(X.cols()):
+            assert X.value(row, col) == 1.0
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/Inertia.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/Inertia.hpp`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <cstddef>
-
-#include "sleipnir/util/Concepts.hpp"
-
-namespace sleipnir {
-
-/**
- * Represents the inertia of a matrix (the number of positive, negative, and
- * zero eigenvalues).
- */
-class Inertia {
- public:
-  size_t positive = 0;
-  size_t negative = 0;
-  size_t zero = 0;
-
-  constexpr Inertia() = default;
-
-  /**
-   * Constructs the Inertia type with the given number of positive, negative,
-   * and zero eigenvalues.
-   *
-   * @param positive The number of positive eigenvalues.
-   * @param negative The number of negative eigenvalues.
-   * @param zero The number of zero eigenvalues.
-   */
-  constexpr Inertia(size_t positive, size_t negative, size_t zero)
-      : positive{positive}, negative{negative}, zero{zero} {}
-
-  /**
-   * Constructs the Inertia type with the inertia of the given LDLT
-   * decomposition.
-   *
-   * @tparam Solver Eigen sparse linear system solver.
-   * @param solver The LDLT decomposition of which to compute the inertia.
-   */
-  template <EigenSolver Solver>
-  explicit Inertia(const Solver& solver) {
-    const auto& D = solver.vectorD();
-    for (int row = 0; row < D.rows(); ++row) {
-      if (D(row) > 0.0) {
-        ++positive;
-      } else if (D(row) < 0.0) {
-        ++negative;
-      } else {
-        ++zero;
-      }
-    }
-  }
-
-  bool operator==(const Inertia&) const = default;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <cstddef>
+
+#include "sleipnir/util/Concepts.hpp"
+
+namespace sleipnir {
+
+/**
+ * Represents the inertia of a matrix (the number of positive, negative, and
+ * zero eigenvalues).
+ */
+class Inertia {
+ public:
+  size_t positive = 0;
+  size_t negative = 0;
+  size_t zero = 0;
+
+  constexpr Inertia() = default;
+
+  /**
+   * Constructs the Inertia type with the given number of positive, negative,
+   * and zero eigenvalues.
+   *
+   * @param positive The number of positive eigenvalues.
+   * @param negative The number of negative eigenvalues.
+   * @param zero The number of zero eigenvalues.
+   */
+  constexpr Inertia(size_t positive, size_t negative, size_t zero)
+      : positive{positive}, negative{negative}, zero{zero} {}
+
+  /**
+   * Constructs the Inertia type with the inertia of the given LDLT
+   * decomposition.
+   *
+   * @tparam Solver Eigen sparse linear system solver.
+   * @param solver The LDLT decomposition of which to compute the inertia.
+   */
+  template <EigenSolver Solver>
+  explicit Inertia(const Solver& solver) {
+    const auto& D = solver.vectorD();
+    for (int row = 0; row < D.rows(); ++row) {
+      if (D(row) > 0.0) {
+        ++positive;
+      } else if (D(row) < 0.0) {
+        ++negative;
+      } else {
+        ++zero;
+      }
+    }
+  }
+
+  bool operator==(const Inertia&) const = default;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/RegularizedLDLT.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/RegularizedLDLT.hpp`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <cmath>
-#include <cstddef>
-
-#include <Eigen/Core>
-#include <Eigen/SparseCholesky>
-#include <Eigen/SparseCore>
-
-#include "optimization/Inertia.hpp"
-
-// See docs/algorithms.md#Works_cited for citation definitions
-
-namespace sleipnir {
-
-/**
- * Solves systems of linear equations using a regularized LDLT factorization.
- */
-class RegularizedLDLT {
- public:
-  using Solver = Eigen::SimplicialLDLT<Eigen::SparseMatrix<double>,
-                                       Eigen::Lower, Eigen::AMDOrdering<int>>;
-
-  /**
-   * Constructs a RegularizedLDLT instance.
-   */
-  RegularizedLDLT() = default;
-
-  /**
-   * Reports whether previous computation was successful.
-   */
-  Eigen::ComputationInfo Info() { return m_info; }
-
-  /**
-   * Computes the regularized LDLT factorization of a matrix.
-   *
-   * @param lhs Left-hand side of the system.
-   * @param numEqualityConstraints The number of equality constraints in the
-   *   system.
-   * @param μ The barrier parameter for the current interior-point iteration.
-   */
-  void Compute(const Eigen::SparseMatrix<double>& lhs,
-               size_t numEqualityConstraints, double μ) {
-    // The regularization procedure is based on algorithm B.1 of [1]
-    m_numDecisionVariables = lhs.rows() - numEqualityConstraints;
-    m_numEqualityConstraints = numEqualityConstraints;
-
-    const Inertia idealInertia{m_numDecisionVariables, m_numEqualityConstraints,
-                               0};
-    Inertia inertia;
-
-    double δ = 0.0;
-    double γ = 0.0;
-
-    AnalyzePattern(lhs);
-    m_solver.factorize(lhs);
-
-    if (m_solver.info() == Eigen::Success) {
-      inertia = Inertia{m_solver};
-
-      // If the inertia is ideal, don't regularize the system
-      if (inertia == idealInertia) {
-        m_info = Eigen::Success;
-        return;
-      }
-    }
-
-    // If the decomposition succeeded and the inertia has some zero eigenvalues,
-    // or the decomposition failed, regularize the equality constraints
-    if ((m_solver.info() == Eigen::Success && inertia.zero > 0) ||
-        m_solver.info() != Eigen::Success) {
-      γ = 1e-8 * std::pow(μ, 0.25);
-    }
-
-    // Also regularize the Hessian. If the Hessian wasn't regularized in a
-    // previous run of Compute(), start at a small value of δ. Otherwise,
-    // attempt a δ half as big as the previous run so δ can trend downwards over
-    // time.
-    if (m_δOld == 0.0) {
-      δ = 1e-4;
-    } else {
-      δ = m_δOld / 2.0;
-    }
-
-    while (true) {
-      // Regularize lhs by adding a multiple of the identity matrix
-      //
-      // lhs = [H + AᵢᵀΣAᵢ + δI   Aₑᵀ]
-      //       [       Aₑ        −γI ]
-      Eigen::SparseMatrix<double> lhsReg = lhs + Regularization(δ, γ);
-      AnalyzePattern(lhsReg);
-      m_solver.factorize(lhsReg);
-      inertia = Inertia{m_solver};
-
-      // If the inertia is ideal, store that value of δ and return.
-      // Otherwise, increase δ by an order of magnitude and try again.
-      if (inertia == idealInertia) {
-        m_δOld = δ;
-        m_info = Eigen::Success;
-        return;
-      } else {
-        δ *= 10.0;
-
-        // If the Hessian perturbation is too high, report failure. This can
-        // happen due to a rank-deficient equality constraint Jacobian with
-        // linearly dependent constraints.
-        if (δ > 1e20) {
-          m_info = Eigen::NumericalIssue;
-          return;
-        }
-      }
-    }
-  }
-
-  /**
-   * Solve the system of equations using a regularized LDLT factorization.
-   *
-   * @param rhs Right-hand side of the system.
-   */
-  template <typename Rhs>
-  auto Solve(const Eigen::MatrixBase<Rhs>& rhs) {
-    return m_solver.solve(rhs);
-  }
-
- private:
-  Solver m_solver;
-
-  Eigen::ComputationInfo m_info = Eigen::Success;
-
-  /// The number of decision variables in the system.
-  size_t m_numDecisionVariables = 0;
-
-  /// The number of equality constraints in the system.
-  size_t m_numEqualityConstraints = 0;
-
-  /// The value of δ from the previous run of Compute().
-  double m_δOld = 0.0;
-
-  // Number of non-zeros in LHS.
-  int m_nonZeros = -1;
-
-  /**
-   * Reanalize LHS matrix's sparsity pattern if it changed.
-   *
-   * @param lhs Matrix to analyze.
-   */
-  void AnalyzePattern(const Eigen::SparseMatrix<double>& lhs) {
-    int nonZeros = lhs.nonZeros();
-    if (m_nonZeros != nonZeros) {
-      m_solver.analyzePattern(lhs);
-      m_nonZeros = nonZeros;
-    }
-  }
-
-  /**
-   * Returns regularization matrix.
-   *
-   * @param δ The Hessian regularization factor.
-   * @param γ The equality constraint Jacobian regularization factor.
-   */
-  Eigen::SparseMatrix<double> Regularization(double δ, double γ) {
-    Eigen::VectorXd vec{m_numDecisionVariables + m_numEqualityConstraints};
-    size_t row = 0;
-    while (row < m_numDecisionVariables) {
-      vec(row) = δ;
-      ++row;
-    }
-    while (row < m_numDecisionVariables + m_numEqualityConstraints) {
-      vec(row) = -γ;
-      ++row;
-    }
-
-    return Eigen::SparseMatrix<double>{vec.asDiagonal()};
-  }
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <cmath>
+#include <cstddef>
+
+#include <Eigen/Core>
+#include <Eigen/SparseCholesky>
+#include <Eigen/SparseCore>
+
+#include "optimization/Inertia.hpp"
+
+// See docs/algorithms.md#Works_cited for citation definitions
+
+namespace sleipnir {
+
+/**
+ * Solves systems of linear equations using a regularized LDLT factorization.
+ */
+class RegularizedLDLT {
+ public:
+  using Solver = Eigen::SimplicialLDLT<Eigen::SparseMatrix<double>,
+                                       Eigen::Lower, Eigen::AMDOrdering<int>>;
+
+  /**
+   * Constructs a RegularizedLDLT instance.
+   */
+  RegularizedLDLT() = default;
+
+  /**
+   * Reports whether previous computation was successful.
+   */
+  Eigen::ComputationInfo Info() { return m_info; }
+
+  /**
+   * Computes the regularized LDLT factorization of a matrix.
+   *
+   * @param lhs Left-hand side of the system.
+   * @param numEqualityConstraints The number of equality constraints in the
+   *   system.
+   * @param μ The barrier parameter for the current interior-point iteration.
+   */
+  void Compute(const Eigen::SparseMatrix<double>& lhs,
+               size_t numEqualityConstraints, double μ) {
+    // The regularization procedure is based on algorithm B.1 of [1]
+    m_numDecisionVariables = lhs.rows() - numEqualityConstraints;
+    m_numEqualityConstraints = numEqualityConstraints;
+
+    const Inertia idealInertia{m_numDecisionVariables, m_numEqualityConstraints,
+                               0};
+    Inertia inertia;
+
+    double δ = 0.0;
+    double γ = 0.0;
+
+    AnalyzePattern(lhs);
+    m_solver.factorize(lhs);
+
+    if (m_solver.info() == Eigen::Success) {
+      inertia = Inertia{m_solver};
+
+      // If the inertia is ideal, don't regularize the system
+      if (inertia == idealInertia) {
+        m_info = Eigen::Success;
+        return;
+      }
+    }
+
+    // If the decomposition succeeded and the inertia has some zero eigenvalues,
+    // or the decomposition failed, regularize the equality constraints
+    if ((m_solver.info() == Eigen::Success && inertia.zero > 0) ||
+        m_solver.info() != Eigen::Success) {
+      γ = 1e-8 * std::pow(μ, 0.25);
+    }
+
+    // Also regularize the Hessian. If the Hessian wasn't regularized in a
+    // previous run of Compute(), start at a small value of δ. Otherwise,
+    // attempt a δ half as big as the previous run so δ can trend downwards over
+    // time.
+    if (m_δOld == 0.0) {
+      δ = 1e-4;
+    } else {
+      δ = m_δOld / 2.0;
+    }
+
+    while (true) {
+      // Regularize lhs by adding a multiple of the identity matrix
+      //
+      // lhs = [H + AᵢᵀΣAᵢ + δI   Aₑᵀ]
+      //       [       Aₑ        −γI ]
+      Eigen::SparseMatrix<double> lhsReg = lhs + Regularization(δ, γ);
+      AnalyzePattern(lhsReg);
+      m_solver.factorize(lhsReg);
+      inertia = Inertia{m_solver};
+
+      // If the inertia is ideal, store that value of δ and return.
+      // Otherwise, increase δ by an order of magnitude and try again.
+      if (inertia == idealInertia) {
+        m_δOld = δ;
+        m_info = Eigen::Success;
+        return;
+      } else {
+        δ *= 10.0;
+
+        // If the Hessian perturbation is too high, report failure. This can
+        // happen due to a rank-deficient equality constraint Jacobian with
+        // linearly dependent constraints.
+        if (δ > 1e20) {
+          m_info = Eigen::NumericalIssue;
+          return;
+        }
+      }
+    }
+  }
+
+  /**
+   * Solve the system of equations using a regularized LDLT factorization.
+   *
+   * @param rhs Right-hand side of the system.
+   */
+  template <typename Rhs>
+  auto Solve(const Eigen::MatrixBase<Rhs>& rhs) {
+    return m_solver.solve(rhs);
+  }
+
+ private:
+  Solver m_solver;
+
+  Eigen::ComputationInfo m_info = Eigen::Success;
+
+  /// The number of decision variables in the system.
+  size_t m_numDecisionVariables = 0;
+
+  /// The number of equality constraints in the system.
+  size_t m_numEqualityConstraints = 0;
+
+  /// The value of δ from the previous run of Compute().
+  double m_δOld = 0.0;
+
+  // Number of non-zeros in LHS.
+  int m_nonZeros = -1;
+
+  /**
+   * Reanalize LHS matrix's sparsity pattern if it changed.
+   *
+   * @param lhs Matrix to analyze.
+   */
+  void AnalyzePattern(const Eigen::SparseMatrix<double>& lhs) {
+    int nonZeros = lhs.nonZeros();
+    if (m_nonZeros != nonZeros) {
+      m_solver.analyzePattern(lhs);
+      m_nonZeros = nonZeros;
+    }
+  }
+
+  /**
+   * Returns regularization matrix.
+   *
+   * @param δ The Hessian regularization factor.
+   * @param γ The equality constraint Jacobian regularization factor.
+   */
+  Eigen::SparseMatrix<double> Regularization(double δ, double γ) {
+    Eigen::VectorXd vec{m_numDecisionVariables + m_numEqualityConstraints};
+    size_t row = 0;
+    while (row < m_numDecisionVariables) {
+      vec(row) = δ;
+      ++row;
+    }
+    while (row < m_numDecisionVariables + m_numEqualityConstraints) {
+      vec(row) = -γ;
+      ++row;
+    }
+
+    return Eigen::SparseMatrix<double>{vec.asDiagonal()};
+  }
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/InteriorPoint.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/InteriorPoint.cpp`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,874 +1,874 @@
-// Copyright (c) Sleipnir contributors
-
-#include "sleipnir/optimization/solver/InteriorPoint.hpp"
-
-#include <algorithm>
-#include <chrono>
-#include <cmath>
-#include <fstream>
-#include <limits>
-#include <vector>
-
-#include <Eigen/SparseCholesky>
-
-#include "optimization/RegularizedLDLT.hpp"
-#include "optimization/solver/util/ErrorEstimate.hpp"
-#include "optimization/solver/util/FeasibilityRestoration.hpp"
-#include "optimization/solver/util/Filter.hpp"
-#include "optimization/solver/util/FractionToTheBoundaryRule.hpp"
-#include "optimization/solver/util/IsLocallyInfeasible.hpp"
-#include "optimization/solver/util/KKTError.hpp"
-#include "sleipnir/autodiff/Gradient.hpp"
-#include "sleipnir/autodiff/Hessian.hpp"
-#include "sleipnir/autodiff/Jacobian.hpp"
-#include "sleipnir/optimization/SolverExitCondition.hpp"
-#include "sleipnir/util/Print.hpp"
-#include "sleipnir/util/Spy.hpp"
-#include "util/ScopeExit.hpp"
-#include "util/ToMilliseconds.hpp"
-
-// See docs/algorithms.md#Works_cited for citation definitions.
-//
-// See docs/algorithms.md#Interior-point_method for a derivation of the
-// interior-point method formulation being used.
-
-namespace sleipnir {
-
-void InteriorPoint(
-    std::span<Variable> decisionVariables,
-    std::span<Variable> equalityConstraints,
-    std::span<Variable> inequalityConstraints, Variable& f,
-    const std::function<bool(const SolverIterationInfo&)>& callback,
-    const SolverConfig& config, bool feasibilityRestoration, Eigen::VectorXd& x,
-    Eigen::VectorXd& s, SolverStatus* status) {
-  const auto solveStartTime = std::chrono::system_clock::now();
-
-  // Map decision variables and constraints to VariableMatrices for Lagrangian
-  VariableMatrix xAD{decisionVariables};
-  xAD.SetValue(x);
-  VariableMatrix c_eAD{equalityConstraints};
-  VariableMatrix c_iAD{inequalityConstraints};
-
-  // Create autodiff variables for s, y, and z for Lagrangian
-  VariableMatrix sAD(inequalityConstraints.size());
-  sAD.SetValue(s);
-  VariableMatrix yAD(equalityConstraints.size());
-  for (auto& y : yAD) {
-    y.SetValue(0.0);
-  }
-  VariableMatrix zAD(inequalityConstraints.size());
-  for (auto& z : zAD) {
-    z.SetValue(1.0);
-  }
-
-  // Lagrangian L
-  //
-  // L(xₖ, sₖ, yₖ, zₖ) = f(xₖ) − yₖᵀcₑ(xₖ) − zₖᵀ(cᵢ(xₖ) − sₖ)
-  auto L = f - (yAD.T() * c_eAD)(0) - (zAD.T() * (c_iAD - sAD))(0);
-
-  // Equality constraint Jacobian Aₑ
-  //
-  //         [∇ᵀcₑ₁(xₖ)]
-  // Aₑ(x) = [∇ᵀcₑ₂(xₖ)]
-  //         [    ⋮    ]
-  //         [∇ᵀcₑₘ(xₖ)]
-  Jacobian jacobianCe{c_eAD, xAD};
-  Eigen::SparseMatrix<double> A_e = jacobianCe.Value();
-
-  // Inequality constraint Jacobian Aᵢ
-  //
-  //         [∇ᵀcᵢ₁(xₖ)]
-  // Aᵢ(x) = [∇ᵀcᵢ₂(xₖ)]
-  //         [    ⋮    ]
-  //         [∇ᵀcᵢₘ(xₖ)]
-  Jacobian jacobianCi{c_iAD, xAD};
-  Eigen::SparseMatrix<double> A_i = jacobianCi.Value();
-
-  // Gradient of f ∇f
-  Gradient gradientF{f, xAD};
-  Eigen::SparseVector<double> g = gradientF.Value();
-
-  // Hessian of the Lagrangian H
-  //
-  // Hₖ = ∇²ₓₓL(xₖ, sₖ, yₖ, zₖ)
-  Hessian hessianL{L, xAD};
-  Eigen::SparseMatrix<double> H = hessianL.Value();
-
-  Eigen::VectorXd y = yAD.Value();
-  Eigen::VectorXd z = zAD.Value();
-  Eigen::VectorXd c_e = c_eAD.Value();
-  Eigen::VectorXd c_i = c_iAD.Value();
-
-  // Check for overconstrained problem
-  if (equalityConstraints.size() > decisionVariables.size()) {
-    if (config.diagnostics) {
-      sleipnir::println("The problem has too few degrees of freedom.");
-      sleipnir::println(
-          "Violated constraints (cₑ(x) = 0) in order of declaration:");
-      for (int row = 0; row < c_e.rows(); ++row) {
-        if (c_e(row) < 0.0) {
-          sleipnir::println("  {}/{}: {} = 0", row + 1, c_e.rows(), c_e(row));
-        }
-      }
-    }
-
-    status->exitCondition = SolverExitCondition::kTooFewDOFs;
-    return;
-  }
-
-  // Check whether initial guess has finite f(xₖ), cₑ(xₖ), and cᵢ(xₖ)
-  if (!std::isfinite(f.Value()) || !c_e.allFinite() || !c_i.allFinite()) {
-    status->exitCondition =
-        SolverExitCondition::kNonfiniteInitialCostOrConstraints;
-    return;
-  }
-
-  // Sparsity pattern files written when spy flag is set in SolverConfig
-  std::ofstream H_spy;
-  std::ofstream A_e_spy;
-  std::ofstream A_i_spy;
-  if (config.spy) {
-    A_e_spy.open("A_e.spy");
-    A_i_spy.open("A_i.spy");
-    H_spy.open("H.spy");
-  }
-
-  if (config.diagnostics && !feasibilityRestoration) {
-    sleipnir::println("Error tolerance: {}\n", config.tolerance);
-  }
-
-  std::chrono::system_clock::time_point iterationsStartTime;
-
-  int iterations = 0;
-
-  // Prints final diagnostics when the solver exits
-  scope_exit exit{[&] {
-    if (config.diagnostics && !feasibilityRestoration) {
-      auto solveEndTime = std::chrono::system_clock::now();
-
-      sleipnir::println("\nSolve time: {:.3f} ms",
-                        ToMilliseconds(solveEndTime - solveStartTime));
-      sleipnir::println("  ↳ {:.3f} ms (solver setup)",
-                        ToMilliseconds(iterationsStartTime - solveStartTime));
-      if (iterations > 0) {
-        sleipnir::println(
-            "  ↳ {:.3f} ms ({} solver iterations; {:.3f} ms average)",
-            ToMilliseconds(solveEndTime - iterationsStartTime), iterations,
-            ToMilliseconds((solveEndTime - iterationsStartTime) / iterations));
-      }
-      sleipnir::println("");
-
-      sleipnir::println("{:^8}   {:^10}   {:^14}   {:^6}", "autodiff",
-                        "setup (ms)", "avg solve (ms)", "solves");
-      sleipnir::println("{:=^47}", "");
-      constexpr auto format = "{:^8}   {:10.3f}   {:14.3f}   {:6}";
-      sleipnir::println(format, "∇f(x)",
-                        gradientF.GetProfiler().SetupDuration(),
-                        gradientF.GetProfiler().AverageSolveDuration(),
-                        gradientF.GetProfiler().SolveMeasurements());
-      sleipnir::println(format, "∇²ₓₓL", hessianL.GetProfiler().SetupDuration(),
-                        hessianL.GetProfiler().AverageSolveDuration(),
-                        hessianL.GetProfiler().SolveMeasurements());
-      sleipnir::println(format, "∂cₑ/∂x",
-                        jacobianCe.GetProfiler().SetupDuration(),
-                        jacobianCe.GetProfiler().AverageSolveDuration(),
-                        jacobianCe.GetProfiler().SolveMeasurements());
-      sleipnir::println(format, "∂cᵢ/∂x",
-                        jacobianCi.GetProfiler().SetupDuration(),
-                        jacobianCi.GetProfiler().AverageSolveDuration(),
-                        jacobianCi.GetProfiler().SolveMeasurements());
-      sleipnir::println("");
-    }
-  }};
-
-  // Barrier parameter minimum
-  const double μ_min = config.tolerance / 10.0;
-
-  // Barrier parameter μ
-  double μ = 0.1;
-
-  // Fraction-to-the-boundary rule scale factor minimum
-  constexpr double τ_min = 0.99;
-
-  // Fraction-to-the-boundary rule scale factor τ
-  double τ = τ_min;
-
-  Filter filter{f, μ};
-
-  // This should be run when the error estimate is below a desired threshold for
-  // the current barrier parameter
-  auto UpdateBarrierParameterAndResetFilter = [&] {
-    // Barrier parameter linear decrease power in "κ_μ μ". Range of (0, 1).
-    constexpr double κ_μ = 0.2;
-
-    // Barrier parameter superlinear decrease power in "μ^(θ_μ)". Range of (1,
-    // 2).
-    constexpr double θ_μ = 1.5;
-
-    // Update the barrier parameter.
-    //
-    //   μⱼ₊₁ = max(εₜₒₗ/10, min(κ_μ μⱼ, μⱼ^θ_μ))
-    //
-    // See equation (7) of [2].
-    μ = std::max(μ_min, std::min(κ_μ * μ, std::pow(μ, θ_μ)));
-
-    // Update the fraction-to-the-boundary rule scaling factor.
-    //
-    //   τⱼ = max(τₘᵢₙ, 1 − μⱼ)
-    //
-    // See equation (8) of [2].
-    τ = std::max(τ_min, 1.0 - μ);
-
-    // Reset the filter when the barrier parameter is updated
-    filter.Reset(μ);
-  };
-
-  // Kept outside the loop so its storage can be reused
-  std::vector<Eigen::Triplet<double>> triplets;
-
-  RegularizedLDLT solver;
-
-  // Variables for determining when a step is acceptable
-  constexpr double α_red_factor = 0.5;
-  int acceptableIterCounter = 0;
-
-  int fullStepRejectedCounter = 0;
-  int stepTooSmallCounter = 0;
-
-  // Error estimate
-  double E_0 = std::numeric_limits<double>::infinity();
-
-  iterationsStartTime = std::chrono::system_clock::now();
-
-  while (E_0 > config.tolerance &&
-         acceptableIterCounter < config.maxAcceptableIterations) {
-    auto innerIterStartTime = std::chrono::system_clock::now();
-
-    // Check for local equality constraint infeasibility
-    if (IsEqualityLocallyInfeasible(A_e, c_e)) {
-      if (config.diagnostics) {
-        sleipnir::println(
-            "The problem is locally infeasible due to violated equality "
-            "constraints.");
-        sleipnir::println(
-            "Violated constraints (cₑ(x) = 0) in order of declaration:");
-        for (int row = 0; row < c_e.rows(); ++row) {
-          if (c_e(row) < 0.0) {
-            sleipnir::println("  {}/{}: {} = 0", row + 1, c_e.rows(), c_e(row));
-          }
-        }
-      }
-
-      status->exitCondition = SolverExitCondition::kLocallyInfeasible;
-      return;
-    }
-
-    // Check for local inequality constraint infeasibility
-    if (IsInequalityLocallyInfeasible(A_i, c_i)) {
-      if (config.diagnostics) {
-        sleipnir::println(
-            "The problem is infeasible due to violated inequality "
-            "constraints.");
-        sleipnir::println(
-            "Violated constraints (cᵢ(x) ≥ 0) in order of declaration:");
-        for (int row = 0; row < c_i.rows(); ++row) {
-          if (c_i(row) < 0.0) {
-            sleipnir::println("  {}/{}: {} ≥ 0", row + 1, c_i.rows(), c_i(row));
-          }
-        }
-      }
-
-      status->exitCondition = SolverExitCondition::kLocallyInfeasible;
-      return;
-    }
-
-    // Check for diverging iterates
-    if (x.lpNorm<Eigen::Infinity>() > 1e20 || !x.allFinite() ||
-        s.lpNorm<Eigen::Infinity>() > 1e20 || !s.allFinite()) {
-      status->exitCondition = SolverExitCondition::kDivergingIterates;
-      return;
-    }
-
-    // Write out spy file contents if that's enabled
-    if (config.spy) {
-      // Gap between sparsity patterns
-      if (iterations > 0) {
-        A_e_spy << "\n";
-        A_i_spy << "\n";
-        H_spy << "\n";
-      }
-
-      Spy(H_spy, H);
-      Spy(A_e_spy, A_e);
-      Spy(A_i_spy, A_i);
-    }
-
-    // Call user callback
-    if (callback({iterations, x, s, g, H, A_e, A_i})) {
-      status->exitCondition = SolverExitCondition::kCallbackRequestedStop;
-      return;
-    }
-
-    //     [s₁ 0 ⋯ 0 ]
-    // S = [0  ⋱   ⋮ ]
-    //     [⋮    ⋱ 0 ]
-    //     [0  ⋯ 0 sₘ]
-    const auto S = s.asDiagonal();
-    Eigen::SparseMatrix<double> Sinv;
-    Sinv = s.cwiseInverse().asDiagonal();
-
-    //     [z₁ 0 ⋯ 0 ]
-    // Z = [0  ⋱   ⋮ ]
-    //     [⋮    ⋱ 0 ]
-    //     [0  ⋯ 0 zₘ]
-    const auto Z = z.asDiagonal();
-    Eigen::SparseMatrix<double> Zinv;
-    Zinv = z.cwiseInverse().asDiagonal();
-
-    // Σ = S⁻¹Z
-    const Eigen::SparseMatrix<double> Σ = Sinv * Z;
-
-    // lhs = [H + AᵢᵀΣAᵢ  Aₑᵀ]
-    //       [    Aₑ       0 ]
-    //
-    // Don't assign upper triangle because solver only uses lower triangle.
-    const Eigen::SparseMatrix<double> topLeft =
-        H.triangularView<Eigen::Lower>() +
-        (A_i.transpose() * Σ * A_i).triangularView<Eigen::Lower>();
-    triplets.clear();
-    triplets.reserve(topLeft.nonZeros() + A_e.nonZeros());
-    for (int col = 0; col < H.cols(); ++col) {
-      // Append column of H + AᵢᵀΣAᵢ lower triangle in top-left quadrant
-      for (Eigen::SparseMatrix<double>::InnerIterator it{topLeft, col}; it;
-           ++it) {
-        triplets.emplace_back(it.row(), it.col(), it.value());
-      }
-      // Append column of Aₑ in bottom-left quadrant
-      for (Eigen::SparseMatrix<double>::InnerIterator it{A_e, col}; it; ++it) {
-        triplets.emplace_back(H.rows() + it.row(), it.col(), it.value());
-      }
-    }
-    Eigen::SparseMatrix<double> lhs(
-        decisionVariables.size() + equalityConstraints.size(),
-        decisionVariables.size() + equalityConstraints.size());
-    lhs.setFromSortedTriplets(triplets.begin(), triplets.end(),
-                              [](const auto& a, const auto& b) { return b; });
-
-    const Eigen::VectorXd e = Eigen::VectorXd::Ones(s.rows());
-
-    // rhs = −[∇f − Aₑᵀy + Aᵢᵀ(S⁻¹(Zcᵢ − μe) − z)]
-    //        [                cₑ                ]
-    Eigen::VectorXd rhs{x.rows() + y.rows()};
-    rhs.segment(0, x.rows()) =
-        -(g - A_e.transpose() * y +
-          A_i.transpose() * (Sinv * (Z * c_i - μ * e) - z));
-    rhs.segment(x.rows(), y.rows()) = -c_e;
-
-    // Solve the Newton-KKT system
-    solver.Compute(lhs, equalityConstraints.size(), μ);
-    Eigen::VectorXd step{x.rows() + y.rows()};
-    if (solver.Info() == Eigen::Success) {
-      step = solver.Solve(rhs);
-    } else {
-      // The regularization procedure failed due to a rank-deficient equality
-      // constraint Jacobian with linearly dependent constraints. Set the step
-      // length to zero and let second-order corrections attempt to restore
-      // feasibility.
-      step.setZero();
-    }
-
-    // step = [ pₖˣ]
-    //        [−pₖʸ]
-    Eigen::VectorXd p_x = step.segment(0, x.rows());
-    Eigen::VectorXd p_y = -step.segment(x.rows(), y.rows());
-
-    // pₖᶻ = −Σcᵢ + μS⁻¹e − ΣAᵢpₖˣ
-    Eigen::VectorXd p_z = -Σ * c_i + μ * Sinv * e - Σ * A_i * p_x;
-
-    // pₖˢ = μZ⁻¹e − s − Z⁻¹Spₖᶻ
-    Eigen::VectorXd p_s = μ * Zinv * e - s - Zinv * S * p_z;
-
-    // αᵐᵃˣ = max(α ∈ (0, 1] : sₖ + αpₖˢ ≥ (1−τⱼ)sₖ)
-    const double α_max = FractionToTheBoundaryRule(s, p_s, τ);
-    double α = α_max;
-
-    // αₖᶻ = max(α ∈ (0, 1] : zₖ + αpₖᶻ ≥ (1−τⱼ)zₖ)
-    double α_z = FractionToTheBoundaryRule(z, p_z, τ);
-
-    // Loop until a step is accepted. If a step becomes acceptable, the loop
-    // will exit early.
-    while (1) {
-      Eigen::VectorXd trial_x = x + α * p_x;
-      Eigen::VectorXd trial_y = y + α_z * p_y;
-      Eigen::VectorXd trial_z = z + α_z * p_z;
-
-      xAD.SetValue(trial_x);
-
-      f.Update();
-
-      for (int row = 0; row < c_e.rows(); ++row) {
-        c_eAD(row).Update();
-      }
-      Eigen::VectorXd trial_c_e = c_eAD.Value();
-
-      for (int row = 0; row < c_i.rows(); ++row) {
-        c_iAD(row).Update();
-      }
-      Eigen::VectorXd trial_c_i = c_iAD.Value();
-
-      // If f(xₖ + αpₖˣ), cₑ(xₖ + αpₖˣ), or cᵢ(xₖ + αpₖˣ) aren't finite, reduce
-      // step size immediately
-      if (!std::isfinite(f.Value()) || !trial_c_e.allFinite() ||
-          !trial_c_i.allFinite()) {
-        // Reduce step size
-        α *= α_red_factor;
-        continue;
-      }
-
-      Eigen::VectorXd trial_s;
-      if (config.feasibleIPM && c_i.cwiseGreater(0.0).all()) {
-        // If the inequality constraints are all feasible, prevent them from
-        // becoming infeasible again.
-        //
-        // See equation (19.30) in [1].
-        trial_s = trial_c_i;
-      } else {
-        trial_s = s + α * p_s;
-      }
-
-      // Check whether filter accepts trial iterate
-      auto entry = filter.MakeEntry(trial_s, trial_c_e, trial_c_i);
-      if (filter.TryAdd(entry)) {
-        // Accept step
-        break;
-      }
-
-      double prevConstraintViolation = c_e.lpNorm<1>() + (c_i - s).lpNorm<1>();
-      double nextConstraintViolation =
-          trial_c_e.lpNorm<1>() + (trial_c_i - trial_s).lpNorm<1>();
-
-      // Second-order corrections
-      //
-      // If first trial point was rejected and constraint violation stayed the
-      // same or went up, apply second-order corrections
-      if (nextConstraintViolation >= prevConstraintViolation) {
-        // Apply second-order corrections. See section 2.4 of [2].
-        Eigen::VectorXd p_x_cor = p_x;
-        Eigen::VectorXd p_y_soc = p_y;
-        Eigen::VectorXd p_z_soc = p_z;
-        Eigen::VectorXd p_s_soc = p_s;
-
-        double α_soc = α;
-        Eigen::VectorXd c_e_soc = c_e;
-
-        bool stepAcceptable = false;
-        for (int soc_iteration = 0; soc_iteration < 5 && !stepAcceptable;
-             ++soc_iteration) {
-          // Rebuild Newton-KKT rhs with updated constraint values.
-          //
-          // rhs = −[∇f − Aₑᵀy + Aᵢᵀ(S⁻¹(Zcᵢ − μe) − z)]
-          //        [              cₑˢᵒᶜ               ]
-          //
-          // where cₑˢᵒᶜ = αc(xₖ) + c(xₖ + αpₖˣ)
-          c_e_soc = α_soc * c_e_soc + trial_c_e;
-          rhs.bottomRows(y.rows()) = -c_e_soc;
-
-          // Solve the Newton-KKT system
-          step = solver.Solve(rhs);
-
-          p_x_cor = step.segment(0, x.rows());
-          p_y_soc = -step.segment(x.rows(), y.rows());
-
-          // pₖᶻ = −Σcᵢ + μS⁻¹e − ΣAᵢpₖˣ
-          p_z_soc = -Σ * c_i + μ * Sinv * e - Σ * A_i * p_x_cor;
-
-          // pₖˢ = μZ⁻¹e − s − Z⁻¹Spₖᶻ
-          p_s_soc = μ * Zinv * e - s - Zinv * S * p_z_soc;
-
-          // αˢᵒᶜ = max(α ∈ (0, 1] : sₖ + αpₖˢ ≥ (1−τⱼ)sₖ)
-          α_soc = FractionToTheBoundaryRule(s, p_s_soc, τ);
-          trial_x = x + α_soc * p_x_cor;
-          trial_s = s + α_soc * p_s_soc;
-
-          // αₖᶻ = max(α ∈ (0, 1] : zₖ + αpₖᶻ ≥ (1−τⱼ)zₖ)
-          double α_z_soc = FractionToTheBoundaryRule(z, p_z_soc, τ);
-          trial_y = y + α_z_soc * p_y_soc;
-          trial_z = z + α_z_soc * p_z_soc;
-
-          xAD.SetValue(trial_x);
-
-          f.Update();
-
-          for (int row = 0; row < c_e.rows(); ++row) {
-            c_eAD(row).Update();
-          }
-          trial_c_e = c_eAD.Value();
-
-          for (int row = 0; row < c_i.rows(); ++row) {
-            c_iAD(row).Update();
-          }
-          trial_c_i = c_iAD.Value();
-
-          // Check whether filter accepts trial iterate
-          entry = filter.MakeEntry(trial_s, trial_c_e, trial_c_i);
-          if (filter.TryAdd(entry)) {
-            p_x = p_x_cor;
-            p_y = p_y_soc;
-            p_z = p_z_soc;
-            p_s = p_s_soc;
-            α = α_soc;
-            α_z = α_z_soc;
-            stepAcceptable = true;
-          }
-        }
-
-        if (stepAcceptable) {
-          // Accept step
-          break;
-        }
-      }
-
-      // If we got here and α is the full step, the full step was rejected.
-      // Increment the full-step rejected counter to keep track of how many full
-      // steps have been rejected in a row.
-      if (α == α_max) {
-        ++fullStepRejectedCounter;
-      }
-
-      // If the full step was rejected enough times in a row, reset the filter
-      // because it may be impeding progress.
-      //
-      // See section 3.2 case I of [2].
-      if (fullStepRejectedCounter >= 4 &&
-          filter.maxConstraintViolation > entry.constraintViolation / 10.0) {
-        filter.maxConstraintViolation *= 0.1;
-        filter.Reset(μ);
-        continue;
-      }
-
-      // Reduce step size
-      α *= α_red_factor;
-
-      // Safety factor for the minimal step size
-      constexpr double α_min_frac = 0.05;
-
-      // If step size hit a minimum, check if the KKT error was reduced. If it
-      // wasn't, invoke feasibility restoration.
-      if (α < α_min_frac * Filter::γConstraint) {
-        double currentKKTError = KKTError(g, A_e, c_e, A_i, c_i, s, y, z, μ);
-
-        Eigen::VectorXd trial_x = x + α_max * p_x;
-        Eigen::VectorXd trial_s = s + α_max * p_s;
-
-        Eigen::VectorXd trial_y = y + α_z * p_y;
-        Eigen::VectorXd trial_z = z + α_z * p_z;
-
-        // Upate autodiff
-        xAD.SetValue(trial_x);
-        sAD.SetValue(trial_s);
-        yAD.SetValue(trial_y);
-        zAD.SetValue(trial_z);
-
-        for (int row = 0; row < c_e.rows(); ++row) {
-          c_eAD(row).Update();
-        }
-        Eigen::VectorXd trial_c_e = c_eAD.Value();
-
-        for (int row = 0; row < c_i.rows(); ++row) {
-          c_iAD(row).Update();
-        }
-        Eigen::VectorXd trial_c_i = c_iAD.Value();
-
-        double nextKKTError = KKTError(gradientF.Value(), jacobianCe.Value(),
-                                       trial_c_e, jacobianCi.Value(), trial_c_i,
-                                       trial_s, trial_y, trial_z, μ);
-
-        // If the step using αᵐᵃˣ reduced the KKT error, accept it anyway
-        if (nextKKTError <= 0.999 * currentKKTError) {
-          α = α_max;
-
-          // Accept step
-          break;
-        }
-
-        // If the step direction was bad and feasibility restoration is
-        // already running, running it again won't help
-        if (feasibilityRestoration) {
-          status->exitCondition = SolverExitCondition::kLocallyInfeasible;
-          return;
-        }
-
-        auto initialEntry = filter.MakeEntry(s, c_e, c_i);
-
-        // Feasibility restoration phase
-        Eigen::VectorXd fr_x = x;
-        Eigen::VectorXd fr_s = s;
-        SolverStatus fr_status;
-        FeasibilityRestoration(
-            decisionVariables, equalityConstraints, inequalityConstraints, f, μ,
-            [&](const SolverIterationInfo& info) {
-              Eigen::VectorXd trial_x =
-                  info.x.segment(0, decisionVariables.size());
-              xAD.SetValue(trial_x);
-
-              Eigen::VectorXd trial_s =
-                  info.s.segment(0, inequalityConstraints.size());
-              sAD.SetValue(trial_s);
-
-              for (int row = 0; row < c_e.rows(); ++row) {
-                c_eAD(row).Update();
-              }
-              Eigen::VectorXd trial_c_e = c_eAD.Value();
-
-              for (int row = 0; row < c_i.rows(); ++row) {
-                c_iAD(row).Update();
-              }
-              Eigen::VectorXd trial_c_i = c_iAD.Value();
-
-              for (int row = 0; row < c_i.rows(); ++row) {
-                c_iAD(row).Update();
-              }
-
-              f.Update();
-
-              // If current iterate is acceptable to normal filter and
-              // constraint violation has sufficiently reduced, stop
-              // feasibility restoration
-              auto entry = filter.MakeEntry(trial_s, trial_c_e, trial_c_i);
-              if (filter.IsAcceptable(entry) &&
-                  entry.constraintViolation <
-                      0.9 * initialEntry.constraintViolation) {
-                return true;
-              }
-
-              return false;
-            },
-            config, fr_x, fr_s, &fr_status);
-
-        if (fr_status.exitCondition ==
-            SolverExitCondition::kCallbackRequestedStop) {
-          p_x = fr_x - x;
-          p_s = fr_s - s;
-
-          // Lagrange mutliplier estimates
-          //
-          //   [y] = (ÂÂᵀ)⁻¹Â[ ∇f]
-          //   [z]           [−μe]
-          //
-          //   where Â = [Aₑ   0]
-          //             [Aᵢ  −S]
-          //
-          // See equation (19.37) of [1].
-          {
-            xAD.SetValue(fr_x);
-            sAD.SetValue(c_iAD.Value());
-
-            A_e = jacobianCe.Value();
-            A_i = jacobianCi.Value();
-            g = gradientF.Value();
-
-            // Â = [Aₑ   0]
-            //     [Aᵢ  −S]
-            triplets.clear();
-            triplets.reserve(A_e.nonZeros() + A_i.nonZeros() + s.rows());
-            for (int col = 0; col < A_e.cols(); ++col) {
-              // Append column of Aₑ in top-left quadrant
-              for (Eigen::SparseMatrix<double>::InnerIterator it{A_e, col}; it;
-                   ++it) {
-                triplets.emplace_back(it.row(), it.col(), it.value());
-              }
-              // Append column of Aᵢ in bottom-left quadrant
-              for (Eigen::SparseMatrix<double>::InnerIterator it{A_i, col}; it;
-                   ++it) {
-                triplets.emplace_back(A_e.rows() + it.row(), it.col(),
-                                      it.value());
-              }
-            }
-            // Append −S in bottom-right quadrant
-            for (int i = 0; i < s.rows(); ++i) {
-              triplets.emplace_back(A_e.rows() + i, A_e.cols() + i, -s(i));
-            }
-            Eigen::SparseMatrix<double> Ahat{A_e.rows() + A_i.rows(),
-                                             A_e.cols() + s.rows()};
-            Ahat.setFromSortedTriplets(
-                triplets.begin(), triplets.end(),
-                [](const auto& a, const auto& b) { return b; });
-
-            // lhs = ÂÂᵀ
-            Eigen::SparseMatrix<double> lhs = Ahat * Ahat.transpose();
-
-            // rhs = Â[ ∇f]
-            //        [−μe]
-            Eigen::VectorXd rhsTemp{g.rows() + e.rows()};
-            rhsTemp.block(0, 0, g.rows(), 1) = g;
-            rhsTemp.block(g.rows(), 0, s.rows(), 1) = -μ * e;
-            Eigen::VectorXd rhs = Ahat * rhsTemp;
-
-            Eigen::SimplicialLDLT<Eigen::SparseMatrix<double>> yzEstimator{lhs};
-            Eigen::VectorXd sol = yzEstimator.solve(rhs);
-
-            p_y = y - sol.block(0, 0, y.rows(), 1);
-            p_z = z - sol.block(y.rows(), 0, z.rows(), 1);
-          }
-
-          α = 1.0;
-          α_z = 1.0;
-
-          // Accept step
-          break;
-        } else if (fr_status.exitCondition == SolverExitCondition::kSuccess) {
-          status->exitCondition = SolverExitCondition::kLocallyInfeasible;
-          x = fr_x;
-          return;
-        } else {
-          status->exitCondition =
-              SolverExitCondition::kFeasibilityRestorationFailed;
-          x = fr_x;
-          return;
-        }
-      }
-    }
-
-    // If full step was accepted, reset full-step rejected counter
-    if (α == α_max) {
-      fullStepRejectedCounter = 0;
-    }
-
-    // Handle very small search directions by letting αₖ = αₖᵐᵃˣ when
-    // max(|pₖˣ(i)|/(1 + |xₖ(i)|)) < 10ε_mach.
-    //
-    // See section 3.9 of [2].
-    double maxStepScaled = 0.0;
-    for (int row = 0; row < x.rows(); ++row) {
-      maxStepScaled = std::max(maxStepScaled,
-                               std::abs(p_x(row)) / (1.0 + std::abs(x(row))));
-    }
-    if (maxStepScaled < 10.0 * std::numeric_limits<double>::epsilon()) {
-      α = α_max;
-      ++stepTooSmallCounter;
-    } else {
-      stepTooSmallCounter = 0;
-    }
-
-    // xₖ₊₁ = xₖ + αₖpₖˣ
-    // sₖ₊₁ = sₖ + αₖpₖˢ
-    // yₖ₊₁ = yₖ + αₖᶻpₖʸ
-    // zₖ₊₁ = zₖ + αₖᶻpₖᶻ
-    x += α * p_x;
-    s += α * p_s;
-    y += α_z * p_y;
-    z += α_z * p_z;
-
-    // A requirement for the convergence proof is that the "primal-dual barrier
-    // term Hessian" Σₖ does not deviate arbitrarily much from the "primal
-    // Hessian" μⱼSₖ⁻². We ensure this by resetting
-    //
-    //   zₖ₊₁⁽ⁱ⁾ = max(min(zₖ₊₁⁽ⁱ⁾, κ_Σ μⱼ/sₖ₊₁⁽ⁱ⁾), μⱼ/(κ_Σ sₖ₊₁⁽ⁱ⁾))
-    //
-    // for some fixed κ_Σ ≥ 1 after each step. See equation (16) of [2].
-    {
-      // Barrier parameter scale factor for inequality constraint Lagrange
-      // multiplier safeguard
-      constexpr double κ_Σ = 1e10;
-
-      for (int row = 0; row < z.rows(); ++row) {
-        z(row) =
-            std::max(std::min(z(row), κ_Σ * μ / s(row)), μ / (κ_Σ * s(row)));
-      }
-    }
-
-    // Update autodiff for Jacobians and Hessian
-    xAD.SetValue(x);
-    sAD.SetValue(s);
-    yAD.SetValue(y);
-    zAD.SetValue(z);
-    A_e = jacobianCe.Value();
-    A_i = jacobianCi.Value();
-    g = gradientF.Value();
-    H = hessianL.Value();
-
-    // Update cₑ
-    for (int row = 0; row < c_e.rows(); ++row) {
-      c_eAD(row).Update();
-    }
-    c_e = c_eAD.Value();
-
-    // Update cᵢ
-    for (int row = 0; row < c_i.rows(); ++row) {
-      c_iAD(row).Update();
-    }
-    c_i = c_iAD.Value();
-
-    // Update the error estimate
-    E_0 = ErrorEstimate(g, A_e, c_e, A_i, c_i, s, y, z, 0.0);
-    if (E_0 < config.acceptableTolerance) {
-      ++acceptableIterCounter;
-    } else {
-      acceptableIterCounter = 0;
-    }
-
-    // Update the barrier parameter if necessary
-    if (E_0 > config.tolerance) {
-      // Barrier parameter scale factor for tolerance checks
-      constexpr double κ_ε = 10.0;
-
-      // While the error estimate is below the desired threshold for this
-      // barrier parameter value, decrease the barrier parameter further
-      double E_μ = ErrorEstimate(g, A_e, c_e, A_i, c_i, s, y, z, μ);
-      while (μ > μ_min && E_μ <= κ_ε * μ) {
-        UpdateBarrierParameterAndResetFilter();
-        E_μ = ErrorEstimate(g, A_e, c_e, A_i, c_i, s, y, z, μ);
-      }
-    }
-
-    const auto innerIterEndTime = std::chrono::system_clock::now();
-
-    // Diagnostics for current iteration
-    if (config.diagnostics) {
-      if (iterations % 20 == 0) {
-        sleipnir::println("{:^4}   {:^9}  {:^13}  {:^13}  {:^13}", "iter",
-                          "time (ms)", "error", "cost", "infeasibility");
-        sleipnir::println("{:=^61}", "");
-      }
-
-      sleipnir::println("{:4}{}  {:9.3f}  {:13e}  {:13e}  {:13e}", iterations,
-                        feasibilityRestoration ? "r" : " ",
-                        ToMilliseconds(innerIterEndTime - innerIterStartTime),
-                        E_0, f.Value(),
-                        c_e.lpNorm<1>() + (c_i - s).lpNorm<1>());
-    }
-
-    ++iterations;
-
-    // Check for max iterations
-    if (iterations >= config.maxIterations) {
-      status->exitCondition = SolverExitCondition::kMaxIterationsExceeded;
-      return;
-    }
-
-    // Check for max wall clock time
-    if (innerIterEndTime - solveStartTime > config.timeout) {
-      status->exitCondition = SolverExitCondition::kTimeout;
-      return;
-    }
-
-    // Check for solve to acceptable tolerance
-    if (E_0 > config.tolerance &&
-        acceptableIterCounter == config.maxAcceptableIterations) {
-      status->exitCondition = SolverExitCondition::kSolvedToAcceptableTolerance;
-      return;
-    }
-
-    // The search direction has been very small twice, so assume the problem has
-    // been solved as well as possible given finite precision and reduce the
-    // barrier parameter.
-    //
-    // See section 3.9 of [2].
-    if (stepTooSmallCounter >= 2 && μ > μ_min) {
-      UpdateBarrierParameterAndResetFilter();
-      continue;
-    }
-  }
-}  // NOLINT(readability/fn_size)
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#include "sleipnir/optimization/solver/InteriorPoint.hpp"
+
+#include <algorithm>
+#include <chrono>
+#include <cmath>
+#include <fstream>
+#include <limits>
+#include <vector>
+
+#include <Eigen/SparseCholesky>
+
+#include "optimization/RegularizedLDLT.hpp"
+#include "optimization/solver/util/ErrorEstimate.hpp"
+#include "optimization/solver/util/FeasibilityRestoration.hpp"
+#include "optimization/solver/util/Filter.hpp"
+#include "optimization/solver/util/FractionToTheBoundaryRule.hpp"
+#include "optimization/solver/util/IsLocallyInfeasible.hpp"
+#include "optimization/solver/util/KKTError.hpp"
+#include "sleipnir/autodiff/Gradient.hpp"
+#include "sleipnir/autodiff/Hessian.hpp"
+#include "sleipnir/autodiff/Jacobian.hpp"
+#include "sleipnir/optimization/SolverExitCondition.hpp"
+#include "sleipnir/util/Print.hpp"
+#include "sleipnir/util/Spy.hpp"
+#include "util/ScopeExit.hpp"
+#include "util/ToMilliseconds.hpp"
+
+// See docs/algorithms.md#Works_cited for citation definitions.
+//
+// See docs/algorithms.md#Interior-point_method for a derivation of the
+// interior-point method formulation being used.
+
+namespace sleipnir {
+
+void InteriorPoint(
+    std::span<Variable> decisionVariables,
+    std::span<Variable> equalityConstraints,
+    std::span<Variable> inequalityConstraints, Variable& f,
+    const std::function<bool(const SolverIterationInfo&)>& callback,
+    const SolverConfig& config, bool feasibilityRestoration, Eigen::VectorXd& x,
+    Eigen::VectorXd& s, SolverStatus* status) {
+  const auto solveStartTime = std::chrono::system_clock::now();
+
+  // Map decision variables and constraints to VariableMatrices for Lagrangian
+  VariableMatrix xAD{decisionVariables};
+  xAD.SetValue(x);
+  VariableMatrix c_eAD{equalityConstraints};
+  VariableMatrix c_iAD{inequalityConstraints};
+
+  // Create autodiff variables for s, y, and z for Lagrangian
+  VariableMatrix sAD(inequalityConstraints.size());
+  sAD.SetValue(s);
+  VariableMatrix yAD(equalityConstraints.size());
+  for (auto& y : yAD) {
+    y.SetValue(0.0);
+  }
+  VariableMatrix zAD(inequalityConstraints.size());
+  for (auto& z : zAD) {
+    z.SetValue(1.0);
+  }
+
+  // Lagrangian L
+  //
+  // L(xₖ, sₖ, yₖ, zₖ) = f(xₖ) − yₖᵀcₑ(xₖ) − zₖᵀ(cᵢ(xₖ) − sₖ)
+  auto L = f - (yAD.T() * c_eAD)(0) - (zAD.T() * (c_iAD - sAD))(0);
+
+  // Equality constraint Jacobian Aₑ
+  //
+  //         [∇ᵀcₑ₁(xₖ)]
+  // Aₑ(x) = [∇ᵀcₑ₂(xₖ)]
+  //         [    ⋮    ]
+  //         [∇ᵀcₑₘ(xₖ)]
+  Jacobian jacobianCe{c_eAD, xAD};
+  Eigen::SparseMatrix<double> A_e = jacobianCe.Value();
+
+  // Inequality constraint Jacobian Aᵢ
+  //
+  //         [∇ᵀcᵢ₁(xₖ)]
+  // Aᵢ(x) = [∇ᵀcᵢ₂(xₖ)]
+  //         [    ⋮    ]
+  //         [∇ᵀcᵢₘ(xₖ)]
+  Jacobian jacobianCi{c_iAD, xAD};
+  Eigen::SparseMatrix<double> A_i = jacobianCi.Value();
+
+  // Gradient of f ∇f
+  Gradient gradientF{f, xAD};
+  Eigen::SparseVector<double> g = gradientF.Value();
+
+  // Hessian of the Lagrangian H
+  //
+  // Hₖ = ∇²ₓₓL(xₖ, sₖ, yₖ, zₖ)
+  Hessian hessianL{L, xAD};
+  Eigen::SparseMatrix<double> H = hessianL.Value();
+
+  Eigen::VectorXd y = yAD.Value();
+  Eigen::VectorXd z = zAD.Value();
+  Eigen::VectorXd c_e = c_eAD.Value();
+  Eigen::VectorXd c_i = c_iAD.Value();
+
+  // Check for overconstrained problem
+  if (equalityConstraints.size() > decisionVariables.size()) {
+    if (config.diagnostics) {
+      sleipnir::println("The problem has too few degrees of freedom.");
+      sleipnir::println(
+          "Violated constraints (cₑ(x) = 0) in order of declaration:");
+      for (int row = 0; row < c_e.rows(); ++row) {
+        if (c_e(row) < 0.0) {
+          sleipnir::println("  {}/{}: {} = 0", row + 1, c_e.rows(), c_e(row));
+        }
+      }
+    }
+
+    status->exitCondition = SolverExitCondition::kTooFewDOFs;
+    return;
+  }
+
+  // Check whether initial guess has finite f(xₖ), cₑ(xₖ), and cᵢ(xₖ)
+  if (!std::isfinite(f.Value()) || !c_e.allFinite() || !c_i.allFinite()) {
+    status->exitCondition =
+        SolverExitCondition::kNonfiniteInitialCostOrConstraints;
+    return;
+  }
+
+  // Sparsity pattern files written when spy flag is set in SolverConfig
+  std::ofstream H_spy;
+  std::ofstream A_e_spy;
+  std::ofstream A_i_spy;
+  if (config.spy) {
+    A_e_spy.open("A_e.spy");
+    A_i_spy.open("A_i.spy");
+    H_spy.open("H.spy");
+  }
+
+  if (config.diagnostics && !feasibilityRestoration) {
+    sleipnir::println("Error tolerance: {}\n", config.tolerance);
+  }
+
+  std::chrono::system_clock::time_point iterationsStartTime;
+
+  int iterations = 0;
+
+  // Prints final diagnostics when the solver exits
+  scope_exit exit{[&] {
+    if (config.diagnostics && !feasibilityRestoration) {
+      auto solveEndTime = std::chrono::system_clock::now();
+
+      sleipnir::println("\nSolve time: {:.3f} ms",
+                        ToMilliseconds(solveEndTime - solveStartTime));
+      sleipnir::println("  ↳ {:.3f} ms (solver setup)",
+                        ToMilliseconds(iterationsStartTime - solveStartTime));
+      if (iterations > 0) {
+        sleipnir::println(
+            "  ↳ {:.3f} ms ({} solver iterations; {:.3f} ms average)",
+            ToMilliseconds(solveEndTime - iterationsStartTime), iterations,
+            ToMilliseconds((solveEndTime - iterationsStartTime) / iterations));
+      }
+      sleipnir::println("");
+
+      sleipnir::println("{:^8}   {:^10}   {:^14}   {:^6}", "autodiff",
+                        "setup (ms)", "avg solve (ms)", "solves");
+      sleipnir::println("{:=^47}", "");
+      constexpr auto format = "{:^8}   {:10.3f}   {:14.3f}   {:6}";
+      sleipnir::println(format, "∇f(x)",
+                        gradientF.GetProfiler().SetupDuration(),
+                        gradientF.GetProfiler().AverageSolveDuration(),
+                        gradientF.GetProfiler().SolveMeasurements());
+      sleipnir::println(format, "∇²ₓₓL", hessianL.GetProfiler().SetupDuration(),
+                        hessianL.GetProfiler().AverageSolveDuration(),
+                        hessianL.GetProfiler().SolveMeasurements());
+      sleipnir::println(format, "∂cₑ/∂x",
+                        jacobianCe.GetProfiler().SetupDuration(),
+                        jacobianCe.GetProfiler().AverageSolveDuration(),
+                        jacobianCe.GetProfiler().SolveMeasurements());
+      sleipnir::println(format, "∂cᵢ/∂x",
+                        jacobianCi.GetProfiler().SetupDuration(),
+                        jacobianCi.GetProfiler().AverageSolveDuration(),
+                        jacobianCi.GetProfiler().SolveMeasurements());
+      sleipnir::println("");
+    }
+  }};
+
+  // Barrier parameter minimum
+  const double μ_min = config.tolerance / 10.0;
+
+  // Barrier parameter μ
+  double μ = 0.1;
+
+  // Fraction-to-the-boundary rule scale factor minimum
+  constexpr double τ_min = 0.99;
+
+  // Fraction-to-the-boundary rule scale factor τ
+  double τ = τ_min;
+
+  Filter filter{f, μ};
+
+  // This should be run when the error estimate is below a desired threshold for
+  // the current barrier parameter
+  auto UpdateBarrierParameterAndResetFilter = [&] {
+    // Barrier parameter linear decrease power in "κ_μ μ". Range of (0, 1).
+    constexpr double κ_μ = 0.2;
+
+    // Barrier parameter superlinear decrease power in "μ^(θ_μ)". Range of (1,
+    // 2).
+    constexpr double θ_μ = 1.5;
+
+    // Update the barrier parameter.
+    //
+    //   μⱼ₊₁ = max(εₜₒₗ/10, min(κ_μ μⱼ, μⱼ^θ_μ))
+    //
+    // See equation (7) of [2].
+    μ = std::max(μ_min, std::min(κ_μ * μ, std::pow(μ, θ_μ)));
+
+    // Update the fraction-to-the-boundary rule scaling factor.
+    //
+    //   τⱼ = max(τₘᵢₙ, 1 − μⱼ)
+    //
+    // See equation (8) of [2].
+    τ = std::max(τ_min, 1.0 - μ);
+
+    // Reset the filter when the barrier parameter is updated
+    filter.Reset(μ);
+  };
+
+  // Kept outside the loop so its storage can be reused
+  std::vector<Eigen::Triplet<double>> triplets;
+
+  RegularizedLDLT solver;
+
+  // Variables for determining when a step is acceptable
+  constexpr double α_red_factor = 0.5;
+  int acceptableIterCounter = 0;
+
+  int fullStepRejectedCounter = 0;
+  int stepTooSmallCounter = 0;
+
+  // Error estimate
+  double E_0 = std::numeric_limits<double>::infinity();
+
+  iterationsStartTime = std::chrono::system_clock::now();
+
+  while (E_0 > config.tolerance &&
+         acceptableIterCounter < config.maxAcceptableIterations) {
+    auto innerIterStartTime = std::chrono::system_clock::now();
+
+    // Check for local equality constraint infeasibility
+    if (IsEqualityLocallyInfeasible(A_e, c_e)) {
+      if (config.diagnostics) {
+        sleipnir::println(
+            "The problem is locally infeasible due to violated equality "
+            "constraints.");
+        sleipnir::println(
+            "Violated constraints (cₑ(x) = 0) in order of declaration:");
+        for (int row = 0; row < c_e.rows(); ++row) {
+          if (c_e(row) < 0.0) {
+            sleipnir::println("  {}/{}: {} = 0", row + 1, c_e.rows(), c_e(row));
+          }
+        }
+      }
+
+      status->exitCondition = SolverExitCondition::kLocallyInfeasible;
+      return;
+    }
+
+    // Check for local inequality constraint infeasibility
+    if (IsInequalityLocallyInfeasible(A_i, c_i)) {
+      if (config.diagnostics) {
+        sleipnir::println(
+            "The problem is infeasible due to violated inequality "
+            "constraints.");
+        sleipnir::println(
+            "Violated constraints (cᵢ(x) ≥ 0) in order of declaration:");
+        for (int row = 0; row < c_i.rows(); ++row) {
+          if (c_i(row) < 0.0) {
+            sleipnir::println("  {}/{}: {} ≥ 0", row + 1, c_i.rows(), c_i(row));
+          }
+        }
+      }
+
+      status->exitCondition = SolverExitCondition::kLocallyInfeasible;
+      return;
+    }
+
+    // Check for diverging iterates
+    if (x.lpNorm<Eigen::Infinity>() > 1e20 || !x.allFinite() ||
+        s.lpNorm<Eigen::Infinity>() > 1e20 || !s.allFinite()) {
+      status->exitCondition = SolverExitCondition::kDivergingIterates;
+      return;
+    }
+
+    // Write out spy file contents if that's enabled
+    if (config.spy) {
+      // Gap between sparsity patterns
+      if (iterations > 0) {
+        A_e_spy << "\n";
+        A_i_spy << "\n";
+        H_spy << "\n";
+      }
+
+      Spy(H_spy, H);
+      Spy(A_e_spy, A_e);
+      Spy(A_i_spy, A_i);
+    }
+
+    // Call user callback
+    if (callback({iterations, x, s, g, H, A_e, A_i})) {
+      status->exitCondition = SolverExitCondition::kCallbackRequestedStop;
+      return;
+    }
+
+    //     [s₁ 0 ⋯ 0 ]
+    // S = [0  ⋱   ⋮ ]
+    //     [⋮    ⋱ 0 ]
+    //     [0  ⋯ 0 sₘ]
+    const auto S = s.asDiagonal();
+    Eigen::SparseMatrix<double> Sinv;
+    Sinv = s.cwiseInverse().asDiagonal();
+
+    //     [z₁ 0 ⋯ 0 ]
+    // Z = [0  ⋱   ⋮ ]
+    //     [⋮    ⋱ 0 ]
+    //     [0  ⋯ 0 zₘ]
+    const auto Z = z.asDiagonal();
+    Eigen::SparseMatrix<double> Zinv;
+    Zinv = z.cwiseInverse().asDiagonal();
+
+    // Σ = S⁻¹Z
+    const Eigen::SparseMatrix<double> Σ = Sinv * Z;
+
+    // lhs = [H + AᵢᵀΣAᵢ  Aₑᵀ]
+    //       [    Aₑ       0 ]
+    //
+    // Don't assign upper triangle because solver only uses lower triangle.
+    const Eigen::SparseMatrix<double> topLeft =
+        H.triangularView<Eigen::Lower>() +
+        (A_i.transpose() * Σ * A_i).triangularView<Eigen::Lower>();
+    triplets.clear();
+    triplets.reserve(topLeft.nonZeros() + A_e.nonZeros());
+    for (int col = 0; col < H.cols(); ++col) {
+      // Append column of H + AᵢᵀΣAᵢ lower triangle in top-left quadrant
+      for (Eigen::SparseMatrix<double>::InnerIterator it{topLeft, col}; it;
+           ++it) {
+        triplets.emplace_back(it.row(), it.col(), it.value());
+      }
+      // Append column of Aₑ in bottom-left quadrant
+      for (Eigen::SparseMatrix<double>::InnerIterator it{A_e, col}; it; ++it) {
+        triplets.emplace_back(H.rows() + it.row(), it.col(), it.value());
+      }
+    }
+    Eigen::SparseMatrix<double> lhs(
+        decisionVariables.size() + equalityConstraints.size(),
+        decisionVariables.size() + equalityConstraints.size());
+    lhs.setFromSortedTriplets(triplets.begin(), triplets.end(),
+                              [](const auto& a, const auto& b) { return b; });
+
+    const Eigen::VectorXd e = Eigen::VectorXd::Ones(s.rows());
+
+    // rhs = −[∇f − Aₑᵀy + Aᵢᵀ(S⁻¹(Zcᵢ − μe) − z)]
+    //        [                cₑ                ]
+    Eigen::VectorXd rhs{x.rows() + y.rows()};
+    rhs.segment(0, x.rows()) =
+        -(g - A_e.transpose() * y +
+          A_i.transpose() * (Sinv * (Z * c_i - μ * e) - z));
+    rhs.segment(x.rows(), y.rows()) = -c_e;
+
+    // Solve the Newton-KKT system
+    solver.Compute(lhs, equalityConstraints.size(), μ);
+    Eigen::VectorXd step{x.rows() + y.rows()};
+    if (solver.Info() == Eigen::Success) {
+      step = solver.Solve(rhs);
+    } else {
+      // The regularization procedure failed due to a rank-deficient equality
+      // constraint Jacobian with linearly dependent constraints. Set the step
+      // length to zero and let second-order corrections attempt to restore
+      // feasibility.
+      step.setZero();
+    }
+
+    // step = [ pₖˣ]
+    //        [−pₖʸ]
+    Eigen::VectorXd p_x = step.segment(0, x.rows());
+    Eigen::VectorXd p_y = -step.segment(x.rows(), y.rows());
+
+    // pₖᶻ = −Σcᵢ + μS⁻¹e − ΣAᵢpₖˣ
+    Eigen::VectorXd p_z = -Σ * c_i + μ * Sinv * e - Σ * A_i * p_x;
+
+    // pₖˢ = μZ⁻¹e − s − Z⁻¹Spₖᶻ
+    Eigen::VectorXd p_s = μ * Zinv * e - s - Zinv * S * p_z;
+
+    // αᵐᵃˣ = max(α ∈ (0, 1] : sₖ + αpₖˢ ≥ (1−τⱼ)sₖ)
+    const double α_max = FractionToTheBoundaryRule(s, p_s, τ);
+    double α = α_max;
+
+    // αₖᶻ = max(α ∈ (0, 1] : zₖ + αpₖᶻ ≥ (1−τⱼ)zₖ)
+    double α_z = FractionToTheBoundaryRule(z, p_z, τ);
+
+    // Loop until a step is accepted. If a step becomes acceptable, the loop
+    // will exit early.
+    while (1) {
+      Eigen::VectorXd trial_x = x + α * p_x;
+      Eigen::VectorXd trial_y = y + α_z * p_y;
+      Eigen::VectorXd trial_z = z + α_z * p_z;
+
+      xAD.SetValue(trial_x);
+
+      f.Update();
+
+      for (int row = 0; row < c_e.rows(); ++row) {
+        c_eAD(row).Update();
+      }
+      Eigen::VectorXd trial_c_e = c_eAD.Value();
+
+      for (int row = 0; row < c_i.rows(); ++row) {
+        c_iAD(row).Update();
+      }
+      Eigen::VectorXd trial_c_i = c_iAD.Value();
+
+      // If f(xₖ + αpₖˣ), cₑ(xₖ + αpₖˣ), or cᵢ(xₖ + αpₖˣ) aren't finite, reduce
+      // step size immediately
+      if (!std::isfinite(f.Value()) || !trial_c_e.allFinite() ||
+          !trial_c_i.allFinite()) {
+        // Reduce step size
+        α *= α_red_factor;
+        continue;
+      }
+
+      Eigen::VectorXd trial_s;
+      if (config.feasibleIPM && c_i.cwiseGreater(0.0).all()) {
+        // If the inequality constraints are all feasible, prevent them from
+        // becoming infeasible again.
+        //
+        // See equation (19.30) in [1].
+        trial_s = trial_c_i;
+      } else {
+        trial_s = s + α * p_s;
+      }
+
+      // Check whether filter accepts trial iterate
+      auto entry = filter.MakeEntry(trial_s, trial_c_e, trial_c_i);
+      if (filter.TryAdd(entry)) {
+        // Accept step
+        break;
+      }
+
+      double prevConstraintViolation = c_e.lpNorm<1>() + (c_i - s).lpNorm<1>();
+      double nextConstraintViolation =
+          trial_c_e.lpNorm<1>() + (trial_c_i - trial_s).lpNorm<1>();
+
+      // Second-order corrections
+      //
+      // If first trial point was rejected and constraint violation stayed the
+      // same or went up, apply second-order corrections
+      if (nextConstraintViolation >= prevConstraintViolation) {
+        // Apply second-order corrections. See section 2.4 of [2].
+        Eigen::VectorXd p_x_cor = p_x;
+        Eigen::VectorXd p_y_soc = p_y;
+        Eigen::VectorXd p_z_soc = p_z;
+        Eigen::VectorXd p_s_soc = p_s;
+
+        double α_soc = α;
+        Eigen::VectorXd c_e_soc = c_e;
+
+        bool stepAcceptable = false;
+        for (int soc_iteration = 0; soc_iteration < 5 && !stepAcceptable;
+             ++soc_iteration) {
+          // Rebuild Newton-KKT rhs with updated constraint values.
+          //
+          // rhs = −[∇f − Aₑᵀy + Aᵢᵀ(S⁻¹(Zcᵢ − μe) − z)]
+          //        [              cₑˢᵒᶜ               ]
+          //
+          // where cₑˢᵒᶜ = αc(xₖ) + c(xₖ + αpₖˣ)
+          c_e_soc = α_soc * c_e_soc + trial_c_e;
+          rhs.bottomRows(y.rows()) = -c_e_soc;
+
+          // Solve the Newton-KKT system
+          step = solver.Solve(rhs);
+
+          p_x_cor = step.segment(0, x.rows());
+          p_y_soc = -step.segment(x.rows(), y.rows());
+
+          // pₖᶻ = −Σcᵢ + μS⁻¹e − ΣAᵢpₖˣ
+          p_z_soc = -Σ * c_i + μ * Sinv * e - Σ * A_i * p_x_cor;
+
+          // pₖˢ = μZ⁻¹e − s − Z⁻¹Spₖᶻ
+          p_s_soc = μ * Zinv * e - s - Zinv * S * p_z_soc;
+
+          // αˢᵒᶜ = max(α ∈ (0, 1] : sₖ + αpₖˢ ≥ (1−τⱼ)sₖ)
+          α_soc = FractionToTheBoundaryRule(s, p_s_soc, τ);
+          trial_x = x + α_soc * p_x_cor;
+          trial_s = s + α_soc * p_s_soc;
+
+          // αₖᶻ = max(α ∈ (0, 1] : zₖ + αpₖᶻ ≥ (1−τⱼ)zₖ)
+          double α_z_soc = FractionToTheBoundaryRule(z, p_z_soc, τ);
+          trial_y = y + α_z_soc * p_y_soc;
+          trial_z = z + α_z_soc * p_z_soc;
+
+          xAD.SetValue(trial_x);
+
+          f.Update();
+
+          for (int row = 0; row < c_e.rows(); ++row) {
+            c_eAD(row).Update();
+          }
+          trial_c_e = c_eAD.Value();
+
+          for (int row = 0; row < c_i.rows(); ++row) {
+            c_iAD(row).Update();
+          }
+          trial_c_i = c_iAD.Value();
+
+          // Check whether filter accepts trial iterate
+          entry = filter.MakeEntry(trial_s, trial_c_e, trial_c_i);
+          if (filter.TryAdd(entry)) {
+            p_x = p_x_cor;
+            p_y = p_y_soc;
+            p_z = p_z_soc;
+            p_s = p_s_soc;
+            α = α_soc;
+            α_z = α_z_soc;
+            stepAcceptable = true;
+          }
+        }
+
+        if (stepAcceptable) {
+          // Accept step
+          break;
+        }
+      }
+
+      // If we got here and α is the full step, the full step was rejected.
+      // Increment the full-step rejected counter to keep track of how many full
+      // steps have been rejected in a row.
+      if (α == α_max) {
+        ++fullStepRejectedCounter;
+      }
+
+      // If the full step was rejected enough times in a row, reset the filter
+      // because it may be impeding progress.
+      //
+      // See section 3.2 case I of [2].
+      if (fullStepRejectedCounter >= 4 &&
+          filter.maxConstraintViolation > entry.constraintViolation / 10.0) {
+        filter.maxConstraintViolation *= 0.1;
+        filter.Reset(μ);
+        continue;
+      }
+
+      // Reduce step size
+      α *= α_red_factor;
+
+      // Safety factor for the minimal step size
+      constexpr double α_min_frac = 0.05;
+
+      // If step size hit a minimum, check if the KKT error was reduced. If it
+      // wasn't, invoke feasibility restoration.
+      if (α < α_min_frac * Filter::γConstraint) {
+        double currentKKTError = KKTError(g, A_e, c_e, A_i, c_i, s, y, z, μ);
+
+        Eigen::VectorXd trial_x = x + α_max * p_x;
+        Eigen::VectorXd trial_s = s + α_max * p_s;
+
+        Eigen::VectorXd trial_y = y + α_z * p_y;
+        Eigen::VectorXd trial_z = z + α_z * p_z;
+
+        // Upate autodiff
+        xAD.SetValue(trial_x);
+        sAD.SetValue(trial_s);
+        yAD.SetValue(trial_y);
+        zAD.SetValue(trial_z);
+
+        for (int row = 0; row < c_e.rows(); ++row) {
+          c_eAD(row).Update();
+        }
+        Eigen::VectorXd trial_c_e = c_eAD.Value();
+
+        for (int row = 0; row < c_i.rows(); ++row) {
+          c_iAD(row).Update();
+        }
+        Eigen::VectorXd trial_c_i = c_iAD.Value();
+
+        double nextKKTError = KKTError(gradientF.Value(), jacobianCe.Value(),
+                                       trial_c_e, jacobianCi.Value(), trial_c_i,
+                                       trial_s, trial_y, trial_z, μ);
+
+        // If the step using αᵐᵃˣ reduced the KKT error, accept it anyway
+        if (nextKKTError <= 0.999 * currentKKTError) {
+          α = α_max;
+
+          // Accept step
+          break;
+        }
+
+        // If the step direction was bad and feasibility restoration is
+        // already running, running it again won't help
+        if (feasibilityRestoration) {
+          status->exitCondition = SolverExitCondition::kLocallyInfeasible;
+          return;
+        }
+
+        auto initialEntry = filter.MakeEntry(s, c_e, c_i);
+
+        // Feasibility restoration phase
+        Eigen::VectorXd fr_x = x;
+        Eigen::VectorXd fr_s = s;
+        SolverStatus fr_status;
+        FeasibilityRestoration(
+            decisionVariables, equalityConstraints, inequalityConstraints, f, μ,
+            [&](const SolverIterationInfo& info) {
+              Eigen::VectorXd trial_x =
+                  info.x.segment(0, decisionVariables.size());
+              xAD.SetValue(trial_x);
+
+              Eigen::VectorXd trial_s =
+                  info.s.segment(0, inequalityConstraints.size());
+              sAD.SetValue(trial_s);
+
+              for (int row = 0; row < c_e.rows(); ++row) {
+                c_eAD(row).Update();
+              }
+              Eigen::VectorXd trial_c_e = c_eAD.Value();
+
+              for (int row = 0; row < c_i.rows(); ++row) {
+                c_iAD(row).Update();
+              }
+              Eigen::VectorXd trial_c_i = c_iAD.Value();
+
+              for (int row = 0; row < c_i.rows(); ++row) {
+                c_iAD(row).Update();
+              }
+
+              f.Update();
+
+              // If current iterate is acceptable to normal filter and
+              // constraint violation has sufficiently reduced, stop
+              // feasibility restoration
+              auto entry = filter.MakeEntry(trial_s, trial_c_e, trial_c_i);
+              if (filter.IsAcceptable(entry) &&
+                  entry.constraintViolation <
+                      0.9 * initialEntry.constraintViolation) {
+                return true;
+              }
+
+              return false;
+            },
+            config, fr_x, fr_s, &fr_status);
+
+        if (fr_status.exitCondition ==
+            SolverExitCondition::kCallbackRequestedStop) {
+          p_x = fr_x - x;
+          p_s = fr_s - s;
+
+          // Lagrange mutliplier estimates
+          //
+          //   [y] = (ÂÂᵀ)⁻¹Â[ ∇f]
+          //   [z]           [−μe]
+          //
+          //   where Â = [Aₑ   0]
+          //             [Aᵢ  −S]
+          //
+          // See equation (19.37) of [1].
+          {
+            xAD.SetValue(fr_x);
+            sAD.SetValue(c_iAD.Value());
+
+            A_e = jacobianCe.Value();
+            A_i = jacobianCi.Value();
+            g = gradientF.Value();
+
+            // Â = [Aₑ   0]
+            //     [Aᵢ  −S]
+            triplets.clear();
+            triplets.reserve(A_e.nonZeros() + A_i.nonZeros() + s.rows());
+            for (int col = 0; col < A_e.cols(); ++col) {
+              // Append column of Aₑ in top-left quadrant
+              for (Eigen::SparseMatrix<double>::InnerIterator it{A_e, col}; it;
+                   ++it) {
+                triplets.emplace_back(it.row(), it.col(), it.value());
+              }
+              // Append column of Aᵢ in bottom-left quadrant
+              for (Eigen::SparseMatrix<double>::InnerIterator it{A_i, col}; it;
+                   ++it) {
+                triplets.emplace_back(A_e.rows() + it.row(), it.col(),
+                                      it.value());
+              }
+            }
+            // Append −S in bottom-right quadrant
+            for (int i = 0; i < s.rows(); ++i) {
+              triplets.emplace_back(A_e.rows() + i, A_e.cols() + i, -s(i));
+            }
+            Eigen::SparseMatrix<double> Ahat{A_e.rows() + A_i.rows(),
+                                             A_e.cols() + s.rows()};
+            Ahat.setFromSortedTriplets(
+                triplets.begin(), triplets.end(),
+                [](const auto& a, const auto& b) { return b; });
+
+            // lhs = ÂÂᵀ
+            Eigen::SparseMatrix<double> lhs = Ahat * Ahat.transpose();
+
+            // rhs = Â[ ∇f]
+            //        [−μe]
+            Eigen::VectorXd rhsTemp{g.rows() + e.rows()};
+            rhsTemp.block(0, 0, g.rows(), 1) = g;
+            rhsTemp.block(g.rows(), 0, s.rows(), 1) = -μ * e;
+            Eigen::VectorXd rhs = Ahat * rhsTemp;
+
+            Eigen::SimplicialLDLT<Eigen::SparseMatrix<double>> yzEstimator{lhs};
+            Eigen::VectorXd sol = yzEstimator.solve(rhs);
+
+            p_y = y - sol.block(0, 0, y.rows(), 1);
+            p_z = z - sol.block(y.rows(), 0, z.rows(), 1);
+          }
+
+          α = 1.0;
+          α_z = 1.0;
+
+          // Accept step
+          break;
+        } else if (fr_status.exitCondition == SolverExitCondition::kSuccess) {
+          status->exitCondition = SolverExitCondition::kLocallyInfeasible;
+          x = fr_x;
+          return;
+        } else {
+          status->exitCondition =
+              SolverExitCondition::kFeasibilityRestorationFailed;
+          x = fr_x;
+          return;
+        }
+      }
+    }
+
+    // If full step was accepted, reset full-step rejected counter
+    if (α == α_max) {
+      fullStepRejectedCounter = 0;
+    }
+
+    // Handle very small search directions by letting αₖ = αₖᵐᵃˣ when
+    // max(|pₖˣ(i)|/(1 + |xₖ(i)|)) < 10ε_mach.
+    //
+    // See section 3.9 of [2].
+    double maxStepScaled = 0.0;
+    for (int row = 0; row < x.rows(); ++row) {
+      maxStepScaled = std::max(maxStepScaled,
+                               std::abs(p_x(row)) / (1.0 + std::abs(x(row))));
+    }
+    if (maxStepScaled < 10.0 * std::numeric_limits<double>::epsilon()) {
+      α = α_max;
+      ++stepTooSmallCounter;
+    } else {
+      stepTooSmallCounter = 0;
+    }
+
+    // xₖ₊₁ = xₖ + αₖpₖˣ
+    // sₖ₊₁ = sₖ + αₖpₖˢ
+    // yₖ₊₁ = yₖ + αₖᶻpₖʸ
+    // zₖ₊₁ = zₖ + αₖᶻpₖᶻ
+    x += α * p_x;
+    s += α * p_s;
+    y += α_z * p_y;
+    z += α_z * p_z;
+
+    // A requirement for the convergence proof is that the "primal-dual barrier
+    // term Hessian" Σₖ does not deviate arbitrarily much from the "primal
+    // Hessian" μⱼSₖ⁻². We ensure this by resetting
+    //
+    //   zₖ₊₁⁽ⁱ⁾ = max(min(zₖ₊₁⁽ⁱ⁾, κ_Σ μⱼ/sₖ₊₁⁽ⁱ⁾), μⱼ/(κ_Σ sₖ₊₁⁽ⁱ⁾))
+    //
+    // for some fixed κ_Σ ≥ 1 after each step. See equation (16) of [2].
+    {
+      // Barrier parameter scale factor for inequality constraint Lagrange
+      // multiplier safeguard
+      constexpr double κ_Σ = 1e10;
+
+      for (int row = 0; row < z.rows(); ++row) {
+        z(row) =
+            std::max(std::min(z(row), κ_Σ * μ / s(row)), μ / (κ_Σ * s(row)));
+      }
+    }
+
+    // Update autodiff for Jacobians and Hessian
+    xAD.SetValue(x);
+    sAD.SetValue(s);
+    yAD.SetValue(y);
+    zAD.SetValue(z);
+    A_e = jacobianCe.Value();
+    A_i = jacobianCi.Value();
+    g = gradientF.Value();
+    H = hessianL.Value();
+
+    // Update cₑ
+    for (int row = 0; row < c_e.rows(); ++row) {
+      c_eAD(row).Update();
+    }
+    c_e = c_eAD.Value();
+
+    // Update cᵢ
+    for (int row = 0; row < c_i.rows(); ++row) {
+      c_iAD(row).Update();
+    }
+    c_i = c_iAD.Value();
+
+    // Update the error estimate
+    E_0 = ErrorEstimate(g, A_e, c_e, A_i, c_i, s, y, z, 0.0);
+    if (E_0 < config.acceptableTolerance) {
+      ++acceptableIterCounter;
+    } else {
+      acceptableIterCounter = 0;
+    }
+
+    // Update the barrier parameter if necessary
+    if (E_0 > config.tolerance) {
+      // Barrier parameter scale factor for tolerance checks
+      constexpr double κ_ε = 10.0;
+
+      // While the error estimate is below the desired threshold for this
+      // barrier parameter value, decrease the barrier parameter further
+      double E_μ = ErrorEstimate(g, A_e, c_e, A_i, c_i, s, y, z, μ);
+      while (μ > μ_min && E_μ <= κ_ε * μ) {
+        UpdateBarrierParameterAndResetFilter();
+        E_μ = ErrorEstimate(g, A_e, c_e, A_i, c_i, s, y, z, μ);
+      }
+    }
+
+    const auto innerIterEndTime = std::chrono::system_clock::now();
+
+    // Diagnostics for current iteration
+    if (config.diagnostics) {
+      if (iterations % 20 == 0) {
+        sleipnir::println("{:^4}   {:^9}  {:^13}  {:^13}  {:^13}", "iter",
+                          "time (ms)", "error", "cost", "infeasibility");
+        sleipnir::println("{:=^61}", "");
+      }
+
+      sleipnir::println("{:4}{}  {:9.3f}  {:13e}  {:13e}  {:13e}", iterations,
+                        feasibilityRestoration ? "r" : " ",
+                        ToMilliseconds(innerIterEndTime - innerIterStartTime),
+                        E_0, f.Value(),
+                        c_e.lpNorm<1>() + (c_i - s).lpNorm<1>());
+    }
+
+    ++iterations;
+
+    // Check for max iterations
+    if (iterations >= config.maxIterations) {
+      status->exitCondition = SolverExitCondition::kMaxIterationsExceeded;
+      return;
+    }
+
+    // Check for max wall clock time
+    if (innerIterEndTime - solveStartTime > config.timeout) {
+      status->exitCondition = SolverExitCondition::kTimeout;
+      return;
+    }
+
+    // Check for solve to acceptable tolerance
+    if (E_0 > config.tolerance &&
+        acceptableIterCounter == config.maxAcceptableIterations) {
+      status->exitCondition = SolverExitCondition::kSolvedToAcceptableTolerance;
+      return;
+    }
+
+    // The search direction has been very small twice, so assume the problem has
+    // been solved as well as possible given finite precision and reduce the
+    // barrier parameter.
+    //
+    // See section 3.9 of [2].
+    if (stepTooSmallCounter >= 2 && μ > μ_min) {
+      UpdateBarrierParameterAndResetFilter();
+      continue;
+    }
+  }
+}  // NOLINT(readability/fn_size)
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/ErrorEstimate.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/ErrorEstimate.hpp`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <algorithm>
-
-#include <Eigen/Core>
-#include <Eigen/SparseCore>
-
-// See docs/algorithms.md#Works_cited for citation definitions
-
-namespace sleipnir {
-
-/**
- * Returns the error estimate using the KKT conditions for the interior-point
- * method.
- *
- * @param g Gradient of the cost function ∇f.
- * @param A_e The problem's equality constraint Jacobian Aₑ(x) evaluated at the
- *   current iterate.
- * @param c_e The problem's equality constraints cₑ(x) evaluated at the current
- *   iterate.
- * @param A_i The problem's inequality constraint Jacobian Aᵢ(x) evaluated at
- *   the current iterate.
- * @param c_i The problem's inequality constraints cᵢ(x) evaluated at the
- *   current iterate.
- * @param s Inequality constraint slack variables.
- * @param y Equality constraint dual variables.
- * @param z Inequality constraint dual variables.
- * @param μ Barrier parameter.
- */
-inline double ErrorEstimate(const Eigen::VectorXd& g,
-                            const Eigen::SparseMatrix<double>& A_e,
-                            const Eigen::VectorXd& c_e,
-                            const Eigen::SparseMatrix<double>& A_i,
-                            const Eigen::VectorXd& c_i,
-                            const Eigen::VectorXd& s, const Eigen::VectorXd& y,
-                            const Eigen::VectorXd& z, double μ) {
-  int numEqualityConstraints = A_e.rows();
-  int numInequalityConstraints = A_i.rows();
-
-  // Update the error estimate using the KKT conditions from equations (19.5a)
-  // through (19.5d) of [1].
-  //
-  //   ∇f − Aₑᵀy − Aᵢᵀz = 0
-  //   Sz − μe = 0
-  //   cₑ = 0
-  //   cᵢ − s = 0
-  //
-  // The error tolerance is the max of the following infinity norms scaled by
-  // s_d and s_c (see equation (5) of [2]).
-  //
-  //   ‖∇f − Aₑᵀy − Aᵢᵀz‖_∞ / s_d
-  //   ‖Sz − μe‖_∞ / s_c
-  //   ‖cₑ‖_∞
-  //   ‖cᵢ − s‖_∞
-
-  // s_d = max(sₘₐₓ, (‖y‖₁ + ‖z‖₁) / (m + n)) / sₘₐₓ
-  constexpr double s_max = 100.0;
-  double s_d =
-      std::max(s_max, (y.lpNorm<1>() + z.lpNorm<1>()) /
-                          (numEqualityConstraints + numInequalityConstraints)) /
-      s_max;
-
-  // s_c = max(sₘₐₓ, ‖z‖₁ / n) / sₘₐₓ
-  double s_c =
-      std::max(s_max, z.lpNorm<1>() / numInequalityConstraints) / s_max;
-
-  const auto S = s.asDiagonal();
-  const Eigen::VectorXd e = Eigen::VectorXd::Ones(s.rows());
-
-  return std::max({(g - A_e.transpose() * y - A_i.transpose() * z)
-                           .lpNorm<Eigen::Infinity>() /
-                       s_d,
-                   (S * z - μ * e).lpNorm<Eigen::Infinity>() / s_c,
-                   c_e.lpNorm<Eigen::Infinity>(),
-                   (c_i - s).lpNorm<Eigen::Infinity>()});
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <algorithm>
+
+#include <Eigen/Core>
+#include <Eigen/SparseCore>
+
+// See docs/algorithms.md#Works_cited for citation definitions
+
+namespace sleipnir {
+
+/**
+ * Returns the error estimate using the KKT conditions for the interior-point
+ * method.
+ *
+ * @param g Gradient of the cost function ∇f.
+ * @param A_e The problem's equality constraint Jacobian Aₑ(x) evaluated at the
+ *   current iterate.
+ * @param c_e The problem's equality constraints cₑ(x) evaluated at the current
+ *   iterate.
+ * @param A_i The problem's inequality constraint Jacobian Aᵢ(x) evaluated at
+ *   the current iterate.
+ * @param c_i The problem's inequality constraints cᵢ(x) evaluated at the
+ *   current iterate.
+ * @param s Inequality constraint slack variables.
+ * @param y Equality constraint dual variables.
+ * @param z Inequality constraint dual variables.
+ * @param μ Barrier parameter.
+ */
+inline double ErrorEstimate(const Eigen::VectorXd& g,
+                            const Eigen::SparseMatrix<double>& A_e,
+                            const Eigen::VectorXd& c_e,
+                            const Eigen::SparseMatrix<double>& A_i,
+                            const Eigen::VectorXd& c_i,
+                            const Eigen::VectorXd& s, const Eigen::VectorXd& y,
+                            const Eigen::VectorXd& z, double μ) {
+  int numEqualityConstraints = A_e.rows();
+  int numInequalityConstraints = A_i.rows();
+
+  // Update the error estimate using the KKT conditions from equations (19.5a)
+  // through (19.5d) of [1].
+  //
+  //   ∇f − Aₑᵀy − Aᵢᵀz = 0
+  //   Sz − μe = 0
+  //   cₑ = 0
+  //   cᵢ − s = 0
+  //
+  // The error tolerance is the max of the following infinity norms scaled by
+  // s_d and s_c (see equation (5) of [2]).
+  //
+  //   ‖∇f − Aₑᵀy − Aᵢᵀz‖_∞ / s_d
+  //   ‖Sz − μe‖_∞ / s_c
+  //   ‖cₑ‖_∞
+  //   ‖cᵢ − s‖_∞
+
+  // s_d = max(sₘₐₓ, (‖y‖₁ + ‖z‖₁) / (m + n)) / sₘₐₓ
+  constexpr double s_max = 100.0;
+  double s_d =
+      std::max(s_max, (y.lpNorm<1>() + z.lpNorm<1>()) /
+                          (numEqualityConstraints + numInequalityConstraints)) /
+      s_max;
+
+  // s_c = max(sₘₐₓ, ‖z‖₁ / n) / sₘₐₓ
+  double s_c =
+      std::max(s_max, z.lpNorm<1>() / numInequalityConstraints) / s_max;
+
+  const auto S = s.asDiagonal();
+  const Eigen::VectorXd e = Eigen::VectorXd::Ones(s.rows());
+
+  return std::max({(g - A_e.transpose() * y - A_i.transpose() * z)
+                           .lpNorm<Eigen::Infinity>() /
+                       s_d,
+                   (S * z - μ * e).lpNorm<Eigen::Infinity>() / s_c,
+                   c_e.lpNorm<Eigen::Infinity>(),
+                   (c_i - s).lpNorm<Eigen::Infinity>()});
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/FeasibilityRestoration.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/FeasibilityRestoration.hpp`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,239 +1,239 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <algorithm>
-#include <cmath>
-#include <functional>
-#include <iterator>
-#include <span>
-#include <vector>
-
-#include <Eigen/Core>
-
-#include "sleipnir/autodiff/Variable.hpp"
-#include "sleipnir/autodiff/VariableMatrix.hpp"
-#include "sleipnir/optimization/SolverConfig.hpp"
-#include "sleipnir/optimization/SolverIterationInfo.hpp"
-#include "sleipnir/optimization/SolverStatus.hpp"
-#include "sleipnir/optimization/solver/InteriorPoint.hpp"
-
-namespace sleipnir {
-
-/**
- * Finds the iterate that minimizes the constraint violation while not deviating
- * too far from the starting point. This is a fallback procedure when the normal
- * interior-point method fails to converge to a feasible point.
- *
- * @param[in] decisionVariables The list of decision variables.
- * @param[in] equalityConstraints The list of equality constraints.
- * @param[in] inequalityConstraints The list of inequality constraints.
- * @param[in] f The cost function.
- * @param[in] μ Barrier parameter.
- * @param[in] callback The user callback.
- * @param[in] config Configuration options for the solver.
- * @param[in,out] x The current iterate from the normal solve.
- * @param[in,out] s The current inequality constraint slack variables from the
- *   normal solve.
- * @param[out] status The solver status.
- */
-inline void FeasibilityRestoration(
-    std::span<Variable> decisionVariables,
-    std::span<Variable> equalityConstraints,
-    std::span<Variable> inequalityConstraints, Variable& f, double μ,
-    const std::function<bool(const SolverIterationInfo&)>& callback,
-    const SolverConfig& config, Eigen::VectorXd& x, Eigen::VectorXd& s,
-    SolverStatus* status) {
-  // Feasibility restoration
-  //
-  //        min  ρ Σ (pₑ + nₑ + pᵢ + nᵢ) + ζ/2 (x - x_R)ᵀD_R(x - x_R)
-  //         x
-  //       pₑ,nₑ
-  //       pᵢ,nᵢ
-  //
-  //   s.t. cₑ(x) - pₑ + nₑ = 0
-  //        cᵢ(x) - s - pᵢ + nᵢ = 0
-  //        pₑ ≥ 0
-  //        nₑ ≥ 0
-  //        pᵢ ≥ 0
-  //        nᵢ ≥ 0
-  //
-  // where ρ = 1000, ζ = √μ where μ is the barrier parameter, x_R is original
-  // iterate before feasibility restoration, and D_R is a scaling matrix defined
-  // by
-  //
-  //   D_R = diag(min(1, 1/|x_R⁽¹⁾|), …, min(1, 1/|x_R|⁽ⁿ⁾)
-
-  constexpr double ρ = 1000.0;
-
-  std::vector<Variable> fr_decisionVariables;
-  fr_decisionVariables.reserve(decisionVariables.size() +
-                               2 * equalityConstraints.size() +
-                               2 * inequalityConstraints.size());
-
-  // Assign x
-  fr_decisionVariables.assign(decisionVariables.begin(),
-                              decisionVariables.end());
-
-  // Allocate pₑ, nₑ, pᵢ, and nᵢ
-  for (size_t row = 0;
-       row < 2 * equalityConstraints.size() + 2 * inequalityConstraints.size();
-       ++row) {
-    fr_decisionVariables.emplace_back();
-  }
-
-  auto it = fr_decisionVariables.cbegin();
-
-  VariableMatrix xAD{std::span{it, it + decisionVariables.size()}};
-  it += decisionVariables.size();
-
-  VariableMatrix p_e{std::span{it, it + equalityConstraints.size()}};
-  it += equalityConstraints.size();
-
-  VariableMatrix n_e{std::span{it, it + equalityConstraints.size()}};
-  it += equalityConstraints.size();
-
-  VariableMatrix p_i{std::span{it, it + inequalityConstraints.size()}};
-  it += inequalityConstraints.size();
-
-  VariableMatrix n_i{std::span{it, it + inequalityConstraints.size()}};
-
-  // Set initial values for pₑ, nₑ, pᵢ, and nᵢ.
-  //
-  //
-  // From equation (33) of [2]:
-  //                       ______________________
-  //       μ − ρ c(x)     /(μ − ρ c(x))²   μ c(x)
-  //   n = −−−−−−−−−− +  / (−−−−−−−−−−)  + −−−−−−     (1)
-  //           2ρ       √  (    2ρ    )      2ρ
-  //
-  // The quadratic formula:
-  //             ________
-  //       -b + √b² - 4ac
-  //   x = −−−−−−−−−−−−−−                             (2)
-  //             2a
-  //
-  // Rearrange (1) to fit the quadratic formula better:
-  //                     _________________________
-  //       μ - ρ c(x) + √(μ - ρ c(x))² + 2ρ μ c(x)
-  //   n = −−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−
-  //                         2ρ
-  //
-  // Solve for coefficients:
-  //
-  //   a = ρ                                         (3)
-  //   b = ρ c(x) - μ                                (4)
-  //
-  //   -4ac = μ c(x) 2ρ
-  //   -4(ρ)c = 2ρ μ c(x)
-  //   -4c = 2μ c(x)
-  //   c = -μ c(x)/2                                 (5)
-  //
-  //   p = c(x) + n                                  (6)
-  for (int row = 0; row < p_e.Rows(); ++row) {
-    double c_e = equalityConstraints[row].Value();
-
-    constexpr double a = 2 * ρ;
-    double b = ρ * c_e - μ;
-    double c = -μ * c_e / 2.0;
-
-    double n = -b * std::sqrt(b * b - 4.0 * a * c) / (2.0 * a);
-    double p = c_e + n;
-
-    p_e(row).SetValue(p);
-    n_e(row).SetValue(n);
-  }
-  for (int row = 0; row < p_i.Rows(); ++row) {
-    double c_i = inequalityConstraints[row].Value() - s(row);
-
-    constexpr double a = 2 * ρ;
-    double b = ρ * c_i - μ;
-    double c = -μ * c_i / 2.0;
-
-    double n = -b * std::sqrt(b * b - 4.0 * a * c) / (2.0 * a);
-    double p = c_i + n;
-
-    p_i(row).SetValue(p);
-    n_i(row).SetValue(n);
-  }
-
-  // cₑ(x) - pₑ + nₑ = 0
-  std::vector<Variable> fr_equalityConstraints;
-  fr_equalityConstraints.assign(equalityConstraints.begin(),
-                                equalityConstraints.end());
-  for (size_t row = 0; row < fr_equalityConstraints.size(); ++row) {
-    auto& constraint = fr_equalityConstraints[row];
-    constraint = constraint - p_e(row) + n_e(row);
-  }
-
-  // cᵢ(x) - s - pᵢ + nᵢ = 0
-  std::vector<Variable> fr_inequalityConstraints;
-  fr_inequalityConstraints.assign(inequalityConstraints.begin(),
-                                  inequalityConstraints.end());
-  for (size_t row = 0; row < fr_inequalityConstraints.size(); ++row) {
-    auto& constraint = fr_inequalityConstraints[row];
-    constraint = constraint - s(row) - p_i(row) + n_i(row);
-  }
-
-  // pₑ ≥ 0
-  std::copy(p_e.begin(), p_e.end(),
-            std::back_inserter(fr_inequalityConstraints));
-
-  // pᵢ ≥ 0
-  std::copy(p_i.begin(), p_i.end(),
-            std::back_inserter(fr_inequalityConstraints));
-
-  // nₑ ≥ 0
-  std::copy(n_e.begin(), n_e.end(),
-            std::back_inserter(fr_inequalityConstraints));
-
-  // nᵢ ≥ 0
-  std::copy(n_i.begin(), n_i.end(),
-            std::back_inserter(fr_inequalityConstraints));
-
-  Variable J = 0.0;
-
-  // J += ρ Σ (pₑ + nₑ + pᵢ + nᵢ)
-  for (auto& elem : p_e) {
-    J += elem;
-  }
-  for (auto& elem : p_i) {
-    J += elem;
-  }
-  for (auto& elem : n_e) {
-    J += elem;
-  }
-  for (auto& elem : n_i) {
-    J += elem;
-  }
-  J *= ρ;
-
-  // D_R = diag(min(1, 1/|x_R⁽¹⁾|), …, min(1, 1/|x_R|⁽ⁿ⁾)
-  Eigen::VectorXd D_R{x.rows()};
-  for (int row = 0; row < D_R.rows(); ++row) {
-    D_R(row) = std::min(1.0, 1.0 / std::abs(x(row)));
-  }
-
-  // J += ζ/2 (x - x_R)ᵀD_R(x - x_R)
-  for (int row = 0; row < x.rows(); ++row) {
-    J += std::sqrt(μ) / 2.0 * D_R(row) * sleipnir::pow(xAD(row) - x(row), 2);
-  }
-
-  Eigen::VectorXd fr_x = VariableMatrix{fr_decisionVariables}.Value();
-
-  // Set up initial value for inequality constraint slack variables
-  Eigen::VectorXd fr_s{fr_inequalityConstraints.size()};
-  fr_s.segment(0, inequalityConstraints.size()) = s;
-  fr_s.segment(inequalityConstraints.size(),
-               fr_s.size() - inequalityConstraints.size())
-      .setOnes();
-
-  InteriorPoint(fr_decisionVariables, fr_equalityConstraints,
-                fr_inequalityConstraints, J, callback, config, true, fr_x, fr_s,
-                status);
-
-  x = fr_x.segment(0, decisionVariables.size());
-  s = fr_s.segment(0, inequalityConstraints.size());
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <algorithm>
+#include <cmath>
+#include <functional>
+#include <iterator>
+#include <span>
+#include <vector>
+
+#include <Eigen/Core>
+
+#include "sleipnir/autodiff/Variable.hpp"
+#include "sleipnir/autodiff/VariableMatrix.hpp"
+#include "sleipnir/optimization/SolverConfig.hpp"
+#include "sleipnir/optimization/SolverIterationInfo.hpp"
+#include "sleipnir/optimization/SolverStatus.hpp"
+#include "sleipnir/optimization/solver/InteriorPoint.hpp"
+
+namespace sleipnir {
+
+/**
+ * Finds the iterate that minimizes the constraint violation while not deviating
+ * too far from the starting point. This is a fallback procedure when the normal
+ * interior-point method fails to converge to a feasible point.
+ *
+ * @param[in] decisionVariables The list of decision variables.
+ * @param[in] equalityConstraints The list of equality constraints.
+ * @param[in] inequalityConstraints The list of inequality constraints.
+ * @param[in] f The cost function.
+ * @param[in] μ Barrier parameter.
+ * @param[in] callback The user callback.
+ * @param[in] config Configuration options for the solver.
+ * @param[in,out] x The current iterate from the normal solve.
+ * @param[in,out] s The current inequality constraint slack variables from the
+ *   normal solve.
+ * @param[out] status The solver status.
+ */
+inline void FeasibilityRestoration(
+    std::span<Variable> decisionVariables,
+    std::span<Variable> equalityConstraints,
+    std::span<Variable> inequalityConstraints, Variable& f, double μ,
+    const std::function<bool(const SolverIterationInfo&)>& callback,
+    const SolverConfig& config, Eigen::VectorXd& x, Eigen::VectorXd& s,
+    SolverStatus* status) {
+  // Feasibility restoration
+  //
+  //        min  ρ Σ (pₑ + nₑ + pᵢ + nᵢ) + ζ/2 (x - x_R)ᵀD_R(x - x_R)
+  //         x
+  //       pₑ,nₑ
+  //       pᵢ,nᵢ
+  //
+  //   s.t. cₑ(x) - pₑ + nₑ = 0
+  //        cᵢ(x) - s - pᵢ + nᵢ = 0
+  //        pₑ ≥ 0
+  //        nₑ ≥ 0
+  //        pᵢ ≥ 0
+  //        nᵢ ≥ 0
+  //
+  // where ρ = 1000, ζ = √μ where μ is the barrier parameter, x_R is original
+  // iterate before feasibility restoration, and D_R is a scaling matrix defined
+  // by
+  //
+  //   D_R = diag(min(1, 1/|x_R⁽¹⁾|), …, min(1, 1/|x_R|⁽ⁿ⁾)
+
+  constexpr double ρ = 1000.0;
+
+  std::vector<Variable> fr_decisionVariables;
+  fr_decisionVariables.reserve(decisionVariables.size() +
+                               2 * equalityConstraints.size() +
+                               2 * inequalityConstraints.size());
+
+  // Assign x
+  fr_decisionVariables.assign(decisionVariables.begin(),
+                              decisionVariables.end());
+
+  // Allocate pₑ, nₑ, pᵢ, and nᵢ
+  for (size_t row = 0;
+       row < 2 * equalityConstraints.size() + 2 * inequalityConstraints.size();
+       ++row) {
+    fr_decisionVariables.emplace_back();
+  }
+
+  auto it = fr_decisionVariables.cbegin();
+
+  VariableMatrix xAD{std::span{it, it + decisionVariables.size()}};
+  it += decisionVariables.size();
+
+  VariableMatrix p_e{std::span{it, it + equalityConstraints.size()}};
+  it += equalityConstraints.size();
+
+  VariableMatrix n_e{std::span{it, it + equalityConstraints.size()}};
+  it += equalityConstraints.size();
+
+  VariableMatrix p_i{std::span{it, it + inequalityConstraints.size()}};
+  it += inequalityConstraints.size();
+
+  VariableMatrix n_i{std::span{it, it + inequalityConstraints.size()}};
+
+  // Set initial values for pₑ, nₑ, pᵢ, and nᵢ.
+  //
+  //
+  // From equation (33) of [2]:
+  //                       ______________________
+  //       μ − ρ c(x)     /(μ − ρ c(x))²   μ c(x)
+  //   n = −−−−−−−−−− +  / (−−−−−−−−−−)  + −−−−−−     (1)
+  //           2ρ       √  (    2ρ    )      2ρ
+  //
+  // The quadratic formula:
+  //             ________
+  //       -b + √b² - 4ac
+  //   x = −−−−−−−−−−−−−−                             (2)
+  //             2a
+  //
+  // Rearrange (1) to fit the quadratic formula better:
+  //                     _________________________
+  //       μ - ρ c(x) + √(μ - ρ c(x))² + 2ρ μ c(x)
+  //   n = −−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−−
+  //                         2ρ
+  //
+  // Solve for coefficients:
+  //
+  //   a = ρ                                         (3)
+  //   b = ρ c(x) - μ                                (4)
+  //
+  //   -4ac = μ c(x) 2ρ
+  //   -4(ρ)c = 2ρ μ c(x)
+  //   -4c = 2μ c(x)
+  //   c = -μ c(x)/2                                 (5)
+  //
+  //   p = c(x) + n                                  (6)
+  for (int row = 0; row < p_e.Rows(); ++row) {
+    double c_e = equalityConstraints[row].Value();
+
+    constexpr double a = 2 * ρ;
+    double b = ρ * c_e - μ;
+    double c = -μ * c_e / 2.0;
+
+    double n = -b * std::sqrt(b * b - 4.0 * a * c) / (2.0 * a);
+    double p = c_e + n;
+
+    p_e(row).SetValue(p);
+    n_e(row).SetValue(n);
+  }
+  for (int row = 0; row < p_i.Rows(); ++row) {
+    double c_i = inequalityConstraints[row].Value() - s(row);
+
+    constexpr double a = 2 * ρ;
+    double b = ρ * c_i - μ;
+    double c = -μ * c_i / 2.0;
+
+    double n = -b * std::sqrt(b * b - 4.0 * a * c) / (2.0 * a);
+    double p = c_i + n;
+
+    p_i(row).SetValue(p);
+    n_i(row).SetValue(n);
+  }
+
+  // cₑ(x) - pₑ + nₑ = 0
+  std::vector<Variable> fr_equalityConstraints;
+  fr_equalityConstraints.assign(equalityConstraints.begin(),
+                                equalityConstraints.end());
+  for (size_t row = 0; row < fr_equalityConstraints.size(); ++row) {
+    auto& constraint = fr_equalityConstraints[row];
+    constraint = constraint - p_e(row) + n_e(row);
+  }
+
+  // cᵢ(x) - s - pᵢ + nᵢ = 0
+  std::vector<Variable> fr_inequalityConstraints;
+  fr_inequalityConstraints.assign(inequalityConstraints.begin(),
+                                  inequalityConstraints.end());
+  for (size_t row = 0; row < fr_inequalityConstraints.size(); ++row) {
+    auto& constraint = fr_inequalityConstraints[row];
+    constraint = constraint - s(row) - p_i(row) + n_i(row);
+  }
+
+  // pₑ ≥ 0
+  std::copy(p_e.begin(), p_e.end(),
+            std::back_inserter(fr_inequalityConstraints));
+
+  // pᵢ ≥ 0
+  std::copy(p_i.begin(), p_i.end(),
+            std::back_inserter(fr_inequalityConstraints));
+
+  // nₑ ≥ 0
+  std::copy(n_e.begin(), n_e.end(),
+            std::back_inserter(fr_inequalityConstraints));
+
+  // nᵢ ≥ 0
+  std::copy(n_i.begin(), n_i.end(),
+            std::back_inserter(fr_inequalityConstraints));
+
+  Variable J = 0.0;
+
+  // J += ρ Σ (pₑ + nₑ + pᵢ + nᵢ)
+  for (auto& elem : p_e) {
+    J += elem;
+  }
+  for (auto& elem : p_i) {
+    J += elem;
+  }
+  for (auto& elem : n_e) {
+    J += elem;
+  }
+  for (auto& elem : n_i) {
+    J += elem;
+  }
+  J *= ρ;
+
+  // D_R = diag(min(1, 1/|x_R⁽¹⁾|), …, min(1, 1/|x_R|⁽ⁿ⁾)
+  Eigen::VectorXd D_R{x.rows()};
+  for (int row = 0; row < D_R.rows(); ++row) {
+    D_R(row) = std::min(1.0, 1.0 / std::abs(x(row)));
+  }
+
+  // J += ζ/2 (x - x_R)ᵀD_R(x - x_R)
+  for (int row = 0; row < x.rows(); ++row) {
+    J += std::sqrt(μ) / 2.0 * D_R(row) * sleipnir::pow(xAD(row) - x(row), 2);
+  }
+
+  Eigen::VectorXd fr_x = VariableMatrix{fr_decisionVariables}.Value();
+
+  // Set up initial value for inequality constraint slack variables
+  Eigen::VectorXd fr_s{fr_inequalityConstraints.size()};
+  fr_s.segment(0, inequalityConstraints.size()) = s;
+  fr_s.segment(inequalityConstraints.size(),
+               fr_s.size() - inequalityConstraints.size())
+      .setOnes();
+
+  InteriorPoint(fr_decisionVariables, fr_equalityConstraints,
+                fr_inequalityConstraints, J, callback, config, true, fr_x, fr_s,
+                status);
+
+  x = fr_x.segment(0, decisionVariables.size());
+  s = fr_s.segment(0, inequalityConstraints.size());
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/Filter.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/Filter.hpp`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <algorithm>
-#include <cmath>
-#include <limits>
-#include <utility>
-#include <vector>
-
-#include <Eigen/Core>
-
-#include "sleipnir/autodiff/Variable.hpp"
-
-namespace sleipnir {
-
-/**
- * Filter entry consisting of cost and constraint violation.
- */
-struct FilterEntry {
-  /// The cost function's value
-  double cost = 0.0;
-
-  /// The constraint violation
-  double constraintViolation = 0.0;
-
-  constexpr FilterEntry() = default;
-
-  /**
-   * Constructs a FilterEntry.
-   *
-   * @param cost The cost function's value.
-   * @param constraintViolation The constraint violation.
-   */
-  FilterEntry(double cost, double constraintViolation)
-      : cost{cost}, constraintViolation{constraintViolation} {}
-
-  /**
-   * Constructs a FilterEntry.
-   *
-   * @param f The cost function.
-   * @param μ The barrier parameter.
-   * @param s The inequality constraint slack variables.
-   * @param c_e The equality constraint values (nonzero means violation).
-   * @param c_i The inequality constraint values (negative means violation).
-   */
-  FilterEntry(const Variable& f, double μ, const Eigen::VectorXd& s,
-              const Eigen::VectorXd& c_e, const Eigen::VectorXd& c_i)
-      : cost{f.Value() - μ * s.array().log().sum()},
-        constraintViolation{c_e.lpNorm<1>() + (c_i - s).lpNorm<1>()} {}
-};
-
-/**
- * Interior-point step filter.
- */
-class Filter {
- public:
-  static constexpr double γCost = 1e-8;
-  static constexpr double γConstraint = 1e-5;
-
-  double maxConstraintViolation = 1e4;
-
-  /**
-   * Construct an empty filter.
-   *
-   * @param f The cost function.
-   * @param μ The barrier parameter.
-   */
-  explicit Filter(Variable& f, double μ) {
-    m_f = &f;
-    m_μ = μ;
-
-    // Initial filter entry rejects constraint violations above max
-    m_filter.emplace_back(std::numeric_limits<double>::infinity(),
-                          maxConstraintViolation);
-  }
-
-  /**
-   * Reset the filter.
-   *
-   * @param μ The new barrier parameter.
-   */
-  void Reset(double μ) {
-    m_μ = μ;
-    m_filter.clear();
-
-    // Initial filter entry rejects constraint violations above max
-    m_filter.emplace_back(std::numeric_limits<double>::infinity(),
-                          maxConstraintViolation);
-  }
-
-  /**
-   * Creates a new filter entry.
-   *
-   * @param s The inequality constraint slack variables.
-   * @param c_e The equality constraint values (nonzero means violation).
-   * @param c_i The inequality constraint values (negative means violation).
-   */
-  FilterEntry MakeEntry(Eigen::VectorXd& s, const Eigen::VectorXd& c_e,
-                        const Eigen::VectorXd& c_i) {
-    return FilterEntry{*m_f, m_μ, s, c_e, c_i};
-  }
-
-  /**
-   * Add a new entry to the filter.
-   *
-   * @param entry The entry to add to the filter.
-   */
-  void Add(const FilterEntry& entry) {
-    // Remove dominated entries
-    std::erase_if(m_filter, [&](const auto& elem) {
-      return entry.cost <= elem.cost &&
-             entry.constraintViolation <= elem.constraintViolation;
-    });
-
-    m_filter.push_back(entry);
-  }
-
-  /**
-   * Add a new entry to the filter.
-   *
-   * @param entry The entry to add to the filter.
-   */
-  void Add(FilterEntry&& entry) {
-    // Remove dominated entries
-    std::erase_if(m_filter, [&](const auto& elem) {
-      return entry.cost <= elem.cost &&
-             entry.constraintViolation <= elem.constraintViolation;
-    });
-
-    m_filter.push_back(entry);
-  }
-
-  /**
-   * Returns true if the given iterate is accepted by the filter.
-   *
-   * @param entry The entry to attempt adding to the filter.
-   */
-  bool TryAdd(const FilterEntry& entry) {
-    if (IsAcceptable(entry)) {
-      Add(entry);
-      return true;
-    } else {
-      return false;
-    }
-  }
-
-  /**
-   * Returns true if the given iterate is accepted by the filter.
-   *
-   * @param entry The entry to attempt adding to the filter.
-   */
-  bool TryAdd(FilterEntry&& entry) {
-    if (IsAcceptable(entry)) {
-      Add(std::move(entry));
-      return true;
-    } else {
-      return false;
-    }
-  }
-
-  /**
-   * Returns true if the given entry is acceptable to the filter.
-   *
-   * @param entry The entry to check.
-   */
-  bool IsAcceptable(const FilterEntry& entry) {
-    if (!std::isfinite(entry.cost) ||
-        !std::isfinite(entry.constraintViolation)) {
-      return false;
-    }
-
-    // If current filter entry is better than all prior ones in some respect,
-    // accept it
-    return std::all_of(m_filter.begin(), m_filter.end(), [&](const auto& elem) {
-      return entry.cost <= elem.cost - γCost * elem.constraintViolation ||
-             entry.constraintViolation <=
-                 (1.0 - γConstraint) * elem.constraintViolation;
-    });
-  }
-
- private:
-  Variable* m_f = nullptr;
-  double m_μ = 0.0;
-  std::vector<FilterEntry> m_filter;
-};
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <algorithm>
+#include <cmath>
+#include <limits>
+#include <utility>
+#include <vector>
+
+#include <Eigen/Core>
+
+#include "sleipnir/autodiff/Variable.hpp"
+
+namespace sleipnir {
+
+/**
+ * Filter entry consisting of cost and constraint violation.
+ */
+struct FilterEntry {
+  /// The cost function's value
+  double cost = 0.0;
+
+  /// The constraint violation
+  double constraintViolation = 0.0;
+
+  constexpr FilterEntry() = default;
+
+  /**
+   * Constructs a FilterEntry.
+   *
+   * @param cost The cost function's value.
+   * @param constraintViolation The constraint violation.
+   */
+  FilterEntry(double cost, double constraintViolation)
+      : cost{cost}, constraintViolation{constraintViolation} {}
+
+  /**
+   * Constructs a FilterEntry.
+   *
+   * @param f The cost function.
+   * @param μ The barrier parameter.
+   * @param s The inequality constraint slack variables.
+   * @param c_e The equality constraint values (nonzero means violation).
+   * @param c_i The inequality constraint values (negative means violation).
+   */
+  FilterEntry(const Variable& f, double μ, const Eigen::VectorXd& s,
+              const Eigen::VectorXd& c_e, const Eigen::VectorXd& c_i)
+      : cost{f.Value() - μ * s.array().log().sum()},
+        constraintViolation{c_e.lpNorm<1>() + (c_i - s).lpNorm<1>()} {}
+};
+
+/**
+ * Interior-point step filter.
+ */
+class Filter {
+ public:
+  static constexpr double γCost = 1e-8;
+  static constexpr double γConstraint = 1e-5;
+
+  double maxConstraintViolation = 1e4;
+
+  /**
+   * Construct an empty filter.
+   *
+   * @param f The cost function.
+   * @param μ The barrier parameter.
+   */
+  explicit Filter(Variable& f, double μ) {
+    m_f = &f;
+    m_μ = μ;
+
+    // Initial filter entry rejects constraint violations above max
+    m_filter.emplace_back(std::numeric_limits<double>::infinity(),
+                          maxConstraintViolation);
+  }
+
+  /**
+   * Reset the filter.
+   *
+   * @param μ The new barrier parameter.
+   */
+  void Reset(double μ) {
+    m_μ = μ;
+    m_filter.clear();
+
+    // Initial filter entry rejects constraint violations above max
+    m_filter.emplace_back(std::numeric_limits<double>::infinity(),
+                          maxConstraintViolation);
+  }
+
+  /**
+   * Creates a new filter entry.
+   *
+   * @param s The inequality constraint slack variables.
+   * @param c_e The equality constraint values (nonzero means violation).
+   * @param c_i The inequality constraint values (negative means violation).
+   */
+  FilterEntry MakeEntry(Eigen::VectorXd& s, const Eigen::VectorXd& c_e,
+                        const Eigen::VectorXd& c_i) {
+    return FilterEntry{*m_f, m_μ, s, c_e, c_i};
+  }
+
+  /**
+   * Add a new entry to the filter.
+   *
+   * @param entry The entry to add to the filter.
+   */
+  void Add(const FilterEntry& entry) {
+    // Remove dominated entries
+    std::erase_if(m_filter, [&](const auto& elem) {
+      return entry.cost <= elem.cost &&
+             entry.constraintViolation <= elem.constraintViolation;
+    });
+
+    m_filter.push_back(entry);
+  }
+
+  /**
+   * Add a new entry to the filter.
+   *
+   * @param entry The entry to add to the filter.
+   */
+  void Add(FilterEntry&& entry) {
+    // Remove dominated entries
+    std::erase_if(m_filter, [&](const auto& elem) {
+      return entry.cost <= elem.cost &&
+             entry.constraintViolation <= elem.constraintViolation;
+    });
+
+    m_filter.push_back(entry);
+  }
+
+  /**
+   * Returns true if the given iterate is accepted by the filter.
+   *
+   * @param entry The entry to attempt adding to the filter.
+   */
+  bool TryAdd(const FilterEntry& entry) {
+    if (IsAcceptable(entry)) {
+      Add(entry);
+      return true;
+    } else {
+      return false;
+    }
+  }
+
+  /**
+   * Returns true if the given iterate is accepted by the filter.
+   *
+   * @param entry The entry to attempt adding to the filter.
+   */
+  bool TryAdd(FilterEntry&& entry) {
+    if (IsAcceptable(entry)) {
+      Add(std::move(entry));
+      return true;
+    } else {
+      return false;
+    }
+  }
+
+  /**
+   * Returns true if the given entry is acceptable to the filter.
+   *
+   * @param entry The entry to check.
+   */
+  bool IsAcceptable(const FilterEntry& entry) {
+    if (!std::isfinite(entry.cost) ||
+        !std::isfinite(entry.constraintViolation)) {
+      return false;
+    }
+
+    // If current filter entry is better than all prior ones in some respect,
+    // accept it
+    return std::all_of(m_filter.begin(), m_filter.end(), [&](const auto& elem) {
+      return entry.cost <= elem.cost - γCost * elem.constraintViolation ||
+             entry.constraintViolation <=
+                 (1.0 - γConstraint) * elem.constraintViolation;
+    });
+  }
+
+ private:
+  Variable* m_f = nullptr;
+  double m_μ = 0.0;
+  std::vector<FilterEntry> m_filter;
+};
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/IsLocallyInfeasible.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/IsLocallyInfeasible.hpp`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <Eigen/Core>
-#include <Eigen/SparseCore>
-
-// See docs/algorithms.md#Works_cited for citation definitions
-
-namespace sleipnir {
-
-/**
- * Returns true if the problem's equality constraints are locally infeasible.
- *
- * @param A_e The problem's equality constraint Jacobian Aₑ(x) evaluated at the
- *   current iterate.
- * @param c_e The problem's equality constraints cₑ(x) evaluated at the current
- *   iterate.
- */
-inline bool IsEqualityLocallyInfeasible(const Eigen::SparseMatrix<double>& A_e,
-                                        const Eigen::VectorXd& c_e) {
-  // The equality constraints are locally infeasible if
-  //
-  //   Aₑᵀcₑ → 0
-  //   ‖cₑ‖ > ε
-  //
-  // See "Infeasibility detection" in section 6 of [3].
-  return A_e.rows() > 0 && (A_e.transpose() * c_e).norm() < 1e-6 &&
-         c_e.norm() > 1e-2;
-}
-
-/**
- * Returns true if the problem's inequality constraints are locally infeasible.
- *
- * @param A_i The problem's inequality constraint Jacobian Aᵢ(x) evaluated at
- *   the current iterate.
- * @param c_i The problem's inequality constraints cᵢ(x) evaluated at the
- *   current iterate.
- */
-inline bool IsInequalityLocallyInfeasible(
-    const Eigen::SparseMatrix<double>& A_i, const Eigen::VectorXd& c_i) {
-  // The inequality constraints are locally infeasible if
-  //
-  //   Aᵢᵀcᵢ⁺ → 0
-  //   ‖cᵢ⁺‖ > ε
-  //
-  // where cᵢ⁺ = min(cᵢ, 0).
-  //
-  // See "Infeasibility detection" in section 6 of [3].
-  //
-  // cᵢ⁺ is used instead of cᵢ⁻ from the paper to follow the convention that
-  // feasible inequality constraints are ≥ 0.
-  if (A_i.rows() > 0) {
-    Eigen::VectorXd c_i_plus = c_i.cwiseMin(0.0);
-    if ((A_i.transpose() * c_i_plus).norm() < 1e-6 && c_i_plus.norm() > 1e-6) {
-      return true;
-    }
-  }
-
-  return false;
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <Eigen/Core>
+#include <Eigen/SparseCore>
+
+// See docs/algorithms.md#Works_cited for citation definitions
+
+namespace sleipnir {
+
+/**
+ * Returns true if the problem's equality constraints are locally infeasible.
+ *
+ * @param A_e The problem's equality constraint Jacobian Aₑ(x) evaluated at the
+ *   current iterate.
+ * @param c_e The problem's equality constraints cₑ(x) evaluated at the current
+ *   iterate.
+ */
+inline bool IsEqualityLocallyInfeasible(const Eigen::SparseMatrix<double>& A_e,
+                                        const Eigen::VectorXd& c_e) {
+  // The equality constraints are locally infeasible if
+  //
+  //   Aₑᵀcₑ → 0
+  //   ‖cₑ‖ > ε
+  //
+  // See "Infeasibility detection" in section 6 of [3].
+  return A_e.rows() > 0 && (A_e.transpose() * c_e).norm() < 1e-6 &&
+         c_e.norm() > 1e-2;
+}
+
+/**
+ * Returns true if the problem's inequality constraints are locally infeasible.
+ *
+ * @param A_i The problem's inequality constraint Jacobian Aᵢ(x) evaluated at
+ *   the current iterate.
+ * @param c_i The problem's inequality constraints cᵢ(x) evaluated at the
+ *   current iterate.
+ */
+inline bool IsInequalityLocallyInfeasible(
+    const Eigen::SparseMatrix<double>& A_i, const Eigen::VectorXd& c_i) {
+  // The inequality constraints are locally infeasible if
+  //
+  //   Aᵢᵀcᵢ⁺ → 0
+  //   ‖cᵢ⁺‖ > ε
+  //
+  // where cᵢ⁺ = min(cᵢ, 0).
+  //
+  // See "Infeasibility detection" in section 6 of [3].
+  //
+  // cᵢ⁺ is used instead of cᵢ⁻ from the paper to follow the convention that
+  // feasible inequality constraints are ≥ 0.
+  if (A_i.rows() > 0) {
+    Eigen::VectorXd c_i_plus = c_i.cwiseMin(0.0);
+    if ((A_i.transpose() * c_i_plus).norm() < 1e-6 && c_i_plus.norm() > 1e-6) {
+      return true;
+    }
+  }
+
+  return false;
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/src/optimization/solver/util/KKTError.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev96/src/optimization/solver/util/KKTError.hpp`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-// Copyright (c) Sleipnir contributors
-
-#pragma once
-
-#include <Eigen/Core>
-#include <Eigen/SparseCore>
-
-// See docs/algorithms.md#Works_cited for citation definitions
-
-namespace sleipnir {
-
-/**
- * Returns the KKT error for the interior-point method.
- *
- * @param g Gradient of the cost function ∇f.
- * @param A_e The problem's equality constraint Jacobian Aₑ(x) evaluated at the
- *   current iterate.
- * @param c_e The problem's equality constraints cₑ(x) evaluated at the current
- *   iterate.
- * @param A_i The problem's inequality constraint Jacobian Aᵢ(x) evaluated at
- *   the current iterate.
- * @param c_i The problem's inequality constraints cᵢ(x) evaluated at the
- *   current iterate.
- * @param s Inequality constraint slack variables.
- * @param y Equality constraint dual variables.
- * @param z Inequality constraint dual variables.
- * @param μ Barrier parameter.
- */
-inline double KKTError(const Eigen::VectorXd& g,
-                       const Eigen::SparseMatrix<double>& A_e,
-                       const Eigen::VectorXd& c_e,
-                       const Eigen::SparseMatrix<double>& A_i,
-                       const Eigen::VectorXd& c_i, const Eigen::VectorXd& s,
-                       const Eigen::VectorXd& y, const Eigen::VectorXd& z,
-                       double μ) {
-  // Compute the KKT error as the 1-norm of the KKT conditions from equations
-  // (19.5a) through (19.5d) of [1].
-  //
-  //   ∇f − Aₑᵀy − Aᵢᵀz = 0
-  //   Sz − μe = 0
-  //   cₑ = 0
-  //   cᵢ − s = 0
-
-  const auto S = s.asDiagonal();
-  const Eigen::VectorXd e = Eigen::VectorXd::Ones(s.rows());
-
-  return (g - A_e.transpose() * y - A_i.transpose() * z).lpNorm<1>() +
-         (S * z - μ * e).lpNorm<1>() + c_e.lpNorm<1>() + (c_i - s).lpNorm<1>();
-}
-
-}  // namespace sleipnir
+// Copyright (c) Sleipnir contributors
+
+#pragma once
+
+#include <Eigen/Core>
+#include <Eigen/SparseCore>
+
+// See docs/algorithms.md#Works_cited for citation definitions
+
+namespace sleipnir {
+
+/**
+ * Returns the KKT error for the interior-point method.
+ *
+ * @param g Gradient of the cost function ∇f.
+ * @param A_e The problem's equality constraint Jacobian Aₑ(x) evaluated at the
+ *   current iterate.
+ * @param c_e The problem's equality constraints cₑ(x) evaluated at the current
+ *   iterate.
+ * @param A_i The problem's inequality constraint Jacobian Aᵢ(x) evaluated at
+ *   the current iterate.
+ * @param c_i The problem's inequality constraints cᵢ(x) evaluated at the
+ *   current iterate.
+ * @param s Inequality constraint slack variables.
+ * @param y Equality constraint dual variables.
+ * @param z Inequality constraint dual variables.
+ * @param μ Barrier parameter.
+ */
+inline double KKTError(const Eigen::VectorXd& g,
+                       const Eigen::SparseMatrix<double>& A_e,
+                       const Eigen::VectorXd& c_e,
+                       const Eigen::SparseMatrix<double>& A_i,
+                       const Eigen::VectorXd& c_i, const Eigen::VectorXd& s,
+                       const Eigen::VectorXd& y, const Eigen::VectorXd& z,
+                       double μ) {
+  // Compute the KKT error as the 1-norm of the KKT conditions from equations
+  // (19.5a) through (19.5d) of [1].
+  //
+  //   ∇f − Aₑᵀy − Aᵢᵀz = 0
+  //   Sz − μe = 0
+  //   cₑ = 0
+  //   cᵢ − s = 0
+
+  const auto S = s.asDiagonal();
+  const Eigen::VectorXd e = Eigen::VectorXd::Ones(s.rows());
+
+  return (g - A_e.transpose() * y - A_i.transpose() * z).lpNorm<1>() +
+         (S * z - μ * e).lpNorm<1>() + c_e.lpNorm<1>() + (c_i - s).lpNorm<1>();
+}
+
+}  // namespace sleipnir
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev95/PKG-INFO` & `sleipnirgroup_jormungandr-0.0.1.dev96/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,252 +1,240 @@
-Metadata-Version: 2.1
-Name: sleipnirgroup-jormungandr
-Version: 0.0.1.dev95
-Summary: A linearity-exploiting sparse nonlinear constrained optimization problem solver that uses the interior-point method.
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-Project-URL: Documentation, https://sleipnirgroup.github.io/Sleipnir/
-
-# Sleipnir
-
-![Build](https://github.com/SleipnirGroup/Sleipnir/actions/workflows/build.yml/badge.svg)
-[![C++ Documentation](https://img.shields.io/badge/documentation-c%2B%2B-blue)](https://sleipnirgroup.github.io/Sleipnir/)
-[![Discord](https://img.shields.io/discord/975739302933856277?color=%23738ADB&label=Join%20our%20Discord&logo=discord&logoColor=white)](https://discord.gg/ad2EEZZwsS)
-
-> Sparsity and Linearity-Exploiting Interior-Point solver - Now Internally Readable
-
-Named after Odin's eight-legged horse from Norse mythology, Sleipnir is a linearity-exploiting sparse nonlinear constrained optimization problem solver that uses the interior-point method.
-
-```cpp
-#include <fmt/core.h>
-#include <sleipnir/OptimizationProblem.hpp>
-
-int main() {
-  // Find the x, y pair with the largest product for which x + 3y = 36
-  sleipnir::OptimizationProblem problem;
-
-  auto x = problem.DecisionVariable();
-  auto y = problem.DecisionVariable();
-
-  problem.Maximize(x * y);
-  problem.SubjectTo(x + 3 * y == 36);
-  problem.Solve();
-
-  // x = 18.0, y = 6.0
-  fmt::println("x = {}, y = {}", x.Value(), y.Value());
-}
-```
-
-```python
-#!/usr/bin/env python3
-
-import jormungandr as jmg
-
-
-def main():
-    # Find the x, y pair with the largest product for which x + 3y = 36
-    problem = jmg.optimization.OptimizationProblem()
-
-    x = problem.decision_variable()
-    y = problem.decision_variable()
-
-    problem.maximize(x * y)
-    problem.subject_to(x + 3 * y == 36)
-    problem.solve()
-
-    # x = 18.0, y = 6.0
-    print(f"x = {x.value()}, y = {y.value()}")
-
-
-if __name__ == "__main__":
-    main()
-```
-
-Sleipnir's internals are intended to be readable by those who aren't domain experts with links to explanatory material for its algorithms.
-
-## Benchmarks
-
-<table><tr>
-  <td><img src="flywheel-scalability-results.png" alt="flywheel-scalability-results"/></td>
-  <td><img src="cart-pole-scalability-results.png" alt="cart-pole-scalability-results"/></td>
-</tr><tr>
-  <td>
-    <a href="flywheel-scalability-results-casadi.csv">
-      flywheel-scalability-results-casadi.csv
-    </a><br>
-    <a href="flywheel-scalability-results-sleipnir.csv">
-      flywheel-scalability-results-sleipnir.csv
-    </a>
-  </td>
-  <td>
-    <a href="cart-pole-scalability-results-casadi.csv">
-      cart-pole-scalability-results-casadi.csv
-    </a><br>
-    <a href="cart-pole-scalability-results-sleipnir.csv">
-      cart-pole-scalability-results-sleipnir.csv
-    </a>
-  </td>
-</tr></table>
-
-Generated by [tools/generate-scalability-results.sh](https://github.com/SleipnirGroup/Sleipnir/tree/main/tools/generate-scalability-results.sh) from [benchmarks/scalability](https://github.com/SleipnirGroup/Sleipnir/tree/main/benchmarks/scalability) source on a AMD Ryzen 7 7840U with 64 GB RAM. The following thirdparty software was used in the benchmarks:
-
-* CasADi 3.6.5 (autodiff and NLP solver frontend)
-* Ipopt 3.14.14 (NLP solver backend)
-* MUMPS 5.6.2 (linear solver)
-
-Ipopt uses MUMPS by default because it has free licensing. Commercial linear solvers may be much faster.
-
-### How we improved performance
-
-#### Make more decisions at compile time
-
-During problem setup, equality and inequality constraints are encoded as different types, so the appropriate setup behavior can be selected at compile time via operator overloads.
-
-#### Reuse autodiff computation results that are still valid (aka caching)
-
-The autodiff library automatically records the linearity of every node in the computational graph. Linear functions have constant first derivatives, and quadratic functions have constant second derivatives. The constant derivatives are computed in the initialization phase and reused for all solver iterations. Only nonlinear parts of the computational graph are recomputed during each solver iteration.
-
-For quadratic problems, we compute the Lagrangian Hessian and constraint Jacobians once with no problem structure hints from the user.
-
-#### Use a performant linear algebra library with fast sparse solvers
-
-[Eigen](https://gitlab.com/libeigen/eigen/) provides these. It also has no required dependencies, which makes cross compilation much easier.
-
-#### Use a pool allocator for autodiff expression nodes
-
-This promotes fast allocation/deallocation and good memory locality.
-
-We could mitigate the solver's high last-level-cache miss rate (~42% on the machine above) further by breaking apart the expression nodes into fields that are commonly iterated together. We used to use a tape, which gave computational graph updates linear access patterns, but tapes are monotonic buffers with no way to reclaim storage.
-
-### Running the benchmarks
-
-Benchmark projects are in the [benchmarks folder](https://github.com/SleipnirGroup/Sleipnir/tree/main/benchmarks). To compile and run them, run the following in the repository root:
-```bash
-# Install CasADi and [matplotlib, numpy, scipy] pip packages first
-cmake -B build -S .
-cmake --build build
-./tools/generate-scalability-results.sh
-```
-
-See the contents of `./tools/generate-scalability-results.sh` for how to run specific benchmarks.
-
-## Examples
-
-See the [examples](https://github.com/SleipnirGroup/Sleipnir/tree/main/examples) and [optimization unit tests](https://github.com/SleipnirGroup/Sleipnir/tree/main/test/optimization).
-
-## Dependencies
-
-* C++20 compiler
-  * On Windows, install [Visual Studio Community 2022](https://visualstudio.microsoft.com/vs/community/) and select the C++ programming language during installation
-  * On Linux, install GCC 11 or greater via `sudo apt install gcc`
-  * On macOS, install the Xcode command-line build tools via `xcode-select --install`. Xcode 13 or later is required.
-* [CMake](https://cmake.org/download/) 3.21 or greater
-  * On Windows, install from the link above
-  * On Linux, install via `sudo apt install cmake`
-  * On macOS, install via `brew install cmake`
-* [Python](https://www.python.org/downloads/) 3.11 or greater
-  * On Windows, install from the link above
-  * On Linux, install via `sudo apt install python`
-  * On macOS, install via `brew install python`
-* [Eigen](https://gitlab.com/libeigen/eigen)
-* [fmtlib](https://github.com/fmtlib/fmt) (internal only)
-* [pybind11](https://github.com/pybind/pybind11) (build only)
-* [Catch2](https://github.com/catchorg/Catch2) (tests only)
-
-Library dependencies which aren't installed locally will be automatically downloaded and built by CMake.
-
-If [CasADi](https://github.com/casadi/casadi) is installed locally, the benchmark executables will be built.
-
-## Build instructions
-
-On Windows, open a [Developer PowerShell](https://learn.microsoft.com/en-us/visualstudio/ide/reference/command-prompt-powershell?view=vs-2022). On Linux or macOS, open a Bash shell.
-
-Clone the repository.
-```bash
-git clone git@github.com:SleipnirGroup/Sleipnir
-cd Sleipnir
-```
-
-### C++ library
-
-```bash
-# Configure; automatically downloads library dependencies
-cmake -B build -S .
-
-# Build
-cmake --build build
-
-# Test
-cd build
-ctest
-cd ..
-
-# Install
-cmake --install build --prefix pkgdir
-```
-
-The following build types can be specified via `-DCMAKE_BUILD_TYPE` during CMake configure:
-
-* Debug
-  * Optimizations off
-  * Debug symbols on
-* Release
-  * Optimizations on
-  * Debug symbols off
-* RelWithDebInfo (default)
-  * Release build type, but with debug info
-* MinSizeRel
-  * Minimum size release build
-* Asan
-  * Enables address sanitizer
-* Tsan
-  * Enables thread sanitizer
-* Ubsan
-  * Enables undefined behavior sanitizer
-* Perf
-  * RelWithDebInfo build type, but with frame pointer so perf utility can use it
-
-### Python library
-
-```bash
-# Setup
-pip install --user build
-
-# Build
-python -m build --wheel
-
-# Install
-pip install --user dist/sleipnirgroup_jormungandr-*.whl
-
-# Test
-pytest
-```
-
-## Test diagnostics
-
-Passing the `--enable-diagnostics` flag to the test executable enables solver diagnostic prints.
-
-Some test problems generate CSV files containing their solutions. These can be plotted with [tools/plot_test_problem_solutions.py](https://github.com/SleipnirGroup/Sleipnir/blob/main/tools/plot_test_problem_solutions.py).
-
-## Branding
-
-### Logo
-
-[SVG](https://github.com/SleipnirGroup/Sleipnir/tree/main/logo/sleipnir.svg), [PNG (1000px)](https://github.com/SleipnirGroup/Sleipnir/tree/main/logo/sleipnir_THcolors_1000px.png)<br>
-Font: [Centaur](https://en.wikipedia.org/wiki/Centaur_(typeface))
-
-### Color palette
-
-<table>
-  <tr>
-    <th>Purple</th>
-    <th>Yellow</th>
-  </tr>
-  <tr>
-    <td style="background-color: #6d3d94; color: white;">6D3D94</td>
-    <td style="background-color: #fdb813; color: white;">FDB813</td>
-  </tr>
-</table>
-
+# Sleipnir
+
+![Build](https://github.com/SleipnirGroup/Sleipnir/actions/workflows/build.yml/badge.svg)
+[![C++ Documentation](https://img.shields.io/badge/documentation-c%2B%2B-blue)](https://sleipnirgroup.github.io/Sleipnir/)
+[![Discord](https://img.shields.io/discord/975739302933856277?color=%23738ADB&label=Join%20our%20Discord&logo=discord&logoColor=white)](https://discord.gg/ad2EEZZwsS)
+
+> Sparsity and Linearity-Exploiting Interior-Point solver - Now Internally Readable
+
+Named after Odin's eight-legged horse from Norse mythology, Sleipnir is a linearity-exploiting sparse nonlinear constrained optimization problem solver that uses the interior-point method.
+
+```cpp
+#include <fmt/core.h>
+#include <sleipnir/OptimizationProblem.hpp>
+
+int main() {
+  // Find the x, y pair with the largest product for which x + 3y = 36
+  sleipnir::OptimizationProblem problem;
+
+  auto x = problem.DecisionVariable();
+  auto y = problem.DecisionVariable();
+
+  problem.Maximize(x * y);
+  problem.SubjectTo(x + 3 * y == 36);
+  problem.Solve();
+
+  // x = 18.0, y = 6.0
+  fmt::println("x = {}, y = {}", x.Value(), y.Value());
+}
+```
+
+```python
+#!/usr/bin/env python3
+
+import jormungandr as jmg
+
+
+def main():
+    # Find the x, y pair with the largest product for which x + 3y = 36
+    problem = jmg.optimization.OptimizationProblem()
+
+    x = problem.decision_variable()
+    y = problem.decision_variable()
+
+    problem.maximize(x * y)
+    problem.subject_to(x + 3 * y == 36)
+    problem.solve()
+
+    # x = 18.0, y = 6.0
+    print(f"x = {x.value()}, y = {y.value()}")
+
+
+if __name__ == "__main__":
+    main()
+```
+
+Sleipnir's internals are intended to be readable by those who aren't domain experts with links to explanatory material for its algorithms.
+
+## Benchmarks
+
+<table><tr>
+  <td><img src="flywheel-scalability-results.png" alt="flywheel-scalability-results"/></td>
+  <td><img src="cart-pole-scalability-results.png" alt="cart-pole-scalability-results"/></td>
+</tr><tr>
+  <td>
+    <a href="flywheel-scalability-results-casadi.csv">
+      flywheel-scalability-results-casadi.csv
+    </a><br>
+    <a href="flywheel-scalability-results-sleipnir.csv">
+      flywheel-scalability-results-sleipnir.csv
+    </a>
+  </td>
+  <td>
+    <a href="cart-pole-scalability-results-casadi.csv">
+      cart-pole-scalability-results-casadi.csv
+    </a><br>
+    <a href="cart-pole-scalability-results-sleipnir.csv">
+      cart-pole-scalability-results-sleipnir.csv
+    </a>
+  </td>
+</tr></table>
+
+Generated by [tools/generate-scalability-results.sh](https://github.com/SleipnirGroup/Sleipnir/tree/main/tools/generate-scalability-results.sh) from [benchmarks/scalability](https://github.com/SleipnirGroup/Sleipnir/tree/main/benchmarks/scalability) source on a AMD Ryzen 7 7840U with 64 GB RAM. The following thirdparty software was used in the benchmarks:
+
+* CasADi 3.6.5 (autodiff and NLP solver frontend)
+* Ipopt 3.14.14 (NLP solver backend)
+* MUMPS 5.6.2 (linear solver)
+
+Ipopt uses MUMPS by default because it has free licensing. Commercial linear solvers may be much faster.
+
+### How we improved performance
+
+#### Make more decisions at compile time
+
+During problem setup, equality and inequality constraints are encoded as different types, so the appropriate setup behavior can be selected at compile time via operator overloads.
+
+#### Reuse autodiff computation results that are still valid (aka caching)
+
+The autodiff library automatically records the linearity of every node in the computational graph. Linear functions have constant first derivatives, and quadratic functions have constant second derivatives. The constant derivatives are computed in the initialization phase and reused for all solver iterations. Only nonlinear parts of the computational graph are recomputed during each solver iteration.
+
+For quadratic problems, we compute the Lagrangian Hessian and constraint Jacobians once with no problem structure hints from the user.
+
+#### Use a performant linear algebra library with fast sparse solvers
+
+[Eigen](https://gitlab.com/libeigen/eigen/) provides these. It also has no required dependencies, which makes cross compilation much easier.
+
+#### Use a pool allocator for autodiff expression nodes
+
+This promotes fast allocation/deallocation and good memory locality.
+
+We could mitigate the solver's high last-level-cache miss rate (~42% on the machine above) further by breaking apart the expression nodes into fields that are commonly iterated together. We used to use a tape, which gave computational graph updates linear access patterns, but tapes are monotonic buffers with no way to reclaim storage.
+
+### Running the benchmarks
+
+Benchmark projects are in the [benchmarks folder](https://github.com/SleipnirGroup/Sleipnir/tree/main/benchmarks). To compile and run them, run the following in the repository root:
+```bash
+# Install CasADi and [matplotlib, numpy, scipy] pip packages first
+cmake -B build -S .
+cmake --build build
+./tools/generate-scalability-results.sh
+```
+
+See the contents of `./tools/generate-scalability-results.sh` for how to run specific benchmarks.
+
+## Examples
+
+See the [examples](https://github.com/SleipnirGroup/Sleipnir/tree/main/examples) and [optimization unit tests](https://github.com/SleipnirGroup/Sleipnir/tree/main/test/optimization).
+
+## Dependencies
+
+* C++20 compiler
+  * On Windows, install [Visual Studio Community 2022](https://visualstudio.microsoft.com/vs/community/) and select the C++ programming language during installation
+  * On Linux, install GCC 11 or greater via `sudo apt install gcc`
+  * On macOS, install the Xcode command-line build tools via `xcode-select --install`. Xcode 13 or later is required.
+* [CMake](https://cmake.org/download/) 3.21 or greater
+  * On Windows, install from the link above
+  * On Linux, install via `sudo apt install cmake`
+  * On macOS, install via `brew install cmake`
+* [Python](https://www.python.org/downloads/) 3.11 or greater
+  * On Windows, install from the link above
+  * On Linux, install via `sudo apt install python`
+  * On macOS, install via `brew install python`
+* [Eigen](https://gitlab.com/libeigen/eigen)
+* [fmtlib](https://github.com/fmtlib/fmt) (internal only)
+* [pybind11](https://github.com/pybind/pybind11) (build only)
+* [Catch2](https://github.com/catchorg/Catch2) (tests only)
+
+Library dependencies which aren't installed locally will be automatically downloaded and built by CMake.
+
+If [CasADi](https://github.com/casadi/casadi) is installed locally, the benchmark executables will be built.
+
+## Build instructions
+
+On Windows, open a [Developer PowerShell](https://learn.microsoft.com/en-us/visualstudio/ide/reference/command-prompt-powershell?view=vs-2022). On Linux or macOS, open a Bash shell.
+
+Clone the repository.
+```bash
+git clone git@github.com:SleipnirGroup/Sleipnir
+cd Sleipnir
+```
+
+### C++ library
+
+```bash
+# Configure; automatically downloads library dependencies
+cmake -B build -S .
+
+# Build
+cmake --build build
+
+# Test
+cd build
+ctest
+cd ..
+
+# Install
+cmake --install build --prefix pkgdir
+```
+
+The following build types can be specified via `-DCMAKE_BUILD_TYPE` during CMake configure:
+
+* Debug
+  * Optimizations off
+  * Debug symbols on
+* Release
+  * Optimizations on
+  * Debug symbols off
+* RelWithDebInfo (default)
+  * Release build type, but with debug info
+* MinSizeRel
+  * Minimum size release build
+* Asan
+  * Enables address sanitizer
+* Tsan
+  * Enables thread sanitizer
+* Ubsan
+  * Enables undefined behavior sanitizer
+* Perf
+  * RelWithDebInfo build type, but with frame pointer so perf utility can use it
+
+### Python library
+
+```bash
+# Setup
+pip install --user build
+
+# Build
+python -m build --wheel
+
+# Install
+pip install --user dist/sleipnirgroup_jormungandr-*.whl
+
+# Test
+pytest
+```
+
+## Test diagnostics
+
+Passing the `--enable-diagnostics` flag to the test executable enables solver diagnostic prints.
+
+Some test problems generate CSV files containing their solutions. These can be plotted with [tools/plot_test_problem_solutions.py](https://github.com/SleipnirGroup/Sleipnir/blob/main/tools/plot_test_problem_solutions.py).
+
+## Branding
+
+### Logo
+
+[SVG](https://github.com/SleipnirGroup/Sleipnir/tree/main/logo/sleipnir.svg), [PNG (1000px)](https://github.com/SleipnirGroup/Sleipnir/tree/main/logo/sleipnir_THcolors_1000px.png)<br>
+Font: [Centaur](https://en.wikipedia.org/wiki/Centaur_(typeface))
+
+### Color palette
+
+<table>
+  <tr>
+    <th>Purple</th>
+    <th>Yellow</th>
+  </tr>
+  <tr>
+    <td style="background-color: #6d3d94; color: white;">6D3D94</td>
+    <td style="background-color: #fdb813; color: white;">FDB813</td>
+  </tr>
+</table>
```

