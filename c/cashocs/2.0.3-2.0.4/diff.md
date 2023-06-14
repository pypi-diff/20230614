# Comparing `tmp/cashocs-2.0.3.tar.gz` & `tmp/cashocs-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashocs-2.0.3.tar", last modified: Tue Jun  6 11:57:03 2023, max compression
+gzip compressed data, was "cashocs-2.0.4.tar", last modified: Fri Jun  9 07:11:26 2023, max compression
```

## Comparing `cashocs-2.0.3.tar` & `cashocs-2.0.4.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.947599 cashocs-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-06 11:56:50.000000 cashocs-2.0.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-06 11:57:03.947599 cashocs-2.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    11025 2023-06-06 11:56:50.000000 cashocs-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4546 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs/_cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_cli/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs/_constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/constrained_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_constraints/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_database/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/form_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/function_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/geometry_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_database/parameter_database.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_forms/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/control_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/general_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/shape_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_forms/shape_regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/cost_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.927599 cashocs-2.0.3/cashocs/_optimization/line_search/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/armijo_line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/line_search/polynomial_line_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/optimal_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/box_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/control_variable_abstractions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21515 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimal_control/optimal_control_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/gradient_descent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/l_bfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/ncg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29701 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/optimization_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/shape_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/shape_optimization/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24150 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_optimization/topology_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_optimization/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.931599 cashocs-2.0.3/cashocs/_pde_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/adjoint_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/control_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/hessian_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/pde_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/shape_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_pde_problems/state_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/interpolations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/_utils/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/boundary_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/deformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/mesh_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/mesh_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/geometry/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/io/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/nonlinear_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/newton_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/nonlinear_solvers/picard_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/cashocs/space_mapping/
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/space_mapping/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/space_mapping/optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-06-06 11:56:50.000000 cashocs-2.0.3/cashocs/space_mapping/shape_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.923599 cashocs-2.0.3/cashocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 11:57:03.000000 cashocs-2.0.3/cashocs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.935599 cashocs-2.0.3/demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.915598 cashocs-2.0.3/demos/documented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.911599 cashocs-2.0.3/demos/documented/cashocs_as_solver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/cashocs_as_solver/control_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/cashocs_as_solver/shape_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.911599 cashocs-2.0.3/demos/documented/misc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/misc/xdmf_io/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/misc/xdmf_io/demo_xdmf_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.915598 cashocs-2.0.3/demos/documented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/box_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5441 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/constraints/demo_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/control_boundary_conditions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/dirichlet_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8197 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/heat_equation/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/iterative_solvers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7527 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/monolithic_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6405 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/multiple_variables/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8034 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/neumann_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5100 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/nonlinear_pdes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/picard_iteration/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11379 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/poisson/demo_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/pre_post_callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/scalar_control_tracking/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/sparse_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/state_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6600 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/optimal_control/stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/optimal_control/stokes/demo_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/documented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/custom_scalar_product/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/eikonal_stiffness/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5712 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/inverse_tomography/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/p_laplacian/
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.939599 cashocs-2.0.3/demos/documented/shape_optimization/regularization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5398 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/regularization/demo_regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/remeshing/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9439 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/remeshing/demo_remeshing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/scaling/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/scaling/demo_scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/shape_poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/shape_stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/test_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/undocumented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/undocumented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/optimal_control/different_state_adjoint_spaces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/demos/undocumented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/shape_optimization/custom_functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/demos/undocumented/shape_optimization/pipe_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-06-06 11:56:50.000000 cashocs-2.0.3/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.919599 cashocs-2.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.943599 cashocs-2.0.3/docs/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4747 2023-06-06 11:56:50.000000 cashocs-2.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-06 11:56:50.000000 cashocs-2.0.3/docs/source/jupytext_process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-06-06 11:56:50.000000 cashocs-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:57:03.947599 cashocs-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:57:03.947599 cashocs-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_control_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19518 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_log_level.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_nonlinear_solvers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25328 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_optimal_control_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_optimal_control_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_p_laplacian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_pde_problems.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_picard_iterations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_remeshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_shape_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40742 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_shape_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_shape_optimization_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_topology_optimization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-06-06 11:56:50.000000 cashocs-2.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.703474 cashocs-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-09 07:11:15.000000 cashocs-2.0.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-09 07:11:26.703474 cashocs-2.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11025 2023-06-09 07:11:15.000000 cashocs-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.683474 cashocs-2.0.4/cashocs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4546 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.683474 cashocs-2.0.4/cashocs/_cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_cli/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.683474 cashocs-2.0.4/cashocs/_constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_constraints/constrained_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_constraints/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.683474 cashocs-2.0.4/cashocs/_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_database/form_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_database/function_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_database/geometry_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_database/parameter_database.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.687474 cashocs-2.0.4/cashocs/_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_forms/control_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_forms/form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_forms/general_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_forms/shape_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_forms/shape_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.687474 cashocs-2.0.4/cashocs/_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/cost_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.687474 cashocs-2.0.4/cashocs/_optimization/line_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/line_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/line_search/armijo_line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/line_search/line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/line_search/polynomial_line_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.687474 cashocs-2.0.4/cashocs/_optimization/optimal_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimal_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimal_control/box_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimal_control/control_variable_abstractions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21515 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimal_control/optimal_control_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.687474 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/gradient_descent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/l_bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/ncg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29701 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/optimization_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.687474 cashocs-2.0.4/cashocs/_optimization/shape_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/shape_optimization/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24150 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.691474 cashocs-2.0.4/cashocs/_optimization/topology_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/topology_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_optimization/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.691474 cashocs-2.0.4/cashocs/_pde_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_pde_problems/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_pde_problems/adjoint_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_pde_problems/control_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_pde_problems/hessian_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_pde_problems/pde_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_pde_problems/shape_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_pde_problems/state_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.691474 cashocs-2.0.4/cashocs/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_utils/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_utils/interpolations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/_utils/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.691474 cashocs-2.0.4/cashocs/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/boundary_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/deformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/mesh_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/mesh_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/geometry/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/cashocs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/io/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/io/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/io/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/cashocs/nonlinear_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/nonlinear_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/nonlinear_solvers/linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/nonlinear_solvers/newton_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/nonlinear_solvers/picard_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/cashocs/space_mapping/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/space_mapping/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/space_mapping/optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-06-09 07:11:15.000000 cashocs-2.0.4/cashocs/space_mapping/shape_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.683474 cashocs-2.0.4/cashocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-09 07:11:26.000000 cashocs-2.0.4/cashocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-09 07:11:26.000000 cashocs-2.0.4/cashocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:11:26.000000 cashocs-2.0.4/cashocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 07:11:26.000000 cashocs-2.0.4/cashocs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-09 07:11:26.000000 cashocs-2.0.4/cashocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 07:11:26.000000 cashocs-2.0.4/cashocs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/documented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/documented/cashocs_as_solver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/cashocs_as_solver/control_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/cashocs_as_solver/shape_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7435 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/documented/misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/misc/xdmf_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/misc/xdmf_io/demo_xdmf_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/documented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/box_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5454 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/constraints/demo_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/control_boundary_conditions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/dirichlet_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8210 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/heat_equation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9065 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/iterative_solvers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/monolithic_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6418 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/multiple_variables/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8060 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/neumann_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5126 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/nonlinear_pdes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/picard_iteration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11431 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/poisson/demo_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/pre_post_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/scalar_control_tracking/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/sparse_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3548 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/state_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6613 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.695474 cashocs-2.0.4/demos/documented/optimal_control/stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/optimal_control/stokes/demo_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/documented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/custom_scalar_product/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4286 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/eikonal_stiffness/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5751 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/inverse_tomography/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/p_laplacian/
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/regularization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5411 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/regularization/demo_regularization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/remeshing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9530 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/remeshing/demo_remeshing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/scaling/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/scaling/demo_scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/shape_poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/shape_stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
+-rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)    20027 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/test_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/undocumented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/undocumented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/undocumented/optimal_control/different_state_adjoint_spaces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/demos/undocumented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/undocumented/shape_optimization/custom_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/demos/undocumented/shape_optimization/pipe_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-06-09 07:11:15.000000 cashocs-2.0.4/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.679474 cashocs-2.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.699474 cashocs-2.0.4/docs/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4747 2023-06-09 07:11:15.000000 cashocs-2.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-09 07:11:15.000000 cashocs-2.0.4/docs/source/jupytext_process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-06-09 07:11:15.000000 cashocs-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:11:26.703474 cashocs-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:11:26.703474 cashocs-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_control_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19518 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_log_level.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_nonlinear_solvers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25328 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_optimal_control_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_optimal_control_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_p_laplacian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_pde_problems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_picard_iterations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_remeshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_shape_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40742 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_shape_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_shape_optimization_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_topology_optimization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-06-09 07:11:15.000000 cashocs-2.0.4/tests/test_utils.py
```

### Comparing `cashocs-2.0.3/COPYING` & `cashocs-2.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/PKG-INFO` & `cashocs-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.3
+Version: 2.0.4
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
 Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
```

### Comparing `cashocs-2.0.3/README.rst` & `cashocs-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/__init__.py` & `cashocs-2.0.4/cashocs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from cashocs.io import convert
 from cashocs.io import import_mesh
 from cashocs.io import load_config
 from cashocs.nonlinear_solvers import linear_solve
 from cashocs.nonlinear_solvers import newton_solve
 from cashocs.nonlinear_solvers import picard_iteration
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 __citation__ = """
 @Article{Blauth2021cashocs,
     author   = {Sebastian Blauth},
     journal  = {SoftwareX},
     title    = {{cashocs: A Computational, Adjoint-Based Shape Optimization and
         Optimal Control Software}},
```

### Comparing `cashocs-2.0.3/cashocs/_cli/__init__.py` & `cashocs-2.0.4/cashocs/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_cli/_convert.py` & `cashocs-2.0.4/cashocs/_cli/_convert.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_constraints/__init__.py` & `cashocs-2.0.4/cashocs/_constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_constraints/constrained_problems.py` & `cashocs-2.0.4/cashocs/_constraints/constrained_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_constraints/constraints.py` & `cashocs-2.0.4/cashocs/_constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_constraints/solvers.py` & `cashocs-2.0.4/cashocs/_constraints/solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_database/__init__.py` & `cashocs-2.0.4/cashocs/_database/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_database/database.py` & `cashocs-2.0.4/cashocs/_database/database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_database/form_database.py` & `cashocs-2.0.4/cashocs/_database/form_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_database/function_database.py` & `cashocs-2.0.4/cashocs/_database/function_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_database/geometry_database.py` & `cashocs-2.0.4/cashocs/_database/geometry_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_database/parameter_database.py` & `cashocs-2.0.4/cashocs/_database/parameter_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_exceptions.py` & `cashocs-2.0.4/cashocs/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_forms/__init__.py` & `cashocs-2.0.4/cashocs/_forms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_forms/control_form_handler.py` & `cashocs-2.0.4/cashocs/_forms/control_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_forms/form_handler.py` & `cashocs-2.0.4/cashocs/_forms/form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_forms/general_form_handler.py` & `cashocs-2.0.4/cashocs/_forms/general_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_forms/shape_form_handler.py` & `cashocs-2.0.4/cashocs/_forms/shape_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_forms/shape_regularization.py` & `cashocs-2.0.4/cashocs/_forms/shape_regularization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_loggers.py` & `cashocs-2.0.4/cashocs/_loggers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/__init__.py` & `cashocs-2.0.4/cashocs/_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/cost_functional.py` & `cashocs-2.0.4/cashocs/_optimization/cost_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/line_search/__init__.py` & `cashocs-2.0.4/cashocs/_optimization/line_search/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/line_search/armijo_line_search.py` & `cashocs-2.0.4/cashocs/_optimization/line_search/armijo_line_search.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/line_search/line_search.py` & `cashocs-2.0.4/cashocs/_optimization/line_search/line_search.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/line_search/polynomial_line_search.py` & `cashocs-2.0.4/cashocs/_optimization/line_search/polynomial_line_search.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimal_control/__init__.py` & `cashocs-2.0.4/cashocs/_optimization/optimal_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimal_control/box_constraints.py` & `cashocs-2.0.4/cashocs/_optimization/optimal_control/box_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimal_control/control_variable_abstractions.py` & `cashocs-2.0.4/cashocs/_optimization/optimal_control/control_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimal_control/optimal_control_problem.py` & `cashocs-2.0.4/cashocs/_optimization/optimal_control/optimal_control_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/__init__.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/callback.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/callback.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/gradient_descent.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/l_bfgs.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/l_bfgs.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/ncg.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/ncg.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/newton.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/newton.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_problem.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/optimization_variable_abstractions.py` & `cashocs-2.0.4/cashocs/_optimization/optimization_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/shape_optimization/__init__.py` & `cashocs-2.0.4/cashocs/_optimization/shape_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_optimization_problem.py` & `cashocs-2.0.4/cashocs/_optimization/shape_optimization/shape_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py` & `cashocs-2.0.4/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/topology_optimization/__init__.py` & `cashocs-2.0.4/cashocs/_optimization/topology_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py` & `cashocs-2.0.4/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py` & `cashocs-2.0.4/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_optimization_problem.py` & `cashocs-2.0.4/cashocs/_optimization/topology_optimization/topology_optimization_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         adjoint_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
         gradient_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
         desired_weights: list[float] | None = None,
+        preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]] = None,
     ) -> None:
         r"""Initializes the topology optimization problem.
 
         Args:
             state_forms: The weak form of the state equation (user implemented). Can be
                 either a single UFL form, or a (ordered) list of UFL forms.
             bcs_list: The list of :py:class:`fenics.DirichletBC` objects describing
@@ -128,28 +129,32 @@
                 configuration, section OptimizationRoutine, key gradient_method).
             desired_weights: A list of values for scaling the cost functional terms. If
                 this is supplied, the cost functional has to be given as list of
                 summands. The individual terms are then scaled, so that term `i` has the
                 magnitude of `desired_weights[i]` for the initial iteration. In case
                 that `desired_weights` is `None`, no scaling is performed. Default is
                 `None`.
+            preconditioner_forms: The list of forms for the preconditioner. The default
+                is `None`, so that the preconditioner matrix is the same as the system
+                matrix.
 
         """
         super().__init__(
             state_forms,
             bcs_list,
             cost_functional_form,
             states,
             adjoints,
             config=config,
             initial_guess=initial_guess,
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
             gradient_ksp_options=gradient_ksp_options,
             desired_weights=desired_weights,
+            preconditioner_forms=preconditioner_forms,
         )
 
         self.db.parameter_db.problem_type = "topology"
         self.mesh_parametrization = None
 
         self.levelset_function = levelset_function
         self.topological_derivative_pos = topological_derivative_pos
```

### Comparing `cashocs-2.0.3/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py` & `cashocs-2.0.4/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_optimization/verification.py` & `cashocs-2.0.4/cashocs/_optimization/verification.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_pde_problems/__init__.py` & `cashocs-2.0.4/cashocs/_pde_problems/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_pde_problems/adjoint_problem.py` & `cashocs-2.0.4/cashocs/_pde_problems/adjoint_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_pde_problems/control_gradient_problem.py` & `cashocs-2.0.4/cashocs/_pde_problems/control_gradient_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_pde_problems/hessian_problems.py` & `cashocs-2.0.4/cashocs/_pde_problems/hessian_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_pde_problems/pde_problem.py` & `cashocs-2.0.4/cashocs/_pde_problems/pde_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_pde_problems/shape_gradient_problem.py` & `cashocs-2.0.4/cashocs/_pde_problems/shape_gradient_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_pde_problems/state_problem.py` & `cashocs-2.0.4/cashocs/_pde_problems/state_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_typing.py` & `cashocs-2.0.4/cashocs/_typing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_utils/__init__.py` & `cashocs-2.0.4/cashocs/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_utils/forms.py` & `cashocs-2.0.4/cashocs/_utils/forms.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_utils/helpers.py` & `cashocs-2.0.4/cashocs/_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_utils/interpolations.py` & `cashocs-2.0.4/cashocs/_utils/interpolations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/_utils/linalg.py` & `cashocs-2.0.4/cashocs/_utils/linalg.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/__init__.py` & `cashocs-2.0.4/cashocs/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/boundary_distance.py` & `cashocs-2.0.4/cashocs/geometry/boundary_distance.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/deformations.py` & `cashocs-2.0.4/cashocs/geometry/deformations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/measure.py` & `cashocs-2.0.4/cashocs/geometry/measure.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/mesh.py` & `cashocs-2.0.4/cashocs/geometry/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/mesh_handler.py` & `cashocs-2.0.4/cashocs/geometry/mesh_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/mesh_testing.py` & `cashocs-2.0.4/cashocs/geometry/mesh_testing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/geometry/quality.py` & `cashocs-2.0.4/cashocs/geometry/quality.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/io/__init__.py` & `cashocs-2.0.4/cashocs/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/io/config.py` & `cashocs-2.0.4/cashocs/io/config.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/io/function.py` & `cashocs-2.0.4/cashocs/io/function.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/io/managers.py` & `cashocs-2.0.4/cashocs/io/managers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/io/mesh.py` & `cashocs-2.0.4/cashocs/io/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/io/output.py` & `cashocs-2.0.4/cashocs/io/output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/nonlinear_solvers/__init__.py` & `cashocs-2.0.4/cashocs/nonlinear_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/nonlinear_solvers/linear_solver.py` & `cashocs-2.0.4/cashocs/nonlinear_solvers/linear_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/nonlinear_solvers/newton_solver.py` & `cashocs-2.0.4/cashocs/nonlinear_solvers/newton_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/nonlinear_solvers/picard_solver.py` & `cashocs-2.0.4/cashocs/nonlinear_solvers/picard_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/space_mapping/__init__.py` & `cashocs-2.0.4/cashocs/space_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/space_mapping/optimal_control.py` & `cashocs-2.0.4/cashocs/space_mapping/optimal_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs/space_mapping/shape_optimization.py` & `cashocs-2.0.4/cashocs/space_mapping/shape_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/cashocs.egg-info/PKG-INFO` & `cashocs-2.0.4/cashocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.3
+Version: 2.0.4
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
 Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
```

### Comparing `cashocs-2.0.3/cashocs.egg-info/SOURCES.txt` & `cashocs-2.0.4/cashocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py` & `cashocs-2.0.4/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py` & `cashocs-2.0.4/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 # Note, that we have to call the
 # {py:meth}`get_vector_field <cashocs.ShapeOptimizationProblem.get_vector_field>` method
 # which returns the UFL object corresponding to $\mathcal{V}$ and which is to be used
 # at its place.
 #
 # ::::{hint}
 # Alternatively, one could define the variable {python}`vector_field` as follows
-# :::python
+# :::{code-block} python
 # space = VectorFunctionSpace(mesh, 'CG', 1)
 # vector_field = TestFunction(space)
 # :::
 #
 # which would yield identical results. However, the shorthand via the
 # {py:meth}`get_vector_field <cashocs.ShapeOptimizationProblem.get_vector_field>`
 # is more convenient, as one does not have to remember to define the correct function
```

### Comparing `cashocs-2.0.3/demos/documented/misc/xdmf_io/demo_xdmf_io.py` & `cashocs-2.0.4/demos/documented/misc/xdmf_io/demo_xdmf_io.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/box_constraints/demo_box_constraints.py` & `cashocs-2.0.4/demos/documented/optimal_control/box_constraints/demo_box_constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 # ::::{note}
 # As an alternative way of specifying the box constraints, one can also use regular
 # float or int objects, in case that they are constant. For example, the constraint that
 # we only want to consider positive value for u, i.e., $0 \leq u \leq +\infty$ can be
 # realized via
 #
-# :::python
+# :::{code-block} python
 # u_a = 0
 # u_b = float('inf')
 # cc = [u_a, u_b]
 # :::
 #
 # and completely analogous with {python}`float('-inf')` for no constraint on the lower
 # bound. Moreover, note that the specification of using either constant {python}`float`
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/constraints/demo_constraints.py` & `cashocs-2.0.4/demos/documented/optimal_control/constraints/demo_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py` & `cashocs-2.0.4/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py` & `cashocs-2.0.4/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 # boundary, there are no strongly enforced ones left, and we define
 
 bcs = []
 
 # ::::{hint}
 # Alternatively, we could have also written
 #
-# :::python
+# :::{code-block} python
 # bcs = None
 # :::
 #
 # which yields exactly the same result, i.e., no strongly enforced Dirichlet
 # boundary conditions.
 # ::::
 #
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/heat_equation/demo_heat_equation.py` & `cashocs-2.0.4/demos/documented/optimal_control/heat_equation/demo_heat_equation.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,63 +195,63 @@
             + Constant(0.5 * dt * alpha) * u * u * dx
         )
     )
 
 # ::::{admonition} Description of the for-loop
 # At the beginning, the 'current' time t is determined from {python}`t_array`, and the
 # expression for the desired state is updated to reflect the current time with the code
-# :::python
+# :::{code-block} python
 # t = t_array[k]
 # y_d_expr.t = t
 # :::
 #
 # The following line sets the object {python}`y` to $y_{k+1}$
-# :::python
+# :::{code-block} python
 # y = states[k]
 # :::
 #
 # For the backward difference in the implicit Euler method, we also need $y_{k}$
 # which we define as follows
-# :::python
+# :::{code-block} python
 # if k == 0:
 #     y_prev = Function(V)
 # else:
 #     y_prev = states[k - 1]
 # :::
 #
 # which ensures that $y_0 = 0$, which corresponds to the initial condition
 # $y^{(0)} = 0$. Hence, {python}`y_prev` indeed corresponds to $y_{k}$.
 #
 # Moreover, we get the current control and adjoint state via
-# :::python
+# :::{code-block} python
 # p = adjoints[k]
 # u = controls[k]
 # :::
 #
 # This allows us to define the state equation at time t as
-# :::python
+# :::{code-block} python
 # state_eq = (
 #     Constant(1 / dt) * (y - y_prev) * p * dx
 #     + inner(grad(y), grad(p)) * dx
 #     - u * p * dx
 # )
 # :::
 #
 # This is then appended to the list of state constraints
-# :::python
+# :::{code-block} python
 # e.append(state_eq)
 # :::
 #
 # Further, we also put the current desired state into the respective list, i.e.,
-# :::python
+# :::{code-block} python
 # y_d.append(interpolate(y_d_expr, V))
 # :::
 #
 # Finally, we can define the k-th summand of the cost functional via
-# :::python
+# :::{code-block} python
 # J_list.append(
 #     cashocs.IntegralFunctional(
 #         Constant(0.5 * dt) * (y - y_d[k]) * (y - y_d[k]) * dx
 #         + Constant(0.5 * dt * alpha) * u * u * dx
 #     )
 # )
 # :::
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py` & `cashocs-2.0.4/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,38 +94,38 @@
 # https://petsc.org/release/docs/manualpages/KSP/) and
 # [Preconditioners](
 # https://petsc.org/release/docs/manualpages/PC/). The
 # relevant options for the command line are described under "Options Database Keys".
 #
 # ::::{note}
 # For example, the first line
-# :::python
+# :::{code-block} python
 # "ksp_type": "cg",
 # :::
 #
 # can be found in [KSPSetType](
 # https://petsc.org/release/docs/manualpages/KSP/KSPSetType/)
 # and the corresponding options are shown under [KSPTYPE](
 # https://petsc.org/release/docs/manualpages/KSP/KSPType/).
 # Here, we see that the above line corresponds to using the conjugate gradient method as
 # krylov solver. The following two lines
-# :::python
+# :::{code-block} python
 # "pc_type": "hypre",
 # "pc_hypre_type": "boomeramg",
 # :::
 #
 # specify that we use the algebraic multigrid preconditioner BOOMERAMG from HYPRE.
 # This is documented in [PCSetType](
 # https://petsc.org/release/docs/manualpages/PC/PCSetType/),
 # [PCTYPE](
 # https://petsc.org/release/docs/manualpages/PC/PCType/), and
 # [PCHYPRE](
 # https://petsc.org/release/docs/manualpages/PC/PCHYPRE/).
 # Finally, the last three lines
-# :::python
+# :::{code-block} python
 # "ksp_rtol": 1e-10,
 # "ksp_atol": 1e-13,
 # "ksp_max_it": 100,
 # :::
 #
 # specify that we use a relative tolerance of 1e-10, an absolute one of 1e-13, and
 # at most 100 iterations for each solve of the linear system, cf. [KSPSetTolerances](
@@ -146,20 +146,20 @@
 # As can be seen, we now use a completely different solver, namely MINRES (the minimal
 # residual method) with a jacobi preconditioner. Finally, the tolerances for the adjoint
 # solver can also be rather different from the ones of the state system, as is shown
 # here.
 #
 # ::::{hint}
 # To verify that the options indeed are used, one can supply the option
-# :::python
+# :::{code-block} python
 # 'ksp_view': None,
 # :::
 #
 # which shows the detailed settings of the solvers, and also
-# :::python
+# :::{code-block} python
 # 'ksp_monitor_true_residual': None,
 # :::
 #
 # which prints the residual of the method over its iterations.
 #
 # For multiple state and adjoint systems, one can proceed analogously to
 # {ref}`demo_multiple_variables`, and one has to create a such a list of options for
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py` & `cashocs-2.0.4/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 # Note, that we directly put the control variables {python}`u` and {python}`v` into a
 # list {python}`controls`, which implies that {python}`u` is the first component of the
 # control variable, and {python}`v` the second one.
 #
 # ::::{hint}
 # An alternative way of specifying the controls would be to reuse the mixed function
 # space and use
-# :::python
+# :::{code-block} python
 # controls = Function(V)
 # u, v = split(controls)
 # :::
 #
 # Although this formulation is slightly different (it uses a
 # {py:class}`fenics.Function` for the controls, and not a list) the de-facto behavior of
 # both methods is completely identical, just the interpretation is slightly different
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py` & `cashocs-2.0.4/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,22 +204,22 @@
 # :::
 #
 # ::::{hint}
 # Note, that for the case that we consider control constraints (see
 # {ref}`demo_box_constraints`) or different Hilbert spaces, e.g., for boundary control
 # (see {ref}`demo_neumann_control`), the corresponding control constraints have also to
 # be put into a joint list, i.e.,
-# :::python
+# :::{code-block} python
 # cc_u = [u_a, u_b]
 # cc_v = [v_a, v_b]
 # cc = [cc_u, cc_v]
 # :::
 #
 # and the corresponding scalar products have to be treated analogously, i.e.,
-# :::python
+# :::{code-block} python
 # scalar_product_u = TrialFunction(V)*TestFunction(V)*dx
 # scalar_product_v = TrialFunction(V)*TestFunction(V)*dx
 # scalar_products = [scalar_product_u, scalar_produt_v]
 # :::
 # ::::
 #
 # In summary, to treat multiple (control or state) variables, the
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/neumann_control/demo_neumann_control.py` & `cashocs-2.0.4/demos/documented/optimal_control/neumann_control/demo_neumann_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 # For this problem, we do not have Dirichlet boundary conditions, so that we
 # use
 
 bcs = []
 
 # ::::{hint}
 # Alternatively, we could have also used
-# :::python
+# :::{code-block} python
 # bcs = None
 # :::
 # ::::
 #
 # ### Definition of the cost functional
 #
 # The definition of the cost functional is nearly identical to before,
@@ -107,15 +107,15 @@
 # bilinear form, so that it induces an actual scalar product on the
 # corresponding space.
 #
 # ::::{note}
 # This means, that we could also define an alternative scalar product for
 # {ref}`demo_poisson`, using the space $H^1(\Omega)$ instead of
 # $L^2(\Omega)$ with the following
-# :::python
+# :::{code-block} python
 # scalar_product = (
 #     inner(grad(TrialFunction(V)), grad(TestFunction(V))) * dx
 #     + TrialFunction(V) * TestFunction(V) * dx
 # )
 # :::
 #
 # This allows a great amount of flexibility in the choice of the control space.
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py` & `cashocs-2.0.4/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py` & `cashocs-2.0.4/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/poisson/demo_poisson.py` & `cashocs-2.0.4/demos/documented/optimal_control/poisson/demo_poisson.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,28 +140,28 @@
 
 e = inner(grad(y), grad(p)) * dx - u * p * dx
 
 # ::::{note}
 # For the clasical definition of this weak form with FEniCS
 # one would write the following code
 #
-# :::python
+# :::{code-block} python
 # y = TrialFunction(V)
 # p = TestFunction(V)
 # u = Function(V)
 # a = inner(grad(y), grad(p)) * dx
 # L = u * p * dx
 # :::
 #
 # as this is a linear problem. However, to have greater flexibility
 # we have to treat the problems as being potentially nonlinear.
 # In this case, the classical FEniCS formulation for this as
 # nonlinear problem would be
 #
-# :::python
+# :::{code-block} python
 # y = Function(V)
 # p = TestFunction(V)
 # u = Function(V)
 # F = inner(grad(y), grad(p)) * dx -u * p * dx
 # :::
 #
 # which could then be solved via the {py:func}`fenics.solve` interface. This
@@ -183,15 +183,15 @@
 
 # This creates Dirichlet boundary conditions with value 0 at the
 # boundaries 1,2,3, and 4, i.e., everywhere.
 #
 # ::::{hint}
 # Classically, these boundary conditions could also be defined via
 #
-# :::python
+# :::{code-block} python
 # def boundary(x, on_bdry):
 #     return on_boundary
 # bc = DirichletBC(V, Constant(0), boundary)
 # :::
 #
 # which would yield a single DirichletBC object, instead of the list returned by
 # {py:func}`create_dirichlet_bcs <cashocs.create_dirichlet_bcs>`. Any of the many
@@ -251,15 +251,15 @@
 # - {python}`algorithm` : Specifies which solution algorithm shall be used.
 # - {python}`rtol` : The relative tolerance for the optimization algorithm.
 # - {python}`atol` : The absolute tolerance for the optimization algorithm.
 # - {python}`max_iter` : The maximum amount of iterations that can be carried out.
 #
 # Hence, we could also use the command
 #
-# :::python
+# :::{code-block} python
 # ocp.solve('lbfgs', 1e-3, 0.0, 100)
 # :::
 #
 # to solve the optimization problem with the L-BFGS method, a relative tolerance of
 # {python}`1e-3`, no absolute tolerance, and a maximum of 100 iterations.
 #
 # The possible values for these arguments are the same as {ref}`the corresponding ones
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py` & `cashocs-2.0.4/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 # Finally, we can inject both hooks via
 
 ocp.inject_pre_callback(pre_callback)
 ocp.inject_post_callback(post_callback)
 
 # ::::{note}
 # We can also save one line and use the code
-# :::python
+# :::{code-block} python
 # ocp.inject_pre_post_hook(pre_hook, post_hook)
 # :::
 #
 # which is equivalent to the above two lines.
 # ::::
 #
 # And in the end, we solve the problem with
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py` & `cashocs-2.0.4/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/sparse_control/demo_sparse_control.py` & `cashocs-2.0.4/demos/documented/optimal_control/sparse_control/demo_sparse_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     Constant(0.5) * (y - y_d) * (y - y_d) * dx + Constant(0.5 * alpha) * abs(u) * dx
 )
 
 # ::::{note}
 # Note that for the regularization term we now do not use
 # {python}`Constant(0.5*alpha)*u*u*dx`,  which corresponds to the $L^2(\Omega)$ norm
 # squared, but rather
-# :::python
+# :::{code-block} python
 # Constant(0.5 * alpha) * abs(u) * dx
 # :::
 #
 # which corresponds to the $L^1(\Omega)$ norm. Other than that, the code is identical.
 # ::::
 #
 # We solve the problem analogously to the previous demos
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/state_constraints/demo_state_constraints.py` & `cashocs-2.0.4/demos/documented/optimal_control/state_constraints/demo_state_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 # or {py:class}`fenics.Expression`, and the method would have worked exactly the same,
 # the corresponding object just has to be a valid input for an UFL form.
 # :::
 #
 # ::::{note}
 # We could have also defined the Moreau-Yosida regularization of the inequality
 # constraint directly, with the following code
-# :::python
+# :::{code-block} python
 # J = cashocs.IntegralFunctional(
 #     J_init_form
 #     + Constant(1 / (2 * gamma)) * pow(Max(0, Constant(gamma) * (y - y_bar)), 2) * dx
 # )
 # :::
 #
 # However, this is directly implemented in
```

### Comparing `cashocs-2.0.3/demos/documented/optimal_control/stokes/demo_stokes.py` & `cashocs-2.0.4/demos/documented/optimal_control/stokes/demo_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py` & `cashocs-2.0.4/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 shape_scalar_product = (
     inner((grad(TrialFunction(VCG))), (grad(TestFunction(VCG)))) * dx
     + inner(TrialFunction(VCG), TestFunction(VCG)) * dx
 )
 
 # ::::{note}
 # Note that we cannot use the formulation
-# :::python
+# :::{code-block} python
 # shape_scalar_product = inner((grad(TrialFunction(VCG))), (grad(TestFunction(VCG))))*dx
 # :::
 #
 # as this would not yield a coercive bilinear form for this problem. This is due to
 # the fact that the entire boundary of $\Omega$ is variable. Hence, we actually
 # need this second term.
 # ::::
```

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py` & `cashocs-2.0.4/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 # mu_min = 5e2
 # mu_max = 1.0
 # smooth_mu = false
 # boundaries_dist = [4]
 # :::
 #
 # The first line
-# :::ini
+# :::{code-block} ini
 # use_distance_mu = True
 # :::
 #
 # ensures that the stiffness will be computed based on the distance to the boundary.
 #
 # The next four lines then specify the behavior of this computation. In particular,
 # we have the following behavior for $\mu$
@@ -92,23 +92,23 @@
 # where $\delta$ denotes the distance to the boundary and $\delta_\mathrm{min}$
 # and $\delta_\mathrm{max}$ correspond to {ini}`dist_min` and {ini}`dist_max`,
 # respectively.
 #
 # The values in-between are given by interpolation. Either a linear, continuous
 # interpolation is used, or a smooth $C^1$ interpolation given by a third order
 # polynomial. These can be selected with the option
-# :::ini
+# :::{code-block} ini
 # smooth_mu = False
 # :::
 #
 # where {ini}`smooth_mu = True` uses the third order polynomial, and
 # {ini}`smooth_mu = False` uses the linear function.
 #
 # Finally, the line
-# :::ini
+# :::{code-block} ini
 # boundaries_dist = [4]
 # :::
 #
 # specifies, which boundaries are considered for the distance computation. These are
 # again specified using the boundary markers, as it was previously explained in
 # {ref}`config_shape_shape_gradient`.
 #
```

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py` & `cashocs-2.0.4/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py` & `cashocs-2.0.4/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/regularization/demo_regularization.py` & `cashocs-2.0.4/demos/documented/shape_optimization/regularization/demo_regularization.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 # The resulting regularization terms are then treated by cashocs, but are, except
 # for these definitions in the config file, invisible for the user.
 #
 # ::::{note}
 # cashocs can also treat the last two terms directly, making use of the
 # {py:class}`ScalarTrackingFunctional <cashocs.ScalarTrackingFunctional>`. Therefore,
 # one would use
-# :::python
+# :::{code-block} python
 # J_vol = cashocs.ScalarTrackingFunctional(Constant(1.0) * dx, 1.5, weight=1.0)
 # J_surf = cashocs.ScalarTrackingFunctional(Constant(1.0) * ds, 4.5, weight = 1.0)
 # :::
 #
 # However, cashocs is not able to treat the curvature regularization directly, this can
 # only be achieved via the config file option, see the {ref}`Section Regularization
 # <config_shape_regularization>`.
```

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/remeshing/demo_remeshing.py` & `cashocs-2.0.4/demos/documented/shape_optimization/remeshing/demo_remeshing.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,63 +174,63 @@
 
 
 # ::::{admonition} Description of the {python}`parametrization` function
 #
 # The code inside the {python}`parametrization` function looks nearly identical to the
 # setup of the problem considered in {ref}`demo_shape_poisson`. First, we load the
 # config file and define the mesh with the commands
-# :::python
+# :::{code-block} python
 # config = cashocs.load_config("./config.ini")
 #
 # mesh, subdomains, boundaries, dx, ds, dS = cashocs.import_mesh(mesh_file)
 # :::
 #
 # Then, we define the {py:class}`fenics.FunctionSpace` and the
 # {py:class}`fenics.Function` objects used for the state and adjoint variables
-# :::python
+# :::{code-block} python
 # V = FunctionSpace(mesh, "CG", 1)
 # u = Function(V)
 # p = Function(V)
 # :::
 #
 # In the following lines, we define the UFL form of the right-hand side
-# :::python
+# :::{code-block} python
 # x = SpatialCoordinate(mesh)
 # f = 2.5 * pow(x[0] + 0.4 - pow(x[1], 2), 2) + pow(x[0], 2) + pow(x[1], 2) - 1
 # :::
 #
 # Next, we define the weak form of the PDE constraint and the corresponding boundary
 # conditions
-# :::python
+# :::{code-block} python
 # e = inner(grad(u), grad(p)) * dx - f * p * dx
 # bcs = DirichletBC(V, Constant(0), boundaries, 1)
 # :::
 #
 # and then the cost functional
-# :::python
+# :::{code-block} python
 # J = cashocs.IntegralFunctional(u * dx)
 # :::
 #
 # with this, we have defined all arguments that are required for the
 # {py:class}`cashocs.ShapeOptimizationProblem`. In order to make them usable, we return
 # them in two objects, the first being the tuple {python}`args`, which defines the
 # positional parameters of the {py:class}`cashocs.ShapeOptimizationProblem`. The second
 # return object is the dictionary {python}`kwargs` containing the keyword arguments.
 # These should be usable analogously to {python}`*args` and {python}`**kwargs`, i.e.,
 # the unpacking operators {python}`*` and {python}`**` should yield the respective
 # arguments. In particular, the return values of the {python}`parametrization` function
 # have to be valid inputs so that
-# :::python
+# :::{code-block} python
 # mesh_file = ...
 # args, kwargs = parametrization(mesh_file)
 # sop = cashocs.ShapeOptimizationProblem(*args, **kwargs)
 # :::
 #
 # is well-defined. Therefore, in our code, we write
-# :::python
+# :::{code-block} python
 # args = (e, bcs, J, u, p, boundaries)
 # kwargs = {"config": config}
 #
 # return args, kwargs
 # :::
 # ::::
 #
```

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/scaling/demo_scaling.py` & `cashocs-2.0.4/demos/documented/shape_optimization/scaling/demo_scaling.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py` & `cashocs-2.0.4/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py` & `cashocs-2.0.4/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py` & `cashocs-2.0.4/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,35 +275,35 @@
 # so that the fine model is actually solved and the cost function value is computed
 # during the call to this method.
 #
 # Let us go over some implementation details of the fine model's
 # {py:meth}`solve_and_evaluate
 # <cashocs.space_mapping.shape_optimization.FineModel.solve_and_evaluate>`
 # method, as defined here. First, an iteration counter is incremented with the line
-# :::python
+# :::{code-block} python
 # self.iter += 1
 # :::
 #
 # Next, the fine model mesh is saved to a file. This is done in order to be able to
 # re-import it with the correct physical tags as defined with Gmsh. This is done with
 # the lines
-# :::python
+# :::{code-block} python
 # cashocs.io.write_out_mesh(
 #     self.mesh, "./mesh/mesh.msh", f"./mesh/fine/mesh_{self.iter}.msh"
 # )
 # cashocs.convert(
 #     f"{dir}/mesh/fine/mesh_{self.iter}.msh", f"{dir}/mesh/fine/mesh.xdmf"
 # )
 # mesh, self.subdomains, boundaries, dx, ds, dS = cashocs.import_mesh(
 #     "./mesh/fine/mesh.xdmf"
 # )
 # :::
 #
 # In the following lines, the fine model state constraint is defined and then solved
-# :::python
+# :::{code-block} python
 # V = FunctionSpace(mesh, "CG", 1)
 # u = Function(V)
 # u_des = Function(V)
 # v = TestFunction(V)
 # F = (
 #     Constant(self.alpha_1) * dot(grad(u), grad(v)) * dx(1)
 #     + Constant(self.alpha_2) * dot(grad(u), grad(v)) * dx(2)
@@ -313,22 +313,22 @@
 # )
 # bcs = cashocs.create_dirichlet_bcs(V, Constant(0.0), boundaries, [1, 2, 3, 4])
 # cashocs.newton_solve(F, u, bcs, verbose=False)
 # :::
 #
 # After solving the fine model PDE constraint, we re-interpolate the desired state to
 # the current mesh with the line
-# :::python
+# :::{code-block} python
 # LagrangeInterpolator.interpolate(u_des, self.u_des_fixed)
 # :::
 #
 # Here, {python}`u_des` is the desired state on the fine model mesh. Finally, we
 # evaluate the cost functional and store the solution of the PDE constraint with the
 # lines
-# :::python
+# :::{code-block} python
 # self.cost_functional_value = assemble(Constant(0.5) * pow(u - u_des, 2) * dx)
 # self.u = u
 # :::
 # ::::
 #
 # :::{attention}
 # Users have to overwrite the attribute {python}`cost_functional_value` of the fine
```

### Comparing `cashocs-2.0.3/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py` & `cashocs-2.0.4/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -314,95 +314,95 @@
 # {py:meth}`solve_and_evaluate <cashocs.space_mapping.shape_optimization.FineModel.solve_and_evaluate>`
 # method.
 #
 # ::::{admonition} Description of the FineModel
 # Let us investigate the fine model in more details in the following. The fine models
 # initialization starts with a call to its parent's {py:meth}`__init__` method, where
 # the mesh is passed
-# :::python
+# :::{code-block} python
 # super().__init__(mesh)
 # :::
 #
 # Next, a list of tracking goals is defined using the {python}`ctypes` module
-# :::python
+# :::{code-block} python
 # self.tracking_goals = [ctypes.c_double(0.0) for _ in range(5, 8)]
 # :::
 #
 # :::{note}
 # The {python}`ctypes` module allows us to make floats in python mutable, i.e., to
 # behave like pointers. This is needed for the parameter extraction step, where we want
 # to find a coarse model "optimum" which achieves the same flow rates as the current
 # iterate of the fine model. In particular, the list {python}`self.tracking_goals` will
 # be used later as input for the parameter extraction.
 # :::
 #
 # Afterwards, we have standard initializations of an iteration counter, the Reynolds
 # number, the inlet flow rate, and an output list, which will be used to save the
 # progress of the space mapping method
-# :::python
+# :::{code-block} python
 # self.iter = 0
 # self.Re = Re
 # self.q_in = q_in
 # self.output_list = output_list
 # :::
 #
 # Let us now take a look at the core of the fine model, its {py:meth}`solve_and_evaluate
 # <cashocs.space_mapping.shape_optimization.FineModel.solve_and_evaluate>`
 # method. It starts by incrementing the iteration counter
-# :::python
+# :::{code-block} python
 # self.iter += 1
 # :::
 #
 # Next, the current mesh is exported to two Gmsh .msh files. The first is used for a
 # possible post-processing (so that the evolution of the geometries is saved) whereas
 # the second is used to define the fine model mesh
-# :::python
+# :::{code-block} python
 # cashocs.io.write_out_mesh(
 #     self.mesh, "./mesh/mesh.msh", f"./mesh/fine/mesh_{self.iter}.msh"
 # )
 # cashocs.io.write_out_mesh(self.mesh, "./mesh/mesh.msh", f"./mesh/fine/mesh.msh")
 # :::
 #
 # Note that we do not use the same discretization for the fine and coarse model in this
 # problem, but we remesh the geometry of the fine model using a higher resolution. To do
 # so, the following Gmsh command is used, which is invoked via the {python}`subprocess`
 # module
-# :::python
+# :::{code-block} python
 # subprocess.run(
 #     ["gmsh", "./mesh/fine.geo", "-2", "-o", "./mesh/fine/fine.msh"],
 #     check=True,
 #     stdout=subprocess.DEVNULL,
 #     stderr=subprocess.DEVNULL,
 # )
 # :::
 #
 # Finally, the mesh generated with the above command is converted to XDMF with
 # {py:func}`cashocs.convert`
-# :::python
+# :::{code-block} python
 # cashocs.convert("./mesh/fine/fine.msh", "./mesh/fine/fine.xdmf")
 # :::
 #
 # Now that we have the geometry of the problem, it is loaded into python and we define
 # the Taylor-Hood Function Space for the Navier-Stokes system
-# :::python
+# :::{code-block} python
 # mesh, subdomains, boundaries, dx, ds, dS = cashocs.import_mesh(
 #     "./mesh/fine/fine.xdmf"
 # )
 # n = FacetNormal(mesh)
 # v_elem = VectorElement("CG", mesh.ufl_cell(), 2)
 # p_elem = FiniteElement("CG", mesh.ufl_cell(), 1)
 # V = FunctionSpace(mesh, v_elem * p_elem)
 #
 # up = Function(V)
 # u, p = split(up)
 # v, q = TestFunctions(V)
 # :::
 #
 # Next, we define the weak form of the problem and its boundary conditions
-# :::python
+# :::{code-block} python
 # F = (
 #     inner(grad(u), grad(v)) * dx
 #     + Constant(self.Re) * inner(grad(u) * u, v) * dx
 #     - p * div(v) * dx
 #     - q * div(u) * dx
 # )
 #
@@ -413,42 +413,42 @@
 # )
 # bc_out = DirichletBC(V.sub(0).sub(0), Constant(0.0), boundaries, 5)
 # bc_pressure = DirichletBC(V.sub(1), Constant(0.0), boundaries, 5)
 # bcs = [bc_in
 # :::
 #
 # The problem is then solved with {py:func}`<cashocs.newton_solve>`
-# :::python
+# :::{code-block} python
 # cashocs.newton_solve(F, up, bcs, verbose=False)
 # :::
 #
 # Finally, after having solved the problem, we first save the solution for later
 # visualization by
-# :::python
+# :::{code-block} python
 # self.u, p = up.split(True)
 #
 # file = File(f"./pvd/u_{self.iter}.pvd")
 # file.write(self.u)
 # :::
 #
 # Next, we evaluate the cost functional with the lines
-# :::python
+# :::{code-block} python
 # J_list = [
 #     cashocs.ScalarTrackingFunctional(dot(self.u, n) * ds(i), self.q_in / 3)
 #     for i in range(5, 8)
 # ]
 # self.cost_functional_value = cashocs._utils.summation(
 #     [J.evaluate() for J in J_list]
 # )
 # :::
 #
 # Finally, we save the values of the outlet flow rate first to our list
 # {python}`self.output_list` and second to the list {python}`self.tracking_goals`, so
 # that the parameter extraction can see the updated flow rates
-# :::python
+# :::{code-block} python
 # self.flow_values = [assemble(dot(self.u, n) * ds(i)) for i in range(5, 8)]
 # self.output_list.append(self.flow_values)
 #
 # for idx in range(len(self.tracking_goals)):
 #     self.tracking_goals[idx].value = self.flow_values[idx]
 # :::
 #
```

### Comparing `cashocs-2.0.3/demos/test.py` & `cashocs-2.0.4/demos/test.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/test_mpi.py` & `cashocs-2.0.4/demos/test_mpi.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py` & `cashocs-2.0.4/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py` & `cashocs-2.0.4/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/undocumented/shape_optimization/custom_functional/custom_functional.py` & `cashocs-2.0.4/demos/undocumented/shape_optimization/custom_functional/custom_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py` & `cashocs-2.0.4/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/docs/source/conf.py` & `cashocs-2.0.4/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "cashocs"
 copyright = "2020-2023, Sebastian Blauth"
 author = "Sebastian Blauth"
 
 # The full version, including alpha/beta/rc tags
-release = "2.0.3"
+release = "2.0.4"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `cashocs-2.0.3/docs/source/jupytext_process.py` & `cashocs-2.0.4/docs/source/jupytext_process.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/pyproject.toml` & `cashocs-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cashocs"
-version = "2.0.3"
+version = "2.0.4"
 description = "Computational Adjoint-Based Shape Optimization and Optimal Control Software"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
 authors = [
 	{name = "Sebastian Blauth"},
 	{email = "sebastian.blauth@itwm.fraunhofer.de"}
```

### Comparing `cashocs-2.0.3/tests/conftest.py` & `cashocs-2.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_cli.py` & `cashocs-2.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_config.py` & `cashocs-2.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_control_constraints.py` & `cashocs-2.0.4/tests/test_control_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_exceptions.py` & `cashocs-2.0.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_geometry.py` & `cashocs-2.0.4/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_log_level.py` & `cashocs-2.0.4/tests/test_log_level.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_nonlinear_solvers.py` & `cashocs-2.0.4/tests/test_nonlinear_solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_optimal_control.py` & `cashocs-2.0.4/tests/test_optimal_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_optimal_control_multiple.py` & `cashocs-2.0.4/tests/test_optimal_control_multiple.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_optimal_control_space_mapping.py` & `cashocs-2.0.4/tests/test_optimal_control_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_output.py` & `cashocs-2.0.4/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_p_laplacian.py` & `cashocs-2.0.4/tests/test_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_pde_problems.py` & `cashocs-2.0.4/tests/test_pde_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_picard_iterations.py` & `cashocs-2.0.4/tests/test_picard_iterations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_remeshing.py` & `cashocs-2.0.4/tests/test_remeshing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_shape_constraints.py` & `cashocs-2.0.4/tests/test_shape_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_shape_optimization.py` & `cashocs-2.0.4/tests/test_shape_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_shape_optimization_space_mapping.py` & `cashocs-2.0.4/tests/test_shape_optimization_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_topology_optimization.py` & `cashocs-2.0.4/tests/test_topology_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.3/tests/test_utils.py` & `cashocs-2.0.4/tests/test_utils.py`

 * *Files identical despite different names*

