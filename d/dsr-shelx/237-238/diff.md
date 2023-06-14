# Comparing `tmp/dsr_shelx-237.tar.gz` & `tmp/dsr_shelx-238.tar.gz`

## Comparing `dsr_shelx-237.tar` & `dsr_shelx-238.tar`

### file list

```diff
@@ -1,367 +1,380 @@
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/__init__.py
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/afix.py
--rw-r--r--   0        0        0    31800 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/atomhandling.py
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/atoms.py
--rw-r--r--   0        0        0    35671 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/cf3fit.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/constants.py
--rw-r--r--   0        0        0    50345 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/dbfile.py
--rwxr-xr-x   0        0        0      298 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/dsr
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/dsr.bat
--rw-r--r--   0        0        0    20846 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/dsr.py
--rw-r--r--   0        0        0   163958 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/dsr_db.txt
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/dsrparse.py
--rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/elements.py
--rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/export.py
--rw-r--r--   0        0        0    39464 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/misc.py
--rw-r--r--   0        0        0    97821 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/olex_dsr_db.txt
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/options.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/pyperclip.py
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/refine.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/resfile.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/resi.py
--rw-r--r--   0        0        0    21682 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/restraints.py
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/selfupdate.py
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/sql_export.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/terminalsize.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/version.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/fit/LICENSE.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/fit/__init__.py
--rw-r--r--   0        0        0    16846 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/fit/quatfit.py
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/__init__.py
--rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/ctx_base.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/ctx_fp.py
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/ctx_iv.py
--rw-r--r--   0        0        0    49448 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/ctx_mp.py
--rw-r--r--   0        0        0    37730 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/ctx_mp_python.py
--rw-r--r--   0        0        0   280518 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/function_docs.py
--rw-r--r--   0        0        0    29253 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/identification.py
--rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/math2.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/rational.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/usertools.py
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/visualization.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/__init__.py
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/approximation.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/calculus.py
--rw-r--r--   0        0        0    20226 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/differentiation.py
--rw-r--r--   0        0        0    73295 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/extrapolation.py
--rw-r--r--   0        0        0    31135 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/inverselaplace.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/odes.py
--rw-r--r--   0        0        0    32856 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/optimization.py
--rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/polynomials.py
--rw-r--r--   0        0        0    38487 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/calculus/quadrature.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/__init__.py
--rw-r--r--   0        0        0    37938 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/bessel.py
--rw-r--r--   0        0        0    42299 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/elliptic.py
--rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/expintegrals.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/factorials.py
--rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/functions.py
--rw-r--r--   0        0        0    51570 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/hypergeometric.py
--rw-r--r--   0        0        0    16097 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/orthogonal.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/qfunctions.py
--rw-r--r--   0        0        0    46184 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/rszeta.py
--rw-r--r--   0        0        0    37320 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/theta.py
--rw-r--r--   0        0        0    36389 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/zeta.py
--rw-r--r--   0        0        0    30858 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/functions/zetazeros.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/__init__.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/backend.py
--rw-r--r--   0        0        0    71458 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/gammazeta.py
--rw-r--r--   0        0        0    43861 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/libelefun.py
--rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/libhyper.py
--rw-r--r--   0        0        0    16688 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/libintmath.py
--rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/libmpc.py
--rw-r--r--   0        0        0    45022 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/libmpf.py
--rw-r--r--   0        0        0    27622 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/libmp/libmpi.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/matrices/__init__.py
--rw-r--r--   0        0        0    18609 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/matrices/calculus.py
--rw-r--r--   0        0        0    24394 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/matrices/eigen.py
--rw-r--r--   0        0        0    58534 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/matrices/eigen_symmetric.py
--rw-r--r--   0        0        0    26962 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/matrices/linalg.py
--rw-r--r--   0        0        0    32168 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/mpmath/matrices/matrices.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/__init__.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/conftest.py
--rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/convert.py
--rw-r--r--   0        0        0    56245 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/convert_matrix.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/exception.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/lazy_imports.py
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/relabel.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/__init__.py
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/asteroidal.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/boundary.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bridges.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/chains.py
--rw-r--r--   0        0        0    14376 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/chordal.py
--rw-r--r--   0        0        0    26631 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/clique.py
--rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/cluster.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/communicability_alg.py
--rw-r--r--   0        0        0    15869 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/core.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/covering.py
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/cuts.py
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/cycles.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/d_separation.py
--rw-r--r--   0        0        0    36881 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/dag.py
--rw-r--r--   0        0        0    22803 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/distance_measures.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/distance_regular.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/dominance.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/dominating.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/efficiency_measures.py
--rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/euler.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/graph_hashing.py
--rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/graphical.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/hierarchy.py
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/hybrid.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isolate.py
--rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/link_prediction.py
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py
--rw-r--r--   0        0        0    42801 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/matching.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/mis.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/moral.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/non_randomness.py
--rw-r--r--   0        0        0    16320 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/planar_drawing.py
--rw-r--r--   0        0        0    39410 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/planarity.py
--rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/polynomials.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/reciprocity.py
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/regular.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/richclub.py
--rw-r--r--   0        0        0    59768 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/similarity.py
--rw-r--r--   0        0        0    30243 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/simple_paths.py
--rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/smallworld.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/smetric.py
--rw-r--r--   0        0        0    10038 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/sparsifiers.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/structuralholes.py
--rw-r--r--   0        0        0    22926 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/summarization.py
--rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/swap.py
--rw-r--r--   0        0        0    31010 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/threshold.py
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tournament.py
--rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/triads.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/vitality.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/voronoi.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/wiener.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/__init__.py
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/clique.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/connectivity.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/distance_measures.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/dominating_set.py
--rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/kcomponents.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/matching.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/maxcut.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/ramsey.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/steinertree.py
--rw-r--r--   0        0        0    54262 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py
--rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/treewidth.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/__init__.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/connectivity.py
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/correlation.py
--rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/mixing.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/pairs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/__init__.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/basic.py
--rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/centrality.py
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/cluster.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/covering.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/edgelist.py
--rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/generators.py
--rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/matching.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/matrix.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/projection.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/redundancy.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/spectral.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/__init__.py
--rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/betweenness.py
--rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/closeness.py
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py
--rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/degree_alg.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/dispersion.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/eigenvector.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py
--rw-r--r--   0        0        0    27731 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/group.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/harmonic.py
--rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/katz.py
--rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/load.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/percolation.py
--rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/reaching.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/second_order.py
--rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/trophic.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/coloring/__init__.py
--rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py
--rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/__init__.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/asyn_fluid.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/centrality.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/community_utils.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/kclique.py
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/kernighan_lin.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/label_propagation.py
--rw-r--r--   0        0        0    13682 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/louvain.py
--rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/lukes.py
--rw-r--r--   0        0        0    19281 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/modularity_max.py
--rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/community/quality.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/components/__init__.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/components/attracting.py
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/components/biconnected.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/components/connected.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/components/semiconnected.py
--rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/components/strongly_connected.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/components/weakly_connected.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/__init__.py
--rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/connectivity.py
--rw-r--r--   0        0        0    22640 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/cuts.py
--rw-r--r--   0        0        0    14425 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py
--rw-r--r--   0        0        0    43788 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py
--rw-r--r--   0        0        0    20687 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py
--rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/utils.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/__init__.py
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/capacityscaling.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py
--rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/edmondskarp.py
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/gomory_hu.py
--rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/maxflow.py
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/mincost.py
--rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/networksimplex.py
--rw-r--r--   0        0        0    15621 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/preflowpush.py
--rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/utils.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/__init__.py
--rw-r--r--   0        0        0    43599 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/ismags.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py
--rw-r--r--   0        0        0    40556 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py
--rw-r--r--   0        0        0    10936 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py
--rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/link_analysis/__init__.py
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/minors/__init__.py
--rw-r--r--   0        0        0    21714 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/minors/contraction.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/__init__.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/hmn.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/lgc.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/utils.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/__init__.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/all.py
--rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/binary.py
--rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/product.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/unary.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/__init__.py
--rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/astar.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/dense.py
--rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/generic.py
--rw-r--r--   0        0        0    14928 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py
--rw-r--r--   0        0        0    80039 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/__init__.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/beamsearch.py
--rw-r--r--   0        0        0    14161 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py
--rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/edgebfs.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/edgedfs.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/__init__.py
--rw-r--r--   0        0        0    36255 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/branchings.py
--rw-r--r--   0        0        0    12987 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/coding.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/decomposition.py
--rw-r--r--   0        0        0    39261 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/mst.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/operations.py
--rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/recognition.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/__init__.py
--rw-r--r--   0        0        0    15471 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/coreviews.py
--rw-r--r--   0        0        0    44427 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/digraph.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/filters.py
--rw-r--r--   0        0        0    36626 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/function.py
--rw-r--r--   0        0        0    66826 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/graph.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/graphviews.py
--rw-r--r--   0        0        0    35867 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/multidigraph.py
--rw-r--r--   0        0        0    45810 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/multigraph.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/ordered.py
--rw-r--r--   0        0        0    45714 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/classes/reportviews.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/drawing/__init__.py
--rw-r--r--   0        0        0    35778 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/drawing/layout.py
--rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/drawing/nx_agraph.py
--rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/drawing/nx_pydot.py
--rw-r--r--   0        0        0    48373 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/drawing/nx_pylab.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/__init__.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/atlas.dat.gz
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/atlas.py
--rw-r--r--   0        0        0    23801 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/classic.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/cographs.py
--rw-r--r--   0        0        0    34429 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/community.py
--rw-r--r--   0        0        0    29817 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/degree_seq.py
--rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/directed.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/duplication.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/ego.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/expanders.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/geometric.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/harary_graph.py
--rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/internet_as_graphs.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/intersection.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/interval_graph.py
--rw-r--r--   0        0        0    24785 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/joint_degree_seq.py
--rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/lattice.py
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/line.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/mycielski.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/nonisomorphic_trees.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/random_clustered.py
--rw-r--r--   0        0        0    44337 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/random_graphs.py
--rw-r--r--   0        0        0    30426 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/small.py
--rw-r--r--   0        0        0    22759 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/social.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/spectral_graph_forge.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/stochastic.py
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/sudoku.py
--rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/trees.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/generators/triads.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/__init__.py
--rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/algebraicconnectivity.py
--rw-r--r--   0        0        0    15658 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/attrmatrix.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/bethehessianmatrix.py
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/graphmatrix.py
--rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/laplacianmatrix.py
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/modularitymatrix.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/linalg/spectrum.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/__init__.py
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/adjlist.py
--rw-r--r--   0        0        0    14079 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/edgelist.py
--rw-r--r--   0        0        0    39511 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/gexf.py
--rw-r--r--   0        0        0    30016 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/gml.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/gpickle.py
--rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/graph6.py
--rw-r--r--   0        0        0    39163 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/graphml.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/leda.py
--rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/multiline_adjlist.py
--rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/nx_shp.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/nx_yaml.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/p2g.py
--rw-r--r--   0        0        0     8636 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/pajek.py
--rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/sparse6.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/text.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/__init__.py
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/adjacency.py
--rw-r--r--   0        0        0     8142 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/jit.py
--rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/node_link.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/tree.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/testing/__init__.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/testing/test.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/testing/utils.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/__init__.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/contextmanagers.py
--rw-r--r--   0        0        0    46493 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/decorators.py
--rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/heaps.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/mapped_queue.py
--rw-r--r--   0        0        0    20390 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/misc.py
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/random_sequence.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/rcm.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 dsr_shelx-237/dsr_shelx/networkx/utils/union_find.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 dsr_shelx-237/.gitignore
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 dsr_shelx-237/README.md
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dsr_shelx-237/pyproject.toml
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 dsr_shelx-237/PKG-INFO
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dsr_shelx-238/.gitattributes
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 dsr_shelx-238/README
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsr_shelx-238/requirements.txt
+-rw-r--r--   0        0        0  1246304 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c.hkl
+-rw-r--r--   0        0        0    11911 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c.res
+-rw-r--r--   0        0        0    18020 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_final.res
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step0.res
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step1.res
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step2.ins
+-rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21c_step3.res
+-rw-r--r--   0        0        0  1259586 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21n_cf3.hkl
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21n_cf3.ins
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 dsr_shelx-238/example/p21n_cf3.res
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/__init__.py
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/afix.py
+-rw-r--r--   0        0        0    31800 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/atomhandling.py
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/atoms.py
+-rw-r--r--   0        0        0    35671 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/cf3fit.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/constants.py
+-rw-r--r--   0        0        0    50324 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dbfile.py
+-rwxr-xr-x   0        0        0      298 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr.bat
+-rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr.py
+-rw-r--r--   0        0        0   163958 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsr_db.txt
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/dsrparse.py
+-rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/elements.py
+-rw-r--r--   0        0        0    15987 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/export.py
+-rw-r--r--   0        0        0    39464 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/misc.py
+-rw-r--r--   0        0        0    97821 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/olex_dsr_db.txt
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/options.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/pyperclip.py
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/refine.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/resfile.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/resi.py
+-rw-r--r--   0        0        0    21682 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/restraints.py
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/selfupdate.py
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/sql_export.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/terminalsize.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/version.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/fit/LICENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/fit/__init__.py
+-rw-r--r--   0        0        0    16846 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/fit/quatfit.py
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/__init__.py
+-rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_base.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_fp.py
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_iv.py
+-rw-r--r--   0        0        0    49448 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp.py
+-rw-r--r--   0        0        0    37730 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp_python.py
+-rw-r--r--   0        0        0   280518 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/function_docs.py
+-rw-r--r--   0        0        0    29253 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/identification.py
+-rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/math2.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/rational.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/usertools.py
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/visualization.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/__init__.py
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/approximation.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/calculus.py
+-rw-r--r--   0        0        0    20226 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/differentiation.py
+-rw-r--r--   0        0        0    73295 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/extrapolation.py
+-rw-r--r--   0        0        0    31135 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/inverselaplace.py
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/odes.py
+-rw-r--r--   0        0        0    32856 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/optimization.py
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/polynomials.py
+-rw-r--r--   0        0        0    38487 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/calculus/quadrature.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/__init__.py
+-rw-r--r--   0        0        0    37938 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/bessel.py
+-rw-r--r--   0        0        0    42299 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/elliptic.py
+-rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/expintegrals.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/factorials.py
+-rw-r--r--   0        0        0    18100 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/functions.py
+-rw-r--r--   0        0        0    51570 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/hypergeometric.py
+-rw-r--r--   0        0        0    16097 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/orthogonal.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/qfunctions.py
+-rw-r--r--   0        0        0    46184 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/rszeta.py
+-rw-r--r--   0        0        0    37320 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/theta.py
+-rw-r--r--   0        0        0    36389 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/zeta.py
+-rw-r--r--   0        0        0    30858 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/functions/zetazeros.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/__init__.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/backend.py
+-rw-r--r--   0        0        0    71458 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/gammazeta.py
+-rw-r--r--   0        0        0    43861 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libelefun.py
+-rw-r--r--   0        0        0    36624 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libhyper.py
+-rw-r--r--   0        0        0    16688 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libintmath.py
+-rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpc.py
+-rw-r--r--   0        0        0    45022 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpf.py
+-rw-r--r--   0        0        0    27622 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpi.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/__init__.py
+-rw-r--r--   0        0        0    18609 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/calculus.py
+-rw-r--r--   0        0        0    24394 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen.py
+-rw-r--r--   0        0        0    58534 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen_symmetric.py
+-rw-r--r--   0        0        0    26962 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/linalg.py
+-rw-r--r--   0        0        0    32168 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/mpmath/matrices/matrices.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/__init__.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/conftest.py
+-rw-r--r--   0        0        0    15858 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/convert.py
+-rw-r--r--   0        0        0    56245 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/convert_matrix.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/exception.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/lazy_imports.py
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/relabel.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/__init__.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/asteroidal.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/boundary.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bridges.py
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chains.py
+-rw-r--r--   0        0        0    14376 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chordal.py
+-rw-r--r--   0        0        0    26631 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/clique.py
+-rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cluster.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/communicability_alg.py
+-rw-r--r--   0        0        0    15869 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/core.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/covering.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cuts.py
+-rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cycles.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/d_separation.py
+-rw-r--r--   0        0        0    36881 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dag.py
+-rw-r--r--   0        0        0    22803 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_measures.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_regular.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominance.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominating.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/efficiency_measures.py
+-rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/euler.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graph_hashing.py
+-rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graphical.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hierarchy.py
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hybrid.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isolate.py
+-rw-r--r--   0        0        0    19792 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_prediction.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py
+-rw-r--r--   0        0        0    42801 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/matching.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/mis.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/moral.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/non_randomness.py
+-rw-r--r--   0        0        0    16320 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planar_drawing.py
+-rw-r--r--   0        0        0    39410 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planarity.py
+-rw-r--r--   0        0        0    10826 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/polynomials.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/reciprocity.py
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/regular.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/richclub.py
+-rw-r--r--   0        0        0    59768 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/similarity.py
+-rw-r--r--   0        0        0    30243 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/simple_paths.py
+-rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smallworld.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smetric.py
+-rw-r--r--   0        0        0    10038 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/sparsifiers.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/structuralholes.py
+-rw-r--r--   0        0        0    22926 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/summarization.py
+-rw-r--r--   0        0        0     9819 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/swap.py
+-rw-r--r--   0        0        0    31010 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/threshold.py
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tournament.py
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/triads.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/vitality.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/voronoi.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/wiener.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/__init__.py
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clique.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py
+-rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/connectivity.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/distance_measures.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/dominating_set.py
+-rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/kcomponents.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/matching.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/maxcut.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/ramsey.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/steinertree.py
+-rw-r--r--   0        0        0    54262 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py
+-rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/treewidth.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/__init__.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/connectivity.py
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/correlation.py
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/mixing.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/pairs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/__init__.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/basic.py
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/centrality.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/cluster.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/covering.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/edgelist.py
+-rw-r--r--   0        0        0    19961 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/generators.py
+-rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matching.py
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matrix.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/projection.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/redundancy.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/spectral.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/__init__.py
+-rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness.py
+-rw-r--r--   0        0        0     9655 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/closeness.py
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py
+-rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/degree_alg.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/dispersion.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/eigenvector.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py
+-rw-r--r--   0        0        0    27731 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/group.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/harmonic.py
+-rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/katz.py
+-rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/load.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/percolation.py
+-rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/reaching.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/second_order.py
+-rw-r--r--   0        0        0     9506 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/trophic.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/__init__.py
+-rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py
+-rw-r--r--   0        0        0    19573 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/__init__.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/asyn_fluid.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/centrality.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/community_utils.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kclique.py
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kernighan_lin.py
+-rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/label_propagation.py
+-rw-r--r--   0        0        0    13682 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/louvain.py
+-rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/lukes.py
+-rw-r--r--   0        0        0    19281 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/modularity_max.py
+-rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/quality.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/__init__.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/attracting.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/biconnected.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/connected.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/semiconnected.py
+-rw-r--r--   0        0        0    11896 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/strongly_connected.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/weakly_connected.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/__init__.py
+-rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/connectivity.py
+-rw-r--r--   0        0        0    22640 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/cuts.py
+-rw-r--r--   0        0        0    14425 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py
+-rw-r--r--   0        0        0    43788 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py
+-rw-r--r--   0        0        0    20687 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py
+-rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/utils.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/__init__.py
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/capacityscaling.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py
+-rw-r--r--   0        0        0     7956 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/edmondskarp.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/gomory_hu.py
+-rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/maxflow.py
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/mincost.py
+-rw-r--r--   0        0        0    25089 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/networksimplex.py
+-rw-r--r--   0        0        0    15621 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/preflowpush.py
+-rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/utils.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/__init__.py
+-rw-r--r--   0        0        0    43599 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/ismags.py
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py
+-rw-r--r--   0        0        0    40556 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py
+-rw-r--r--   0        0        0    10936 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py
+-rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py
+-rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/__init__.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/__init__.py
+-rw-r--r--   0        0        0    21714 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/contraction.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/__init__.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/hmn.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/lgc.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/utils.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/__init__.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/all.py
+-rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/binary.py
+-rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/product.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/unary.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/__init__.py
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/astar.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/dense.py
+-rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/generic.py
+-rw-r--r--   0        0        0    14928 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py
+-rw-r--r--   0        0        0    80039 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/__init__.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/beamsearch.py
+-rw-r--r--   0        0        0    14161 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py
+-rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgebfs.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgedfs.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/__init__.py
+-rw-r--r--   0        0        0    36255 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/branchings.py
+-rw-r--r--   0        0        0    12987 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/coding.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/decomposition.py
+-rw-r--r--   0        0        0    39261 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/mst.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/operations.py
+-rw-r--r--   0        0        0     7497 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/recognition.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/__init__.py
+-rw-r--r--   0        0        0    15471 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/coreviews.py
+-rw-r--r--   0        0        0    44427 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/digraph.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/filters.py
+-rw-r--r--   0        0        0    36626 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/function.py
+-rw-r--r--   0        0        0    66826 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/graph.py
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/graphviews.py
+-rw-r--r--   0        0        0    35867 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/multidigraph.py
+-rw-r--r--   0        0        0    45810 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/multigraph.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/ordered.py
+-rw-r--r--   0        0        0    45714 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/classes/reportviews.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/__init__.py
+-rw-r--r--   0        0        0    35778 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/layout.py
+-rw-r--r--   0        0        0    15396 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_agraph.py
+-rw-r--r--   0        0        0    14091 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pydot.py
+-rw-r--r--   0        0        0    48373 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pylab.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/__init__.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.dat.gz
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.py
+-rw-r--r--   0        0        0    23801 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/classic.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/cographs.py
+-rw-r--r--   0        0        0    34429 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/community.py
+-rw-r--r--   0        0        0    29817 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/degree_seq.py
+-rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/directed.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/duplication.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/ego.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/expanders.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/geometric.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/harary_graph.py
+-rw-r--r--   0        0        0    14128 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/internet_as_graphs.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/intersection.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/interval_graph.py
+-rw-r--r--   0        0        0    24785 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/joint_degree_seq.py
+-rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/lattice.py
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/line.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/mycielski.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/nonisomorphic_trees.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/random_clustered.py
+-rw-r--r--   0        0        0    44337 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/random_graphs.py
+-rw-r--r--   0        0        0    30426 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/small.py
+-rw-r--r--   0        0        0    22759 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/social.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/spectral_graph_forge.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/stochastic.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/sudoku.py
+-rw-r--r--   0        0        0    14146 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/trees.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/generators/triads.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/__init__.py
+-rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/algebraicconnectivity.py
+-rw-r--r--   0        0        0    15658 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/attrmatrix.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/bethehessianmatrix.py
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/graphmatrix.py
+-rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/laplacianmatrix.py
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/modularitymatrix.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/linalg/spectrum.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/__init__.py
+-rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/adjlist.py
+-rw-r--r--   0        0        0    14079 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/edgelist.py
+-rw-r--r--   0        0        0    39511 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gexf.py
+-rw-r--r--   0        0        0    30016 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gml.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gpickle.py
+-rw-r--r--   0        0        0    11301 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graph6.py
+-rw-r--r--   0        0        0    39163 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graphml.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/leda.py
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/multiline_adjlist.py
+-rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_shp.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_yaml.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/p2g.py
+-rw-r--r--   0        0        0     8636 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/pajek.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/sparse6.py
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/text.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/__init__.py
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/adjacency.py
+-rw-r--r--   0        0        0     8142 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/jit.py
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/node_link.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/tree.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/testing/__init__.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/testing/test.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/testing/utils.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/__init__.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/contextmanagers.py
+-rw-r--r--   0        0        0    46493 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/decorators.py
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/heaps.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/mapped_queue.py
+-rw-r--r--   0        0        0    20390 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/misc.py
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/random_sequence.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/rcm.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 dsr_shelx-238/src/dsr_shelx/networkx/utils/union_find.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 dsr_shelx-238/.gitignore
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 dsr_shelx-238/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 dsr_shelx-238/pyproject.toml
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 dsr_shelx-238/PKG-INFO
```

### Comparing `dsr_shelx-237/dsr_shelx/afix.py` & `dsr_shelx-238/src/dsr_shelx/afix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/atomhandling.py` & `dsr_shelx-238/src/dsr_shelx/atomhandling.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/atoms.py` & `dsr_shelx-238/src/dsr_shelx/atoms.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/cf3fit.py` & `dsr_shelx-238/src/dsr_shelx/cf3fit.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/constants.py` & `dsr_shelx-238/src/dsr_shelx/constants.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/dbfile.py` & `dsr_shelx-238/src/dsr_shelx/dbfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,25 +941,24 @@
         tmp = []
         for line in filehandle:
             if not isinstance(line, str):
                 line = line.decode('ascii')
             tmp.append(line)
         return tmp
 
-    def get_name_from_pdbfile(self):
-        # type: () -> str
+    def get_name_from_pdbfile(self) -> str:
         """
         get the fragment name from the pdbfile.txt file
 
         >>> db = ParseDB('./src/dsr_shelx/dsr_db.txt')
         >>> mog = ImportGRADE('./tests/test-data/ALA.gradeserver_all.tgz', db)
         >>> mog.get_name_from_pdbfile()
         'Alanine'
         """
-        full_name = None
+        full_name = ''
         full_name_regex = re.compile(r'^.*Compound full name.*')
         for line in self._pdbfile:
             if not isinstance(line, str):
                 line = line.decode('ascii')
             if not line:
                 continue
             if full_name_regex.match(line):
```

### Comparing `dsr_shelx-237/dsr_shelx/dsr.bat` & `dsr_shelx-238/src/dsr_shelx/dsr.bat`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/dsr.py` & `dsr_shelx-238/src/dsr_shelx/dsr.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,25 +349,25 @@
             # SADI\n
             same_resi = ["SAME_{} {} > {}\n".format(resi.get_residue_class, new_atomnames[-1], new_atomnames[0])]
         # Adds a "SAME_resiclass firstatom > lastatom" to the afix:
         if not self.options.rigid_group:
             restraints += same_resi
             # if dsrp.resiflag:  # <- Or should I do this?
             restraints += ["SIMU 0.04 0.08 1"]
-        if not options.external_restr:
+        if not self.options.external_restr:
             restraints = remove_duplicate_restraints(self.reslist, restraints, resi.get_residue_class)
         restraints = wrap_headlines(restraints)
         dfx_file_name = ''
         if dsrp.part:
             afix_entry = "PART {}  {}\n".format(dsrp.part, dsrp.occupancy) + afix_entry + "\nPART 0"
         if dsrp.resiflag:
             afix_entry = 'RESI {} {}\n{}\nRESI 0'.format(resi.get_residue_class, resi.get_resinumber, afix_entry)
         if self.options.rigid_group:
             afix_entry = 'AFIX 9\n' + afix_entry
-        if options.external_restr and not self.rigid:
+        if self.options.external_restr and not self.rigid:
             pname, ext = os.path.splitext(basefilename + '.dfix')
             if dsrp.dfix:
                 dfx_file_name = pname + "_dfx" + ext
             else:
                 dfx_file_name = pname + ext
             dfx_file_name = write_dbhead_to_file(dsrp, dfx_file_name, restraints, resi.get_residue_class,
                                                  resi.get_resinumber)
@@ -438,16 +438,15 @@
                 res = getattr(f, attr, *args)(*a, **kw)
             return res
 
         return g
 
 
 def main():
-    global options, dsr
-    options = False
+    options = None
     lstfile = ''
     is_listfile = False
     try:
         lstfile = open('./dsr-log.lst', 'w')
     except IOError:
         pass
     else:
@@ -456,15 +455,15 @@
         is_listfile = True
     try:
         options = OptionsParser(program_name)
         if is_listfile:
             lstfile.write('Python version: {}\n'.format(sys.version))
             lstfile.write("Date: {} \n".format(datetime.now().strftime("%Y-%m-%d %H:%M:%S")))
             lstfile.write(options.__str__())
-        dsr = DSR(options)
+        DSR(options)
     except Exception:
         import platform
 
         if is_listfile:
             lstpath = os.path.abspath(lstfile.name)
             lst = 'the file "{}" \nand '.format(lstpath)
         else:
```

### Comparing `dsr_shelx-237/dsr_shelx/dsr_db.txt` & `dsr_shelx-238/src/dsr_shelx/dsr_db.txt`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/dsrparse.py` & `dsr_shelx-238/src/dsr_shelx/dsrparse.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/elements.py` & `dsr_shelx-238/src/dsr_shelx/elements.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/export.py` & `dsr_shelx-238/src/dsr_shelx/export.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/misc.py` & `dsr_shelx-238/src/dsr_shelx/misc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/olex_dsr_db.txt` & `dsr_shelx-238/src/dsr_shelx/olex_dsr_db.txt`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/options.py` & `dsr_shelx-238/src/dsr_shelx/options.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/pyperclip.py` & `dsr_shelx-238/src/dsr_shelx/pyperclip.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/refine.py` & `dsr_shelx-238/src/dsr_shelx/refine.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/resfile.py` & `dsr_shelx-238/src/dsr_shelx/resfile.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/resi.py` & `dsr_shelx-238/src/dsr_shelx/resi.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/restraints.py` & `dsr_shelx-238/src/dsr_shelx/restraints.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/selfupdate.py` & `dsr_shelx-238/src/dsr_shelx/selfupdate.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/sql_export.py` & `dsr_shelx-238/src/dsr_shelx/sql_export.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/terminalsize.py` & `dsr_shelx-238/src/dsr_shelx/terminalsize.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/fit/LICENSE.txt` & `dsr_shelx-238/src/dsr_shelx/fit/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/fit/quatfit.py` & `dsr_shelx-238/src/dsr_shelx/fit/quatfit.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/__init__.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/ctx_base.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_base.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/ctx_fp.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_fp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/ctx_iv.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_iv.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/ctx_mp.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/ctx_mp_python.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/ctx_mp_python.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/function_docs.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/function_docs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/identification.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/identification.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/math2.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/math2.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/rational.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/rational.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/usertools.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/usertools.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/visualization.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/visualization.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/approximation.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/approximation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/differentiation.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/differentiation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/extrapolation.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/extrapolation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/inverselaplace.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/inverselaplace.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/odes.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/odes.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/optimization.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/optimization.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/polynomials.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/polynomials.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/calculus/quadrature.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/calculus/quadrature.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/bessel.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/bessel.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/elliptic.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/elliptic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/expintegrals.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/expintegrals.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/factorials.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/factorials.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/functions.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/functions.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/hypergeometric.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/orthogonal.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/orthogonal.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/qfunctions.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/qfunctions.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/rszeta.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/rszeta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/theta.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/theta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/zeta.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/zeta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/functions/zetazeros.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/functions/zetazeros.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/__init__.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/backend.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/backend.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/gammazeta.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/gammazeta.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/libelefun.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libelefun.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/libhyper.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libhyper.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/libintmath.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libintmath.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/libmpc.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/libmpf.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpf.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/libmp/libmpi.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/libmp/libmpi.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/matrices/calculus.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/calculus.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/matrices/eigen.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/matrices/eigen_symmetric.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/eigen_symmetric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/matrices/linalg.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/linalg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/mpmath/matrices/matrices.py` & `dsr_shelx-238/src/dsr_shelx/mpmath/matrices/matrices.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/conftest.py` & `dsr_shelx-238/src/dsr_shelx/networkx/conftest.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/convert.py` & `dsr_shelx-238/src/dsr_shelx/networkx/convert.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/convert_matrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/convert_matrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/exception.py` & `dsr_shelx-238/src/dsr_shelx/networkx/exception.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/lazy_imports.py` & `dsr_shelx-238/src/dsr_shelx/networkx/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/relabel.py` & `dsr_shelx-238/src/dsr_shelx/networkx/relabel.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/asteroidal.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/asteroidal.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/boundary.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/boundary.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bridges.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bridges.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/chains.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chains.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/chordal.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/chordal.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/clique.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/clique.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/cluster.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cluster.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/communicability_alg.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/communicability_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/core.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/core.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/covering.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/covering.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/cuts.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cuts.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/cycles.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/cycles.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/d_separation.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/d_separation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/dag.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dag.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/distance_measures.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_measures.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/distance_regular.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/distance_regular.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/dominance.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominance.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/dominating.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/dominating.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/efficiency_measures.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/efficiency_measures.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/euler.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/euler.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/graph_hashing.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graph_hashing.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/graphical.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/graphical.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/hierarchy.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hierarchy.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/hybrid.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/hybrid.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isolate.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isolate.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/link_prediction.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_prediction.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/lowest_common_ancestors.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/matching.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/matching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/mis.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/mis.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/moral.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/moral.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/non_randomness.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/non_randomness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/planar_drawing.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planar_drawing.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/planarity.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/planarity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/polynomials.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/polynomials.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/reciprocity.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/reciprocity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/regular.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/regular.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/richclub.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/richclub.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/similarity.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/similarity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/simple_paths.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/simple_paths.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/smallworld.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smallworld.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/smetric.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/smetric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/sparsifiers.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/sparsifiers.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/structuralholes.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/structuralholes.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/summarization.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/summarization.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/swap.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/swap.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/threshold.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/threshold.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/tournament.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tournament.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/triads.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/triads.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/vitality.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/vitality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/voronoi.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/voronoi.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/wiener.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/wiener.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/clique.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clique.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/clustering_coefficient.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/connectivity.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/connectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/distance_measures.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/distance_measures.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/dominating_set.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/dominating_set.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/kcomponents.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/kcomponents.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/matching.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/matching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/maxcut.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/maxcut.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/ramsey.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/ramsey.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/steinertree.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/steinertree.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/traveling_salesman.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/treewidth.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/treewidth.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/approximation/vertex_cover.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/connectivity.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/connectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/correlation.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/correlation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/mixing.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/mixing.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/neighbor_degree.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/assortativity/pairs.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/assortativity/pairs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/basic.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/basic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/centrality.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/centrality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/cluster.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/cluster.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/covering.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/covering.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/edgelist.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/edgelist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/generators.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/generators.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/matching.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/matrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/matrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/projection.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/projection.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/redundancy.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/redundancy.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/bipartite/spectral.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/bipartite/spectral.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/betweenness.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/betweenness_subset.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/closeness.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/closeness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_betweenness_subset.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/current_flow_closeness.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/degree_alg.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/degree_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/dispersion.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/dispersion.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/eigenvector.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/eigenvector.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/flow_matrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/group.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/group.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/harmonic.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/harmonic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/katz.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/katz.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/load.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/load.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/percolation.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/percolation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/reaching.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/reaching.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/second_order.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/second_order.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/subgraph_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/trophic.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/trophic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/centrality/voterank_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/equitable_coloring.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/coloring/greedy_coloring.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/asyn_fluid.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/asyn_fluid.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/centrality.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/centrality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/community_utils.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/community_utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/kclique.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kclique.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/kernighan_lin.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/kernighan_lin.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/label_propagation.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/label_propagation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/louvain.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/louvain.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/lukes.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/lukes.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/modularity_max.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/modularity_max.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/community/quality.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/community/quality.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/components/attracting.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/attracting.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/components/biconnected.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/biconnected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/components/connected.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/connected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/components/semiconnected.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/semiconnected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/components/strongly_connected.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/strongly_connected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/components/weakly_connected.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/components/weakly_connected.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/connectivity.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/connectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/cuts.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/cuts.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/disjoint_paths.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_augmentation.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/edge_kcomponents.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcomponents.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/kcutsets.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/stoerwagner.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/connectivity/utils.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/connectivity/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/boykovkolmogorov.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/capacityscaling.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/capacityscaling.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/dinitz_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/edmondskarp.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/edmondskarp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/gomory_hu.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/gomory_hu.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/maxflow.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/maxflow.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/mincost.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/mincost.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/networksimplex.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/networksimplex.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/preflowpush.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/preflowpush.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/shortestaugmentingpath.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/flow/utils.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/flow/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/ismags.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/ismags.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/isomorphvf2.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/matchhelpers.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/temporalisomorphvf2.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/tree_isomorphism.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/isomorphism/vf2userfunc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/hits_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/link_analysis/pagerank_alg.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/minors/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/minors/contraction.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/minors/contraction.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/hmn.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/hmn.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/lgc.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/lgc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/node_classification/utils.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/node_classification/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/all.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/all.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/binary.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/binary.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/product.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/product.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/operators/unary.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/operators/unary.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/astar.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/astar.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/dense.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/dense.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/generic.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/generic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/unweighted.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/shortest_paths/weighted.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/beamsearch.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/beamsearch.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/breadth_first_search.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/depth_first_search.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/edgebfs.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgebfs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/traversal/edgedfs.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/traversal/edgedfs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/branchings.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/branchings.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/coding.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/coding.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/decomposition.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/decomposition.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/mst.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/mst.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/operations.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/operations.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/algorithms/tree/recognition.py` & `dsr_shelx-238/src/dsr_shelx/networkx/algorithms/tree/recognition.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/coreviews.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/coreviews.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/digraph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/digraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/filters.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/filters.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/function.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/function.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/graph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/graph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/graphviews.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/graphviews.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/multidigraph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/multidigraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/multigraph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/multigraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/ordered.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/ordered.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/classes/reportviews.py` & `dsr_shelx-238/src/dsr_shelx/networkx/classes/reportviews.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/drawing/layout.py` & `dsr_shelx-238/src/dsr_shelx/networkx/drawing/layout.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/drawing/nx_agraph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_agraph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/drawing/nx_pydot.py` & `dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pydot.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/drawing/nx_pylab.py` & `dsr_shelx-238/src/dsr_shelx/networkx/drawing/nx_pylab.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/atlas.dat.gz` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.dat.gz`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/atlas.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/atlas.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/classic.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/classic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/cographs.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/cographs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/community.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/community.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/degree_seq.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/degree_seq.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/directed.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/directed.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/duplication.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/duplication.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/ego.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/ego.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/expanders.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/expanders.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/geometric.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/geometric.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/harary_graph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/harary_graph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/internet_as_graphs.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/internet_as_graphs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/intersection.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/intersection.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/interval_graph.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/interval_graph.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/joint_degree_seq.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/joint_degree_seq.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/lattice.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/lattice.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/line.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/line.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/mycielski.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/mycielski.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/nonisomorphic_trees.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/nonisomorphic_trees.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/random_clustered.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/random_clustered.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/random_graphs.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/random_graphs.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/small.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/small.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/social.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/social.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/spectral_graph_forge.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/spectral_graph_forge.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/stochastic.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/stochastic.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/sudoku.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/sudoku.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/trees.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/trees.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/generators/triads.py` & `dsr_shelx-238/src/dsr_shelx/networkx/generators/triads.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/algebraicconnectivity.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/algebraicconnectivity.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/attrmatrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/attrmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/bethehessianmatrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/bethehessianmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/graphmatrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/graphmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/laplacianmatrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/laplacianmatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/modularitymatrix.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/modularitymatrix.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/linalg/spectrum.py` & `dsr_shelx-238/src/dsr_shelx/networkx/linalg/spectrum.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/adjlist.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/adjlist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/edgelist.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/edgelist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/gexf.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gexf.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/gml.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gml.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/gpickle.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/gpickle.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/graph6.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graph6.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/graphml.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/graphml.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/leda.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/leda.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/multiline_adjlist.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/multiline_adjlist.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/nx_shp.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_shp.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/nx_yaml.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/nx_yaml.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/p2g.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/p2g.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/pajek.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/pajek.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/sparse6.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/sparse6.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/text.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/text.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/__init__.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/adjacency.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/adjacency.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/cytoscape.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/jit.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/jit.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/node_link.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/node_link.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/readwrite/json_graph/tree.py` & `dsr_shelx-238/src/dsr_shelx/networkx/readwrite/json_graph/tree.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/testing/test.py` & `dsr_shelx-238/src/dsr_shelx/networkx/testing/test.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/testing/utils.py` & `dsr_shelx-238/src/dsr_shelx/networkx/testing/utils.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/contextmanagers.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/decorators.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/heaps.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/heaps.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/mapped_queue.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/mapped_queue.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/misc.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/random_sequence.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/random_sequence.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/rcm.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/rcm.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/dsr_shelx/networkx/utils/union_find.py` & `dsr_shelx-238/src/dsr_shelx/networkx/utils/union_find.py`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/.gitignore` & `dsr_shelx-238/.gitignore`

 * *Files identical despite different names*

### Comparing `dsr_shelx-237/README.md` & `dsr_shelx-238/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,163 +1,187 @@
-00000000: 5b21 5b55 6e69 7420 7465 7374 735d 2868  [![Unit tests](h
-00000010: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000020: 6d2f 646b 7261 747a 6572 742f 4453 522f  m/dkratzert/DSR/
-00000030: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000040: 732f 7079 7468 6f6e 6170 702e 796d 6c2f  s/pythonapp.yml/
-00000050: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-00000060: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00000070: 6b72 6174 7a65 7274 2f44 5352 2f61 6374  kratzert/DSR/act
-00000080: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00000090: 7974 686f 6e61 7070 2e79 6d6c 290a 215b  ythonapp.yml).![
-000000a0: 436f 6e74 7269 6275 7469 6f6e 735d 2868  Contributions](h
-000000b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000000c0: 6473 2e69 6f2f 6261 6467 652f 636f 6e74  ds.io/badge/cont
-000000d0: 7269 6275 7469 6f6e 732d 7765 6c63 6f6d  ributions-welcom
-000000e0: 652d 626c 7565 290a 0a44 5352 0a3d 3d3d  e-blue)..DSR.===
-000000f0: 0a0a 5468 6520 7072 6f67 7261 6d20 4453  ..The program DS
-00000100: 5220 636f 6e73 6973 7473 206f 6620 6120  R consists of a 
-00000110: 7465 7874 2064 6174 6162 6173 6520 7769  text database wi
-00000120: 7468 2066 7261 676d 656e 7473 206f 6620  th fragments of 
-00000130: 6d6f 6c65 6375 6c65 7320 616e 6420 7468  molecules and th
-00000140: 6520 4453 5220 7072 6f67 7261 6d2e 200a  e DSR program. .
-00000150: 4974 2061 6374 7320 6173 2061 2070 7265  It acts as a pre
-00000160: 7072 6f63 6573 736f 7220 666f 7220 5348  processor for SH
-00000170: 454c 584c 202e 7265 7320 6669 6c65 732e  ELXL .res files.
-00000180: 2054 6865 2075 7365 7220 696e 7365 7274   The user insert
-00000190: 7320 6120 7370 6563 6961 6c20 636f 6d6d  s a special comm
-000001a0: 616e 6420 696e 2074 6865 2053 4845 4c58  and in the SHELX
-000001b0: 4c20 2e72 6573 2066 696c 6520 0a61 6e64  L .res file .and
-000001c0: 2074 6865 2044 5352 2070 726f 6772 616d   the DSR program
-000001d0: 2072 6561 6473 2074 6869 7320 696e 666f   reads this info
-000001e0: 726d 6174 696f 6e20 746f 2070 7574 2061  rmation to put a
-000001f0: 206d 6f6c 6563 756c 6520 6f72 2066 7261   molecule or fra
-00000200: 676d 656e 7420 7769 7468 2074 6865 2064  gment with the d
-00000210: 6573 6972 6564 2061 746f 6d73 206f 6e20  esired atoms on 
-00000220: 7468 6520 706f 7369 7469 6f6e 200a 6f66  the position .of
-00000230: 2074 6865 2074 6172 6765 7420 6174 6f6d   the target atom
-00000240: 7320 6f72 2071 2d70 6561 6b73 2069 6e20  s or q-peaks in 
-00000250: 7468 6520 756e 6974 2063 656c 6c2e 2042  the unit cell. B
-00000260: 6f6e 6420 7265 7374 7261 696e 7473 2063  ond restraints c
-00000270: 616e 2062 6520 6569 7468 6572 2061 7070  an be either app
-00000280: 6c69 6564 2066 726f 6d20 7468 6520 6461  lied from the da
-00000290: 7461 6261 7365 2074 6f20 7468 6520 6d6f  tabase to the mo
-000002a0: 6c65 6375 6c65 200a 6f72 2061 7574 6f6d  lecule .or autom
-000002b0: 6174 6963 616c 6c79 2067 656e 6572 6174  atically generat
-000002c0: 6564 2e0a 0a2a 205b 5468 6520 686f 6d65  ed...* [The home
-000002d0: 7061 6765 5d28 6874 7470 733a 2f2f 646b  page](https://dk
-000002e0: 7261 747a 6572 742e 6465 2f64 7372 2e68  ratzert.de/dsr.h
-000002f0: 746d 6c29 0a0a 4920 6170 6f6c 6f67 697a  tml)..I apologiz
-00000300: 6520 666f 7220 7468 6520 6d65 7373 7920  e for the messy 
-00000310: 636f 6465 2e20 5468 6973 2077 6173 206d  code. This was m
-00000320: 7920 6669 7273 7420 6269 6767 6572 2070  y first bigger p
-00000330: 726f 6a65 6374 2e2e 2e0a 0a59 6f75 2068  roject.....You h
-00000340: 6176 6520 6569 7468 6572 2061 2063 6f6d  ave either a com
-00000350: 6d61 6e64 206c 696e 6520 7665 7273 696f  mand line versio
-00000360: 6e3a 0a60 6060 0a43 3a5c 5573 6572 735c  n:.```.C:\Users\
-00000370: 6461 6e69 656c 3e64 7372 0a2d 2d2d 2d2d  daniel>dsr.-----
-00000380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003b0: 2044 2053 2052 202d 2076 3231 3120 2d2d   D S R - v211 --
-000003c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003e0: 2d2d 2d0a 4469 736f 7264 6572 6564 2053  ---.Disordered S
-000003f0: 7472 7563 7475 7265 2052 6566 696e 656d  tructure Refinem
-00000400: 656e 7420 2844 5352 290a 0a45 7861 6d70  ent (DSR)..Examp
-00000410: 6c65 2044 5352 202e 7265 7320 6669 6c65  le DSR .res file
-00000420: 2063 6f6d 6d61 6e64 206c 696e 653a 0a52   command line:.R
-00000430: 454d 2044 5352 2050 5554 2f52 4550 4c41  EM DSR PUT/REPLA
-00000440: 4345 2022 4672 6167 6d65 6e74 2220 5749  CE "Fragment" WI
-00000450: 5448 2043 3120 4332 2043 3320 4f4e 2051  TH C1 C2 C3 ON Q
-00000460: 3120 5132 2051 3320 5041 5254 2031 204f  1 Q2 Q3 PART 1 O
-00000470: 4343 202d 3231 203d 0a20 2052 4553 4920  CC -21 =.  RESI 
-00000480: 4446 4958 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  DFIX.-----------
-00000490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000004e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-000004f0: 2020 5055 543a 2020 2020 204a 7573 7420    PUT:     Just 
-00000500: 7075 7420 7468 6520 6672 6167 6d65 6e74  put the fragment
-00000510: 2073 6f75 7263 6520 6174 6f6d 7320 6865   source atoms he
-00000520: 7265 2e0a 2020 2052 4550 4c41 4345 3a20  re..   REPLACE: 
-00000530: 5265 706c 6163 6520 6174 6f6d 7320 6f66  Replace atoms of
-00000540: 2050 4152 5420 3020 696e 2031 2e33 2041   PART 0 in 1.3 A
-00000550: 2064 6973 7461 6e63 6520 6172 6f75 6e64   distance around
-00000560: 2074 6172 6765 7420 6174 6f6d 732e 0a2d   target atoms..-
-00000570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005d0: 2d2d 2d2d 2d2d 2d2d 0a0a 6f70 7469 6f6e  --------..option
-000005e0: 616c 2061 7267 756d 656e 7473 3a0a 2020  al arguments:.  
-000005f0: 2d68 2c20 2d2d 6865 6c70 2020 2020 2020  -h, --help      
-00000600: 2020 2020 2020 7368 6f77 2074 6869 7320        show this 
-00000610: 6865 6c70 206d 6573 7361 6765 2061 6e64  help message and
-00000620: 2065 7869 740a 2020 2d72 2022 7265 7320   exit.  -r "res 
-00000630: 6669 6c65 2220 5b22 7265 7320 6669 6c65  file" ["res file
-00000640: 2220 2e2e 2e5d 0a20 2020 2020 2020 2020  " ...].         
-00000650: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000660: 6573 2066 696c 6520 7769 7468 2044 5352  es file with DSR
-00000670: 2063 6f6d 6d61 6e64 0a20 202d 7265 2022   command.  -re "
-00000680: 7265 7320 6669 6c65 2220 5b22 7265 7320  res file" ["res 
-00000690: 6669 6c65 2220 2e2e 2e5d 0a20 2020 2020  file" ...].     
-000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006b0: 2020 2072 6573 2066 696c 6520 7769 7468     res file with
-000006c0: 2044 5352 2063 6f6d 6d61 6e64 2028 7772   DSR command (wr
-000006d0: 6974 6520 7265 7374 7261 696e 7473 2074  ite restraints t
-000006e0: 6f20 6578 7465 726e 616c 2066 696c 6529  o external file)
-000006f0: 0a20 202d 6520 2266 7261 676d 656e 7422  .  -e "fragment"
-00000700: 2020 2020 2020 2020 2065 7870 6f72 7420           export 
-00000710: 6672 6167 6d65 6e74 2061 7320 2e72 6573  fragment as .res
-00000720: 2f2e 706e 6720 6669 6c65 0a20 202d 6320  /.png file.  -c 
-00000730: 2266 7261 676d 656e 7422 2020 2020 2020  "fragment"      
-00000740: 2020 2065 7870 6f72 7420 6672 6167 6d65     export fragme
-00000750: 6e74 2074 6f20 636c 6970 626f 6172 640a  nt to clipboard.
-00000760: 2020 2d74 2020 2020 2020 2020 2020 2020    -t            
-00000770: 2020 2020 2020 2020 696e 7665 7274 7320          inverts 
-00000780: 7468 6520 6375 7272 656e 7420 6672 6167  the current frag
-00000790: 6d65 6e74 0a20 202d 6920 2274 677a 2066  ment.  -i "tgz f
-000007a0: 696c 6522 2020 2020 2020 2020 2069 6d70  ile"         imp
-000007b0: 6f72 7420 6120 6672 6167 6d65 6e74 2066  ort a fragment f
-000007c0: 726f 6d20 4752 4144 4520 286e 6565 6473  rom GRADE (needs
-000007d0: 202e 7467 7a20 6669 6c65 290a 2020 2d6c   .tgz file).  -l
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 2020 2020 6c69 7374 206e 616d 6573 206f      list names o
-00000800: 6620 616c 6c20 6461 7461 6261 7365 2065  f all database e
-00000810: 6e74 7269 6573 0a20 202d 7320 2273 7472  ntries.  -s "str
-00000820: 696e 6722 2020 2020 2020 2020 2020 2073  ing"           s
-00000830: 6561 7263 6820 7468 6520 6461 7461 6261  earch the databa
-00000840: 7365 2066 6f72 2061 206e 616d 650a 2020  se for a name.  
-00000850: 2d67 2020 2020 2020 2020 2020 2020 2020  -g              
-00000860: 2020 2020 2020 6b65 6570 2067 726f 7570        keep group
-00000870: 2072 6967 6964 2028 6e6f 2072 6573 7472   rigid (no restr
-00000880: 6169 6e74 7329 0a20 202d 7520 2020 2020  aints).  -u     
-00000890: 2020 2020 2020 2020 2020 2020 2020 2055                 U
-000008a0: 7064 6174 6520 4453 5220 746f 2074 6865  pdate DSR to the
-000008b0: 206d 6f73 7420 6375 7272 656e 7420 7665   most current ve
-000008c0: 7273 696f 6e0a 2020 2d6e 2020 2020 2020  rsion.  -n      
-000008d0: 2020 2020 2020 2020 2020 2020 2020 646f                do
-000008e0: 206e 6f74 2072 6566 696e 6520 6166 7465   not refine afte
-000008f0: 7220 6672 6167 6d65 6e74 2074 7261 6e73  r fragment trans
-00000900: 6665 720a 6060 600a 0a4f 7220 6120 6772  fer.```..Or a gr
-00000910: 6170 6869 6361 6c20 7573 6572 2069 6e74  aphical user int
-00000920: 6572 6661 6365 2069 6e20 5b53 6865 6c58  erface in [ShelX
-00000930: 6c65 5d28 6874 7470 733a 2f2f 7777 772e  le](https://www.
-00000940: 7368 656c 786c 652e 6f72 672f 7368 656c  shelxle.org/shel
-00000950: 782f 6569 6e67 6162 652e 7068 7029 3a0a  x/eingabe.php):.
-00000960: 0a21 5b44 5352 206d 6169 6e20 7769 6e64  .![DSR main wind
-00000970: 6f77 5d28 6874 7470 733a 2f2f 6769 7468  ow](https://gith
-00000980: 7562 2e63 6f6d 2f64 6b72 6174 7a65 7274  ub.com/dkratzert
-00000990: 2f44 5352 2f62 6c6f 622f 6d61 7374 6572  /DSR/blob/master
-000009a0: 2f70 6963 7475 7265 732f 6473 725f 7368  /pictures/dsr_sh
-000009b0: 656c 786c 652e 706e 673f 7261 773d 7472  elxle.png?raw=tr
-000009c0: 7565 290a 0a21 5b44 5352 2065 6469 746f  ue)..![DSR edito
-000009d0: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
-000009e0: 622e 636f 6d2f 646b 7261 747a 6572 742f  b.com/dkratzert/
-000009f0: 4453 522f 626c 6f62 2f6d 6173 7465 722f  DSR/blob/master/
-00000a00: 7069 6374 7572 6573 2f64 7372 5f65 6469  pictures/dsr_edi
-00000a10: 746f 722e 706e 673f 7261 773d 7472 7565  tor.png?raw=true
-00000a20: 290a                                     ).
+00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000010: 2f72 6570 6f6c 6f67 792e 6f72 672f 7072  /repology.org/pr
+00000020: 6f6a 6563 742f 6473 722f 7665 7273 696f  oject/dsr/versio
+00000030: 6e73 223e 0a20 2020 203c 696d 6720 7372  ns">.    <img sr
+00000040: 633d 2268 7474 7073 3a2f 2f72 6570 6f6c  c="https://repol
+00000050: 6f67 792e 6f72 672f 6261 6467 652f 7665  ogy.org/badge/ve
+00000060: 7274 6963 616c 2d61 6c6c 7265 706f 732f  rtical-allrepos/
+00000070: 6473 722e 7376 6722 2061 6c74 3d22 5061  dsr.svg" alt="Pa
+00000080: 636b 6167 696e 6720 7374 6174 7573 2220  ckaging status" 
+00000090: 616c 6967 6e3d 2272 6967 6874 223e 0a3c  align="right">.<
+000000a0: 2f61 3e0a 0a21 5b4c 6174 6573 2052 656c  /a>..![Lates Rel
+000000b0: 6561 7365 5d28 6874 7470 733a 2f2f 696d  ease](https://im
+000000c0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000000d0: 6875 622f 762f 7461 672f 646b 7261 747a  hub/v/tag/dkratz
+000000e0: 6572 742f 4453 523f 6c61 6265 6c3d 5265  ert/DSR?label=Re
+000000f0: 6c65 6173 6529 0a5b 215b 556e 6974 2074  lease).[![Unit t
+00000100: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
+00000110: 7468 7562 2e63 6f6d 2f64 6b72 6174 7a65  thub.com/dkratze
+00000120: 7274 2f44 5352 2f61 6374 696f 6e73 2f77  rt/DSR/actions/w
+00000130: 6f72 6b66 6c6f 7773 2f70 7974 686f 6e61  orkflows/pythona
+00000140: 7070 2e79 6d6c 2f62 6164 6765 2e73 7667  pp.yml/badge.svg
+00000150: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000160: 622e 636f 6d2f 646b 7261 747a 6572 742f  b.com/dkratzert/
+00000170: 4453 522f 6163 7469 6f6e 732f 776f 726b  DSR/actions/work
+00000180: 666c 6f77 732f 7079 7468 6f6e 6170 702e  flows/pythonapp.
+00000190: 796d 6c29 0a21 5b43 6f6e 7472 6962 7574  yml).![Contribut
+000001a0: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
+000001b0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000001c0: 6765 2f63 6f6e 7472 6962 7574 696f 6e73  ge/contributions
+000001d0: 2d77 656c 636f 6d65 2d62 6c75 6529 0a5b  -welcome-blue).[
+000001e0: 215b 5079 5049 2070 6163 6b61 6765 5d28  ![PyPI package](
+000001f0: 6874 7470 733a 2f2f 7265 706f 6c6f 6779  https://repology
+00000200: 2e6f 7267 2f62 6164 6765 2f76 6572 7369  .org/badge/versi
+00000210: 6f6e 2d66 6f72 2d72 6570 6f2f 7079 7069  on-for-repo/pypi
+00000220: 2f70 7974 686f 6e3a 6473 722d 7368 656c  /python:dsr-shel
+00000230: 782e 7376 6729 5d28 6874 7470 733a 2f2f  x.svg)](https://
+00000240: 7265 706f 6c6f 6779 2e6f 7267 2f70 726f  repology.org/pro
+00000250: 6a65 6374 2f70 7974 686f 6e3a 6473 722d  ject/python:dsr-
+00000260: 7368 656c 782f 7665 7273 696f 6e73 290a  shelx/versions).
+00000270: 0a0a 4453 520a 3d3d 3d0a 0a54 6865 2070  ..DSR.===..The p
+00000280: 726f 6772 616d 2044 5352 2063 6f6e 7369  rogram DSR consi
+00000290: 7374 7320 6f66 2061 2074 6578 7420 6461  sts of a text da
+000002a0: 7461 6261 7365 2077 6974 6820 6672 6167  tabase with frag
+000002b0: 6d65 6e74 7320 6f66 206d 6f6c 6563 756c  ments of molecul
+000002c0: 6573 2061 6e64 2074 6865 2044 5352 2070  es and the DSR p
+000002d0: 726f 6772 616d 2e20 0a49 7420 6163 7473  rogram. .It acts
+000002e0: 2061 7320 6120 7072 6570 726f 6365 7373   as a preprocess
+000002f0: 6f72 2066 6f72 2053 4845 4c58 4c20 2e72  or for SHELXL .r
+00000300: 6573 2066 696c 6573 2e20 5468 6520 7573  es files. The us
+00000310: 6572 2069 6e73 6572 7473 2061 2073 7065  er inserts a spe
+00000320: 6369 616c 2063 6f6d 6d61 6e64 2069 6e20  cial command in 
+00000330: 7468 6520 5348 454c 584c 202e 7265 7320  the SHELXL .res 
+00000340: 6669 6c65 200a 616e 6420 7468 6520 4453  file .and the DS
+00000350: 5220 7072 6f67 7261 6d20 7265 6164 7320  R program reads 
+00000360: 7468 6973 2069 6e66 6f72 6d61 7469 6f6e  this information
+00000370: 2074 6f20 7075 7420 6120 6d6f 6c65 6375   to put a molecu
+00000380: 6c65 206f 7220 6672 6167 6d65 6e74 2077  le or fragment w
+00000390: 6974 6820 7468 6520 6465 7369 7265 6420  ith the desired 
+000003a0: 6174 6f6d 7320 6f6e 2074 6865 2070 6f73  atoms on the pos
+000003b0: 6974 696f 6e20 0a6f 6620 7468 6520 7461  ition .of the ta
+000003c0: 7267 6574 2061 746f 6d73 206f 7220 712d  rget atoms or q-
+000003d0: 7065 616b 7320 696e 2074 6865 2075 6e69  peaks in the uni
+000003e0: 7420 6365 6c6c 2e20 426f 6e64 2072 6573  t cell. Bond res
+000003f0: 7472 6169 6e74 7320 6361 6e20 6265 2065  traints can be e
+00000400: 6974 6865 7220 6170 706c 6965 6420 6672  ither applied fr
+00000410: 6f6d 2074 6865 2064 6174 6162 6173 6520  om the database 
+00000420: 746f 2074 6865 206d 6f6c 6563 756c 6520  to the molecule 
+00000430: 0a6f 7220 6175 746f 6d61 7469 6361 6c6c  .or automaticall
+00000440: 7920 6765 6e65 7261 7465 642e 0a0a 2a20  y generated...* 
+00000450: 5b54 6865 2068 6f6d 6570 6167 655d 2868  [The homepage](h
+00000460: 7474 7073 3a2f 2f64 6b72 6174 7a65 7274  ttps://dkratzert
+00000470: 2e64 652f 6473 722e 6874 6d6c 290a 0a49  .de/dsr.html)..I
+00000480: 2061 706f 6c6f 6769 7a65 2066 6f72 2074   apologize for t
+00000490: 6865 206d 6573 7379 2063 6f64 652e 2054  he messy code. T
+000004a0: 6869 7320 7761 7320 6d79 2066 6972 7374  his was my first
+000004b0: 2062 6967 6765 7220 7072 6f6a 6563 742e   bigger project.
+000004c0: 2e2e 0a0a 596f 7520 6861 7665 2065 6974  ....You have eit
+000004d0: 6865 7220 6120 636f 6d6d 616e 6420 6c69  her a command li
+000004e0: 6e65 2076 6572 7369 6f6e 3a0a 6060 600a  ne version:.```.
+000004f0: 433a 5c55 7365 7273 5c64 616e 6965 6c3e  C:\Users\daniel>
+00000500: 6473 720a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  dsr.------------
+00000510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000530: 2d2d 2d2d 2d2d 2d2d 2d20 4420 5320 5220  --------- D S R 
+00000540: 2d20 7632 3131 202d 2d2d 2d2d 2d2d 2d2d  - v211 ---------
+00000550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a44 6973  ------------.Dis
+00000570: 6f72 6465 7265 6420 5374 7275 6374 7572  ordered Structur
+00000580: 6520 5265 6669 6e65 6d65 6e74 2028 4453  e Refinement (DS
+00000590: 5229 0a0a 4578 616d 706c 6520 4453 5220  R)..Example DSR 
+000005a0: 2e72 6573 2066 696c 6520 636f 6d6d 616e  .res file comman
+000005b0: 6420 6c69 6e65 3a0a 5245 4d20 4453 5220  d line:.REM DSR 
+000005c0: 5055 542f 5245 504c 4143 4520 2246 7261  PUT/REPLACE "Fra
+000005d0: 676d 656e 7422 2057 4954 4820 4331 2043  gment" WITH C1 C
+000005e0: 3220 4333 204f 4e20 5131 2051 3220 5133  2 C3 ON Q1 Q2 Q3
+000005f0: 2050 4152 5420 3120 4f43 4320 2d32 3120   PART 1 OCC -21 
+00000600: 3d0a 2020 5245 5349 2044 4649 580a 2d2d  =.  RESI DFIX.--
+00000610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000670: 2d2d 2d2d 2d2d 2d0a 2020 2050 5554 3a20  -------.   PUT: 
+00000680: 2020 2020 4a75 7374 2070 7574 2074 6865      Just put the
+00000690: 2066 7261 676d 656e 7420 736f 7572 6365   fragment source
+000006a0: 2061 746f 6d73 2068 6572 652e 0a20 2020   atoms here..   
+000006b0: 5245 504c 4143 453a 2052 6570 6c61 6365  REPLACE: Replace
+000006c0: 2061 746f 6d73 206f 6620 5041 5254 2030   atoms of PART 0
+000006d0: 2069 6e20 312e 3320 4120 6469 7374 616e   in 1.3 A distan
+000006e0: 6365 2061 726f 756e 6420 7461 7267 6574  ce around target
+000006f0: 2061 746f 6d73 2e0a 2d2d 2d2d 2d2d 2d2d   atoms..--------
+00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000760: 2d0a 0a6f 7074 696f 6e61 6c20 6172 6775  -..optional argu
+00000770: 6d65 6e74 733a 0a20 202d 682c 202d 2d68  ments:.  -h, --h
+00000780: 656c 7020 2020 2020 2020 2020 2020 2073  elp            s
+00000790: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
+000007a0: 7373 6167 6520 616e 6420 6578 6974 0a20  ssage and exit. 
+000007b0: 202d 7220 2272 6573 2066 696c 6522 205b   -r "res file" [
+000007c0: 2272 6573 2066 696c 6522 202e 2e2e 5d0a  "res file" ...].
+000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007e0: 2020 2020 2020 2020 7265 7320 6669 6c65          res file
+000007f0: 2077 6974 6820 4453 5220 636f 6d6d 616e   with DSR comman
+00000800: 640a 2020 2d72 6520 2272 6573 2066 696c  d.  -re "res fil
+00000810: 6522 205b 2272 6573 2066 696c 6522 202e  e" ["res file" .
+00000820: 2e2e 5d0a 2020 2020 2020 2020 2020 2020  ..].            
+00000830: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00000840: 6669 6c65 2077 6974 6820 4453 5220 636f  file with DSR co
+00000850: 6d6d 616e 6420 2877 7269 7465 2072 6573  mmand (write res
+00000860: 7472 6169 6e74 7320 746f 2065 7874 6572  traints to exter
+00000870: 6e61 6c20 6669 6c65 290a 2020 2d65 2022  nal file).  -e "
+00000880: 6672 6167 6d65 6e74 2220 2020 2020 2020  fragment"       
+00000890: 2020 6578 706f 7274 2066 7261 676d 656e    export fragmen
+000008a0: 7420 6173 202e 7265 732f 2e70 6e67 2066  t as .res/.png f
+000008b0: 696c 650a 2020 2d63 2022 6672 6167 6d65  ile.  -c "fragme
+000008c0: 6e74 2220 2020 2020 2020 2020 6578 706f  nt"         expo
+000008d0: 7274 2066 7261 676d 656e 7420 746f 2063  rt fragment to c
+000008e0: 6c69 7062 6f61 7264 0a20 202d 7420 2020  lipboard.  -t   
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 2069 6e76 6572 7473 2074 6865 2063 7572   inverts the cur
+00000910: 7265 6e74 2066 7261 676d 656e 740a 2020  rent fragment.  
+00000920: 2d69 2022 7467 7a20 6669 6c65 2220 2020  -i "tgz file"   
+00000930: 2020 2020 2020 696d 706f 7274 2061 2066        import a f
+00000940: 7261 676d 656e 7420 6672 6f6d 2047 5241  ragment from GRA
+00000950: 4445 2028 6e65 6564 7320 2e74 677a 2066  DE (needs .tgz f
+00000960: 696c 6529 0a20 202d 6c20 2020 2020 2020  ile).  -l       
+00000970: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+00000980: 7420 6e61 6d65 7320 6f66 2061 6c6c 2064  t names of all d
+00000990: 6174 6162 6173 6520 656e 7472 6965 730a  atabase entries.
+000009a0: 2020 2d73 2022 7374 7269 6e67 2220 2020    -s "string"   
+000009b0: 2020 2020 2020 2020 7365 6172 6368 2074          search t
+000009c0: 6865 2064 6174 6162 6173 6520 666f 7220  he database for 
+000009d0: 6120 6e61 6d65 0a20 202d 6720 2020 2020  a name.  -g     
+000009e0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+000009f0: 6565 7020 6772 6f75 7020 7269 6769 6420  eep group rigid 
+00000a00: 286e 6f20 7265 7374 7261 696e 7473 290a  (no restraints).
+00000a10: 2020 2d75 2020 2020 2020 2020 2020 2020    -u            
+00000a20: 2020 2020 2020 2020 5570 6461 7465 2044          Update D
+00000a30: 5352 2074 6f20 7468 6520 6d6f 7374 2063  SR to the most c
+00000a40: 7572 7265 6e74 2076 6572 7369 6f6e 0a20  urrent version. 
+00000a50: 202d 6e20 2020 2020 2020 2020 2020 2020   -n             
+00000a60: 2020 2020 2020 2064 6f20 6e6f 7420 7265         do not re
+00000a70: 6669 6e65 2061 6674 6572 2066 7261 676d  fine after fragm
+00000a80: 656e 7420 7472 616e 7366 6572 0a60 6060  ent transfer.```
+00000a90: 0a0a 4f72 2061 2067 7261 7068 6963 616c  ..Or a graphical
+00000aa0: 2075 7365 7220 696e 7465 7266 6163 6520   user interface 
+00000ab0: 696e 205b 5368 656c 586c 655d 2868 7474  in [ShelXle](htt
+00000ac0: 7073 3a2f 2f77 7777 2e73 6865 6c78 6c65  ps://www.shelxle
+00000ad0: 2e6f 7267 2f73 6865 6c78 2f65 696e 6761  .org/shelx/einga
+00000ae0: 6265 2e70 6870 293a 0a0a 215b 4453 5220  be.php):..![DSR 
+00000af0: 6d61 696e 2077 696e 646f 775d 2868 7474  main window](htt
+00000b00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000b10: 646b 7261 747a 6572 742f 4453 522f 626c  dkratzert/DSR/bl
+00000b20: 6f62 2f6d 6173 7465 722f 7069 6374 7572  ob/master/pictur
+00000b30: 6573 2f64 7372 5f73 6865 6c78 6c65 2e70  es/dsr_shelxle.p
+00000b40: 6e67 3f72 6177 3d74 7275 6529 0a0a 215b  ng?raw=true)..![
+00000b50: 4453 5220 6564 6974 6f72 5d28 6874 7470  DSR editor](http
+00000b60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000b70: 6b72 6174 7a65 7274 2f44 5352 2f62 6c6f  kratzert/DSR/blo
+00000b80: 622f 6d61 7374 6572 2f70 6963 7475 7265  b/master/picture
+00000b90: 732f 6473 725f 6564 6974 6f72 2e70 6e67  s/dsr_editor.png
+00000ba0: 3f72 6177 3d74 7275 6529 0a              ?raw=true).
```

### Comparing `dsr_shelx-237/pyproject.toml` & `dsr_shelx-238/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
+[tool.hatch.metadata.hooks.requirements_txt]
+files = ["requirements.txt"]
+
 [project]
 name = "dsr_shelx"
-version = "237"
+dynamic = ["version", "dependencies"]
 authors = [
     { name = "Daniel Kratzert", email = "dkratzert@gmx.de" },
 ]
 description = "A program to model disorder in small-molecule X-ray structures"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -20,26 +23,27 @@
     "Programming Language :: Python :: 3",
 ]
 
 [project.urls]
 "Homepage" = "https://dkratzert.de/dsr.html"
 "Bug Tracker" = "https://github.com/dkratzert/DSR/issues"
 
+[tool.hatch.version]
+path = "src/dsr_shelx/version.py"
+pattern = "VERSION\\s*=\\s*'(?P<version>\\d+\\.{0,1}\\d{0,1})'"
+
 [tool.hatch.build.targets.sdist]
-only-include = ["src/dsr_shelx"]
-sources = ["src"]
 exclude = [
     "/.github",
     "/pictures",
     "/scripts",
     "/setup",
     "/tests",
     "/manuals",
     "/olex_dsr_db.txt",
     "/requirements-devel.txt",
-    "/requirements.txt",
     "/make_release.sh",
     "/venv*",
 ]
 
 [project.scripts]
 dsr = "dsr_shelx.dsr:main"
```

### Comparing `dsr_shelx-237/PKG-INFO` & `dsr_shelx-238/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6473 725f  : 2.1.Name: dsr_
 00000020: 7368 656c 780a 5665 7273 696f 6e3a 2032  shelx.Version: 2
-00000030: 3337 0a53 756d 6d61 7279 3a20 4120 7072  37.Summary: A pr
+00000030: 3338 0a53 756d 6d61 7279 3a20 4120 7072  38.Summary: A pr
 00000040: 6f67 7261 6d20 746f 206d 6f64 656c 2064  ogram to model d
 00000050: 6973 6f72 6465 7220 696e 2073 6d61 6c6c  isorder in small
 00000060: 2d6d 6f6c 6563 756c 6520 582d 7261 7920  -molecule X-ray 
 00000070: 7374 7275 6374 7572 6573 0a50 726f 6a65  structures.Proje
 00000080: 6374 2d55 524c 3a20 486f 6d65 7061 6765  ct-URL: Homepage
 00000090: 2c20 6874 7470 733a 2f2f 646b 7261 747a  , https://dkratz
 000000a0: 6572 742e 6465 2f64 7372 2e68 746d 6c0a  ert.de/dsr.html.
@@ -32,170 +32,195 @@
 000001f0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
 00000200: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
 00000210: 696e 6565 7269 6e67 203a 3a20 4368 656d  ineering :: Chem
 00000220: 6973 7472 790a 5265 7175 6972 6573 2d50  istry.Requires-P
 00000230: 7974 686f 6e3a 203e 3d33 2e39 0a44 6573  ython: >=3.9.Des
 00000240: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
 00000250: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000260: 646f 776e 0a0a 5b21 5b55 6e69 7420 7465  down..[![Unit te
-00000270: 7374 735d 2868 7474 7073 3a2f 2f67 6974  sts](https://git
-00000280: 6875 622e 636f 6d2f 646b 7261 747a 6572  hub.com/dkratzer
-00000290: 742f 4453 522f 6163 7469 6f6e 732f 776f  t/DSR/actions/wo
-000002a0: 726b 666c 6f77 732f 7079 7468 6f6e 6170  rkflows/pythonap
-000002b0: 702e 796d 6c2f 6261 6467 652e 7376 6729  p.yml/badge.svg)
-000002c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000002d0: 2e63 6f6d 2f64 6b72 6174 7a65 7274 2f44  .com/dkratzert/D
-000002e0: 5352 2f61 6374 696f 6e73 2f77 6f72 6b66  SR/actions/workf
-000002f0: 6c6f 7773 2f70 7974 686f 6e61 7070 2e79  lows/pythonapp.y
-00000300: 6d6c 290a 215b 436f 6e74 7269 6275 7469  ml).![Contributi
-00000310: 6f6e 735d 2868 7474 7073 3a2f 2f69 6d67  ons](https://img
-00000320: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000330: 652f 636f 6e74 7269 6275 7469 6f6e 732d  e/contributions-
-00000340: 7765 6c63 6f6d 652d 626c 7565 290a 0a44  welcome-blue)..D
-00000350: 5352 0a3d 3d3d 0a0a 5468 6520 7072 6f67  SR.===..The prog
-00000360: 7261 6d20 4453 5220 636f 6e73 6973 7473  ram DSR consists
-00000370: 206f 6620 6120 7465 7874 2064 6174 6162   of a text datab
-00000380: 6173 6520 7769 7468 2066 7261 676d 656e  ase with fragmen
-00000390: 7473 206f 6620 6d6f 6c65 6375 6c65 7320  ts of molecules 
-000003a0: 616e 6420 7468 6520 4453 5220 7072 6f67  and the DSR prog
-000003b0: 7261 6d2e 200a 4974 2061 6374 7320 6173  ram. .It acts as
-000003c0: 2061 2070 7265 7072 6f63 6573 736f 7220   a preprocessor 
-000003d0: 666f 7220 5348 454c 584c 202e 7265 7320  for SHELXL .res 
-000003e0: 6669 6c65 732e 2054 6865 2075 7365 7220  files. The user 
-000003f0: 696e 7365 7274 7320 6120 7370 6563 6961  inserts a specia
-00000400: 6c20 636f 6d6d 616e 6420 696e 2074 6865  l command in the
-00000410: 2053 4845 4c58 4c20 2e72 6573 2066 696c   SHELXL .res fil
-00000420: 6520 0a61 6e64 2074 6865 2044 5352 2070  e .and the DSR p
-00000430: 726f 6772 616d 2072 6561 6473 2074 6869  rogram reads thi
-00000440: 7320 696e 666f 726d 6174 696f 6e20 746f  s information to
-00000450: 2070 7574 2061 206d 6f6c 6563 756c 6520   put a molecule 
-00000460: 6f72 2066 7261 676d 656e 7420 7769 7468  or fragment with
-00000470: 2074 6865 2064 6573 6972 6564 2061 746f   the desired ato
-00000480: 6d73 206f 6e20 7468 6520 706f 7369 7469  ms on the positi
-00000490: 6f6e 200a 6f66 2074 6865 2074 6172 6765  on .of the targe
-000004a0: 7420 6174 6f6d 7320 6f72 2071 2d70 6561  t atoms or q-pea
-000004b0: 6b73 2069 6e20 7468 6520 756e 6974 2063  ks in the unit c
-000004c0: 656c 6c2e 2042 6f6e 6420 7265 7374 7261  ell. Bond restra
-000004d0: 696e 7473 2063 616e 2062 6520 6569 7468  ints can be eith
-000004e0: 6572 2061 7070 6c69 6564 2066 726f 6d20  er applied from 
-000004f0: 7468 6520 6461 7461 6261 7365 2074 6f20  the database to 
-00000500: 7468 6520 6d6f 6c65 6375 6c65 200a 6f72  the molecule .or
-00000510: 2061 7574 6f6d 6174 6963 616c 6c79 2067   automatically g
-00000520: 656e 6572 6174 6564 2e0a 0a2a 205b 5468  enerated...* [Th
-00000530: 6520 686f 6d65 7061 6765 5d28 6874 7470  e homepage](http
-00000540: 733a 2f2f 646b 7261 747a 6572 742e 6465  s://dkratzert.de
-00000550: 2f64 7372 2e68 746d 6c29 0a0a 4920 6170  /dsr.html)..I ap
-00000560: 6f6c 6f67 697a 6520 666f 7220 7468 6520  ologize for the 
-00000570: 6d65 7373 7920 636f 6465 2e20 5468 6973  messy code. This
-00000580: 2077 6173 206d 7920 6669 7273 7420 6269   was my first bi
-00000590: 6767 6572 2070 726f 6a65 6374 2e2e 2e0a  gger project....
-000005a0: 0a59 6f75 2068 6176 6520 6569 7468 6572  .You have either
-000005b0: 2061 2063 6f6d 6d61 6e64 206c 696e 6520   a command line 
-000005c0: 7665 7273 696f 6e3a 0a60 6060 0a43 3a5c  version:.```.C:\
-000005d0: 5573 6572 735c 6461 6e69 656c 3e64 7372  Users\daniel>dsr
-000005e0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-000005f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000610: 2d2d 2d2d 2d2d 2044 2053 2052 202d 2076  ------ D S R - v
-00000620: 3231 3120 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  211 ------------
-00000630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000640: 2d2d 2d2d 2d2d 2d2d 2d0a 4469 736f 7264  ---------.Disord
-00000650: 6572 6564 2053 7472 7563 7475 7265 2052  ered Structure R
-00000660: 6566 696e 656d 656e 7420 2844 5352 290a  efinement (DSR).
-00000670: 0a45 7861 6d70 6c65 2044 5352 202e 7265  .Example DSR .re
-00000680: 7320 6669 6c65 2063 6f6d 6d61 6e64 206c  s file command l
-00000690: 696e 653a 0a52 454d 2044 5352 2050 5554  ine:.REM DSR PUT
-000006a0: 2f52 4550 4c41 4345 2022 4672 6167 6d65  /REPLACE "Fragme
-000006b0: 6e74 2220 5749 5448 2043 3120 4332 2043  nt" WITH C1 C2 C
-000006c0: 3320 4f4e 2051 3120 5132 2051 3320 5041  3 ON Q1 Q2 Q3 PA
-000006d0: 5254 2031 204f 4343 202d 3231 203d 0a20  RT 1 OCC -21 =. 
-000006e0: 2052 4553 4920 4446 4958 0a2d 2d2d 2d2d   RESI DFIX.-----
-000006f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000750: 2d2d 2d2d 0a20 2020 5055 543a 2020 2020  ----.   PUT:    
-00000760: 204a 7573 7420 7075 7420 7468 6520 6672   Just put the fr
-00000770: 6167 6d65 6e74 2073 6f75 7263 6520 6174  agment source at
-00000780: 6f6d 7320 6865 7265 2e0a 2020 2052 4550  oms here..   REP
-00000790: 4c41 4345 3a20 5265 706c 6163 6520 6174  LACE: Replace at
-000007a0: 6f6d 7320 6f66 2050 4152 5420 3020 696e  oms of PART 0 in
-000007b0: 2031 2e33 2041 2064 6973 7461 6e63 6520   1.3 A distance 
-000007c0: 6172 6f75 6e64 2074 6172 6765 7420 6174  around target at
-000007d0: 6f6d 732e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  oms..-----------
-000007e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000007f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00000840: 6f70 7469 6f6e 616c 2061 7267 756d 656e  optional argumen
-00000850: 7473 3a0a 2020 2d68 2c20 2d2d 6865 6c70  ts:.  -h, --help
-00000860: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-00000870: 2074 6869 7320 6865 6c70 206d 6573 7361   this help messa
-00000880: 6765 2061 6e64 2065 7869 740a 2020 2d72  ge and exit.  -r
-00000890: 2022 7265 7320 6669 6c65 2220 5b22 7265   "res file" ["re
-000008a0: 7320 6669 6c65 2220 2e2e 2e5d 0a20 2020  s file" ...].   
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 2020 2020 2072 6573 2066 696c 6520 7769       res file wi
-000008d0: 7468 2044 5352 2063 6f6d 6d61 6e64 0a20  th DSR command. 
-000008e0: 202d 7265 2022 7265 7320 6669 6c65 2220   -re "res file" 
-000008f0: 5b22 7265 7320 6669 6c65 2220 2e2e 2e5d  ["res file" ...]
-00000900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000910: 2020 2020 2020 2020 2072 6573 2066 696c           res fil
-00000920: 6520 7769 7468 2044 5352 2063 6f6d 6d61  e with DSR comma
-00000930: 6e64 2028 7772 6974 6520 7265 7374 7261  nd (write restra
-00000940: 696e 7473 2074 6f20 6578 7465 726e 616c  ints to external
-00000950: 2066 696c 6529 0a20 202d 6520 2266 7261   file).  -e "fra
-00000960: 676d 656e 7422 2020 2020 2020 2020 2065  gment"         e
-00000970: 7870 6f72 7420 6672 6167 6d65 6e74 2061  xport fragment a
-00000980: 7320 2e72 6573 2f2e 706e 6720 6669 6c65  s .res/.png file
-00000990: 0a20 202d 6320 2266 7261 676d 656e 7422  .  -c "fragment"
-000009a0: 2020 2020 2020 2020 2065 7870 6f72 7420           export 
-000009b0: 6672 6167 6d65 6e74 2074 6f20 636c 6970  fragment to clip
-000009c0: 626f 6172 640a 2020 2d74 2020 2020 2020  board.  -t      
-000009d0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000009e0: 7665 7274 7320 7468 6520 6375 7272 656e  verts the curren
-000009f0: 7420 6672 6167 6d65 6e74 0a20 202d 6920  t fragment.  -i 
-00000a00: 2274 677a 2066 696c 6522 2020 2020 2020  "tgz file"      
-00000a10: 2020 2069 6d70 6f72 7420 6120 6672 6167     import a frag
-00000a20: 6d65 6e74 2066 726f 6d20 4752 4144 4520  ment from GRADE 
-00000a30: 286e 6565 6473 202e 7467 7a20 6669 6c65  (needs .tgz file
-00000a40: 290a 2020 2d6c 2020 2020 2020 2020 2020  ).  -l          
-00000a50: 2020 2020 2020 2020 2020 6c69 7374 206e            list n
-00000a60: 616d 6573 206f 6620 616c 6c20 6461 7461  ames of all data
-00000a70: 6261 7365 2065 6e74 7269 6573 0a20 202d  base entries.  -
-00000a80: 7320 2273 7472 696e 6722 2020 2020 2020  s "string"      
-00000a90: 2020 2020 2073 6561 7263 6820 7468 6520       search the 
-00000aa0: 6461 7461 6261 7365 2066 6f72 2061 206e  database for a n
-00000ab0: 616d 650a 2020 2d67 2020 2020 2020 2020  ame.  -g        
-00000ac0: 2020 2020 2020 2020 2020 2020 6b65 6570              keep
-00000ad0: 2067 726f 7570 2072 6967 6964 2028 6e6f   group rigid (no
-00000ae0: 2072 6573 7472 6169 6e74 7329 0a20 202d   restraints).  -
-00000af0: 7520 2020 2020 2020 2020 2020 2020 2020  u               
-00000b00: 2020 2020 2055 7064 6174 6520 4453 5220       Update DSR 
-00000b10: 746f 2074 6865 206d 6f73 7420 6375 7272  to the most curr
-00000b20: 656e 7420 7665 7273 696f 6e0a 2020 2d6e  ent version.  -n
-00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b40: 2020 2020 646f 206e 6f74 2072 6566 696e      do not refin
-00000b50: 6520 6166 7465 7220 6672 6167 6d65 6e74  e after fragment
-00000b60: 2074 7261 6e73 6665 720a 6060 600a 0a4f   transfer.```..O
-00000b70: 7220 6120 6772 6170 6869 6361 6c20 7573  r a graphical us
-00000b80: 6572 2069 6e74 6572 6661 6365 2069 6e20  er interface in 
-00000b90: 5b53 6865 6c58 6c65 5d28 6874 7470 733a  [ShelXle](https:
-00000ba0: 2f2f 7777 772e 7368 656c 786c 652e 6f72  //www.shelxle.or
-00000bb0: 672f 7368 656c 782f 6569 6e67 6162 652e  g/shelx/eingabe.
-00000bc0: 7068 7029 3a0a 0a21 5b44 5352 206d 6169  php):..![DSR mai
-00000bd0: 6e20 7769 6e64 6f77 5d28 6874 7470 733a  n window](https:
-00000be0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6b72  //github.com/dkr
-00000bf0: 6174 7a65 7274 2f44 5352 2f62 6c6f 622f  atzert/DSR/blob/
-00000c00: 6d61 7374 6572 2f70 6963 7475 7265 732f  master/pictures/
-00000c10: 6473 725f 7368 656c 786c 652e 706e 673f  dsr_shelxle.png?
-00000c20: 7261 773d 7472 7565 290a 0a21 5b44 5352  raw=true)..![DSR
-00000c30: 2065 6469 746f 725d 2868 7474 7073 3a2f   editor](https:/
-00000c40: 2f67 6974 6875 622e 636f 6d2f 646b 7261  /github.com/dkra
-00000c50: 747a 6572 742f 4453 522f 626c 6f62 2f6d  tzert/DSR/blob/m
-00000c60: 6173 7465 722f 7069 6374 7572 6573 2f64  aster/pictures/d
-00000c70: 7372 5f65 6469 746f 722e 706e 673f 7261  sr_editor.png?ra
-00000c80: 773d 7472 7565 290a                      w=true).
+00000260: 646f 776e 0a0a 3c61 2068 7265 663d 2268  down..<a href="h
+00000270: 7474 7073 3a2f 2f72 6570 6f6c 6f67 792e  ttps://repology.
+00000280: 6f72 672f 7072 6f6a 6563 742f 6473 722f  org/project/dsr/
+00000290: 7665 7273 696f 6e73 223e 0a20 2020 203c  versions">.    <
+000002a0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000002b0: 2f72 6570 6f6c 6f67 792e 6f72 672f 6261  /repology.org/ba
+000002c0: 6467 652f 7665 7274 6963 616c 2d61 6c6c  dge/vertical-all
+000002d0: 7265 706f 732f 6473 722e 7376 6722 2061  repos/dsr.svg" a
+000002e0: 6c74 3d22 5061 636b 6167 696e 6720 7374  lt="Packaging st
+000002f0: 6174 7573 2220 616c 6967 6e3d 2272 6967  atus" align="rig
+00000300: 6874 223e 0a3c 2f61 3e0a 0a21 5b4c 6174  ht">.</a>..![Lat
+00000310: 6573 2052 656c 6561 7365 5d28 6874 7470  es Release](http
+00000320: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000330: 696f 2f67 6974 6875 622f 762f 7461 672f  io/github/v/tag/
+00000340: 646b 7261 747a 6572 742f 4453 523f 6c61  dkratzert/DSR?la
+00000350: 6265 6c3d 5265 6c65 6173 6529 0a5b 215b  bel=Release).[![
+00000360: 556e 6974 2074 6573 7473 5d28 6874 7470  Unit tests](http
+00000370: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000380: 6b72 6174 7a65 7274 2f44 5352 2f61 6374  kratzert/DSR/act
+00000390: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+000003a0: 7974 686f 6e61 7070 2e79 6d6c 2f62 6164  ythonapp.yml/bad
+000003b0: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
+000003c0: 2f67 6974 6875 622e 636f 6d2f 646b 7261  /github.com/dkra
+000003d0: 747a 6572 742f 4453 522f 6163 7469 6f6e  tzert/DSR/action
+000003e0: 732f 776f 726b 666c 6f77 732f 7079 7468  s/workflows/pyth
+000003f0: 6f6e 6170 702e 796d 6c29 0a21 5b43 6f6e  onapp.yml).![Con
+00000400: 7472 6962 7574 696f 6e73 5d28 6874 7470  tributions](http
+00000410: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000420: 696f 2f62 6164 6765 2f63 6f6e 7472 6962  io/badge/contrib
+00000430: 7574 696f 6e73 2d77 656c 636f 6d65 2d62  utions-welcome-b
+00000440: 6c75 6529 0a5b 215b 5079 5049 2070 6163  lue).[![PyPI pac
+00000450: 6b61 6765 5d28 6874 7470 733a 2f2f 7265  kage](https://re
+00000460: 706f 6c6f 6779 2e6f 7267 2f62 6164 6765  pology.org/badge
+00000470: 2f76 6572 7369 6f6e 2d66 6f72 2d72 6570  /version-for-rep
+00000480: 6f2f 7079 7069 2f70 7974 686f 6e3a 6473  o/pypi/python:ds
+00000490: 722d 7368 656c 782e 7376 6729 5d28 6874  r-shelx.svg)](ht
+000004a0: 7470 733a 2f2f 7265 706f 6c6f 6779 2e6f  tps://repology.o
+000004b0: 7267 2f70 726f 6a65 6374 2f70 7974 686f  rg/project/pytho
+000004c0: 6e3a 6473 722d 7368 656c 782f 7665 7273  n:dsr-shelx/vers
+000004d0: 696f 6e73 290a 0a0a 4453 520a 3d3d 3d0a  ions)...DSR.===.
+000004e0: 0a54 6865 2070 726f 6772 616d 2044 5352  .The program DSR
+000004f0: 2063 6f6e 7369 7374 7320 6f66 2061 2074   consists of a t
+00000500: 6578 7420 6461 7461 6261 7365 2077 6974  ext database wit
+00000510: 6820 6672 6167 6d65 6e74 7320 6f66 206d  h fragments of m
+00000520: 6f6c 6563 756c 6573 2061 6e64 2074 6865  olecules and the
+00000530: 2044 5352 2070 726f 6772 616d 2e20 0a49   DSR program. .I
+00000540: 7420 6163 7473 2061 7320 6120 7072 6570  t acts as a prep
+00000550: 726f 6365 7373 6f72 2066 6f72 2053 4845  rocessor for SHE
+00000560: 4c58 4c20 2e72 6573 2066 696c 6573 2e20  LXL .res files. 
+00000570: 5468 6520 7573 6572 2069 6e73 6572 7473  The user inserts
+00000580: 2061 2073 7065 6369 616c 2063 6f6d 6d61   a special comma
+00000590: 6e64 2069 6e20 7468 6520 5348 454c 584c  nd in the SHELXL
+000005a0: 202e 7265 7320 6669 6c65 200a 616e 6420   .res file .and 
+000005b0: 7468 6520 4453 5220 7072 6f67 7261 6d20  the DSR program 
+000005c0: 7265 6164 7320 7468 6973 2069 6e66 6f72  reads this infor
+000005d0: 6d61 7469 6f6e 2074 6f20 7075 7420 6120  mation to put a 
+000005e0: 6d6f 6c65 6375 6c65 206f 7220 6672 6167  molecule or frag
+000005f0: 6d65 6e74 2077 6974 6820 7468 6520 6465  ment with the de
+00000600: 7369 7265 6420 6174 6f6d 7320 6f6e 2074  sired atoms on t
+00000610: 6865 2070 6f73 6974 696f 6e20 0a6f 6620  he position .of 
+00000620: 7468 6520 7461 7267 6574 2061 746f 6d73  the target atoms
+00000630: 206f 7220 712d 7065 616b 7320 696e 2074   or q-peaks in t
+00000640: 6865 2075 6e69 7420 6365 6c6c 2e20 426f  he unit cell. Bo
+00000650: 6e64 2072 6573 7472 6169 6e74 7320 6361  nd restraints ca
+00000660: 6e20 6265 2065 6974 6865 7220 6170 706c  n be either appl
+00000670: 6965 6420 6672 6f6d 2074 6865 2064 6174  ied from the dat
+00000680: 6162 6173 6520 746f 2074 6865 206d 6f6c  abase to the mol
+00000690: 6563 756c 6520 0a6f 7220 6175 746f 6d61  ecule .or automa
+000006a0: 7469 6361 6c6c 7920 6765 6e65 7261 7465  tically generate
+000006b0: 642e 0a0a 2a20 5b54 6865 2068 6f6d 6570  d...* [The homep
+000006c0: 6167 655d 2868 7474 7073 3a2f 2f64 6b72  age](https://dkr
+000006d0: 6174 7a65 7274 2e64 652f 6473 722e 6874  atzert.de/dsr.ht
+000006e0: 6d6c 290a 0a49 2061 706f 6c6f 6769 7a65  ml)..I apologize
+000006f0: 2066 6f72 2074 6865 206d 6573 7379 2063   for the messy c
+00000700: 6f64 652e 2054 6869 7320 7761 7320 6d79  ode. This was my
+00000710: 2066 6972 7374 2062 6967 6765 7220 7072   first bigger pr
+00000720: 6f6a 6563 742e 2e2e 0a0a 596f 7520 6861  oject.....You ha
+00000730: 7665 2065 6974 6865 7220 6120 636f 6d6d  ve either a comm
+00000740: 616e 6420 6c69 6e65 2076 6572 7369 6f6e  and line version
+00000750: 3a0a 6060 600a 433a 5c55 7365 7273 5c64  :.```.C:\Users\d
+00000760: 616e 6965 6c3e 6473 720a 2d2d 2d2d 2d2d  aniel>dsr.------
+00000770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20  --------------- 
+000007a0: 4420 5320 5220 2d20 7632 3131 202d 2d2d  D S R - v211 ---
+000007b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000007c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000007d0: 2d2d 0a44 6973 6f72 6465 7265 6420 5374  --.Disordered St
+000007e0: 7275 6374 7572 6520 5265 6669 6e65 6d65  ructure Refineme
+000007f0: 6e74 2028 4453 5229 0a0a 4578 616d 706c  nt (DSR)..Exampl
+00000800: 6520 4453 5220 2e72 6573 2066 696c 6520  e DSR .res file 
+00000810: 636f 6d6d 616e 6420 6c69 6e65 3a0a 5245  command line:.RE
+00000820: 4d20 4453 5220 5055 542f 5245 504c 4143  M DSR PUT/REPLAC
+00000830: 4520 2246 7261 676d 656e 7422 2057 4954  E "Fragment" WIT
+00000840: 4820 4331 2043 3220 4333 204f 4e20 5131  H C1 C2 C3 ON Q1
+00000850: 2051 3220 5133 2050 4152 5420 3120 4f43   Q2 Q3 PART 1 OC
+00000860: 4320 2d32 3120 3d0a 2020 5245 5349 2044  C -21 =.  RESI D
+00000870: 4649 580a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  FIX.------------
+00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+000008e0: 2050 5554 3a20 2020 2020 4a75 7374 2070   PUT:     Just p
+000008f0: 7574 2074 6865 2066 7261 676d 656e 7420  ut the fragment 
+00000900: 736f 7572 6365 2061 746f 6d73 2068 6572  source atoms her
+00000910: 652e 0a20 2020 5245 504c 4143 453a 2052  e..   REPLACE: R
+00000920: 6570 6c61 6365 2061 746f 6d73 206f 6620  eplace atoms of 
+00000930: 5041 5254 2030 2069 6e20 312e 3320 4120  PART 0 in 1.3 A 
+00000940: 6469 7374 616e 6365 2061 726f 756e 6420  distance around 
+00000950: 7461 7267 6574 2061 746f 6d73 2e0a 2d2d  target atoms..--
+00000960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000009a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000009b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000009c0: 2d2d 2d2d 2d2d 2d0a 0a6f 7074 696f 6e61  -------..optiona
+000009d0: 6c20 6172 6775 6d65 6e74 733a 0a20 202d  l arguments:.  -
+000009e0: 682c 202d 2d68 656c 7020 2020 2020 2020  h, --help       
+000009f0: 2020 2020 2073 686f 7720 7468 6973 2068       show this h
+00000a00: 656c 7020 6d65 7373 6167 6520 616e 6420  elp message and 
+00000a10: 6578 6974 0a20 202d 7220 2272 6573 2066  exit.  -r "res f
+00000a20: 696c 6522 205b 2272 6573 2066 696c 6522  ile" ["res file"
+00000a30: 202e 2e2e 5d0a 2020 2020 2020 2020 2020   ...].          
+00000a40: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000a50: 7320 6669 6c65 2077 6974 6820 4453 5220  s file with DSR 
+00000a60: 636f 6d6d 616e 640a 2020 2d72 6520 2272  command.  -re "r
+00000a70: 6573 2066 696c 6522 205b 2272 6573 2066  es file" ["res f
+00000a80: 696c 6522 202e 2e2e 5d0a 2020 2020 2020  ile" ...].      
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 7265 7320 6669 6c65 2077 6974 6820    res file with 
+00000ab0: 4453 5220 636f 6d6d 616e 6420 2877 7269  DSR command (wri
+00000ac0: 7465 2072 6573 7472 6169 6e74 7320 746f  te restraints to
+00000ad0: 2065 7874 6572 6e61 6c20 6669 6c65 290a   external file).
+00000ae0: 2020 2d65 2022 6672 6167 6d65 6e74 2220    -e "fragment" 
+00000af0: 2020 2020 2020 2020 6578 706f 7274 2066          export f
+00000b00: 7261 676d 656e 7420 6173 202e 7265 732f  ragment as .res/
+00000b10: 2e70 6e67 2066 696c 650a 2020 2d63 2022  .png file.  -c "
+00000b20: 6672 6167 6d65 6e74 2220 2020 2020 2020  fragment"       
+00000b30: 2020 6578 706f 7274 2066 7261 676d 656e    export fragmen
+00000b40: 7420 746f 2063 6c69 7062 6f61 7264 0a20  t to clipboard. 
+00000b50: 202d 7420 2020 2020 2020 2020 2020 2020   -t             
+00000b60: 2020 2020 2020 2069 6e76 6572 7473 2074         inverts t
+00000b70: 6865 2063 7572 7265 6e74 2066 7261 676d  he current fragm
+00000b80: 656e 740a 2020 2d69 2022 7467 7a20 6669  ent.  -i "tgz fi
+00000b90: 6c65 2220 2020 2020 2020 2020 696d 706f  le"         impo
+00000ba0: 7274 2061 2066 7261 676d 656e 7420 6672  rt a fragment fr
+00000bb0: 6f6d 2047 5241 4445 2028 6e65 6564 7320  om GRADE (needs 
+00000bc0: 2e74 677a 2066 696c 6529 0a20 202d 6c20  .tgz file).  -l 
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 2020 206c 6973 7420 6e61 6d65 7320 6f66     list names of
+00000bf0: 2061 6c6c 2064 6174 6162 6173 6520 656e   all database en
+00000c00: 7472 6965 730a 2020 2d73 2022 7374 7269  tries.  -s "stri
+00000c10: 6e67 2220 2020 2020 2020 2020 2020 7365  ng"           se
+00000c20: 6172 6368 2074 6865 2064 6174 6162 6173  arch the databas
+00000c30: 6520 666f 7220 6120 6e61 6d65 0a20 202d  e for a name.  -
+00000c40: 6720 2020 2020 2020 2020 2020 2020 2020  g               
+00000c50: 2020 2020 206b 6565 7020 6772 6f75 7020       keep group 
+00000c60: 7269 6769 6420 286e 6f20 7265 7374 7261  rigid (no restra
+00000c70: 696e 7473 290a 2020 2d75 2020 2020 2020  ints).  -u      
+00000c80: 2020 2020 2020 2020 2020 2020 2020 5570                Up
+00000c90: 6461 7465 2044 5352 2074 6f20 7468 6520  date DSR to the 
+00000ca0: 6d6f 7374 2063 7572 7265 6e74 2076 6572  most current ver
+00000cb0: 7369 6f6e 0a20 202d 6e20 2020 2020 2020  sion.  -n       
+00000cc0: 2020 2020 2020 2020 2020 2020 2064 6f20               do 
+00000cd0: 6e6f 7420 7265 6669 6e65 2061 6674 6572  not refine after
+00000ce0: 2066 7261 676d 656e 7420 7472 616e 7366   fragment transf
+00000cf0: 6572 0a60 6060 0a0a 4f72 2061 2067 7261  er.```..Or a gra
+00000d00: 7068 6963 616c 2075 7365 7220 696e 7465  phical user inte
+00000d10: 7266 6163 6520 696e 205b 5368 656c 586c  rface in [ShelXl
+00000d20: 655d 2868 7474 7073 3a2f 2f77 7777 2e73  e](https://www.s
+00000d30: 6865 6c78 6c65 2e6f 7267 2f73 6865 6c78  helxle.org/shelx
+00000d40: 2f65 696e 6761 6265 2e70 6870 293a 0a0a  /eingabe.php):..
+00000d50: 215b 4453 5220 6d61 696e 2077 696e 646f  ![DSR main windo
+00000d60: 775d 2868 7474 7073 3a2f 2f67 6974 6875  w](https://githu
+00000d70: 622e 636f 6d2f 646b 7261 747a 6572 742f  b.com/dkratzert/
+00000d80: 4453 522f 626c 6f62 2f6d 6173 7465 722f  DSR/blob/master/
+00000d90: 7069 6374 7572 6573 2f64 7372 5f73 6865  pictures/dsr_she
+00000da0: 6c78 6c65 2e70 6e67 3f72 6177 3d74 7275  lxle.png?raw=tru
+00000db0: 6529 0a0a 215b 4453 5220 6564 6974 6f72  e)..![DSR editor
+00000dc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000dd0: 2e63 6f6d 2f64 6b72 6174 7a65 7274 2f44  .com/dkratzert/D
+00000de0: 5352 2f62 6c6f 622f 6d61 7374 6572 2f70  SR/blob/master/p
+00000df0: 6963 7475 7265 732f 6473 725f 6564 6974  ictures/dsr_edit
+00000e00: 6f72 2e70 6e67 3f72 6177 3d74 7275 6529  or.png?raw=true)
+00000e10: 0a                                       .
```

