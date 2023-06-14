# Comparing `tmp/spotPython-0.2.7.tar.gz` & `tmp/spotPython-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.2.7.tar", last modified: Wed May 31 23:42:29 2023, max compression
+gzip compressed data, was "spotPython-0.2.9.tar", last modified: Fri Jun  2 12:53:25 2023, max compression
```

## Comparing `spotPython-0.2.7.tar` & `spotPython-0.2.9.tar`

### file list

```diff
@@ -1,237 +1,245 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.115930 spotPython-0.2.7/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.078656 spotPython-0.2.7/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.082532 spotPython-0.2.7/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.2.7/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    13211 2023-05-31 08:10:07.000000 spotPython-0.2.7/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.2.7/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.088262 spotPython-0.2.7/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.2.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.2.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.2.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.2.7/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.2.7/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.2.7/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-31 23:42:29.115744 spotPython-0.2.7/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-23 19:35:10.000000 spotPython-0.2.7/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.089246 spotPython-0.2.7/docs/
--rw-r--r--   0 bartz      (501) staff       (20)   208086 2023-05-29 18:21:43.000000 spotPython-0.2.7/docs/bart23e.html
--rw-r--r--   0 bartz      (501) staff       (20)   713146 2023-05-29 18:21:50.000000 spotPython-0.2.7/docs/bart23e.pdf
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.091117 spotPython-0.2.7/docs/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.2.7/docs/figures/parallel.png
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.091286 spotPython-0.2.7/docs/img/
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.2.7/docs/img/spotLogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-29 18:21:50.000000 spotPython-0.2.7/docs/index.html
--rw-r--r--   0 bartz      (501) staff       (20)    64921 2023-05-29 18:21:50.000000 spotPython-0.2.7/docs/search.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.079437 spotPython-0.2.7/docs/site_libs/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.092111 spotPython-0.2.7/docs/site_libs/bootstrap/
--rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap-icons.css
--rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap-icons.woff
--rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-29 18:21:41.000000 spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap.min.css
--rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.092286 spotPython-0.2.7/docs/site_libs/clipboard/
--rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/clipboard/clipboard.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.093091 spotPython-0.2.7/docs/site_libs/quarto-html/
--rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-html/anchor.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-html/popper.min.js
--rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-23 19:54:10.000000 spotPython-0.2.7/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
--rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-html/quarto.js
--rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-html/tippy.css
--rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-html/tippy.umd.min.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.093239 spotPython-0.2.7/docs/site_libs/quarto-nav/
--rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-nav/quarto-nav.js
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.093682 spotPython-0.2.7/docs/site_libs/quarto-search/
--rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-search/autocomplete.umd.js
--rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-search/fuse.min.js
--rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.2.7/docs/site_libs/quarto-search/quarto-search.js
--rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.2.7/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.2.7/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.103529 spotPython-0.2.7/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.2.7/notebooks/00_spot_doc.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.2.7/notebooks/01_spot_intro.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.2.7/notebooks/02_spot_multidim.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.2.7/notebooks/03_spot_anisotropic.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.2.7/notebooks/04_spot_sklearn_surrogate.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.2.7/notebooks/05_spot_sklearn_optimizers.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.2.7/notebooks/06_spot_gaussian.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.2.7/notebooks/07_spot_ei.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.2.7/notebooks/08_spot_noisy.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.2.7/notebooks/09_spot_ocba.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.2.7/notebooks/10_spot_hpt_sklearn_classification.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    23403 2023-05-27 07:00:04.000000 spotPython-0.2.7/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    28481 2023-05-27 07:00:42.000000 spotPython-0.2.7/notebooks/12_spot_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.2.7/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   110777 2023-05-31 23:00:41.000000 spotPython-0.2.7/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.2.7/notebooks/15_spot_hpt_sklearn_regression.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)  1475255 2023-05-31 08:15:56.000000 spotPython-0.2.7/notebooks/16_spot_hpt_sklearn_multiclass_classification_randomforest.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)  1048139 2023-05-31 23:00:50.000000 spotPython-0.2.7/notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   563052 2023-05-31 17:16:05.000000 spotPython-0.2.7/notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   674714 2023-05-30 15:26:52.000000 spotPython-0.2.7/notebooks/19_spot_hpt_sklearn_multiclass_classification_knn.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   494299 2023-05-31 23:36:24.000000 spotPython-0.2.7/notebooks/20_spot_torch_vbdp.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.079817 spotPython-0.2.7/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.103702 spotPython-0.2.7/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.2.7/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.2.7/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.105871 spotPython-0.2.7/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.2.7/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.2.7/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.2.7/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 18:09:24.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-23 19:31:10.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)   110037 2023-05-28 06:32:18.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png
--rw-r--r--   0 bartz      (501) staff       (20)    29542 2023-05-28 06:32:18.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    41583 2023-05-28 06:32:18.000000 spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    38033 2023-05-31 23:33:45.000000 spotPython-0.2.7/notebooks/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)     1354 2023-05-31 23:41:03.000000 spotPython-0.2.7/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-05-31 23:42:29.115973 spotPython-0.2.7/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.080115 spotPython-0.2.7/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.106034 spotPython-0.2.7/src/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)      214 2023-05-31 23:42:28.000000 spotPython-0.2.7/src/spotPython/_version.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.106799 spotPython-0.2.7/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.2.7/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.107121 spotPython-0.2.7/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.2.7/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.2.7/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.108032 spotPython-0.2.7/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.2.7/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.2.7/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.2.7/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.2.7/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     6955 2023-05-31 23:41:38.000000 spotPython-0.2.7/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.2.7/src/spotPython/data/torch_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)      459 2023-05-28 07:19:43.000000 spotPython-0.2.7/src/spotPython/data/torchdata.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.108386 spotPython-0.2.7/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.2.7/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.2.7/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.2.7/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.108785 spotPython-0.2.7/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     3770 2023-05-30 15:26:52.000000 spotPython-0.2.7/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     4911 2023-05-27 18:18:59.000000 spotPython-0.2.7/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.2.7/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.109212 spotPython-0.2.7/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.2.7/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     4137 2023-05-27 19:48:36.000000 spotPython-0.2.7/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    26033 2023-05-28 07:22:58.000000 spotPython-0.2.7/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.109504 spotPython-0.2.7/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-05-29 06:13:03.000000 spotPython-0.2.7/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.2.7/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.109650 spotPython-0.2.7/src/spotPython/sklearn/
--rw-r--r--   0 bartz      (501) staff       (20)     3711 2023-05-29 20:57:16.000000 spotPython-0.2.7/src/spotPython/sklearn/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.109785 spotPython-0.2.7/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    33049 2023-05-29 06:29:51.000000 spotPython-0.2.7/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.110756 spotPython-0.2.7/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 19:01:06.000000 spotPython-0.2.7/src/spotPython/torch/dataframedataset.py
--rw-r--r--   0 bartz      (501) staff       (20)     2411 2023-05-30 22:07:35.000000 spotPython-0.2.7/src/spotPython/torch/mapk.py
--rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.2.7/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.2.7/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.2.7/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)     1480 2023-05-31 23:42:25.000000 spotPython-0.2.7/src/spotPython/torch/netvbdp.py
--rw-r--r--   0 bartz      (501) staff       (20)    13535 2023-05-31 20:08:28.000000 spotPython-0.2.7/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.112821 spotPython-0.2.7/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.2.7/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.2.7/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.2.7/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.2.7/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.2.7/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.2.7/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.2.7/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     1445 2023-05-28 07:30:22.000000 spotPython-0.2.7/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-30 21:09:07.000000 spotPython-0.2.7/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      845 2023-04-13 18:37:01.000000 spotPython-0.2.7/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.2.7/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.2.7/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.106671 spotPython-0.2.7/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-05-31 23:42:28.000000 spotPython-0.2.7/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)    10615 2023-05-31 23:42:29.000000 spotPython-0.2.7/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-05-31 23:42:28.000000 spotPython-0.2.7/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       59 2023-05-31 23:42:28.000000 spotPython-0.2.7/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-05-31 23:42:28.000000 spotPython-0.2.7/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-05-31 23:42:29.115477 spotPython-0.2.7/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.2.7/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.2.7/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.2.7/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.2.7/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.2.7/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.168488 spotPython-0.2.9/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.066413 spotPython-0.2.9/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.071853 spotPython-0.2.9/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.2.9/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    17456 2023-06-02 12:52:07.000000 spotPython-0.2.9/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.2.9/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.084983 spotPython-0.2.9/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.2.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.2.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.2.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.2.9/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.2.9/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.2.9/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-06-02 12:53:25.168300 spotPython-0.2.9/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6577 2023-05-23 19:35:10.000000 spotPython-0.2.9/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.087877 spotPython-0.2.9/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)   208086 2023-05-29 18:21:43.000000 spotPython-0.2.9/docs/bart23e.html
+-rw-r--r--   0 bartz      (501) staff       (20)   713146 2023-05-29 18:21:50.000000 spotPython-0.2.9/docs/bart23e.pdf
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.091850 spotPython-0.2.9/docs/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94077 2023-05-19 17:04:41.000000 spotPython-0.2.9/docs/figures/parallel.png
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.092205 spotPython-0.2.9/docs/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.2.9/docs/img/spotLogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      231 2023-05-29 18:21:50.000000 spotPython-0.2.9/docs/index.html
+-rw-r--r--   0 bartz      (501) staff       (20)    64921 2023-05-29 18:21:50.000000 spotPython-0.2.9/docs/search.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.067199 spotPython-0.2.9/docs/site_libs/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.094524 spotPython-0.2.9/docs/site_libs/bootstrap/
+-rw-r--r--   0 bartz      (501) staff       (20)    95517 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 bartz      (501) staff       (20)   164168 2023-05-12 19:56:28.000000 spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap-icons.woff
+-rw-r--r--   0 bartz      (501) staff       (20)   308771 2023-05-29 18:21:41.000000 spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap.min.css
+-rw-r--r--   0 bartz      (501) staff       (20)    78129 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.094888 spotPython-0.2.9/docs/site_libs/clipboard/
+-rw-r--r--   0 bartz      (501) staff       (20)     9160 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/clipboard/clipboard.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.096581 spotPython-0.2.9/docs/site_libs/quarto-html/
+-rw-r--r--   0 bartz      (501) staff       (20)     6008 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-html/anchor.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    19728 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-html/popper.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)     3135 2023-05-23 19:54:10.000000 spotPython-0.2.9/docs/site_libs/quarto-html/quarto-syntax-highlighting.css
+-rw-r--r--   0 bartz      (501) staff       (20)    28407 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-html/quarto.js
+-rw-r--r--   0 bartz      (501) staff       (20)     1409 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-html/tippy.css
+-rw-r--r--   0 bartz      (501) staff       (20)    24033 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-html/tippy.umd.min.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.096810 spotPython-0.2.9/docs/site_libs/quarto-nav/
+-rw-r--r--   0 bartz      (501) staff       (20)     8250 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-nav/quarto-nav.js
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.097808 spotPython-0.2.9/docs/site_libs/quarto-search/
+-rw-r--r--   0 bartz      (501) staff       (20)    70711 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-search/autocomplete.umd.js
+-rw-r--r--   0 bartz      (501) staff       (20)    23539 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-search/fuse.min.js
+-rw-r--r--   0 bartz      (501) staff       (20)    32789 2023-05-12 19:57:05.000000 spotPython-0.2.9/docs/site_libs/quarto-search/quarto-search.js
+-rwxr-xr-x   0 bartz      (501) staff       (20)      123 2023-04-26 22:09:11.000000 spotPython-0.2.9/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)      437 2023-02-02 22:52:12.000000 spotPython-0.2.9/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.136548 spotPython-0.2.9/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    34275 2023-05-20 05:31:37.000000 spotPython-0.2.9/notebooks/00_spot_doc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     6585 2023-05-08 22:27:42.000000 spotPython-0.2.9/notebooks/01_spot_intro.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8780 2023-05-20 08:33:47.000000 spotPython-0.2.9/notebooks/02_spot_multidim.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     9719 2023-05-08 22:28:54.000000 spotPython-0.2.9/notebooks/03_spot_anisotropic.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    15781 2023-05-08 22:29:50.000000 spotPython-0.2.9/notebooks/04_spot_sklearn_surrogate.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)     8787 2023-05-08 22:30:17.000000 spotPython-0.2.9/notebooks/05_spot_sklearn_optimizers.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    14206 2023-05-08 22:30:52.000000 spotPython-0.2.9/notebooks/06_spot_gaussian.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    36749 2023-05-08 22:31:54.000000 spotPython-0.2.9/notebooks/07_spot_ei.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    11665 2023-05-08 22:32:20.000000 spotPython-0.2.9/notebooks/08_spot_noisy.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    12100 2023-05-08 22:32:53.000000 spotPython-0.2.9/notebooks/09_spot_ocba.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   125645 2023-05-20 08:34:43.000000 spotPython-0.2.9/notebooks/10_spot_hpt_sklearn_classification.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    23403 2023-05-27 07:00:04.000000 spotPython-0.2.9/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    28481 2023-05-27 07:00:42.000000 spotPython-0.2.9/notebooks/12_spot_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    22216 2023-05-20 08:37:13.000000 spotPython-0.2.9/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   110777 2023-05-31 23:00:41.000000 spotPython-0.2.9/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)    26705 2023-05-20 08:39:17.000000 spotPython-0.2.9/notebooks/15_spot_hpt_sklearn_regression.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1475255 2023-05-31 08:15:56.000000 spotPython-0.2.9/notebooks/16_spot_hpt_sklearn_multiclass_classification_randomforest.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1048139 2023-05-31 23:00:50.000000 spotPython-0.2.9/notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   563052 2023-05-31 17:16:05.000000 spotPython-0.2.9/notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   674714 2023-05-30 15:26:52.000000 spotPython-0.2.9/notebooks/19_spot_hpt_sklearn_multiclass_classification_knn.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  2722255 2023-06-01 06:44:06.000000 spotPython-0.2.9/notebooks/20_spot_torch_vbdp.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  2722255 2023-06-01 06:49:25.000000 spotPython-0.2.9/notebooks/20_spot_torch_vbdp_big_09.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)  1636245 2023-06-01 18:40:28.000000 spotPython-0.2.9/notebooks/20_spot_torch_vbdp_maans03.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   691598 2023-06-01 18:42:21.000000 spotPython-0.2.9/notebooks/21_spot_torch_vbdp.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   446028 2023-06-01 18:40:28.000000 spotPython-0.2.9/notebooks/22_spot_torch_vbdp.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   147625 2023-06-02 12:53:00.000000 spotPython-0.2.9/notebooks/23_spot_torch_vbdp.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   122015 2023-06-02 12:46:19.000000 spotPython-0.2.9/notebooks/24_spot_torch_regression.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.067428 spotPython-0.2.9/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.136715 spotPython-0.2.9/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.2.9/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.2.9/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.146322 spotPython-0.2.9/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.2.9/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.2.9/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.2.9/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21112 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21979 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23390 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22172 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23463 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24987 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    10009 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7783 2023-05-22 18:09:24.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21663 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22544 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22042 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21676 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21232 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22317 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9376 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6836 2023-05-23 19:31:10.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22179 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21553 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23439 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22108 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23180 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23993 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9057 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6972 2023-05-19 16:57:48.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)   110037 2023-05-28 06:32:18.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29542 2023-05-28 06:32:18.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41583 2023-05-28 06:32:18.000000 spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    42858 2023-06-02 11:23:26.000000 spotPython-0.2.9/notebooks/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1393 2023-06-01 19:07:40.000000 spotPython-0.2.9/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-06-02 12:53:25.168544 spotPython-0.2.9/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.067774 spotPython-0.2.9/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.146618 spotPython-0.2.9/src/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)      216 2023-06-02 12:53:24.000000 spotPython-0.2.9/src/spotPython/_version.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.147551 spotPython-0.2.9/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     2772 2023-04-13 18:20:56.000000 spotPython-0.2.9/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.148687 spotPython-0.2.9/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    40135 2023-04-13 19:26:45.000000 spotPython-0.2.9/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.2.9/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.151239 spotPython-0.2.9/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.2.9/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.2.9/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.2.9/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.2.9/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9051 2023-06-01 21:24:43.000000 spotPython-0.2.9/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.2.9/src/spotPython/data/torch_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)      459 2023-05-28 07:19:43.000000 spotPython-0.2.9/src/spotPython/data/torchdata.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3131 2023-06-01 18:44:39.000000 spotPython-0.2.9/src/spotPython/data/vbdp.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.151928 spotPython-0.2.9/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.2.9/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.2.9/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.2.9/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.152525 spotPython-0.2.9/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     3770 2023-05-30 15:26:52.000000 spotPython-0.2.9/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5839 2023-06-02 11:35:23.000000 spotPython-0.2.9/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    18970 2023-05-06 16:12:25.000000 spotPython-0.2.9/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.154326 spotPython-0.2.9/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.2.9/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4137 2023-05-27 19:48:36.000000 spotPython-0.2.9/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26018 2023-06-01 18:49:41.000000 spotPython-0.2.9/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.155170 spotPython-0.2.9/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-05-29 06:13:03.000000 spotPython-0.2.9/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4614 2023-05-20 08:41:56.000000 spotPython-0.2.9/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.155588 spotPython-0.2.9/src/spotPython/sklearn/
+-rw-r--r--   0 bartz      (501) staff       (20)     3711 2023-05-29 20:57:16.000000 spotPython-0.2.9/src/spotPython/sklearn/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.155848 spotPython-0.2.9/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    33077 2023-06-01 22:26:59.000000 spotPython-0.2.9/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.158731 spotPython-0.2.9/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 19:01:06.000000 spotPython-0.2.9/src/spotPython/torch/dataframedataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2411 2023-05-30 22:07:35.000000 spotPython-0.2.9/src/spotPython/torch/mapk.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.2.9/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.2.9/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.2.9/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1566 2023-06-01 21:28:05.000000 spotPython-0.2.9/src/spotPython/torch/netregression.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1565 2023-06-01 18:55:33.000000 spotPython-0.2.9/src/spotPython/torch/netvbdp.py
+-rw-r--r--   0 bartz      (501) staff       (20)    15897 2023-06-02 11:24:41.000000 spotPython-0.2.9/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.162834 spotPython-0.2.9/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.2.9/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.2.9/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.2.9/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2023-05-20 08:44:33.000000 spotPython-0.2.9/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      598 2023-05-07 19:27:47.000000 spotPython-0.2.9/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3600 2023-05-09 21:08:48.000000 spotPython-0.2.9/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)      461 2023-04-26 18:22:38.000000 spotPython-0.2.9/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2136 2023-06-01 22:55:38.000000 spotPython-0.2.9/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-30 21:09:07.000000 spotPython-0.2.9/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      912 2023-06-01 22:37:01.000000 spotPython-0.2.9/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.2.9/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4964 2023-05-09 23:09:07.000000 spotPython-0.2.9/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.147411 spotPython-0.2.9/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     7347 2023-06-02 12:53:24.000000 spotPython-0.2.9/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)    10912 2023-06-02 12:53:25.000000 spotPython-0.2.9/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-06-02 12:53:24.000000 spotPython-0.2.9/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       84 2023-06-02 12:53:24.000000 spotPython-0.2.9/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-06-02 12:53:24.000000 spotPython-0.2.9/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-06-02 12:53:25.167960 spotPython-0.2.9/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.2.9/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.2.9/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.2.9/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.2.9/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.2.9/tox.ini
```

### Comparing `spotPython-0.2.7/.github/workflows/test.yml` & `spotPython-0.2.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.2.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.2.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.2.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.2.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.2.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.2.9/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/LICENSE.txt` & `spotPython-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/PKG-INFO` & `spotPython-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.2.7
+Version: 0.2.9
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.2.7/README.md` & `spotPython-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/bart23e.html` & `spotPython-0.2.9/docs/bart23e.html`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/bart23e.pdf` & `spotPython-0.2.9/docs/bart23e.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.2.9/docs/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/figures/parallel.png` & `spotPython-0.2.9/docs/figures/parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/img/spotLogo.png` & `spotPython-0.2.9/docs/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/search.json` & `spotPython-0.2.9/docs/search.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap-icons.css` & `spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap-icons.woff` & `spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap.min.css` & `spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/bootstrap/bootstrap.min.js` & `spotPython-0.2.9/docs/site_libs/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/clipboard/clipboard.min.js` & `spotPython-0.2.9/docs/site_libs/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-html/anchor.min.js` & `spotPython-0.2.9/docs/site_libs/quarto-html/anchor.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-html/popper.min.js` & `spotPython-0.2.9/docs/site_libs/quarto-html/popper.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-html/quarto-syntax-highlighting.css` & `spotPython-0.2.9/docs/site_libs/quarto-html/quarto-syntax-highlighting.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-html/quarto.js` & `spotPython-0.2.9/docs/site_libs/quarto-html/quarto.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-html/tippy.css` & `spotPython-0.2.9/docs/site_libs/quarto-html/tippy.css`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-html/tippy.umd.min.js` & `spotPython-0.2.9/docs/site_libs/quarto-html/tippy.umd.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-nav/quarto-nav.js` & `spotPython-0.2.9/docs/site_libs/quarto-nav/quarto-nav.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-search/autocomplete.umd.js` & `spotPython-0.2.9/docs/site_libs/quarto-search/autocomplete.umd.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-search/fuse.min.js` & `spotPython-0.2.9/docs/site_libs/quarto-search/fuse.min.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/docs/site_libs/quarto-search/quarto-search.js` & `spotPython-0.2.9/docs/site_libs/quarto-search/quarto-search.js`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/00_spot_doc.ipynb` & `spotPython-0.2.9/notebooks/00_spot_doc.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/01_spot_intro.ipynb` & `spotPython-0.2.9/notebooks/01_spot_intro.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/02_spot_multidim.ipynb` & `spotPython-0.2.9/notebooks/02_spot_multidim.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/03_spot_anisotropic.ipynb` & `spotPython-0.2.9/notebooks/03_spot_anisotropic.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/04_spot_sklearn_surrogate.ipynb` & `spotPython-0.2.9/notebooks/04_spot_sklearn_surrogate.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/05_spot_sklearn_optimizers.ipynb` & `spotPython-0.2.9/notebooks/05_spot_sklearn_optimizers.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/06_spot_gaussian.ipynb` & `spotPython-0.2.9/notebooks/06_spot_gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/07_spot_ei.ipynb` & `spotPython-0.2.9/notebooks/07_spot_ei.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/08_spot_noisy.ipynb` & `spotPython-0.2.9/notebooks/08_spot_noisy.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/09_spot_ocba.ipynb` & `spotPython-0.2.9/notebooks/09_spot_ocba.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/10_spot_hpt_sklearn_classification.ipynb` & `spotPython-0.2.9/notebooks/10_spot_hpt_sklearn_classification.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb` & `spotPython-0.2.9/notebooks/11_spot_hpt_torch_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/12_spot_hpt_torch_cifar10.ipynb` & `spotPython-0.2.9/notebooks/12_spot_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb` & `spotPython-0.2.9/notebooks/13_spot_hpt_torch_cv_fashion_mnist.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb` & `spotPython-0.2.9/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/15_spot_hpt_sklearn_regression.ipynb` & `spotPython-0.2.9/notebooks/15_spot_hpt_sklearn_regression.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/16_spot_hpt_sklearn_multiclass_classification_randomforest.ipynb` & `spotPython-0.2.9/notebooks/16_spot_hpt_sklearn_multiclass_classification_randomforest.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb` & `spotPython-0.2.9/notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb` & `spotPython-0.2.9/notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/19_spot_hpt_sklearn_multiclass_classification_knn.ipynb` & `spotPython-0.2.9/notebooks/19_spot_hpt_sklearn_multiclass_classification_knn.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/20_spot_torch_vbdp.ipynb` & `spotPython-0.2.9/notebooks/22_spot_torch_vbdp.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960347706251913%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'subtitle: Version 0.2.7\\n')], delete: [2]}}, 6: "*

 * *            "{'source': ['* feature engineering: 6112 features']}, 7: {'outputs': [], 'source': "*

 * *            "['BIG_INPUT = False\\n', 'if BIG_INPUT:\\n', '    # convert all train.df columns to "*

 * *            'int   \\n\', \'    train_0 = train_df.astype(int)\\n\', "    col_prognosis = '*

 * *            'train_0[\'prognosis\']\\n", "    train_x = train_0.drop(columns=[\'prognosis\'])\\n", '*

 * *            '\'    train_x = […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 "---\n",
                 "title: PyTorch Hyperparameter Tuning --- A Tutorial for spotPython\n",
-                "subtitle: Version 0.2.6\n",
+                "subtitle: Version 0.2.7\n",
                 "format:\n",
                 "  pdf:\n",
                 "    template: bart23e_template.tex\n",
                 "    fig-width: 7\n",
                 "    fig-height: 5\n",
                 "    keep-tex: true\n",
                 "    linenumbers: false\n",
@@ -227,28 +227,53 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "* feature engineering:"
+                "* feature engineering: 6112 features"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
+            "outputs": [],
+            "source": [
+                "BIG_INPUT = False\n",
+                "if BIG_INPUT:\n",
+                "    # convert all train.df columns to int   \n",
+                "    train_0 = train_df.astype(int)\n",
+                "    col_prognosis = train_0['prognosis']\n",
+                "    train_x = train_0.drop(columns=['prognosis'])\n",
+                "    train_x = combine_features(train_x)\n",
+                "    train_x['prognosis'] = col_prognosis\n",
+                "    train_df = train_x.copy()\n",
+                "    train_df.head()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "* feature engineering: 69 features"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/var/folders/dw/pvtj6mt91znd0hftcztqb0k00000gn/T/ipykernel_70912/2233068463.py:6: PerformanceWarning: DataFrame is highly fragmented.  This is usually the result of calling `frame.insert` many times, which has poor performance.  Consider joining all columns at once using pd.concat(axis=1) instead. To get a de-fragmented frame, use `newframe = frame.copy()`\n",
-                        "  train_x['prognosis'] = col_prognosis\n"
+                        "Estimated number of clusters: 10\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -275,23 +300,23 @@
                             "      <th>muscle_pain</th>\n",
                             "      <th>joint_pain</th>\n",
                             "      <th>vomiting</th>\n",
                             "      <th>rash</th>\n",
                             "      <th>diarrhea</th>\n",
                             "      <th>hypotension</th>\n",
                             "      <th>...</th>\n",
-                            "      <th>6039</th>\n",
-                            "      <th>6040</th>\n",
-                            "      <th>6041</th>\n",
-                            "      <th>6042</th>\n",
-                            "      <th>6043</th>\n",
-                            "      <th>6044</th>\n",
-                            "      <th>6045</th>\n",
-                            "      <th>6046</th>\n",
-                            "      <th>6047</th>\n",
+                            "      <th>ulcers</th>\n",
+                            "      <th>toenail_loss</th>\n",
+                            "      <th>speech_problem</th>\n",
+                            "      <th>bullseye_rash</th>\n",
+                            "      <th>c_0</th>\n",
+                            "      <th>c_1</th>\n",
+                            "      <th>c_2</th>\n",
+                            "      <th>c_3</th>\n",
+                            "      <th>cluster</th>\n",
                             "      <th>prognosis</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1</td>\n",
@@ -305,19 +330,19 @@
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>5</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>2</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>9</td>\n",
                             "      <td>3</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
@@ -331,17 +356,17 @@
                             "      <td>...</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>5</td>\n",
                             "      <td>7</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
@@ -349,22 +374,22 @@
                             "      <td>0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1</td>\n",
                             "      <td>0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>1</td>\n",
                             "      <td>1</td>\n",
+                            "      <td>6</td>\n",
+                            "      <td>3</td>\n",
+                            "      <td>4</td>\n",
+                            "      <td>2</td>\n",
                             "      <td>0</td>\n",
                             "      <td>3</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
@@ -377,19 +402,19 @@
                             "      <td>0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>4</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>3</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>1</td>\n",
                             "      <td>10</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
@@ -397,98 +422,83 @@
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>0</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>0</td>\n",
                             "      <td>0</td>\n",
+                            "      <td>5</td>\n",
                             "      <td>6</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>5 rows \u00d7 6113 columns</p>\n",
+                            "<p>5 rows \u00d7 70 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "   sudden_fever  headache  mouth_bleed  nose_bleed  muscle_pain  joint_pain   \n",
                             "0             1         1            0           1            1           1  \\\n",
                             "1             0         0            0           0            0           0   \n",
                             "2             0         1            1           1            0           1   \n",
                             "3             0         0            1           1            1           1   \n",
                             "4             0         0            0           0            0           0   \n",
                             "\n",
-                            "   vomiting  rash  diarrhea  hypotension  ...  6039  6040  6041  6042  6043   \n",
-                            "0         1     0         1            1  ...     0     0     0     0     0  \\\n",
-                            "1         1     0         1            0  ...     0     0     0     0     0   \n",
-                            "2         1     1         1            1  ...     1     1     0     1     1   \n",
-                            "3         0     1         0            1  ...     0     0     0     0     0   \n",
-                            "4         0     0         1            0  ...     0     1     1     0     1   \n",
+                            "   vomiting  rash  diarrhea  hypotension  ...  ulcers  toenail_loss   \n",
+                            "0         1     0         1            1  ...       0             0  \\\n",
+                            "1         1     0         1            0  ...       0             0   \n",
+                            "2         1     1         1            1  ...       0             1   \n",
+                            "3         0     1         0            1  ...       0             0   \n",
+                            "4         0     0         1            0  ...       1             1   \n",
                             "\n",
-                            "   6044  6045  6046  6047  prognosis  \n",
-                            "0     0     0     0     0          3  \n",
-                            "1     0     0     0     0          7  \n",
-                            "2     0     1     1     0          3  \n",
-                            "3     0     0     0     0         10  \n",
-                            "4     1     0     0     0          6  \n",
+                            "   speech_problem  bullseye_rash  c_0  c_1  c_2  c_3  cluster  prognosis  \n",
+                            "0               0              0    5    0    2    0        9          3  \n",
+                            "1               0              0    0    0    1    1        5          7  \n",
+                            "2               1              1    6    3    4    2        0          3  \n",
+                            "3               0              0    4    1    3    2        1         10  \n",
+                            "4               0              0    0    1    0    0        5          6  \n",
                             "\n",
-                            "[5 rows x 6113 columns]"
+                            "[5 rows x 70 columns]"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# convert all train.df columns to int   \n",
-                "train_0 = train_df.astype(int)\n",
-                "col_prognosis = train_0['prognosis']\n",
-                "train_x = train_0.drop(columns=['prognosis'])\n",
-                "train_x = combine_features(train_x)\n",
-                "train_x['prognosis'] = col_prognosis\n",
-                "train_df = train_x.copy()\n",
+                "if BIG_INPUT == False:\n",
+                "    # convert all train.df columns to int   \n",
+                "    train_df = train_df.astype(int)\n",
+                "    col_prognosis = train_df['prognosis']\n",
+                "    train_features = cluster_features(train_df.drop(columns=['prognosis']))    \n",
+                "    train_df = affinity_propagation_features(train_features)\n",
+                "    train_df['prognosis'] = col_prognosis\n",
                 "train_df.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "\n",
-                "# col_prognosis = train_df['prognosis']\n",
-                "# train_features = cluster_features(train_df.drop(columns=['prognosis']))\n",
-                "# # train_features = cluster_features(train_df)\n",
-                "# train_df = affinity_propagation_features(train_features)\n",
-                "# train_df['prognosis'] = col_prognosis\n",
-                "# train_df.head()"
-            ]
-        },
-        {
-            "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(707, 6113)\n",
-                        "(530, 6113)\n",
-                        "(177, 6113)\n"
+                        "(707, 70)\n",
+                        "(530, 70)\n",
+                        "(177, 70)\n"
                     ]
                 }
             ],
             "source": [
                 "n_samples = train_df.shape[0]\n",
                 "n_features = train_df.shape[1] - 1\n",
                 "train_df.columns = [f\"x{i}\" for i in range(1, n_features+1)] + [target_column]\n",
@@ -532,19 +542,25 @@
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "torch.Size([2, 6112])\n",
+                        "torch.Size([2, 69])\n",
                         "torch.Size([2])\n",
-                        "tensor([[1., 0., 1.,  ..., 0., 0., 0.],\n",
-                        "        [0., 1., 0.,  ..., 0., 0., 0.]])\n",
-                        "tensor([6, 1])\n"
+                        "tensor([[0., 0., 0., 0., 0., 0., 1., 0., 1., 0., 0., 0., 0., 0., 1., 1., 0., 0.,\n",
+                        "         0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.,\n",
+                        "         0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.,\n",
+                        "         0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 5.],\n",
+                        "        [1., 0., 0., 0., 1., 0., 1., 1., 0., 0., 0., 0., 1., 0., 0., 0., 1., 1.,\n",
+                        "         1., 0., 0., 1., 1., 0., 1., 1., 1., 1., 0., 0., 0., 1., 1., 1., 1., 1.,\n",
+                        "         1., 1., 1., 1., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 0.,\n",
+                        "         0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 5., 0., 2., 1., 2.]])\n",
+                        "tensor([0, 6])\n"
                     ]
                 }
             ],
             "source": [
                 "from spotPython.torch.traintest import create_train_val_data_loaders\n",
                 "trainloader, testloader = create_train_val_data_loaders(train, 2, True, 0)\n",
                 "for i, data in enumerate(trainloader, 0):\n",
@@ -569,18 +585,18 @@
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "tensor([[0.0909, 0.1030, 0.0861, 0.0927, 0.0907, 0.0871, 0.1055, 0.0899, 0.0959,\n",
-                        "         0.0833, 0.0748],\n",
-                        "        [0.0841, 0.1089, 0.0806, 0.0911, 0.0907, 0.1073, 0.0819, 0.0790, 0.0952,\n",
-                        "         0.1045, 0.0767]], grad_fn=<SoftmaxBackward0>)\n"
+                        "tensor([[0.0883, 0.0806, 0.0974, 0.0812, 0.1050, 0.1131, 0.0840, 0.0935, 0.0985,\n",
+                        "         0.0760, 0.0823],\n",
+                        "        [0.0930, 0.0777, 0.0947, 0.0654, 0.0988, 0.1218, 0.0723, 0.1029, 0.0986,\n",
+                        "         0.0903, 0.0846]], grad_fn=<SoftmaxBackward0>)\n"
                     ]
                 }
             ],
             "source": [
                 "class Net(nn.Module):\n",
                 "    def __init__(self):\n",
                 "        super(Net, self).__init__()\n",
@@ -664,1308 +680,912 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
-                        "config: {'l1': 2048, 'dropout_prob': 0.39461789811977777, 'lr_mult': 0.001, 'batch_size': 4, 'epochs': 64, 'k_folds': 1, 'patience': 19, 'optimizer': 'Adam', 'sgd_momentum': 0.9}\n",
+                        "config: {'l1': 4096, 'dropout_prob': 0.7103122166156, 'lr_mult': 0.001, 'batch_size': 4, 'epochs': 64, 'k_folds': 1, 'patience': 32, 'optimizer': 'AdamW', 'sgd_momentum': 0.9}\n",
                         "Epoch: 1\n",
-                        "Loss on hold-out set: 2.3981054728885867\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.06132075471698113\n",
+                        "Loss on hold-out set: 2.3978939236335033\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.13836477987421386\n",
                         "Epoch: 2\n",
-                        "Loss on hold-out set: 2.398018531079562\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.06839622641509434\n",
+                        "Loss on hold-out set: 2.39775938357947\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.15330188679245282\n",
                         "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3979288497061098\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.08097484276729561\n",
+                        "Loss on hold-out set: 2.3978627357842788\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.14937106918238993\n",
                         "Epoch: 4\n",
-                        "Loss on hold-out set: 2.3977927936697907\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.07940251572327044\n",
+                        "Loss on hold-out set: 2.3977065671165034\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.14072327044025157\n",
                         "Epoch: 5\n",
-                        "Loss on hold-out set: 2.3978659611827924\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.07547169811320754\n",
+                        "Loss on hold-out set: 2.397652270658961\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.15487421383647795\n",
                         "Epoch: 6\n",
-                        "Loss on hold-out set: 2.3977153706100753\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.09198113207547169\n",
+                        "Loss on hold-out set: 2.397515409397629\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.1540880503144654\n",
                         "Epoch: 7\n",
-                        "Loss on hold-out set: 2.3976804310420774\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.09119496855345911\n",
+                        "Loss on hold-out set: 2.3976816861134655\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.16194968553459121\n",
                         "Epoch: 8\n",
-                        "Loss on hold-out set: 2.397596975542464\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.07861635220125784\n",
+                        "Loss on hold-out set: 2.397676211483074\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.17059748427672952\n",
                         "Epoch: 9\n",
-                        "Loss on hold-out set: 2.397560182607399\n",
-                        "Accuracy on hold-out set: 0.10377358490566038\n",
-                        "Metric value on hold-out data: 0.08962264150943396\n",
+                        "Loss on hold-out set: 2.39749558016939\n",
+                        "Accuracy on hold-out set: 0.08962264150943396\n",
+                        "Metric value on hold-out data: 0.16588050314465408\n",
                         "Epoch: 10\n",
-                        "Loss on hold-out set: 2.397514410738675\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.12028301886792453\n",
+                        "Loss on hold-out set: 2.3974832408833056\n",
+                        "Accuracy on hold-out set: 0.08962264150943396\n",
+                        "Metric value on hold-out data: 0.16430817610062892\n",
                         "Epoch: 11\n",
-                        "Loss on hold-out set: 2.3974012473844133\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.13443396226415094\n",
+                        "Loss on hold-out set: 2.3974960615050116\n",
+                        "Accuracy on hold-out set: 0.08018867924528301\n",
+                        "Metric value on hold-out data: 0.17138364779874213\n",
                         "Epoch: 12\n",
-                        "Loss on hold-out set: 2.397248758459991\n",
-                        "Accuracy on hold-out set: 0.15566037735849056\n",
-                        "Metric value on hold-out data: 0.15251572327044027\n",
+                        "Loss on hold-out set: 2.3972228113210425\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.17295597484276726\n",
                         "Epoch: 13\n",
-                        "Loss on hold-out set: 2.397258479640169\n",
-                        "Accuracy on hold-out set: 0.16981132075471697\n",
-                        "Metric value on hold-out data: 0.1509433962264151\n",
+                        "Loss on hold-out set: 2.3971738410445877\n",
+                        "Accuracy on hold-out set: 0.08962264150943396\n",
+                        "Metric value on hold-out data: 0.18553459119496854\n",
                         "Epoch: 14\n",
-                        "Loss on hold-out set: 2.397017726358378\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.17767295597484276\n",
+                        "Loss on hold-out set: 2.3971438048020848\n",
+                        "Accuracy on hold-out set: 0.10377358490566038\n",
+                        "Metric value on hold-out data: 0.1941823899371069\n",
                         "Epoch: 15\n",
-                        "Loss on hold-out set: 2.396956002937173\n",
-                        "Accuracy on hold-out set: 0.2028301886792453\n",
+                        "Loss on hold-out set: 2.3971408942960344\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
                         "Metric value on hold-out data: 0.19496855345911948\n",
                         "Epoch: 16\n",
-                        "Loss on hold-out set: 2.3969310589556425\n",
-                        "Accuracy on hold-out set: 0.24056603773584906\n",
-                        "Metric value on hold-out data: 0.21540880503144652\n",
+                        "Loss on hold-out set: 2.3971898195878514\n",
+                        "Accuracy on hold-out set: 0.09433962264150944\n",
+                        "Metric value on hold-out data: 0.1831761006289308\n",
                         "Epoch: 17\n",
-                        "Loss on hold-out set: 2.3967338867907255\n",
-                        "Accuracy on hold-out set: 0.2358490566037736\n",
-                        "Metric value on hold-out data: 0.21776729559748426\n",
+                        "Loss on hold-out set: 2.3969930702785276\n",
+                        "Accuracy on hold-out set: 0.10377358490566038\n",
+                        "Metric value on hold-out data: 0.19968553459119495\n",
                         "Epoch: 18\n",
-                        "Loss on hold-out set: 2.3966646419381195\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.19261006289308175\n",
+                        "Loss on hold-out set: 2.3970751042635934\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.18396226415094338\n",
                         "Epoch: 19\n",
-                        "Loss on hold-out set: 2.3967656639387025\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.19025157232704404\n",
+                        "Loss on hold-out set: 2.3968534829481594\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.21147798742138363\n",
                         "Epoch: 20\n",
-                        "Loss on hold-out set: 2.396334508679948\n",
-                        "Accuracy on hold-out set: 0.2358490566037736\n",
-                        "Metric value on hold-out data: 0.23427672955974838\n",
+                        "Loss on hold-out set: 2.39699221107195\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.22484276729559743\n",
                         "Epoch: 21\n",
-                        "Loss on hold-out set: 2.3962493167733245\n",
-                        "Accuracy on hold-out set: 0.19339622641509435\n",
-                        "Metric value on hold-out data: 0.2091194968553459\n",
+                        "Loss on hold-out set: 2.3970084865138217\n",
+                        "Accuracy on hold-out set: 0.09433962264150944\n",
+                        "Metric value on hold-out data: 0.19496855345911948\n",
                         "Epoch: 22\n",
-                        "Loss on hold-out set: 2.396019643207766\n",
-                        "Accuracy on hold-out set: 0.2028301886792453\n",
-                        "Metric value on hold-out data: 0.2232704402515723\n",
+                        "Loss on hold-out set: 2.396779667656377\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.19654088050314467\n",
                         "Epoch: 23\n",
-                        "Loss on hold-out set: 2.3956679263204896\n",
-                        "Accuracy on hold-out set: 0.21226415094339623\n",
-                        "Metric value on hold-out data: 0.22562893081761004\n",
+                        "Loss on hold-out set: 2.396829497139409\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.18474842767295596\n",
                         "Epoch: 24\n",
-                        "Loss on hold-out set: 2.3956065627763854\n",
-                        "Accuracy on hold-out set: 0.25\n",
-                        "Metric value on hold-out data: 0.25157232704402516\n",
+                        "Loss on hold-out set: 2.3964509514142884\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.22798742138364778\n",
                         "Epoch: 25\n",
-                        "Loss on hold-out set: 2.395278332368383\n",
-                        "Accuracy on hold-out set: 0.22169811320754718\n",
-                        "Metric value on hold-out data: 0.23820754716981132\n",
+                        "Loss on hold-out set: 2.3966743496229066\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.2177672955974843\n",
                         "Epoch: 26\n",
-                        "Loss on hold-out set: 2.3953239018062376\n",
-                        "Accuracy on hold-out set: 0.22641509433962265\n",
-                        "Metric value on hold-out data: 0.23977987421383648\n",
+                        "Loss on hold-out set: 2.3963668976189956\n",
+                        "Accuracy on hold-out set: 0.14622641509433962\n",
+                        "Metric value on hold-out data: 0.2429245283018868\n",
                         "Epoch: 27\n",
-                        "Loss on hold-out set: 2.3950539040115646\n",
-                        "Accuracy on hold-out set: 0.22169811320754718\n",
-                        "Metric value on hold-out data: 0.23113207547169812\n",
+                        "Loss on hold-out set: 2.3964109060899266\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.22562893081761004\n",
                         "Epoch: 28\n",
-                        "Loss on hold-out set: 2.394899201842974\n",
-                        "Accuracy on hold-out set: 0.22169811320754718\n",
-                        "Metric value on hold-out data: 0.24685534591194966\n",
+                        "Loss on hold-out set: 2.3963884272665346\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.23191823899371067\n",
                         "Epoch: 29\n",
-                        "Loss on hold-out set: 2.3946531448724135\n",
-                        "Accuracy on hold-out set: 0.2169811320754717\n",
-                        "Metric value on hold-out data: 0.24606918238993705\n",
+                        "Loss on hold-out set: 2.3966390861655182\n",
+                        "Accuracy on hold-out set: 0.10377358490566038\n",
+                        "Metric value on hold-out data: 0.18632075471698112\n",
                         "Epoch: 30\n",
-                        "Loss on hold-out set: 2.394345575908445\n",
-                        "Accuracy on hold-out set: 0.22169811320754718\n",
-                        "Metric value on hold-out data: 0.2421383647798742\n",
+                        "Loss on hold-out set: 2.396441216738719\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.22091194968553457\n",
                         "Epoch: 31\n",
-                        "Loss on hold-out set: 2.394149996199698\n",
-                        "Accuracy on hold-out set: 0.21226415094339623\n",
-                        "Metric value on hold-out data: 0.22955974842767293\n",
+                        "Loss on hold-out set: 2.396127511870186\n",
+                        "Accuracy on hold-out set: 0.13679245283018868\n",
+                        "Metric value on hold-out data: 0.23349056603773585\n",
                         "Epoch: 32\n",
-                        "Loss on hold-out set: 2.393515357431376\n",
-                        "Accuracy on hold-out set: 0.23113207547169812\n",
-                        "Metric value on hold-out data: 0.23742138364779872\n",
+                        "Loss on hold-out set: 2.3963316071708247\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.21776729559748426\n",
                         "Epoch: 33\n",
-                        "Loss on hold-out set: 2.3934304939126068\n",
-                        "Accuracy on hold-out set: 0.2358490566037736\n",
-                        "Metric value on hold-out data: 0.24764150943396226\n",
+                        "Loss on hold-out set: 2.3962549128622377\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.21540880503144652\n",
                         "Epoch: 34\n",
-                        "Loss on hold-out set: 2.392375928051067\n",
-                        "Accuracy on hold-out set: 0.24528301886792453\n",
-                        "Metric value on hold-out data: 0.2437106918238994\n",
+                        "Loss on hold-out set: 2.396062468582729\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.20754716981132076\n",
                         "Epoch: 35\n",
-                        "Loss on hold-out set: 2.392353741627819\n",
-                        "Accuracy on hold-out set: 0.16981132075471697\n",
-                        "Metric value on hold-out data: 0.20597484276729558\n",
+                        "Loss on hold-out set: 2.3960731794249335\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.20833333333333334\n",
                         "Epoch: 36\n",
-                        "Loss on hold-out set: 2.3922538667354942\n",
-                        "Accuracy on hold-out set: 0.2028301886792453\n",
-                        "Metric value on hold-out data: 0.21305031446540876\n",
+                        "Loss on hold-out set: 2.3960699135402463\n",
+                        "Accuracy on hold-out set: 0.14622641509433962\n",
+                        "Metric value on hold-out data: 0.2389937106918239\n",
                         "Epoch: 37\n",
-                        "Loss on hold-out set: 2.3916672310739195\n",
-                        "Accuracy on hold-out set: 0.21226415094339623\n",
+                        "Loss on hold-out set: 2.3958040138460555\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
                         "Metric value on hold-out data: 0.2224842767295597\n",
                         "Epoch: 38\n",
-                        "Loss on hold-out set: 2.3914520335647294\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.20361635220125782\n",
+                        "Loss on hold-out set: 2.395740895901086\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.220125786163522\n",
                         "Epoch: 39\n",
-                        "Loss on hold-out set: 2.390610114583429\n",
-                        "Accuracy on hold-out set: 0.19811320754716982\n",
-                        "Metric value on hold-out data: 0.2075471698113207\n",
+                        "Loss on hold-out set: 2.3958055478221967\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.21305031446540879\n",
                         "Epoch: 40\n",
-                        "Loss on hold-out set: 2.3898312730609246\n",
-                        "Accuracy on hold-out set: 0.19339622641509435\n",
-                        "Metric value on hold-out data: 0.21383647798742136\n",
+                        "Loss on hold-out set: 2.3956313763024673\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.22562893081761004\n",
                         "Epoch: 41\n",
-                        "Loss on hold-out set: 2.389569732378114\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.20518867924528303\n",
+                        "Loss on hold-out set: 2.395484011128264\n",
+                        "Accuracy on hold-out set: 0.1509433962264151\n",
+                        "Metric value on hold-out data: 0.2389937106918239\n",
                         "Epoch: 42\n",
-                        "Loss on hold-out set: 2.3891800709490507\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.19889937106918237\n",
+                        "Loss on hold-out set: 2.3955796169784835\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.24135220125786164\n",
                         "Epoch: 43\n",
-                        "Loss on hold-out set: 2.3882435267826296\n",
-                        "Accuracy on hold-out set: 0.17452830188679244\n",
-                        "Metric value on hold-out data: 0.19261006289308175\n",
+                        "Loss on hold-out set: 2.3954142534507894\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.220125786163522\n",
                         "Epoch: 44\n",
-                        "Loss on hold-out set: 2.3880089453931124\n",
-                        "Accuracy on hold-out set: 0.19811320754716982\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
+                        "Loss on hold-out set: 2.3950169356364124\n",
+                        "Accuracy on hold-out set: 0.14150943396226415\n",
+                        "Metric value on hold-out data: 0.2382075471698113\n",
                         "Epoch: 45\n",
-                        "Loss on hold-out set: 2.386331576221394\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.1941823899371069\n",
+                        "Loss on hold-out set: 2.3951897261277684\n",
+                        "Accuracy on hold-out set: 0.14150943396226415\n",
+                        "Metric value on hold-out data: 0.23270440251572325\n",
                         "Epoch: 46\n",
-                        "Loss on hold-out set: 2.386682798277657\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.1894654088050314\n",
+                        "Loss on hold-out set: 2.3949293685409256\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.23349056603773585\n",
                         "Epoch: 47\n",
-                        "Loss on hold-out set: 2.3855139534428433\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.19889937106918235\n",
+                        "Loss on hold-out set: 2.3947447470898897\n",
+                        "Accuracy on hold-out set: 0.13679245283018868\n",
+                        "Metric value on hold-out data: 0.23506289308176098\n",
                         "Epoch: 48\n",
-                        "Loss on hold-out set: 2.3856807564789393\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.1957547169811321\n",
+                        "Loss on hold-out set: 2.3951278947434336\n",
+                        "Accuracy on hold-out set: 0.13679245283018868\n",
+                        "Metric value on hold-out data: 0.22562893081761004\n",
                         "Epoch: 49\n",
-                        "Loss on hold-out set: 2.3852964842094564\n",
-                        "Accuracy on hold-out set: 0.17452830188679244\n",
-                        "Metric value on hold-out data: 0.1957547169811321\n",
+                        "Loss on hold-out set: 2.3948106900700985\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.22877358490566038\n",
                         "Epoch: 50\n",
-                        "Loss on hold-out set: 2.3835379087700033\n",
-                        "Accuracy on hold-out set: 0.17452830188679244\n",
-                        "Metric value on hold-out data: 0.18789308176100628\n",
+                        "Loss on hold-out set: 2.394408734339588\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.22955974842767293\n",
                         "Epoch: 51\n",
-                        "Loss on hold-out set: 2.3825755209293007\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.20518867924528303\n",
+                        "Loss on hold-out set: 2.3947187459693766\n",
+                        "Accuracy on hold-out set: 0.12735849056603774\n",
+                        "Metric value on hold-out data: 0.22562893081761004\n",
                         "Epoch: 52\n",
-                        "Loss on hold-out set: 2.3831953372595445\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.19261006289308175\n",
+                        "Loss on hold-out set: 2.3941260283848025\n",
+                        "Accuracy on hold-out set: 0.14150943396226415\n",
+                        "Metric value on hold-out data: 0.23742138364779872\n",
                         "Epoch: 53\n",
-                        "Loss on hold-out set: 2.3818091986314305\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.20361635220125784\n",
+                        "Loss on hold-out set: 2.3942266860098207\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.23820754716981132\n",
                         "Epoch: 54\n",
-                        "Loss on hold-out set: 2.3822837910562193\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.2012578616352201\n",
+                        "Loss on hold-out set: 2.394010989171154\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.22955974842767293\n",
                         "Epoch: 55\n",
-                        "Loss on hold-out set: 2.381450940977852\n",
-                        "Accuracy on hold-out set: 0.19811320754716982\n",
-                        "Metric value on hold-out data: 0.21226415094339623\n",
+                        "Loss on hold-out set: 2.3939469625365057\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.23270440251572325\n",
                         "Epoch: 56\n",
-                        "Loss on hold-out set: 2.3790929677351467\n",
-                        "Accuracy on hold-out set: 0.19811320754716982\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
+                        "Loss on hold-out set: 2.3934816279501283\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.2421383647798742\n",
                         "Epoch: 57\n",
-                        "Loss on hold-out set: 2.379202374872172\n",
-                        "Accuracy on hold-out set: 0.19339622641509435\n",
-                        "Metric value on hold-out data: 0.2083333333333333\n",
+                        "Loss on hold-out set: 2.3934031972345315\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.23349056603773582\n",
                         "Epoch: 58\n",
-                        "Loss on hold-out set: 2.378715991973877\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
+                        "Loss on hold-out set: 2.3932295925212355\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.22327044025157233\n",
                         "Epoch: 59\n",
-                        "Loss on hold-out set: 2.3763908980027684\n",
-                        "Accuracy on hold-out set: 0.20754716981132076\n",
-                        "Metric value on hold-out data: 0.21226415094339618\n",
+                        "Loss on hold-out set: 2.3930805764108336\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.2366352201257861\n",
                         "Epoch: 60\n",
-                        "Loss on hold-out set: 2.376155007560298\n",
-                        "Accuracy on hold-out set: 0.20754716981132076\n",
-                        "Metric value on hold-out data: 0.21540880503144652\n",
+                        "Loss on hold-out set: 2.3935058071928204\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.23270440251572325\n",
                         "Epoch: 61\n",
-                        "Loss on hold-out set: 2.376491708575555\n",
-                        "Accuracy on hold-out set: 0.21226415094339623\n",
-                        "Metric value on hold-out data: 0.21305031446540879\n",
+                        "Loss on hold-out set: 2.393243636725084\n",
+                        "Accuracy on hold-out set: 0.13679245283018868\n",
+                        "Metric value on hold-out data: 0.24135220125786164\n",
                         "Epoch: 62\n",
-                        "Loss on hold-out set: 2.3747395794346646\n",
-                        "Accuracy on hold-out set: 0.22169811320754718\n",
-                        "Metric value on hold-out data: 0.22641509433962265\n",
+                        "Loss on hold-out set: 2.392829377696199\n",
+                        "Accuracy on hold-out set: 0.13679245283018868\n",
+                        "Metric value on hold-out data: 0.23820754716981132\n",
                         "Epoch: 63\n",
-                        "Loss on hold-out set: 2.373830457903304\n",
-                        "Accuracy on hold-out set: 0.22641509433962265\n",
-                        "Metric value on hold-out data: 0.23113207547169812\n",
+                        "Loss on hold-out set: 2.392202030937627\n",
+                        "Accuracy on hold-out set: 0.13679245283018868\n",
+                        "Metric value on hold-out data: 0.24371069182389937\n",
                         "Epoch: 64\n",
-                        "Loss on hold-out set: 2.374308406182055\n",
-                        "Accuracy on hold-out set: 0.22169811320754718\n",
-                        "Metric value on hold-out data: 0.23270440251572325\n",
-                        "Returned to Spot: Validation loss: 2.374308406182055\n",
+                        "Loss on hold-out set: 2.3926828672301093\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.2429245283018868\n",
+                        "Returned to Spot: Validation loss: 2.3926828672301093\n",
                         "----------------------------------------------\n",
                         "\n",
-                        "config: {'l1': 512, 'dropout_prob': 0.07234256022028937, 'lr_mult': 0.001, 'batch_size': 8, 'epochs': 64, 'k_folds': 1, 'patience': 15, 'optimizer': 'Adam', 'sgd_momentum': 0.9}\n",
+                        "config: {'l1': 1024, 'dropout_prob': 0.13021660839652088, 'lr_mult': 0.001, 'batch_size': 8, 'epochs': 64, 'k_folds': 1, 'patience': 16, 'optimizer': 'Adagrad', 'sgd_momentum': 0.9}\n",
                         "Epoch: 1\n",
-                        "Loss on hold-out set: 2.398621603294655\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.3978185918596058\n",
+                        "Accuracy on hold-out set: 0.04716981132075472\n",
+                        "Metric value on hold-out data: 0.15251572327044022\n",
                         "Epoch: 2\n",
-                        "Loss on hold-out set: 2.3985382980770535\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397808799037227\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.14622641509433962\n",
                         "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3985648949941\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.3977924982706704\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.1580188679245283\n",
                         "Epoch: 4\n",
-                        "Loss on hold-out set: 2.3985551993052163\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.3977862199147544\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.1611635220125786\n",
                         "Epoch: 5\n",
-                        "Loss on hold-out set: 2.398563058288009\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.3977967456535056\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.1470125786163522\n",
                         "Epoch: 6\n",
-                        "Loss on hold-out set: 2.398517891212746\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397767455489547\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 7\n",
-                        "Loss on hold-out set: 2.398453809596874\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397750651394879\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.15015723270440254\n",
                         "Epoch: 8\n",
-                        "Loss on hold-out set: 2.398458224755746\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.3977799768801087\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.16273584905660377\n",
                         "Epoch: 9\n",
-                        "Loss on hold-out set: 2.3984116006780556\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397786573127464\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.1470125786163522\n",
                         "Epoch: 10\n",
-                        "Loss on hold-out set: 2.398384359147814\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397786440672698\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.1540880503144654\n",
                         "Epoch: 11\n",
-                        "Loss on hold-out set: 2.398391838426943\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397733626542268\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.154874213836478\n",
                         "Epoch: 12\n",
-                        "Loss on hold-out set: 2.3983223526566118\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397743852050216\n",
+                        "Accuracy on hold-out set: 0.04716981132075472\n",
+                        "Metric value on hold-out data: 0.1430817610062893\n",
                         "Epoch: 13\n",
-                        "Loss on hold-out set: 2.3983462298357927\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.1391509433962264\n",
+                        "Loss on hold-out set: 2.397776382940787\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 14\n",
-                        "Loss on hold-out set: 2.398298660914103\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.3977049456702337\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.1792452830188679\n",
                         "Epoch: 15\n",
-                        "Loss on hold-out set: 2.398263198358041\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397721449534098\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.175314465408805\n",
                         "Epoch: 16\n",
-                        "Loss on hold-out set: 2.398226914582429\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.1391509433962264\n",
+                        "Loss on hold-out set: 2.39769857901114\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.1572327044025157\n",
                         "Epoch: 17\n",
-                        "Loss on hold-out set: 2.3982527256011963\n",
-                        "Accuracy on hold-out set: 0.07075471698113207\n",
-                        "Metric value on hold-out data: 0.13522012578616352\n",
+                        "Loss on hold-out set: 2.397750642564562\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.16037735849056603\n",
                         "Epoch: 18\n",
-                        "Loss on hold-out set: 2.3981768466808178\n",
-                        "Accuracy on hold-out set: 0.08018867924528301\n",
-                        "Metric value on hold-out data: 0.139937106918239\n",
+                        "Loss on hold-out set: 2.3977688506797508\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.15015723270440248\n",
                         "Epoch: 19\n",
-                        "Loss on hold-out set: 2.398127070179692\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13757861635220126\n",
+                        "Loss on hold-out set: 2.397757150508739\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
                         "Epoch: 20\n",
-                        "Loss on hold-out set: 2.3980964378074363\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.14465408805031446\n",
+                        "Loss on hold-out set: 2.3977322666733354\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.1611635220125786\n",
                         "Epoch: 21\n",
-                        "Loss on hold-out set: 2.3980763223436146\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.14622641509433962\n",
+                        "Loss on hold-out set: 2.397728619752107\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.16194968553459116\n",
                         "Epoch: 22\n",
-                        "Loss on hold-out set: 2.3979833126068115\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.14622641509433962\n",
+                        "Loss on hold-out set: 2.397732761171129\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 23\n",
-                        "Loss on hold-out set: 2.397993396829676\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.14386792452830188\n",
+                        "Loss on hold-out set: 2.397667081267745\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.17059748427672955\n",
                         "Epoch: 24\n",
-                        "Loss on hold-out set: 2.3979679213629828\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.14229559748427673\n",
+                        "Loss on hold-out set: 2.397706075950905\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.1470125786163522\n",
                         "Epoch: 25\n",
-                        "Loss on hold-out set: 2.397877013241803\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.1509433962264151\n",
+                        "Loss on hold-out set: 2.3976862607178866\n",
+                        "Accuracy on hold-out set: 0.04245283018867924\n",
+                        "Metric value on hold-out data: 0.15880503144654087\n",
                         "Epoch: 26\n",
-                        "Loss on hold-out set: 2.3978866117971913\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1501572327044025\n",
+                        "Loss on hold-out set: 2.3977313306596546\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.1540880503144654\n",
                         "Epoch: 27\n",
-                        "Loss on hold-out set: 2.3978260887993708\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.1470125786163522\n",
+                        "Loss on hold-out set: 2.397729414480704\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.1721698113207547\n",
                         "Epoch: 28\n",
-                        "Loss on hold-out set: 2.397790864661888\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.14937106918238993\n",
+                        "Loss on hold-out set: 2.3977426952785916\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.1611635220125786\n",
                         "Epoch: 29\n",
-                        "Loss on hold-out set: 2.397690022433246\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1540880503144654\n",
+                        "Loss on hold-out set: 2.3976884153154163\n",
+                        "Accuracy on hold-out set: 0.04716981132075472\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 30\n",
-                        "Loss on hold-out set: 2.397740770269323\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.1509433962264151\n",
+                        "Loss on hold-out set: 2.3976377734431513\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.16430817610062892\n",
                         "Epoch: 31\n",
-                        "Loss on hold-out set: 2.3977119481122053\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.15644654088050314\n",
+                        "Loss on hold-out set: 2.3976722911552146\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.16037735849056603\n",
                         "Epoch: 32\n",
-                        "Loss on hold-out set: 2.3976342236554182\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1540880503144654\n",
+                        "Loss on hold-out set: 2.3976691828833685\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.1580188679245283\n",
                         "Epoch: 33\n",
-                        "Loss on hold-out set: 2.3976695096051253\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1611635220125786\n",
+                        "Loss on hold-out set: 2.3977338119789406\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.1572327044025157\n",
                         "Epoch: 34\n",
-                        "Loss on hold-out set: 2.3976621981020325\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1540880503144654\n",
+                        "Loss on hold-out set: 2.3977428807152643\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.15644654088050314\n",
                         "Epoch: 35\n",
-                        "Loss on hold-out set: 2.397641102472941\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1509433962264151\n",
+                        "Loss on hold-out set: 2.3977352071691445\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 36\n",
-                        "Loss on hold-out set: 2.3975503621277987\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.15172955974842767\n",
+                        "Loss on hold-out set: 2.397707771371912\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.16352201257861634\n",
                         "Epoch: 37\n",
-                        "Loss on hold-out set: 2.3975599341922336\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.15959119496855342\n",
+                        "Loss on hold-out set: 2.397698896902579\n",
+                        "Accuracy on hold-out set: 0.04245283018867924\n",
+                        "Metric value on hold-out data: 0.14858490566037735\n",
                         "Epoch: 38\n",
-                        "Loss on hold-out set: 2.3974230466065585\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15566037735849056\n",
+                        "Loss on hold-out set: 2.3976289166344538\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.15959119496855342\n",
                         "Epoch: 39\n",
-                        "Loss on hold-out set: 2.397432389082732\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1658805031446541\n",
+                        "Loss on hold-out set: 2.3977057050775596\n",
+                        "Accuracy on hold-out set: 0.08018867924528301\n",
+                        "Metric value on hold-out data: 0.16981132075471694\n",
                         "Epoch: 40\n",
-                        "Loss on hold-out set: 2.3973543820557772\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.1690251572327044\n",
+                        "Loss on hold-out set: 2.397685828032317\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.17531446540880502\n",
                         "Epoch: 41\n",
-                        "Loss on hold-out set: 2.397287536550451\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16352201257861634\n",
+                        "Loss on hold-out set: 2.397723736586394\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.15487421383647795\n",
                         "Epoch: 42\n",
-                        "Loss on hold-out set: 2.39732207192315\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16430817610062892\n",
+                        "Loss on hold-out set: 2.397614487895259\n",
+                        "Accuracy on hold-out set: 0.08018867924528301\n",
+                        "Metric value on hold-out data: 0.1682389937106918\n",
                         "Epoch: 43\n",
-                        "Loss on hold-out set: 2.3973352290965892\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16666666666666669\n",
-                        "Epoch: 44\n",
-                        "Loss on hold-out set: 2.3971631791856556\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Loss on hold-out set: 2.397654074209708\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
                         "Metric value on hold-out data: 0.16823899371069181\n",
+                        "Epoch: 44\n",
+                        "Loss on hold-out set: 2.3976557519700794\n",
+                        "Accuracy on hold-out set: 0.08018867924528301\n",
+                        "Metric value on hold-out data: 0.1690251572327044\n",
                         "Epoch: 45\n",
-                        "Loss on hold-out set: 2.397234589965255\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.17845911949685533\n",
+                        "Loss on hold-out set: 2.3976608382331\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
                         "Epoch: 46\n",
-                        "Loss on hold-out set: 2.397164892267298\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16430817610062892\n",
+                        "Loss on hold-out set: 2.397616465886434\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.14937106918238993\n",
                         "Epoch: 47\n",
-                        "Loss on hold-out set: 2.3971985799294933\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16666666666666666\n",
+                        "Loss on hold-out set: 2.3976390626695423\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.1572327044025157\n",
                         "Epoch: 48\n",
-                        "Loss on hold-out set: 2.3971541546009205\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.16352201257861634\n",
+                        "Loss on hold-out set: 2.3976178610766374\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 49\n",
-                        "Loss on hold-out set: 2.3970036065136946\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.17452830188679244\n",
+                        "Loss on hold-out set: 2.397597551345825\n",
+                        "Accuracy on hold-out set: 0.0660377358490566\n",
+                        "Metric value on hold-out data: 0.16981132075471697\n",
                         "Epoch: 50\n",
-                        "Loss on hold-out set: 2.3970601382078947\n",
-                        "Accuracy on hold-out set: 0.08018867924528301\n",
-                        "Metric value on hold-out data: 0.17138364779874213\n",
+                        "Loss on hold-out set: 2.397609251516837\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.16430817610062895\n",
                         "Epoch: 51\n",
-                        "Loss on hold-out set: 2.396933679227476\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1800314465408805\n",
+                        "Loss on hold-out set: 2.39769587693391\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.16194968553459116\n",
                         "Epoch: 52\n",
-                        "Loss on hold-out set: 2.3969930366233543\n",
-                        "Accuracy on hold-out set: 0.08018867924528301\n",
-                        "Metric value on hold-out data: 0.17374213836477986\n",
+                        "Loss on hold-out set: 2.3977417327739574\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.14622641509433962\n",
                         "Epoch: 53\n",
-                        "Loss on hold-out set: 2.3969560464223227\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.17295597484276728\n",
+                        "Loss on hold-out set: 2.3975724202615245\n",
+                        "Accuracy on hold-out set: 0.08018867924528301\n",
+                        "Metric value on hold-out data: 0.17059748427672952\n",
                         "Epoch: 54\n",
-                        "Loss on hold-out set: 2.396885907208478\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.1792452830188679\n",
+                        "Loss on hold-out set: 2.3976441754235163\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.17138364779874213\n",
                         "Epoch: 55\n",
-                        "Loss on hold-out set: 2.3968406694906728\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.18946540880503143\n",
+                        "Loss on hold-out set: 2.3975998560587564\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.17059748427672955\n",
                         "Epoch: 56\n",
-                        "Loss on hold-out set: 2.3967945134198225\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.18946540880503143\n",
+                        "Loss on hold-out set: 2.3976108851256193\n",
+                        "Accuracy on hold-out set: 0.05188679245283019\n",
+                        "Metric value on hold-out data: 0.15330188679245282\n",
                         "Epoch: 57\n",
-                        "Loss on hold-out set: 2.3967492315504284\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.17845911949685533\n",
+                        "Loss on hold-out set: 2.3975879351298013\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.1792452830188679\n",
                         "Epoch: 58\n",
-                        "Loss on hold-out set: 2.3968848387400308\n",
+                        "Loss on hold-out set: 2.397624695742572\n",
                         "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.18081761006289307\n",
+                        "Metric value on hold-out data: 0.17138364779874213\n",
                         "Epoch: 59\n",
-                        "Loss on hold-out set: 2.3965117931365967\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.19732704402515722\n",
+                        "Loss on hold-out set: 2.3976704721097595\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.15880503144654087\n",
                         "Epoch: 60\n",
-                        "Loss on hold-out set: 2.3964751649785927\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.21069182389937108\n",
+                        "Loss on hold-out set: 2.3976544274224176\n",
+                        "Accuracy on hold-out set: 0.04716981132075472\n",
+                        "Metric value on hold-out data: 0.15251572327044022\n",
                         "Epoch: 61\n",
-                        "Loss on hold-out set: 2.3964628731762923\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.2091194968553459\n",
+                        "Loss on hold-out set: 2.3975575588367604\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
                         "Epoch: 62\n",
-                        "Loss on hold-out set: 2.3965328092928284\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.20676100628930816\n",
+                        "Loss on hold-out set: 2.397552454913104\n",
+                        "Accuracy on hold-out set: 0.05660377358490566\n",
+                        "Metric value on hold-out data: 0.15330188679245282\n",
                         "Epoch: 63\n",
-                        "Loss on hold-out set: 2.3963339417069047\n",
-                        "Accuracy on hold-out set: 0.13679245283018868\n",
-                        "Metric value on hold-out data: 0.22955974842767293\n",
+                        "Loss on hold-out set: 2.3976587454477944\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.16588050314465408\n",
                         "Epoch: 64\n",
-                        "Loss on hold-out set: 2.3963725213651306\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.20676100628930816\n",
-                        "Returned to Spot: Validation loss: 2.3963725213651306\n",
+                        "Loss on hold-out set: 2.3976620656472667\n",
+                        "Accuracy on hold-out set: 0.09433962264150944\n",
+                        "Metric value on hold-out data: 0.1823899371069182\n",
+                        "Returned to Spot: Validation loss: 2.3976620656472667\n",
                         "----------------------------------------------\n",
                         "\n",
-                        "config: {'l1': 256, 'dropout_prob': 0.27862370366249045, 'lr_mult': 0.001, 'batch_size': 16, 'epochs': 256, 'k_folds': 1, 'patience': 2, 'optimizer': 'SGD', 'sgd_momentum': 0.9}\n",
+                        "config: {'l1': 256, 'dropout_prob': 0.5015226665924828, 'lr_mult': 0.001, 'batch_size': 16, 'epochs': 256, 'k_folds': 1, 'patience': 2, 'optimizer': 'NAdam', 'sgd_momentum': 0.9}\n",
                         "Epoch: 1\n",
-                        "Loss on hold-out set: 2.39814361504146\n",
+                        "Loss on hold-out set: 2.3978573254176547\n",
                         "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.17138364779874216\n",
+                        "Metric value on hold-out data: 0.17767295597484276\n",
                         "Epoch: 2\n",
-                        "Loss on hold-out set: 2.3981014830725536\n",
+                        "Loss on hold-out set: 2.397653715951102\n",
                         "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.17138364779874216\n",
+                        "Metric value on hold-out data: 0.1761006289308176\n",
                         "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3980645963123868\n",
+                        "Loss on hold-out set: 2.397729124341692\n",
                         "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.16981132075471697\n",
+                        "Metric value on hold-out data: 0.17374213836477986\n",
                         "Epoch: 4\n",
-                        "Loss on hold-out set: 2.398202521460397\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.17138364779874216\n",
-                        "Epoch: 5\n",
-                        "Loss on hold-out set: 2.3981470550809587\n",
+                        "Loss on hold-out set: 2.3978255135672435\n",
                         "Accuracy on hold-out set: 0.09433962264150944\n",
                         "Metric value on hold-out data: 0.17059748427672958\n",
-                        "Early stopping at epoch 4\n",
-                        "Returned to Spot: Validation loss: 2.3981470550809587\n",
+                        "Early stopping at epoch 3\n",
+                        "Returned to Spot: Validation loss: 2.3978255135672435\n",
                         "----------------------------------------------\n",
                         "\n",
-                        "config: {'l1': 512, 'dropout_prob': 0.14818349631472857, 'lr_mult': 0.001, 'batch_size': 8, 'epochs': 32, 'k_folds': 1, 'patience': 7, 'optimizer': 'SGD', 'sgd_momentum': 0.9}\n",
+                        "config: {'l1': 512, 'dropout_prob': 0.26673029336651144, 'lr_mult': 0.001, 'batch_size': 8, 'epochs': 32, 'k_folds': 1, 'patience': 4, 'optimizer': 'Adamax', 'sgd_momentum': 0.9}\n",
                         "Epoch: 1\n",
-                        "Loss on hold-out set: 2.397899521721734\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17138364779874213\n",
+                        "Loss on hold-out set: 2.3979083078878896\n",
+                        "Accuracy on hold-out set: 0.12735849056603774\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
                         "Epoch: 2\n",
-                        "Loss on hold-out set: 2.397863476364701\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.17295597484276728\n",
+                        "Loss on hold-out set: 2.39787048763699\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.16037735849056603\n",
                         "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3978229805275246\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17374213836477986\n",
+                        "Loss on hold-out set: 2.3979297832206443\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.16037735849056603\n",
                         "Epoch: 4\n",
-                        "Loss on hold-out set: 2.3978375417214854\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.17059748427672955\n",
+                        "Loss on hold-out set: 2.3979586053777626\n",
+                        "Accuracy on hold-out set: 0.12735849056603774\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
                         "Epoch: 5\n",
-                        "Loss on hold-out set: 2.3978341862007424\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17452830188679244\n",
+                        "Loss on hold-out set: 2.3979275403199374\n",
+                        "Accuracy on hold-out set: 0.12735849056603774\n",
+                        "Metric value on hold-out data: 0.16430817610062895\n",
                         "Epoch: 6\n",
-                        "Loss on hold-out set: 2.397893331668995\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17531446540880502\n",
-                        "Epoch: 7\n",
-                        "Loss on hold-out set: 2.3978056289531566\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17295597484276728\n",
-                        "Epoch: 8\n",
-                        "Loss on hold-out set: 2.397886867876406\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17452830188679244\n",
-                        "Epoch: 9\n",
-                        "Loss on hold-out set: 2.397837038393374\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.17138364779874213\n",
-                        "Epoch: 10\n",
-                        "Loss on hold-out set: 2.3978577808097556\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17374213836477986\n",
-                        "Epoch: 11\n",
-                        "Loss on hold-out set: 2.3978946385560214\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.17374213836477986\n",
-                        "Epoch: 12\n",
-                        "Loss on hold-out set: 2.39782542652554\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17845911949685533\n",
-                        "Epoch: 13\n",
-                        "Loss on hold-out set: 2.397847299222593\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17295597484276728\n",
-                        "Epoch: 14\n",
-                        "Loss on hold-out set: 2.397842795760543\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.17452830188679244\n",
-                        "Early stopping at epoch 13\n",
-                        "Returned to Spot: Validation loss: 2.397842795760543\n",
+                        "Loss on hold-out set: 2.397910789207176\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.16273584905660377\n",
+                        "Early stopping at epoch 5\n",
+                        "Returned to Spot: Validation loss: 2.397910789207176\n",
                         "----------------------------------------------\n",
                         "\n",
-                        "config: {'l1': 1024, 'dropout_prob': 0.4985105083239768, 'lr_mult': 0.001, 'batch_size': 2, 'epochs': 128, 'k_folds': 1, 'patience': 9, 'optimizer': 'Adam', 'sgd_momentum': 0.9}\n",
+                        "config: {'l1': 4096, 'dropout_prob': 0.8973189149831583, 'lr_mult': 0.001, 'batch_size': 2, 'epochs': 128, 'k_folds': 1, 'patience': 8, 'optimizer': 'Adam', 'sgd_momentum': 0.9}\n",
                         "Epoch: 1\n",
-                        "Loss on hold-out set: 2.3984706649240457\n",
-                        "Accuracy on hold-out set: 0.07075471698113207\n",
-                        "Metric value on hold-out data: 0.125\n",
+                        "Loss on hold-out set: 2.3974252421900912\n",
+                        "Accuracy on hold-out set: 0.08018867924528301\n",
+                        "Metric value on hold-out data: 0.160377358490566\n",
                         "Epoch: 2\n",
-                        "Loss on hold-out set: 2.3985311107815437\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.12735849056603774\n",
+                        "Loss on hold-out set: 2.397167354259851\n",
+                        "Accuracy on hold-out set: 0.08962264150943396\n",
+                        "Metric value on hold-out data: 0.17452830188679244\n",
                         "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3984468770477005\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.12735849056603774\n",
+                        "Loss on hold-out set: 2.39734241197694\n",
+                        "Accuracy on hold-out set: 0.12735849056603774\n",
+                        "Metric value on hold-out data: 0.20361635220125784\n",
                         "Epoch: 4\n",
-                        "Loss on hold-out set: 2.398400698068007\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.125\n",
+                        "Loss on hold-out set: 2.396712690029504\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 5\n",
-                        "Loss on hold-out set: 2.3983855517405384\n",
-                        "Accuracy on hold-out set: 0.0660377358490566\n",
-                        "Metric value on hold-out data: 0.12185534591194966\n",
+                        "Loss on hold-out set: 2.3971359572320616\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.19968553459119495\n",
                         "Epoch: 6\n",
-                        "Loss on hold-out set: 2.3984305093873224\n",
-                        "Accuracy on hold-out set: 0.08018867924528301\n",
-                        "Metric value on hold-out data: 0.13286163522012578\n",
+                        "Loss on hold-out set: 2.39687288257311\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.2059748427672956\n",
                         "Epoch: 7\n",
-                        "Loss on hold-out set: 2.3984723878356644\n",
-                        "Accuracy on hold-out set: 0.07075471698113207\n",
-                        "Metric value on hold-out data: 0.1312893081761006\n",
+                        "Loss on hold-out set: 2.3965237680471168\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.190251572327044\n",
                         "Epoch: 8\n",
-                        "Loss on hold-out set: 2.398266803543523\n",
-                        "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.13443396226415094\n",
+                        "Loss on hold-out set: 2.396331690392404\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1808176100628931\n",
                         "Epoch: 9\n",
-                        "Loss on hold-out set: 2.398327208914847\n",
+                        "Loss on hold-out set: 2.3969954544643186\n",
                         "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.14229559748427673\n",
+                        "Metric value on hold-out data: 0.16981132075471697\n",
                         "Epoch: 10\n",
-                        "Loss on hold-out set: 2.398228020038245\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.14465408805031446\n",
+                        "Loss on hold-out set: 2.3965100612280503\n",
+                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Metric value on hold-out data: 0.19968553459119495\n",
                         "Epoch: 11\n",
-                        "Loss on hold-out set: 2.398125655246231\n",
+                        "Loss on hold-out set: 2.3968354148684807\n",
                         "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1501572327044025\n",
+                        "Metric value on hold-out data: 0.18553459119496854\n",
                         "Epoch: 12\n",
-                        "Loss on hold-out set: 2.398153266816769\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.16194968553459116\n",
+                        "Loss on hold-out set: 2.396859533381912\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19261006289308175\n",
                         "Epoch: 13\n",
-                        "Loss on hold-out set: 2.39807631834498\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.16352201257861634\n",
+                        "Loss on hold-out set: 2.396657705307007\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.1957547169811321\n",
                         "Epoch: 14\n",
-                        "Loss on hold-out set: 2.398075837009358\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.16194968553459116\n",
+                        "Loss on hold-out set: 2.396268797370623\n",
+                        "Accuracy on hold-out set: 0.10377358490566038\n",
+                        "Metric value on hold-out data: 0.18867924528301888\n",
                         "Epoch: 15\n",
-                        "Loss on hold-out set: 2.397934947373732\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.16666666666666666\n",
+                        "Loss on hold-out set: 2.39629372560753\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19889937106918237\n",
                         "Epoch: 16\n",
-                        "Loss on hold-out set: 2.3979991404515393\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.1792452830188679\n",
+                        "Loss on hold-out set: 2.3963710901872166\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.2028301886792453\n",
                         "Epoch: 17\n",
-                        "Loss on hold-out set: 2.397973229300301\n",
-                        "Accuracy on hold-out set: 0.13679245283018868\n",
-                        "Metric value on hold-out data: 0.17138364779874216\n",
+                        "Loss on hold-out set: 2.3960609031173417\n",
+                        "Accuracy on hold-out set: 0.10377358490566038\n",
+                        "Metric value on hold-out data: 0.19496855345911948\n",
                         "Epoch: 18\n",
-                        "Loss on hold-out set: 2.3982589492258035\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.17688679245283018\n",
+                        "Loss on hold-out set: 2.396002321873071\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19103773584905662\n",
                         "Epoch: 19\n",
-                        "Loss on hold-out set: 2.397810265703021\n",
-                        "Accuracy on hold-out set: 0.14622641509433962\n",
-                        "Metric value on hold-out data: 0.18946540880503143\n",
+                        "Loss on hold-out set: 2.395084277638849\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1988993710691824\n",
                         "Epoch: 20\n",
-                        "Loss on hold-out set: 2.397795796394348\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.1792452830188679\n",
+                        "Loss on hold-out set: 2.396092381117479\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1941823899371069\n",
                         "Epoch: 21\n",
-                        "Loss on hold-out set: 2.3974974222902983\n",
-                        "Accuracy on hold-out set: 0.15566037735849056\n",
-                        "Metric value on hold-out data: 0.20047169811320756\n",
+                        "Loss on hold-out set: 2.3957636603769266\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1949685534591195\n",
                         "Epoch: 22\n",
-                        "Loss on hold-out set: 2.3976023512066535\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.17845911949685533\n",
+                        "Loss on hold-out set: 2.3949042941039465\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19418238993710688\n",
                         "Epoch: 23\n",
-                        "Loss on hold-out set: 2.3976079945294364\n",
-                        "Accuracy on hold-out set: 0.15566037735849056\n",
-                        "Metric value on hold-out data: 0.19103773584905662\n",
+                        "Loss on hold-out set: 2.395458952435907\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20361635220125787\n",
                         "Epoch: 24\n",
-                        "Loss on hold-out set: 2.397568408048378\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.19811320754716982\n",
+                        "Loss on hold-out set: 2.3959749059857063\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.18474842767295596\n",
                         "Epoch: 25\n",
-                        "Loss on hold-out set: 2.3972808302573436\n",
-                        "Accuracy on hold-out set: 0.14622641509433962\n",
-                        "Metric value on hold-out data: 0.20047169811320756\n",
+                        "Loss on hold-out set: 2.395475873407328\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1988993710691824\n",
                         "Epoch: 26\n",
-                        "Loss on hold-out set: 2.3972933854696885\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.18160377358490565\n",
+                        "Loss on hold-out set: 2.3953974696825133\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20518867924528303\n",
                         "Epoch: 27\n",
-                        "Loss on hold-out set: 2.397120660206057\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.18553459119496857\n",
+                        "Loss on hold-out set: 2.3954039182303086\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1957547169811321\n",
                         "Epoch: 28\n",
-                        "Loss on hold-out set: 2.397097353665334\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.1871069182389937\n",
+                        "Loss on hold-out set: 2.395362428899081\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 29\n",
-                        "Loss on hold-out set: 2.3970767304582417\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.19968553459119495\n",
-                        "Epoch: 30\n",
-                        "Loss on hold-out set: 2.396994602005437\n",
-                        "Accuracy on hold-out set: 0.13679245283018868\n",
+                        "Loss on hold-out set: 2.3953650649988427\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
                         "Metric value on hold-out data: 0.20518867924528303\n",
+                        "Epoch: 30\n",
+                        "Loss on hold-out set: 2.3948268552996077\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1957547169811321\n",
                         "Epoch: 31\n",
-                        "Loss on hold-out set: 2.3966026238675386\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.190251572327044\n",
+                        "Loss on hold-out set: 2.3949433835047595\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515724\n",
                         "Epoch: 32\n",
-                        "Loss on hold-out set: 2.3968309636385934\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.19654088050314464\n",
+                        "Loss on hold-out set: 2.394887346141743\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20047169811320756\n",
                         "Epoch: 33\n",
-                        "Loss on hold-out set: 2.396765245581573\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.19496855345911948\n",
+                        "Loss on hold-out set: 2.395097991205611\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20047169811320756\n",
                         "Epoch: 34\n",
-                        "Loss on hold-out set: 2.3963446032326177\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.19654088050314467\n",
+                        "Loss on hold-out set: 2.3945818847080447\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19889937106918237\n",
                         "Epoch: 35\n",
-                        "Loss on hold-out set: 2.396624601112222\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.1941823899371069\n",
+                        "Loss on hold-out set: 2.394891415002211\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.18946540880503143\n",
                         "Epoch: 36\n",
-                        "Loss on hold-out set: 2.396144797217171\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.19339622641509435\n",
+                        "Loss on hold-out set: 2.394350571452447\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20047169811320756\n",
                         "Epoch: 37\n",
-                        "Loss on hold-out set: 2.395833861153081\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.19968553459119495\n",
+                        "Loss on hold-out set: 2.3938301464296736\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19889937106918237\n",
                         "Epoch: 38\n",
-                        "Loss on hold-out set: 2.3964456252332003\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.18946540880503143\n",
+                        "Loss on hold-out set: 2.3942759711787387\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 39\n",
-                        "Loss on hold-out set: 2.3959577713372573\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.20361635220125784\n",
+                        "Loss on hold-out set: 2.393760046868954\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1957547169811321\n",
                         "Epoch: 40\n",
-                        "Loss on hold-out set: 2.3956829197001905\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.2020440251572327\n",
+                        "Loss on hold-out set: 2.393799014811246\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20047169811320756\n",
                         "Epoch: 41\n",
-                        "Loss on hold-out set: 2.395629698375486\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.1957547169811321\n",
+                        "Loss on hold-out set: 2.3944950486129186\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 42\n",
-                        "Loss on hold-out set: 2.3958063395518177\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.19339622641509435\n",
+                        "Loss on hold-out set: 2.3938607742201605\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19889937106918237\n",
                         "Epoch: 43\n",
-                        "Loss on hold-out set: 2.395712344151623\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.18946540880503143\n",
+                        "Loss on hold-out set: 2.393720012790752\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19889937106918235\n",
                         "Epoch: 44\n",
-                        "Loss on hold-out set: 2.3954653784913837\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.2012578616352201\n",
+                        "Loss on hold-out set: 2.3936962159174793\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1941823899371069\n",
                         "Epoch: 45\n",
-                        "Loss on hold-out set: 2.395172935611797\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.2020440251572327\n",
+                        "Loss on hold-out set: 2.3934320008979655\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19261006289308175\n",
                         "Epoch: 46\n",
-                        "Loss on hold-out set: 2.394848938258189\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
+                        "Loss on hold-out set: 2.393129431976462\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1957547169811321\n",
                         "Epoch: 47\n",
-                        "Loss on hold-out set: 2.3947587058229267\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.20440251572327042\n",
+                        "Loss on hold-out set: 2.392929477511712\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 48\n",
-                        "Loss on hold-out set: 2.3943354723588475\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.20754716981132076\n",
+                        "Loss on hold-out set: 2.393271785862041\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19889937106918237\n",
                         "Epoch: 49\n",
-                        "Loss on hold-out set: 2.394335445368065\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20676100628930816\n",
+                        "Loss on hold-out set: 2.3927366216227695\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.2020440251572327\n",
                         "Epoch: 50\n",
-                        "Loss on hold-out set: 2.393751990120366\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
+                        "Loss on hold-out set: 2.392670858581111\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 51\n",
-                        "Loss on hold-out set: 2.393896240108418\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.2012578616352201\n",
+                        "Loss on hold-out set: 2.3928990386567026\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20047169811320756\n",
                         "Epoch: 52\n",
-                        "Loss on hold-out set: 2.3942593043705203\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.19339622641509435\n",
+                        "Loss on hold-out set: 2.3923709572486156\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1957547169811321\n",
                         "Epoch: 53\n",
-                        "Loss on hold-out set: 2.393578770025721\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.19968553459119495\n",
+                        "Loss on hold-out set: 2.392177608777892\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.20047169811320756\n",
                         "Epoch: 54\n",
-                        "Loss on hold-out set: 2.3928858086747944\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.2099056603773585\n",
+                        "Loss on hold-out set: 2.3920937709088594\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 55\n",
-                        "Loss on hold-out set: 2.3934241735710287\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.2020440251572327\n",
+                        "Loss on hold-out set: 2.3927634009775125\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 56\n",
-                        "Loss on hold-out set: 2.3935234749092245\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.20833333333333331\n",
+                        "Loss on hold-out set: 2.393366375059452\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1941823899371069\n",
                         "Epoch: 57\n",
-                        "Loss on hold-out set: 2.392237256158073\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.19182389937106917\n",
-                        "Epoch: 58\n",
-                        "Loss on hold-out set: 2.392963760304001\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Loss on hold-out set: 2.392240339854978\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
                         "Metric value on hold-out data: 0.19732704402515722\n",
-                        "Epoch: 59\n",
-                        "Loss on hold-out set: 2.3927618400105892\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
+                        "Epoch: 58\n",
+                        "Loss on hold-out set: 2.392733115070271\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
                         "Metric value on hold-out data: 0.20047169811320756\n",
+                        "Epoch: 59\n",
+                        "Loss on hold-out set: 2.3923156036520905\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 60\n",
-                        "Loss on hold-out set: 2.3920663640184223\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
+                        "Loss on hold-out set: 2.393243029432477\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.19732704402515722\n",
                         "Epoch: 61\n",
-                        "Loss on hold-out set: 2.3913381662008897\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.21147798742138363\n",
-                        "Epoch: 62\n",
-                        "Loss on hold-out set: 2.3914709113678843\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.20361635220125784\n",
-                        "Epoch: 63\n",
-                        "Loss on hold-out set: 2.3922014596327297\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.1957547169811321\n",
-                        "Epoch: 64\n",
-                        "Loss on hold-out set: 2.3921572622263207\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.2091194968553459\n",
-                        "Epoch: 65\n",
-                        "Loss on hold-out set: 2.3913895926385558\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.20597484276729558\n",
-                        "Epoch: 66\n",
-                        "Loss on hold-out set: 2.3914309875020443\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20833333333333331\n",
-                        "Epoch: 67\n",
-                        "Loss on hold-out set: 2.390503028653703\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20047169811320756\n",
-                        "Epoch: 68\n",
-                        "Loss on hold-out set: 2.391280693827935\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
-                        "Epoch: 69\n",
-                        "Loss on hold-out set: 2.3915035072362647\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
-                        "Epoch: 70\n",
-                        "Loss on hold-out set: 2.3906592782938256\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2020440251572327\n",
-                        "Epoch: 71\n",
-                        "Loss on hold-out set: 2.390226222434134\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20676100628930816\n",
-                        "Epoch: 72\n",
-                        "Loss on hold-out set: 2.3902140855789185\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20911949685534592\n",
-                        "Epoch: 73\n",
-                        "Loss on hold-out set: 2.3884516099713884\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.21226415094339623\n",
-                        "Epoch: 74\n",
-                        "Loss on hold-out set: 2.390740081949054\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20754716981132076\n",
-                        "Epoch: 75\n",
-                        "Loss on hold-out set: 2.3898368803959973\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20518867924528303\n",
-                        "Epoch: 76\n",
-                        "Loss on hold-out set: 2.3884831599469454\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2020440251572327\n",
-                        "Epoch: 77\n",
-                        "Loss on hold-out set: 2.3903399998286985\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2020440251572327\n",
-                        "Epoch: 78\n",
-                        "Loss on hold-out set: 2.3866485537223094\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2099056603773585\n",
-                        "Epoch: 79\n",
-                        "Loss on hold-out set: 2.3878014762446567\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.21462264150943397\n",
-                        "Epoch: 80\n",
-                        "Loss on hold-out set: 2.3902634922063575\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.20361635220125784\n",
-                        "Epoch: 81\n",
-                        "Loss on hold-out set: 2.3885116307240613\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2028301886792453\n",
-                        "Epoch: 82\n",
-                        "Loss on hold-out set: 2.3900096663888895\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.20754716981132076\n",
-                        "Epoch: 83\n",
-                        "Loss on hold-out set: 2.3891540023515807\n",
-                        "Accuracy on hold-out set: 0.14150943396226415\n",
-                        "Metric value on hold-out data: 0.2091194968553459\n",
-                        "Epoch: 84\n",
-                        "Loss on hold-out set: 2.387304389251853\n",
-                        "Accuracy on hold-out set: 0.14150943396226415\n",
-                        "Metric value on hold-out data: 0.19968553459119495\n",
-                        "Epoch: 85\n",
-                        "Loss on hold-out set: 2.389448141152004\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.20518867924528303\n",
-                        "Epoch: 86\n",
-                        "Loss on hold-out set: 2.387848620144826\n",
-                        "Accuracy on hold-out set: 0.1509433962264151\n",
-                        "Metric value on hold-out data: 0.21147798742138366\n",
-                        "Epoch: 87\n",
-                        "Loss on hold-out set: 2.386700990065089\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.21540880503144652\n",
-                        "Early stopping at epoch 86\n",
-                        "Returned to Spot: Validation loss: 2.386700990065089\n",
-                        "----------------------------------------------\n",
-                        "\n",
-                        "config: {'l1': 2048, 'dropout_prob': 0.09938113979846144, 'lr_mult': 0.001, 'batch_size': 16, 'epochs': 16, 'k_folds': 1, 'patience': 20, 'optimizer': 'Adam', 'sgd_momentum': 0.9}\n",
-                        "Epoch: 1\n",
-                        "Loss on hold-out set: 2.3977260249001637\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.17374213836477986\n",
-                        "Epoch: 2\n",
-                        "Loss on hold-out set: 2.397668753351484\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.16666666666666666\n",
-                        "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3976011276245117\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.18238993710691823\n",
-                        "Epoch: 4\n",
-                        "Loss on hold-out set: 2.397585017340524\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.20125786163522014\n",
-                        "Epoch: 5\n",
-                        "Loss on hold-out set: 2.397540671484811\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.19103773584905662\n",
-                        "Epoch: 6\n",
-                        "Loss on hold-out set: 2.397476179259164\n",
-                        "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.19496855345911948\n",
-                        "Epoch: 7\n",
-                        "Loss on hold-out set: 2.3973847116742815\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.19339622641509435\n",
-                        "Epoch: 8\n",
-                        "Loss on hold-out set: 2.397370065961565\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.2020440251572327\n",
-                        "Epoch: 9\n",
-                        "Loss on hold-out set: 2.3973048414502824\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Loss on hold-out set: 2.3923851566494636\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
                         "Metric value on hold-out data: 0.2020440251572327\n",
-                        "Epoch: 10\n",
-                        "Loss on hold-out set: 2.397292443684169\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Epoch: 62\n",
+                        "Loss on hold-out set: 2.39214533454967\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
                         "Metric value on hold-out data: 0.19732704402515722\n",
-                        "Epoch: 11\n",
-                        "Loss on hold-out set: 2.3972138336726596\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.190251572327044\n",
-                        "Epoch: 12\n",
-                        "Loss on hold-out set: 2.397153990609305\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.2091194968553459\n",
-                        "Epoch: 13\n",
-                        "Loss on hold-out set: 2.397108316421509\n",
-                        "Accuracy on hold-out set: 0.14150943396226415\n",
-                        "Metric value on hold-out data: 0.21855345911949683\n",
-                        "Epoch: 14\n",
-                        "Loss on hold-out set: 2.3970647028514316\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.22091194968553457\n",
-                        "Epoch: 15\n",
-                        "Loss on hold-out set: 2.39692177091326\n",
-                        "Accuracy on hold-out set: 0.1509433962264151\n",
-                        "Metric value on hold-out data: 0.2389937106918239\n",
-                        "Epoch: 16\n",
-                        "Loss on hold-out set: 2.3969111101967946\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.2303459119496855\n",
-                        "Returned to Spot: Validation loss: 2.3969111101967946\n",
+                        "Early stopping at epoch 61\n",
+                        "Returned to Spot: Validation loss: 2.39214533454967\n",
                         "----------------------------------------------\n",
-                        "spotPython tuning: [##--------] 15.42% \n",
-                        "config: {'l1': 2048, 'dropout_prob': 0.3872037912868407, 'lr_mult': 0.001, 'batch_size': 4, 'epochs': 64, 'k_folds': 1, 'patience': 16, 'optimizer': 'Adam', 'sgd_momentum': 0.9}\n",
+                        "\n",
+                        "config: {'l1': 4096, 'dropout_prob': 0.877584251284408, 'lr_mult': 0.001, 'batch_size': 2, 'epochs': 16, 'k_folds': 1, 'patience': 16, 'optimizer': 'Adam', 'sgd_momentum': 0.9}\n",
                         "Epoch: 1\n",
-                        "Loss on hold-out set: 2.3975199528460234\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.1761006289308176\n",
+                        "Loss on hold-out set: 2.39812204972753\n",
+                        "Accuracy on hold-out set: 0.06132075471698113\n",
+                        "Metric value on hold-out data: 0.11949685534591192\n",
                         "Epoch: 2\n",
-                        "Loss on hold-out set: 2.397514028369256\n",
+                        "Loss on hold-out set: 2.3979568953784005\n",
                         "Accuracy on hold-out set: 0.07547169811320754\n",
-                        "Metric value on hold-out data: 0.17610062893081763\n",
+                        "Metric value on hold-out data: 0.13364779874213836\n",
                         "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3974955351847522\n",
-                        "Accuracy on hold-out set: 0.10377358490566038\n",
-                        "Metric value on hold-out data: 0.18867924528301888\n",
+                        "Loss on hold-out set: 2.3975181399651295\n",
+                        "Accuracy on hold-out set: 0.07075471698113207\n",
+                        "Metric value on hold-out data: 0.1509433962264151\n",
                         "Epoch: 4\n",
-                        "Loss on hold-out set: 2.397429974573963\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.19261006289308177\n",
+                        "Loss on hold-out set: 2.3979145288467407\n",
+                        "Accuracy on hold-out set: 0.08018867924528301\n",
+                        "Metric value on hold-out data: 0.13443396226415094\n",
                         "Epoch: 5\n",
-                        "Loss on hold-out set: 2.397345192027542\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.19496855345911948\n",
+                        "Loss on hold-out set: 2.3979776220501594\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.1501572327044025\n",
                         "Epoch: 6\n",
-                        "Loss on hold-out set: 2.397298075118155\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.19654088050314464\n",
+                        "Loss on hold-out set: 2.397381015543668\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.15015723270440248\n",
                         "Epoch: 7\n",
-                        "Loss on hold-out set: 2.3971176237430214\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.21855345911949683\n",
+                        "Loss on hold-out set: 2.3975596877763854\n",
+                        "Accuracy on hold-out set: 0.07547169811320754\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 8\n",
-                        "Loss on hold-out set: 2.397198501622902\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.21933962264150944\n",
+                        "Loss on hold-out set: 2.3975577241969557\n",
+                        "Accuracy on hold-out set: 0.09433962264150944\n",
+                        "Metric value on hold-out data: 0.1580188679245283\n",
                         "Epoch: 9\n",
-                        "Loss on hold-out set: 2.397252132307808\n",
-                        "Accuracy on hold-out set: 0.08018867924528301\n",
-                        "Metric value on hold-out data: 0.19732704402515722\n",
+                        "Loss on hold-out set: 2.3973420048659704\n",
+                        "Accuracy on hold-out set: 0.10377358490566038\n",
+                        "Metric value on hold-out data: 0.16273584905660377\n",
                         "Epoch: 10\n",
-                        "Loss on hold-out set: 2.3969808929371386\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.20676100628930816\n",
+                        "Loss on hold-out set: 2.3973369913281135\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17531446540880502\n",
                         "Epoch: 11\n",
-                        "Loss on hold-out set: 2.397060956595079\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.21619496855345913\n",
+                        "Loss on hold-out set: 2.397305949678961\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.16981132075471697\n",
                         "Epoch: 12\n",
-                        "Loss on hold-out set: 2.396922358926737\n",
-                        "Accuracy on hold-out set: 0.13679245283018868\n",
-                        "Metric value on hold-out data: 0.2272012578616352\n",
+                        "Loss on hold-out set: 2.3970576929596237\n",
+                        "Accuracy on hold-out set: 0.08962264150943396\n",
+                        "Metric value on hold-out data: 0.15566037735849056\n",
                         "Epoch: 13\n",
-                        "Loss on hold-out set: 2.396929277563995\n",
-                        "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.21147798742138363\n",
+                        "Loss on hold-out set: 2.396699365579857\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.18160377358490565\n",
                         "Epoch: 14\n",
-                        "Loss on hold-out set: 2.3966498554877513\n",
-                        "Accuracy on hold-out set: 0.1179245283018868\n",
-                        "Metric value on hold-out data: 0.2161949685534591\n",
+                        "Loss on hold-out set: 2.3968509818023107\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.17767295597484273\n",
                         "Epoch: 15\n",
-                        "Loss on hold-out set: 2.3966342593139074\n",
-                        "Accuracy on hold-out set: 0.10377358490566038\n",
-                        "Metric value on hold-out data: 0.20518867924528303\n",
+                        "Loss on hold-out set: 2.3967030385755144\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.1988993710691824\n",
                         "Epoch: 16\n",
-                        "Loss on hold-out set: 2.3964818693556875\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.22248427672955978\n",
-                        "Epoch: 17\n",
-                        "Loss on hold-out set: 2.3964703173007607\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.22405660377358488\n",
-                        "Epoch: 18\n",
-                        "Loss on hold-out set: 2.3962703785806334\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.2272012578616352\n",
-                        "Epoch: 19\n",
-                        "Loss on hold-out set: 2.3961621860288225\n",
+                        "Loss on hold-out set: 2.396169626487876\n",
                         "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.2272012578616352\n",
-                        "Epoch: 20\n",
-                        "Loss on hold-out set: 2.396049198114647\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.22641509433962265\n",
-                        "Epoch: 21\n",
-                        "Loss on hold-out set: 2.3960129539921597\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.23663522012578614\n",
-                        "Epoch: 22\n",
-                        "Loss on hold-out set: 2.3957479674861117\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.23349056603773585\n",
-                        "Epoch: 23\n",
-                        "Loss on hold-out set: 2.39578865609079\n",
-                        "Accuracy on hold-out set: 0.14150943396226415\n",
-                        "Metric value on hold-out data: 0.24449685534591195\n",
-                        "Epoch: 24\n",
-                        "Loss on hold-out set: 2.395629932295601\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.22877358490566038\n",
-                        "Epoch: 25\n",
-                        "Loss on hold-out set: 2.3954727784642635\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.2366352201257862\n",
-                        "Epoch: 26\n",
-                        "Loss on hold-out set: 2.395096445983311\n",
-                        "Accuracy on hold-out set: 0.17452830188679244\n",
-                        "Metric value on hold-out data: 0.27122641509433965\n",
-                        "Epoch: 27\n",
-                        "Loss on hold-out set: 2.3951486371598154\n",
-                        "Accuracy on hold-out set: 0.1509433962264151\n",
-                        "Metric value on hold-out data: 0.25393081761006286\n",
-                        "Epoch: 28\n",
-                        "Loss on hold-out set: 2.394606608264851\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.26493710691823896\n",
-                        "Epoch: 29\n",
-                        "Loss on hold-out set: 2.3944551000055276\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.25393081761006286\n",
-                        "Epoch: 30\n",
-                        "Loss on hold-out set: 2.3942494527348934\n",
-                        "Accuracy on hold-out set: 0.1509433962264151\n",
-                        "Metric value on hold-out data: 0.25078616352201255\n",
-                        "Epoch: 31\n",
-                        "Loss on hold-out set: 2.3939217936317876\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.25393081761006286\n",
-                        "Epoch: 32\n",
-                        "Loss on hold-out set: 2.3938396336897365\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.2610062893081761\n",
-                        "Epoch: 33\n",
-                        "Loss on hold-out set: 2.3935969325731383\n",
-                        "Accuracy on hold-out set: 0.16037735849056603\n",
-                        "Metric value on hold-out data: 0.25471698113207547\n",
-                        "Epoch: 34\n",
-                        "Loss on hold-out set: 2.393201378156554\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.2562893081761006\n",
-                        "Epoch: 35\n",
-                        "Loss on hold-out set: 2.3931515036888844\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.25864779874213834\n",
-                        "Epoch: 36\n",
-                        "Loss on hold-out set: 2.3926245266536497\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.26572327044025157\n",
-                        "Epoch: 37\n",
-                        "Loss on hold-out set: 2.3925997221244955\n",
-                        "Accuracy on hold-out set: 0.17452830188679244\n",
-                        "Metric value on hold-out data: 0.25707547169811323\n",
-                        "Epoch: 38\n",
-                        "Loss on hold-out set: 2.3923681861949415\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.2492138364779874\n",
-                        "Epoch: 39\n",
-                        "Loss on hold-out set: 2.391703925042782\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.2680817610062893\n",
-                        "Epoch: 40\n",
-                        "Loss on hold-out set: 2.3911529397064784\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.2743710691823899\n",
-                        "Epoch: 41\n",
-                        "Loss on hold-out set: 2.3910829346134976\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.25078616352201255\n",
-                        "Epoch: 42\n",
-                        "Loss on hold-out set: 2.3909124428371213\n",
-                        "Accuracy on hold-out set: 0.15566037735849056\n",
-                        "Metric value on hold-out data: 0.2484276729559748\n",
-                        "Epoch: 43\n",
-                        "Loss on hold-out set: 2.390134330065745\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.255503144654088\n",
-                        "Epoch: 44\n",
-                        "Loss on hold-out set: 2.3897271696126685\n",
-                        "Accuracy on hold-out set: 0.17452830188679244\n",
-                        "Metric value on hold-out data: 0.25786163522012573\n",
-                        "Epoch: 45\n",
-                        "Loss on hold-out set: 2.38967553624567\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.2460691823899371\n",
-                        "Epoch: 46\n",
-                        "Loss on hold-out set: 2.3891041143885197\n",
-                        "Accuracy on hold-out set: 0.2028301886792453\n",
-                        "Metric value on hold-out data: 0.25707547169811323\n",
-                        "Epoch: 47\n",
-                        "Loss on hold-out set: 2.3887231934745357\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.2562893081761006\n",
-                        "Epoch: 48\n",
-                        "Loss on hold-out set: 2.387767827735757\n",
-                        "Accuracy on hold-out set: 0.2028301886792453\n",
-                        "Metric value on hold-out data: 0.2672955974842767\n",
-                        "Epoch: 49\n",
-                        "Loss on hold-out set: 2.387149207996872\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.25393081761006286\n",
-                        "Epoch: 50\n",
-                        "Loss on hold-out set: 2.386414275979096\n",
-                        "Accuracy on hold-out set: 0.19811320754716982\n",
-                        "Metric value on hold-out data: 0.25864779874213834\n",
-                        "Epoch: 51\n",
-                        "Loss on hold-out set: 2.3859116986112774\n",
-                        "Accuracy on hold-out set: 0.23113207547169812\n",
-                        "Metric value on hold-out data: 0.28380503144654085\n",
-                        "Epoch: 52\n",
-                        "Loss on hold-out set: 2.3858340821176207\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.24449685534591192\n",
-                        "Epoch: 53\n",
-                        "Loss on hold-out set: 2.384917398668685\n",
-                        "Accuracy on hold-out set: 0.19811320754716982\n",
-                        "Metric value on hold-out data: 0.25943396226415094\n",
-                        "Epoch: 54\n",
-                        "Loss on hold-out set: 2.383883980085265\n",
-                        "Accuracy on hold-out set: 0.20754716981132076\n",
-                        "Metric value on hold-out data: 0.2562893081761006\n",
-                        "Epoch: 55\n",
-                        "Loss on hold-out set: 2.384816628582073\n",
-                        "Accuracy on hold-out set: 0.20754716981132076\n",
-                        "Metric value on hold-out data: 0.2610062893081761\n",
-                        "Epoch: 56\n",
-                        "Loss on hold-out set: 2.3837408839531666\n",
-                        "Accuracy on hold-out set: 0.2028301886792453\n",
-                        "Metric value on hold-out data: 0.25235849056603776\n",
-                        "Epoch: 57\n",
-                        "Loss on hold-out set: 2.382753421675484\n",
-                        "Accuracy on hold-out set: 0.21226415094339623\n",
-                        "Metric value on hold-out data: 0.26257861635220126\n",
-                        "Epoch: 58\n",
-                        "Loss on hold-out set: 2.3819254614272207\n",
-                        "Accuracy on hold-out set: 0.25\n",
-                        "Metric value on hold-out data: 0.27908805031446543\n",
-                        "Epoch: 59\n",
-                        "Loss on hold-out set: 2.381116214788185\n",
-                        "Accuracy on hold-out set: 0.2169811320754717\n",
-                        "Metric value on hold-out data: 0.255503144654088\n",
-                        "Epoch: 60\n",
-                        "Loss on hold-out set: 2.3806882399433063\n",
-                        "Accuracy on hold-out set: 0.2358490566037736\n",
-                        "Metric value on hold-out data: 0.26572327044025157\n",
-                        "Epoch: 61\n",
-                        "Loss on hold-out set: 2.3807215105812505\n",
-                        "Accuracy on hold-out set: 0.2169811320754717\n",
-                        "Metric value on hold-out data: 0.25864779874213834\n",
-                        "Epoch: 62\n",
-                        "Loss on hold-out set: 2.377534025120285\n",
-                        "Accuracy on hold-out set: 0.2358490566037736\n",
-                        "Metric value on hold-out data: 0.2680817610062893\n",
-                        "Epoch: 63\n",
-                        "Loss on hold-out set: 2.3783269288404933\n",
-                        "Accuracy on hold-out set: 0.25\n",
-                        "Metric value on hold-out data: 0.27358490566037735\n",
-                        "Epoch: 64\n",
-                        "Loss on hold-out set: 2.378141115296562\n",
-                        "Accuracy on hold-out set: 0.2358490566037736\n",
-                        "Metric value on hold-out data: 0.2665094339622642\n",
-                        "Returned to Spot: Validation loss: 2.378141115296562\n",
+                        "Metric value on hold-out data: 0.1988993710691824\n",
+                        "Returned to Spot: Validation loss: 2.396169626487876\n",
                         "----------------------------------------------\n",
                         "spotPython tuning: [##########] 100.00% Done...\n",
                         "\r"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "<spotPython.spot.spot.Spot at 0x2a97a7220>"
+                            "<spotPython.spot.spot.Spot at 0x16e1cae90>"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1974,15 +1594,15 @@
                 "# add the nn model to the fun_control dictionary\n",
                 "fun_control = add_core_model_to_fun_control(core_model=Net_vbdp,\n",
                 "                              fun_control=fun_control,\n",
                 "                              hyper_dict=TorchHyperDict)\n",
                 "# modify the hyperparameter levels\n",
                 "fun_control = modify_hyper_parameter_bounds(fun_control, \"lr_mult\", bounds=[1e-3, 1e-3])\n",
                 "fun_control = modify_hyper_parameter_bounds(fun_control, \"sgd_momentum\", bounds=[0.9, 0.9])\n",
-                "fun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\",[\"Adam\", \"SGD\"])\n",
+                "fun_control = modify_hyper_parameter_levels(fun_control, \"optimizer\",[\"Adadelta\", \"Adagrad\", \"Adam\", \"AdamW\", \"Adamax\", \"ASGD\", \"NAdam\"])\n",
                 "# select metric and loss function\n",
                 "# metric_torch = torchmetrics.Accuracy(task=\"multiclass\", num_classes=11)\n",
                 "metric_torch = MAPK(k=3)\n",
                 "loss_torch = CrossEntropyLoss()\n",
                 "# loss_torch = NLLLoss()\n",
                 "fun_control.update({\n",
                 "               \"metric_torch\": metric_torch,\n",
@@ -2039,15 +1659,15 @@
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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XygzM1P33nuvamtrVVBQoMWLF2vnzp1Xuacjj6dj16OhoUGtra3uIyIi4ir1cOSqrq5Wbm6u9u/fr4qKCp0/f14ZGRnq6Ojot85f/vIXPfLII1q0aJFqampks9lks9lUX18/hD0fft6MnSSFhob2mndffvnlEPV45IiJidGLL76oQ4cO6eDBg/rpT3+q+fPn67PPPuuzPHPue56OncSc68uBAwf0xhtvaMqUKQOWY+71bbDjJzH/ekyaNKnXOOzdu7ffsiN63hm44iQZZWVlA5b51a9+ZUyaNKnXawsXLjTuv//+q9izkW8wY/fhhx8akozTp08PSZ+uJV9//bUhyaiuru63zMMPP2xkZmb2em369OnGk08+ebW7N6INZuzWr19vhIWFDV2nriE/+tGPjDfffLPP95hzAxto7JhzFztz5oxxyy23GBUVFcY999xj5Ofn91uWuXcxT8aP+ddtxYoVxp133jno8iN53nHHf5js27dP6enpvV67//77tW/fvmHq0bUnOTlZUVFRmjNnjj766KPh7s6I4HA4JEnh4eH9lmHu9W0wYydJZ8+e1YQJExQbG3vJO7Vm0NXVpU2bNqmjo0N33313n2WYc30bzNhJzLkL5ebmKjMz86I51Rfm3sU8GT+J+dejsbFR0dHRuvnmm/XYY4/pxIkT/ZYdyfPuuuHugFmdPHlSN954Y6/XbrzxRrW3t+vbb79VUFDQMPVs5IuKitLvf/97paamyul06s0331RaWpo+/vhjpaSkDHf3ho3L5VJBQYFmzpypyZMn91uuv7lnxmckegx27BITE/X2229rypQpcjgcevnllzVjxgx99tlniomJGcIeD7+6ujrdfffd+u677xQSEqKysjLdfvvtfZZlzvXmydgx53rbtGmTPvnkEx04cGBQ5Zl7vXk6fsy/btOnT9c777yjxMREtba26vnnn9esWbNUX18vi8VyUfmRPO8I/rjmJCYmKjEx0f33jBkzdPz4ca1evVolJSXD2LPhlZubq/r6+gHXHaJvgx27u+++u9ed2RkzZui2227TG2+8oeLi4qvdzRElMTFRtbW1cjgc2rJli5544glVV1f3G2DxPU/Gjjn3vebmZuXn56uiosKUD5heLm/Gj/nXbd68ee7/nzJliqZPn64JEybo3Xff1aJFi4axZ54j+A+TyMhItbW19Xqtra1NoaGh3O33wo9//GNTB968vDxt27ZNu3fvvuRdmP7mXmRk5NXs4ojlydhdaMyYMbrrrrt07Nixq9S7kcvf318JCQmSpKlTp+rAgQN69dVX9cYbb1xUljnXmydjdyEzz7lDhw7p66+/7vXNbldXl3bv3q3f/e53cjqd8vPz61WHufc9b8bvQmaefz80btw43Xrrrf2Ow0ied6zxHyZ33323Kisre71WUVEx4DpP9K+2tlZRUVHD3Y0hZxiG8vLyVFZWpl27dmnixImXrMPc6+bN2F2oq6tLdXV1ppx7F3K5XHI6nX2+x5wb2EBjdyEzz7n77rtPdXV1qq2tdR+pqal67LHHVFtb22doZe59z5vxu5CZ598PnT17VsePH+93HEb0vBvup4tHizNnzhg1NTVGTU2NIcl45ZVXjJqaGuPLL780DMMwli5dajz++OPu8k1NTUZwcLDx3HPPGUeOHDFee+01w8/Pz3j//feH6xKGjadjt3r1amPr1q1GY2OjUVdXZ+Tn5xu+vr7Gn//85+G6hGHz1FNPGWFhYUZVVZXR2trqPs6dO+cu8/jjjxtLly51//3RRx8Z1113nfHyyy8bR44cMVasWGGMGTPGqKurG45LGDbejN3zzz9v7Ny50zh+/Lhx6NAh4+c//7kRGBhofPbZZ8NxCcNm6dKlRnV1tfHFF18Yhw8fNpYuXWr4+PgYH3zwgWEYzLmBeDp2zLmBXbgrDXPPM5caP+Zft2effdaoqqoyvvjiC+Ojjz4y0tPTjRtuuMH4+uuvDcO4tuYdwf8K6dli8sLjiSeeMAzDMJ544gnjnnvuuahOcnKy4e/vb9x8883G+vXrh7zfI4GnY7dq1SojPj7eCAwMNMLDw420tDRj165dw9P5YdbXuEnqNZfuuece91j2ePfdd41bb73V8Pf3NyZNmmT86U9/GtqOjwDejF1BQYERFxdn+Pv7GzfeeKPxwAMPGJ988snQd36Y/eM//qMxYcIEw9/f37BarcZ9993nDq6GwZwbiKdjx5wb2IXBlbnnmUuNH/Ov28KFC42oqCjD39/fGD9+vLFw4ULj2LFj7vevpXnnYxiGMXTfLwAAAAAYDqzxBwAAAEyA4A8AAACYAMEfAAAAMAGCPwAAAGACBH8AAADABAj+AAAAgAkQ/AEAAAATIPgDAAAAJkDwBwAAAEyA4A8AAACYAMEfAAAAMIH/BxlrWYjR6QtYAAAAAElFTkSuQmCC",
                         "text/plain": [
                             "<Figure size 900x600 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -2063,25 +1683,25 @@
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "| name         | type   | default   |   lower |   upper |               tuned | transform             |   importance | stars   |\n",
-                        "|--------------|--------|-----------|---------|---------|---------------------|-----------------------|--------------|---------|\n",
-                        "| l1           | int    | 8         |     8.0 |    11.0 |                11.0 | transform_power_2_int |         0.00 |         |\n",
-                        "| dropout_prob | float  | 0.01      |     0.0 |     0.5 | 0.39461789811977777 | None                  |        69.79 | **      |\n",
-                        "| lr_mult      | float  | 1.0       |   0.001 |   0.001 |               0.001 | None                  |         0.00 |         |\n",
-                        "| batch_size   | int    | 4         |     1.0 |     4.0 |                 2.0 | transform_power_2_int |         0.00 |         |\n",
-                        "| epochs       | int    | 4         |     4.0 |     9.0 |                 6.0 | transform_power_2_int |         0.00 |         |\n",
-                        "| k_folds      | int    | 1         |     1.0 |     1.0 |                 1.0 | None                  |         0.00 |         |\n",
-                        "| patience     | int    | 5         |     2.0 |    20.0 |                19.0 | None                  |        20.08 | *       |\n",
-                        "| optimizer    | factor | SGD       |     0.0 |     1.0 |                 0.0 | None                  |       100.00 | ***     |\n",
-                        "| sgd_momentum | float  | 0.0       |     0.9 |     0.9 |                 0.9 | None                  |         0.00 |         |\n"
+                        "| name         | type   | default   |   lower |   upper |              tuned | transform             |   importance | stars   |\n",
+                        "|--------------|--------|-----------|---------|---------|--------------------|-----------------------|--------------|---------|\n",
+                        "| l1           | int    | 8         |     8.0 |    13.0 |               12.0 | transform_power_2_int |        19.95 | *       |\n",
+                        "| dropout_prob | float  | 0.01      |     0.0 |     0.9 | 0.8973189149831583 | None                  |         0.00 |         |\n",
+                        "| lr_mult      | float  | 1.0       |   0.001 |   0.001 |              0.001 | None                  |         0.00 |         |\n",
+                        "| batch_size   | int    | 4         |     1.0 |     4.0 |                1.0 | transform_power_2_int |         0.00 |         |\n",
+                        "| epochs       | int    | 4         |     4.0 |     9.0 |                7.0 | transform_power_2_int |         6.37 | *       |\n",
+                        "| k_folds      | int    | 1         |     1.0 |     1.0 |                1.0 | None                  |         0.00 |         |\n",
+                        "| patience     | int    | 2         |     1.0 |     5.0 |                3.0 | transform_power_2_int |         0.00 |         |\n",
+                        "| optimizer    | factor | SGD       |     0.0 |     6.0 |                2.0 | None                  |       100.00 | ***     |\n",
+                        "| sgd_momentum | float  | 0.0       |     0.9 |     0.9 |                0.9 | None                  |         0.00 |         |\n"
                     ]
                 }
             ],
             "source": [
                 "#| echo: true\n",
                 "#| eval: false\n",
                 "from spotPython.utils.eda import gen_design_table\n",
@@ -2091,15 +1711,15 @@
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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FxenjIwMZ1l5ebluvPFGNW/eXG63Wz169NCaNWvq4KsGf6iurtZtt92mFi1aKDw8XBdeeKEKCgok/f5zzdKlSzVkyBBVVFQ4z18TJ06UdOhLPC6XS08//bSuuOIKNWzYUCkpKcrLy9P333+v7t27KzIyUhdccIE2bNjg3Obgl3hq7+PAS2JiorP866+/1qWXXqqoqCh5PB7dcMMN2rp1q7O89vssMzNTzZo1U3p6uv+/oPUMgVLHxowZo2XLluntt9/Whx9+qKVLl2r16tU+6zzyyCM699xz9fnnn2vcuHEqLCzU1Vdfrf79++urr77SxIkTNW7cOM2dO9fndg8//LBzu7Fjx2rUqFFasmSJpP0fHdC7d29t27ZNy5Yt05IlS/TDDz/ommuuOeq5z5gxQ6mpqRo2bJi2bNmiLVu2HPUnSI8ZM0aPPvqoCgoK1Lx5c/Xq1Ut79+51lu/atUtTp07Vc889p2+++UYtWrTQ4MGDtWrVKi1atEh5eXkyxuiyyy475HYPPPCAXnzxRS1fvlzl5eXq37//UT8m/DHz5s1TcHCwVq5cqRkzZuixxx7Tc889J0nau3evpkyZojVr1mjhwoXatGmTEyEJCQl68803JUlFRUXasmWLZsyYcdj7yMjIUF5enl599VV9+eWX6tevny655BKfSN21a5ceeeQRvfTSS/rkk09UXFysO++801n+1FNPacSIERo+fLi++uorLVq0SKeddpqzvF+/fiorK9P777+vwsJCtW/fXj179tS2bdv8/SWDH9x111168803NW/ePK1evVqnnXaa0tPTff6/fuu55oILLtD06dPldrud568D95WD1f6i+MUXXyg5OVnXXXedbrrpJmVlZWnVqlUyxvjE7sFq72PLli36/vvvddppp+lvf/ubpP1h3KNHD7Vr106rVq3S4sWLVVpaqquvvtpnG/PmzVNoaKiWL1+u2bNnH+dX7wRgUGd27NhhQkNDzeuvv+6M/fLLLyYiIsKMGjXKGGNMq1atTJ8+fXxud91115m///3vPmNjxowxbdu2da63atXKXHLJJT7rXHPNNebSSy81xhjz4YcfmgYNGpji4mJn+TfffGMkmZUrVxpjjBk0aJDp3bu3zzZGjRplunXr5lzv1q2bM9ej8fHHHxtJ5tVXXz3kMb/22mvGGGPmzJljJJkvvvjCWWfdunVGklm+fLkztnXrVhMREeF8/Wpvt2LFCmedtWvXGkkmPz//qOeIY9OtWzeTkpJiampqnLG7777bpKSkHHb9goICI8ns2LHDGPP/+8T27dsP2W7tvvXjjz+aBg0amJ9++slnnZ49e5qsrCxjzP///3///ffO8pycHOPxeJzr8fHx5t577z3svP7zn/8Yt9ttdu/e7TPeunVr8/TTTx/hK4BAqKqqMiEhIWb+/PnO2J49e0x8fLyZNm3aUT/XxMTEHLLtVq1amccff9y5Lsncd999zvW8vDwjyTz//PPO2CuvvGLCw8Od6xMmTDDnnnvuIduuqakxV155penQoYPZtWuXMcaYKVOmmIsvvthnvZKSEiPJFBUVGWP2fz+0a9fuKL4yJw+OoNShDRs2aM+ePercubMz1qRJE51xxhk+63Xs2NHn+tq1a9W1a1efsa5du2r9+vXat2+fM3bwByumpqZq7dq1zjYSEhJ8jni0bdtWjRo1ctapSwfOrfYxH3i/oaGhOuecc5zra9euVXBwsM/XqmnTpofcLjg4WOeff75zPTk5+U97TCezLl26yOVyOddTU1Od/bGwsFC9evVSy5YtFR0drW7dukna/xLj0frqq6+0b98+nX766c5r+1FRUVq2bJnPYfWGDRuqdevWzvW4uDjn5aSysjJt3rxZPXv2POx9rFmzRlVVVWratKnPfWzcuNHnPmCHDRs2aO/evT7PhSEhIerUqZPP9/vvPdccrQOfj2o/cuXss8/2Gdu9e7cqKyuPuJ177rlHeXl5evvttxURESFp/7738ccf++x3ycnJzuOs1aFDh2Oe94mMk2QtEBkZGZD7DQoKcs4jqHXgyyl1KSIiwucHHuqn3bt3Kz09Xenp6Zo/f76aN2+u4uJipaena8+ePUe9naqqKjVo0ECFhYVq0KCBz7IDT0QMCQnxWeZyuZx9uPaHwZHuIy4uzue8llq8fR0H7lu1z02HG6upqfnNbfzrX//S448/rqVLl+qUU05xxquqqtSrVy9NnTr1kNvExcU5/w7UzwJbcQSlDrVu3VohISHKz893xrZv365169Yd8XYpKSlavny5z9jy5ct1+umn+zx5r1ixwmedFStWKCUlxdlGSUmJzwmk3377rcrLy9W2bVtJ+89kP/gEwy+++MLnemhoqM9Rm6N14NxqH3Pt3A4nJSVFv/76q8/X6pdfflFRUZEzX0n69ddftWrVKud6UVGRysvLj7htHL8D/1+k/f+/bdq00XfffadffvlFDz30kP76178qOTnZOaJRq/adCEfaj9q1a6d9+/aprKxMp512ms8lNjb2qOYYHR2txMTE33zrZ/v27eX1ehUcHHzIfTRr1uyo7gN/ntatWzvnY9Tau3evCgoKfJ4TjvRc80efv/6IvLw83XjjjXr66afVpUsXn2Xt27fXN998o8TExEP2PaLktxEodSgqKkpDhw7VmDFj9NFHH+nrr7/W4MGDf/fttHfccYdyc3M1ZcoUrVu3TvPmzdMTTzxxyAley5cv17Rp07Ru3Trl5OTojTfe0KhRoyRJaWlpOvvsszVgwACtXr1aK1eu1MCBA9WtWzfnJaUePXpo1apVevHFF7V+/XpNmDDB59020v6z3fPz87Vp0yZt3br1iL89HGjy5MnKzc11HnOzZs0OecfQgdq0aaPevXtr2LBh+vTTT7VmzRpdf/31OuWUU9S7d29nvZCQEI0cOVL5+fkqLCzU4MGD1aVLF3Xq1Omo5oU/pri4WKNHj1ZRUZFeeeUVzZo1S6NGjVLLli0VGhqqWbNm6YcfftCiRYsO+dsmrVq1ksvl0rvvvquff/5ZVVVVh2z/9NNP14ABAzRw4EC99dZb2rhxo1auXKns7Gy99957Rz3PiRMn6tFHH9XMmTO1fv16rV69WrNmzZK0/3siNTVVffr00YcffqhNmzbps88+07333usTvbBDZGSkbrnlFo0ZM0aLFy/Wt99+q2HDhmnXrl0aOnSos96RnmsSExNVVVWl3Nxcbd26Vbt27aqTuXq9Xl155ZXq37+/0tPT5fV65fV69fPPP0uSRowYoW3btunaa69VQUGBNmzYoA8++EBDhgz50wKqXgr0STAnuh07dpjrr7/eNGzY0Hg8HjNt2jSfkwMPPlmr1r///W/Ttm1bExISYlq2bGkefvhhn+WtWrUykyZNMv369TMNGzY0sbGxZsaMGT7r/Pjjj+Yf//iHiYyMNNHR0aZfv37G6/X6rDN+/Hjj8XhMTEyMuf32201GRobPSbJFRUWmS5cuJiIiwkgyGzduPOLjrT1x7Z133jFnnnmmCQ0NNZ06dTJr1qxx1vmtE9e2bdtmbrjhBhMTE2MiIiJMenq6Wbdu3SG3e/PNN81f/vIXExYWZtLS0syPP/54xDnh+HTr1s3ceuut5uabbzZut9s0btzY3HPPPc5Jsy+//LJJTEw0YWFhJjU11SxatMhIMp9//rmzjcmTJ5vY2FjjcrnMoEGDnO0eeAL2nj17zPjx401iYqIJCQkxcXFx5sorrzRffvmlMebw+82CBQvMwU9js2fPNmeccYazjZEjRzrLKisrzciRI018fLwJCQkxCQkJZsCAAT4nk8Me//vf/8zIkSNNs2bNTFhYmOnatatzkv/RPNcYY8zNN99smjZtaiSZCRMmGGMOf5LsggULnOsbN248ZB8++GTvA0+SrV128KVVq1bO7detW2euvPJK06hRIxMREWGSk5NNZmam8310rG9IOBm4jDnoJATUC4mJicrMzLTur7wuXbpUF110kbZv387r+ieI7t2767zzzjvuPw0O+BPPNSc+XuIBAADWIVBwTG6++Waft8odeLn55psDPT0AwAmCl3hwTMrKyn7z7wC43W61aNHiT54RAOBERKAAAADr8BIPAACwDoECAACsQ6AAAADrECgAAMA6BAoAALAOgQIAAKxDoAAAAOsQKAAAwDr/By8FPhhSOwZQAAAAAElFTkSuQmCC",
+                        "image/png": "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19KlS93n33LLLXrhhRdUUlKibdu2adGiRerYsWPQHA888IDmz5+vTZs2KSoqSrfddpu7bezYsTrzzDNVWVmpqqoqTZs2TdHR0S37g0HITJ06Va+88oqWLVumzZs3q2fPnsrJydG+ffvcfb7uHBsyZIiKi4uVkJCgzz77TJ999pkmT578tV9r9uzZuuWWW7Rlyxb17t1bN954o+68804VFhZq06ZNchxHEydO/NrnH/8an332mXbu3KmePXvqkksukSTV1dXp8ssvV//+/bVp0yaVlZWptrZW1113XdAxli1bppiYGK1bt06lpaWn+dNrAxz8oF166aXOvffeG7Ru165djiTn/fffD8tMsO/QoUNO+/btnffeey9o/fjx450bbrjBeeeddxxJzsqVK91t//3vf524uDjnxRdfdBzHcW688UbnyiuvDHr+lClTnMzMTMdxHKe6utqR5Lz11lvNznD8a/z1r391161evdqR5Bw8eNBxHMeJj493li5devrfML539fX1TnR0tLNixQp33eHDh53U1FRn3rx53+ocW7JkiZOYmHjCsXv06OEsWLDAfSzJefDBB93HFRUVjiRn8eLF7roXXnjBiY2NdR/PnDnT6dev3wnHbmpqckaPHu0MGDDAOXDggOM4jjN79mznqquuCtqvpqbGkeRUV1c7jnPs3+L+/ft/i5/MDwdXUACcsp07d+rAgQO68sor1bFjR3dZvnx50GXwL3/4Z1JSks455xxt27ZNkrRt2zYNHTo06LhDhw7Vjh07dPToUW3ZskWRkZG69NJLTzrL+eef7/65W7dukqS9e/dKOvaZX7fffruys7M1Z86coNlg28cff6wjR44EnSPR0dG6+OKL3XNIOvk5diq+fB4d/8iVvn37Bq07dOiQAoHASY/z61//WhUVFXrttdcUFxcn6dhLje+8807Q35XevXu73+dxAwYMOOW527KwfRYPgNarvr5ekrR69Wr96Ec/Ctrm8XhCEgLH/3H/Jl9+ySYiIkLSsftjpGP3Cdx4441avXq13nzzTc2cOVMrV67U6NGjT3s+tC3NnUcnO7ea8/vf/14LFizQmjVrgv5e1NfXa+TIkc2+AeF4VEtShw4dvvs30AZxBQXAKcvMzJTH49Hu3bvVs2fPoCUtLc3db/369e6f9+/fr+3bt6tPnz6SpD59+mjdunVBx123bp3OPvtsRUZGqm/fvmpqagq6p+W7OPvss1VQUKC//OUvuvbaa7VkyZLTOh6+H2eddZZ7P8ZxR44cUWVlpTIzM911JzvHYmJidPTo0e9l3oqKCt1+++1atGiRBg8eHLTtwgsv1EcffaT09PQT/r4QJV+PKyhw7du3T7t379aePXskyX03REpKilJSUsI5GoyJj4/X5MmTVVBQoKamJg0bNkx+v1/r1q1TQkKCevToIUl6+OGHlZycLK/XqwceeECdO3fWqFGjJEn33XefLrroIs2ePVvXX3+9Kioq9OSTT+qpp56SdOydFrfeeqtuu+02lZSUqF+/fvrXv/6lvXv3nnBzYXMOHjyoKVOm6Gc/+5kyMjL06aefqrKyUmPGjGmxnwtCp0OHDrrrrrs0ZcoUJSUlqXv37po3b54OHDig8ePHa+vWrZJOfo6lp6ervr5e5eXl6tevn9q3b3/aby9ujs/n0+jRo5Wbm6ucnBz5fD5JUmRkpLp06aK8vDw9++yzuuGGGzR16lQlJSVp586dWrlypX73u98pMjIy5DO1CeG+CQbh9eWbZJcsWeJIOmGZOXNmWGeETU1NTU5xcbFzzjnnONHR0U6XLl2cnJwcZ+3ate4NjK+//rpz7rnnOjExMc7FF1/sbN26NegYL7/8spOZmelER0c73bt3d37zm98EbT948KBTUFDgdOvWzYmJiXF69uzpPPfcc47j/P9Nsvv373f3f//99x1Jzq5du5zGxkYnNzfXSUtLc2JiYpzU1FRn4sSJ7g20sO/gwYPO3Xff7XTu3NnxeDzO0KFDnY0bNzqO43zrc+yXv/ylk5ycHPRvWXM3ya5atcp93NwbBb56vn35Jtnj27669OjRw33+9u3bndGjRzudOnVy4uLinN69ezv5+flOU1OT4zjNv2Hhhy7CcRzn+44iAG3bmjVrdNlll2n//v3N/iZP4HRxjrV93IMCAADMIVAAAIA5vMQDAADM4QoKAAAwh0ABAADmECgAAMAcAgUAAJhDoAAAAHMIFAAAYA6BAgAAzCFQAACAOQQKAAAw5/8Akh4yuvWimCwAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -2115,22 +1735,23 @@
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Net_vbdp(\n",
-                            "  (fc1): Linear(in_features=6112, out_features=2048, bias=True)\n",
-                            "  (fc2): Linear(in_features=2048, out_features=1024, bias=True)\n",
-                            "  (fc3): Linear(in_features=1024, out_features=512, bias=True)\n",
-                            "  (fc4): Linear(in_features=512, out_features=256, bias=True)\n",
-                            "  (fc5): Linear(in_features=256, out_features=11, bias=True)\n",
+                            "  (fc1): Linear(in_features=69, out_features=4096, bias=True)\n",
+                            "  (fc2): Linear(in_features=4096, out_features=2048, bias=True)\n",
+                            "  (fc3): Linear(in_features=2048, out_features=1024, bias=True)\n",
+                            "  (fc4): Linear(in_features=1024, out_features=512, bias=True)\n",
+                            "  (fc5): Linear(in_features=512, out_features=11, bias=True)\n",
                             "  (relu): ReLU()\n",
                             "  (softmax): Softmax(dim=1)\n",
-                            "  (dropout): Dropout(p=0.39461789811977777, inplace=False)\n",
+                            "  (dropout1): Dropout(p=0.8973189149831583, inplace=False)\n",
+                            "  (dropout2): Dropout(p=0.44865945749157915, inplace=False)\n",
                             ")"
                         ]
                     },
                     "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -2149,270 +1770,183 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Epoch: 1\n",
-                        "Loss on hold-out set: 2.3979998714518995\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.09040880503144653\n",
+                        "Loss on hold-out set: 2.3974600827918864\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
                         "Epoch: 2\n",
-                        "Loss on hold-out set: 2.3978512242155254\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.08569182389937106\n",
-                        "Epoch: 3\n",
-                        "Loss on hold-out set: 2.3977421274724997\n",
+                        "Loss on hold-out set: 2.3973923291800157\n",
                         "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.09905660377358491\n",
-                        "Epoch: 4\n",
-                        "Loss on hold-out set: 2.397848147266316\n",
+                        "Metric value on hold-out data: 0.19182389937106917\n",
+                        "Epoch: 3\n",
+                        "Loss on hold-out set: 2.3974333169325344\n",
                         "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.0959119496855346\n",
-                        "Epoch: 5\n",
-                        "Loss on hold-out set: 2.3976949925692574\n",
+                        "Metric value on hold-out data: 0.18867924528301888\n",
+                        "Epoch: 4\n",
+                        "Loss on hold-out set: 2.397642540481855\n",
                         "Accuracy on hold-out set: 0.12264150943396226\n",
-                        "Metric value on hold-out data: 0.09827044025157233\n",
+                        "Metric value on hold-out data: 0.1800314465408805\n",
+                        "Epoch: 5\n",
+                        "Loss on hold-out set: 2.397508963099066\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.17845911949685533\n",
                         "Epoch: 6\n",
-                        "Loss on hold-out set: 2.3977391359941014\n",
-                        "Accuracy on hold-out set: 0.14150943396226415\n",
-                        "Metric value on hold-out data: 0.09669811320754718\n",
+                        "Loss on hold-out set: 2.3971782292959825\n",
+                        "Accuracy on hold-out set: 0.11320754716981132\n",
+                        "Metric value on hold-out data: 0.18081761006289307\n",
                         "Epoch: 7\n",
-                        "Loss on hold-out set: 2.3976587844344803\n",
-                        "Accuracy on hold-out set: 0.13679245283018868\n",
-                        "Metric value on hold-out data: 0.10220125786163523\n",
+                        "Loss on hold-out set: 2.3975993372359365\n",
+                        "Accuracy on hold-out set: 0.09433962264150944\n",
+                        "Metric value on hold-out data: 0.1737421383647799\n",
                         "Epoch: 8\n",
-                        "Loss on hold-out set: 2.397642437017189\n",
-                        "Accuracy on hold-out set: 0.1509433962264151\n",
-                        "Metric value on hold-out data: 0.10927672955974842\n",
+                        "Loss on hold-out set: 2.396914779015307\n",
+                        "Accuracy on hold-out set: 0.12735849056603774\n",
+                        "Metric value on hold-out data: 0.19811320754716982\n",
                         "Epoch: 9\n",
-                        "Loss on hold-out set: 2.3976219195239947\n",
-                        "Accuracy on hold-out set: 0.17452830188679244\n",
-                        "Metric value on hold-out data: 0.12264150943396226\n",
+                        "Loss on hold-out set: 2.39737258767182\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17059748427672952\n",
                         "Epoch: 10\n",
-                        "Loss on hold-out set: 2.3976108847924\n",
-                        "Accuracy on hold-out set: 0.14622641509433962\n",
-                        "Metric value on hold-out data: 0.10849056603773585\n",
+                        "Loss on hold-out set: 2.3975391905262784\n",
+                        "Accuracy on hold-out set: 0.10377358490566038\n",
+                        "Metric value on hold-out data: 0.17531446540880505\n",
                         "Epoch: 11\n",
-                        "Loss on hold-out set: 2.3974821792458587\n",
-                        "Accuracy on hold-out set: 0.15566037735849056\n",
-                        "Metric value on hold-out data: 0.12971698113207547\n",
+                        "Loss on hold-out set: 2.397455721531274\n",
+                        "Accuracy on hold-out set: 0.1320754716981132\n",
+                        "Metric value on hold-out data: 0.18867924528301888\n",
                         "Epoch: 12\n",
-                        "Loss on hold-out set: 2.397318520635929\n",
-                        "Accuracy on hold-out set: 0.19339622641509435\n",
-                        "Metric value on hold-out data: 0.15172955974842767\n",
+                        "Loss on hold-out set: 2.397198796272278\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.18396226415094338\n",
                         "Epoch: 13\n",
-                        "Loss on hold-out set: 2.39740241698499\n",
-                        "Accuracy on hold-out set: 0.1792452830188679\n",
-                        "Metric value on hold-out data: 0.14465408805031446\n",
+                        "Loss on hold-out set: 2.397275202679184\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.19496855345911948\n",
                         "Epoch: 14\n",
-                        "Loss on hold-out set: 2.397287800626935\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.1540880503144654\n",
+                        "Loss on hold-out set: 2.3970512061748863\n",
+                        "Accuracy on hold-out set: 0.08962264150943396\n",
+                        "Metric value on hold-out data: 0.16116352201257858\n",
                         "Epoch: 15\n",
-                        "Loss on hold-out set: 2.3973036981978506\n",
-                        "Accuracy on hold-out set: 0.16037735849056603\n",
-                        "Metric value on hold-out data: 0.15644654088050314\n",
+                        "Loss on hold-out set: 2.3973692070763066\n",
+                        "Accuracy on hold-out set: 0.08490566037735849\n",
+                        "Metric value on hold-out data: 0.17059748427672955\n",
                         "Epoch: 16\n",
-                        "Loss on hold-out set: 2.3973520566832343\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.15959119496855342\n",
+                        "Loss on hold-out set: 2.3968730017823994\n",
+                        "Accuracy on hold-out set: 0.12264150943396226\n",
+                        "Metric value on hold-out data: 0.18553459119496857\n",
                         "Epoch: 17\n",
-                        "Loss on hold-out set: 2.3970124451619275\n",
-                        "Accuracy on hold-out set: 0.18867924528301888\n",
-                        "Metric value on hold-out data: 0.18238993710691823\n",
+                        "Loss on hold-out set: 2.396972402086798\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17845911949685533\n",
                         "Epoch: 18\n",
-                        "Loss on hold-out set: 2.396883694630749\n",
-                        "Accuracy on hold-out set: 0.20754716981132076\n",
-                        "Metric value on hold-out data: 0.19339622641509435\n",
+                        "Loss on hold-out set: 2.3969434252325095\n",
+                        "Accuracy on hold-out set: 0.09433962264150944\n",
+                        "Metric value on hold-out data: 0.1808176100628931\n",
                         "Epoch: 19\n",
-                        "Loss on hold-out set: 2.396961009727334\n",
-                        "Accuracy on hold-out set: 0.18396226415094338\n",
-                        "Metric value on hold-out data: 0.1871069182389937\n",
+                        "Loss on hold-out set: 2.396807058802191\n",
+                        "Accuracy on hold-out set: 0.10849056603773585\n",
+                        "Metric value on hold-out data: 0.18946540880503143\n",
                         "Epoch: 20\n",
-                        "Loss on hold-out set: 2.3967281512494356\n",
-                        "Accuracy on hold-out set: 0.15566037735849056\n",
-                        "Metric value on hold-out data: 0.17059748427672952\n",
+                        "Loss on hold-out set: 2.397344170876269\n",
+                        "Accuracy on hold-out set: 0.08962264150943396\n",
+                        "Metric value on hold-out data: 0.17531446540880505\n",
                         "Epoch: 21\n",
-                        "Loss on hold-out set: 2.3968697313992484\n",
-                        "Accuracy on hold-out set: 0.16037735849056603\n",
-                        "Metric value on hold-out data: 0.16430817610062892\n",
+                        "Loss on hold-out set: 2.3968090898585768\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.18396226415094338\n",
                         "Epoch: 22\n",
-                        "Loss on hold-out set: 2.3968204867165044\n",
-                        "Accuracy on hold-out set: 0.15566037735849056\n",
-                        "Metric value on hold-out data: 0.1658805031446541\n",
+                        "Loss on hold-out set: 2.3967214620338297\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17688679245283018\n",
                         "Epoch: 23\n",
-                        "Loss on hold-out set: 2.3964888914576115\n",
-                        "Accuracy on hold-out set: 0.14622641509433962\n",
-                        "Metric value on hold-out data: 0.1572327044025157\n",
+                        "Loss on hold-out set: 2.396907781654934\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.1808176100628931\n",
                         "Epoch: 24\n",
-                        "Loss on hold-out set: 2.39647679508857\n",
-                        "Accuracy on hold-out set: 0.1650943396226415\n",
-                        "Metric value on hold-out data: 0.16981132075471697\n",
+                        "Loss on hold-out set: 2.3971822801625953\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17531446540880502\n",
                         "Epoch: 25\n",
-                        "Loss on hold-out set: 2.396405152554782\n",
-                        "Accuracy on hold-out set: 0.14622641509433962\n",
-                        "Metric value on hold-out data: 0.15251572327044022\n",
+                        "Loss on hold-out set: 2.3964761293159342\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.18632075471698112\n",
                         "Epoch: 26\n",
-                        "Loss on hold-out set: 2.3961248982627437\n",
-                        "Accuracy on hold-out set: 0.14150943396226415\n",
-                        "Metric value on hold-out data: 0.15880503144654087\n",
+                        "Loss on hold-out set: 2.397053435163678\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.16823899371069181\n",
                         "Epoch: 27\n",
-                        "Loss on hold-out set: 2.3960445512015864\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.15330188679245282\n",
+                        "Loss on hold-out set: 2.3964457354455626\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.18396226415094338\n",
                         "Epoch: 28\n",
-                        "Loss on hold-out set: 2.3957734467848293\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.15959119496855342\n",
+                        "Loss on hold-out set: 2.3965258193465897\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17531446540880502\n",
                         "Epoch: 29\n",
-                        "Loss on hold-out set: 2.3956498919792897\n",
-                        "Accuracy on hold-out set: 0.1320754716981132\n",
-                        "Metric value on hold-out data: 0.1588050314465409\n",
+                        "Loss on hold-out set: 2.3968056822722814\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.1690251572327044\n",
                         "Epoch: 30\n",
-                        "Loss on hold-out set: 2.395675006902443\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.16116352201257864\n",
+                        "Loss on hold-out set: 2.3967400564337678\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17059748427672955\n",
                         "Epoch: 31\n",
-                        "Loss on hold-out set: 2.395716500732134\n",
-                        "Accuracy on hold-out set: 0.12735849056603774\n",
-                        "Metric value on hold-out data: 0.1572327044025157\n",
+                        "Loss on hold-out set: 2.3963877479985074\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.1690251572327044\n",
                         "Epoch: 32\n",
-                        "Loss on hold-out set: 2.3953244956034534\n",
-                        "Accuracy on hold-out set: 0.10377358490566038\n",
-                        "Metric value on hold-out data: 0.16116352201257864\n",
+                        "Loss on hold-out set: 2.3966873051985256\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17059748427672955\n",
                         "Epoch: 33\n",
-                        "Loss on hold-out set: 2.3954470922362128\n",
-                        "Accuracy on hold-out set: 0.10849056603773585\n",
-                        "Metric value on hold-out data: 0.15880503144654087\n",
+                        "Loss on hold-out set: 2.396476486943803\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.15959119496855342\n",
                         "Epoch: 34\n",
-                        "Loss on hold-out set: 2.394825890379132\n",
-                        "Accuracy on hold-out set: 0.11320754716981132\n",
-                        "Metric value on hold-out data: 0.16273584905660377\n",
+                        "Loss on hold-out set: 2.3962079691437057\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.1690251572327044\n",
                         "Epoch: 35\n",
-                        "Loss on hold-out set: 2.39506976559477\n",
-                        "Accuracy on hold-out set: 0.10377358490566038\n",
-                        "Metric value on hold-out data: 0.15959119496855342\n",
+                        "Loss on hold-out set: 2.3966402625137904\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17059748427672952\n",
                         "Epoch: 36\n",
-                        "Loss on hold-out set: 2.394251971874597\n",
+                        "Loss on hold-out set: 2.3969672738381154\n",
                         "Accuracy on hold-out set: 0.09905660377358491\n",
-                        "Metric value on hold-out data: 0.1588050314465409\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
                         "Epoch: 37\n",
-                        "Loss on hold-out set: 2.3945410206632793\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.15959119496855342\n",
+                        "Loss on hold-out set: 2.3962434800166004\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.16981132075471697\n",
                         "Epoch: 38\n",
-                        "Loss on hold-out set: 2.3943148603979147\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1580188679245283\n",
+                        "Loss on hold-out set: 2.3964536392463827\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.17295597484276728\n",
                         "Epoch: 39\n",
-                        "Loss on hold-out set: 2.39438392531197\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.154874213836478\n",
+                        "Loss on hold-out set: 2.39664056166163\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.16745283018867924\n",
                         "Epoch: 40\n",
-                        "Loss on hold-out set: 2.393499477854315\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.1580188679245283\n",
+                        "Loss on hold-out set: 2.396369938580495\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.16666666666666666\n",
                         "Epoch: 41\n",
-                        "Loss on hold-out set: 2.3942598396877073\n",
-                        "Accuracy on hold-out set: 0.09433962264150944\n",
-                        "Metric value on hold-out data: 0.15644654088050314\n",
+                        "Loss on hold-out set: 2.396285592385058\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.16430817610062892\n",
                         "Epoch: 42\n",
-                        "Loss on hold-out set: 2.3929953979996017\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16194968553459121\n",
-                        "Epoch: 43\n",
-                        "Loss on hold-out set: 2.3943119094056904\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1580188679245283\n",
-                        "Epoch: 44\n",
-                        "Loss on hold-out set: 2.39370825155726\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15959119496855342\n",
-                        "Epoch: 45\n",
-                        "Loss on hold-out set: 2.3940290729954556\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15644654088050314\n",
-                        "Epoch: 46\n",
-                        "Loss on hold-out set: 2.3929045920102103\n",
-                        "Accuracy on hold-out set: 0.08962264150943396\n",
-                        "Metric value on hold-out data: 0.15959119496855342\n",
-                        "Epoch: 47\n",
-                        "Loss on hold-out set: 2.3938033805703216\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15644654088050314\n",
-                        "Epoch: 48\n",
-                        "Loss on hold-out set: 2.392647180917128\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1572327044025157\n",
-                        "Epoch: 49\n",
-                        "Loss on hold-out set: 2.3933454549537516\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15880503144654087\n",
-                        "Epoch: 50\n",
-                        "Loss on hold-out set: 2.3941867351531982\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15251572327044022\n",
-                        "Epoch: 51\n",
-                        "Loss on hold-out set: 2.3924622220813103\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1572327044025157\n",
-                        "Epoch: 52\n",
-                        "Loss on hold-out set: 2.3930525014985284\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1540880503144654\n",
-                        "Epoch: 53\n",
-                        "Loss on hold-out set: 2.3934245649373755\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15330188679245282\n",
-                        "Epoch: 54\n",
-                        "Loss on hold-out set: 2.394263798335813\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15723270440251574\n",
-                        "Epoch: 55\n",
-                        "Loss on hold-out set: 2.39298766064194\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1572327044025157\n",
-                        "Epoch: 56\n",
-                        "Loss on hold-out set: 2.393838162692088\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15566037735849056\n",
-                        "Epoch: 57\n",
-                        "Loss on hold-out set: 2.3927098895018957\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15251572327044022\n",
-                        "Epoch: 58\n",
-                        "Loss on hold-out set: 2.3929288027421483\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1580188679245283\n",
-                        "Epoch: 59\n",
-                        "Loss on hold-out set: 2.3932194844731747\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.1588050314465409\n",
-                        "Epoch: 60\n",
-                        "Loss on hold-out set: 2.3932346982775994\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16194968553459116\n",
-                        "Epoch: 61\n",
-                        "Loss on hold-out set: 2.394061857799314\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15880503144654087\n",
-                        "Epoch: 62\n",
-                        "Loss on hold-out set: 2.3937397677943393\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15172955974842767\n",
-                        "Epoch: 63\n",
-                        "Loss on hold-out set: 2.393394002374613\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.16037735849056603\n",
-                        "Epoch: 64\n",
-                        "Loss on hold-out set: 2.393550157546997\n",
-                        "Accuracy on hold-out set: 0.08490566037735849\n",
-                        "Metric value on hold-out data: 0.15880503144654087\n",
-                        "Returned to Spot: Validation loss: 2.393550157546997\n",
+                        "Loss on hold-out set: 2.3964599146033234\n",
+                        "Accuracy on hold-out set: 0.09905660377358491\n",
+                        "Metric value on hold-out data: 0.1650943396226415\n",
+                        "Early stopping at epoch 41\n",
+                        "Returned to Spot: Validation loss: 2.3964599146033234\n",
                         "----------------------------------------------\n"
                     ]
                 }
             ],
             "source": [
                 "from spotPython.torch.mapk import MAPK\n",
                 "metric_torch = MAPK(k=3)\n",
@@ -2433,26 +1967,26 @@
             "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Loss on hold-out set: 2.375984536276923\n",
-                        "Accuracy on hold-out set: 0.12429378531073447\n",
-                        "Metric value on hold-out data: 0.20433145009416195\n",
-                        "Final evaluation: Validation loss: 2.375984536276923\n",
-                        "Final evaluation: Validation metric: 0.20433145009416195\n",
+                        "Loss on hold-out set: 2.3920064910074297\n",
+                        "Accuracy on hold-out set: 0.11864406779661017\n",
+                        "Metric value on hold-out data: 0.19585687382297554\n",
+                        "Final evaluation: Validation loss: 2.3920064910074297\n",
+                        "Final evaluation: Validation metric: 0.19585687382297554\n",
                         "----------------------------------------------\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "(2.375984536276923, nan, 0.20433145009416195)"
+                            "(2.3920064910074297, nan, 0.19585687382297554)"
                         ]
                     },
                     "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2469,42 +2003,42 @@
             "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "dropout_prob:  69.79375982811641\n",
-                        "patience:  20.07622456914753\n",
-                        "optimizer:  99.99999999999999\n"
+                        "l1:  19.950567044707373\n",
+                        "epochs:  6.3682105955519015\n",
+                        "optimizer:  100.0\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAuoAAAEnCAYAAAD/+WZRAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAADwe0lEQVR4nOydeXxU5b3/3+ecmUkm+75CQhKWsBogyOZCLYLW1h+t3mtXhbq14kpXba1tXehyq/a2am1r0aKol4pLrTsqbuCCBAhLSMKShSRkTyaTzHLO8/tjmCGTTJKZkA143veVWzLnOec85xDD53zP5/l8FSGEQCKRSCQSiUQikYwp1NGegEQikUgkEolEIumNFOoSiUQikUgkEskYRAp1iUQikUgkEolkDCKFukQikUgkEolEMgaRQl0ikUgkEolEIhmDSKEukUgkEolEIpGMQaRQl0gkEolEIpFIxiBSqEskEolEIpFIJGMQKdQlEolEIpFIJJIxiBTqEolEIpFIJBLJGEQKdclJs3v3bi6//HKys7MJDw8nMzOTCy+8kD/96U+jPbVh55VXXuGXv/zlaE9DIpFIJBLJaYgihBCjPQnJqctHH33EF77wBbKysrjqqqtIS0ujsrKSbdu2UV5eTllZ2WhPcVi58cYbeeihh5D/GUkkEolEIhlqTKM9Acmpzb333ktsbCyffvopcXFxftuOHTs2JOfo6OggMjKy1+dCCLq6urBarUNyHolEIpFIJJKxhLS+SE6K8vJypk+f3kukA6SkpABw+PBhFEXh8ccf7zVGURQ/68gvf/lLFEVh7969fPOb3yQ+Pp5zzjkHgAkTJvDlL3+Z119/ncLCQqxWK48++igABw8e5L/+679ISEggIiKCBQsW8J///KfX+Y4cOcKll15KZGQkKSkp3Hbbbbz++usoisK7777rG/f+++/zX//1X2RlZREWFsb48eO57bbb6Ozs9I1ZuXIlDz30kO86vF9eDMPgwQcfZPr06YSHh5Oamsr1119Pc3Nz0PdXIpFIJBLJmYusqEtOiuzsbLZu3UpxcTEzZswYsuP+13/9F5MmTeK+++7zs5WUlJTwjW98g+uvv55rr72WKVOmUFdXx6JFi7Db7dx8880kJibyxBNPcOmll/Kvf/2Lr371q4CnMn/BBRdQU1PDLbfcQlpaGhs2bOCdd97pdf6NGzdit9v5/ve/T2JiIp988gl/+tOfqKqqYuPGjQBcf/31HD16lDfffJP169f3Osb111/P448/zqpVq7j55ps5dOgQf/7zn9mxYwcffvghZrN5yO6XRCKRSCSS0xAhkZwEb7zxhtA0TWiaJhYuXCh+/OMfi9dff104nU7fmEOHDglArFu3rtf+gLjrrrt83991110CEN/4xjd6jc3OzhaAeO211/w+v/XWWwUg3n//fd9n7e3tIicnR0yYMEHoui6EEOIPf/iDAMQLL7zgG9fZ2Sny8/MFIN555x3f53a7vdf5165dKxRFEUeOHPF9tnr1ahHoP6P3339fAOKpp57y+/y1114L+LlEIpFIJBJJT6T1RXJSXHjhhWzdupVLL72UnTt38rvf/Y7ly5eTmZnJSy+9NOjjfu973wv4eU5ODsuXL/f77JVXXuHss8/2WWQAoqKiuO666zh8+DB79+4F4LXXXiMzM5NLL73UNy48PJxrr72213m6+947OjpoaGhg0aJFCCHYsWPHgPPfuHEjsbGxXHjhhTQ0NPi+5s6dS1RUVMAqvkQikUgkEkl3pFCXnDTz5s1j06ZNNDc388knn3D77bfT3t7O5Zdf7hPJoZKTkxP050eOHGHKlCm9Pp86dapvu/d/8/Ly/HzkABMnTuy1b0VFBStXriQhIYGoqCiSk5M5//zzAWhtbR1w/qWlpbS2tpKSkkJycrLfl81mG7KFthKJRCKRSE5fpEddMmRYLBbmzZvHvHnzmDx5MqtWrWLjxo2sXLky4Hhd1/s8Vl9JLiOR8KLrOhdeeCFNTU385Cc/IT8/n8jISKqrq1m5ciWGYQx4DMMwSElJ4amnngq4PTk5eainLZFIJBKJ5DRDCnXJsFBYWAhATU0N8fHxALS0tPiN8Va6T5bs7GxKSkp6fb5//37fdu//7t27FyGEX1W9Z9b77t27OXDgAE888QRXXnml7/M333yz1zl6Vue95OXl8dZbb7F48WIZHymRSCQSiWRQSOuL5KR45513Ajb7eeWVVwCYMmUKMTExJCUl8d577/mNefjhh4dkDl/60pf45JNP2Lp1q++zjo4O/vrXvzJhwgSmTZsGwPLly6murvbzznd1dfG3v/3N73iapgH4XZcQgj/+8Y+9zu3Nd+/5EPLf//3f6LrO3Xff3Wsft9vda7xEIpFIJBJJT2RFXXJS3HTTTdjtdr761a+Sn5+P0+nko48+4tlnn2XChAmsWrUKgGuuuYbf/OY3XHPNNRQWFvLee+9x4MCBIZnDT3/6U55++mkuvvhibr75ZhISEnjiiSc4dOgQzz33HKrqeR69/vrr+fOf/8w3vvENbrnlFtLT03nqqacIDw8HTlTH8/PzycvL44c//CHV1dXExMTw3HPPBcw/nzt3LgA333wzy5cvR9M0vv71r3P++edz/fXXs3btWoqKili2bBlms5nS0lI2btzIH//4Ry6//PIhuX6JRCKRSCSnKaOaOSM55Xn11VfFd7/7XZGfny+ioqKExWIREydOFDfddJOoq6vzjbPb7eLqq68WsbGxIjo6Wvz3f/+3OHbsWJ/xjPX19b3OlZ2dLS655JKA8ygvLxeXX365iIuLE+Hh4eLss88WL7/8cq9xBw8eFJdccomwWq0iOTlZ/OAHPxDPPfecAMS2bdt84/bu3SuWLl0qoqKiRFJSkrj22mvFzp07e8VMut1ucdNNN4nk5GShKEqvqMa//vWvYu7cucJqtYro6Ggxc+ZM8eMf/1gcPXo02FsskUgkEonkDEURIoBvQSI5g3jwwQe57bbbqKqqIjMzc7SnI5FIJBKJRAKAFOqSM4rOzk6/xZ1dXV3Mnj0bXdeHzIojkUgkEolEMhRIj7rkjOJrX/saWVlZFBQU0NraypNPPsn+/fv7jFGUSCQSiUQiGS2kUJecUSxfvpy///3vPPXUU+i6zrRp03jmmWe44oorRntqEolEIpFIJH6Majzj2rVrmTdvHtHR0aSkpLBixYpeedhdXV2sXr2axMREoqKiuOyyy6irqxulGUtOdW699VaKi4ux2Wx0dnayfft2KdIlI0Ywv/N6smnTJgoLC4mLiyMyMpKCggLWr1/vN6auro6VK1eSkZFBREQEF110EaWlpb7thw8fRlGUgF8bN270jQu0/ZlnnhnamyCRSCSSoBlVob5lyxZWr17Ntm3bePPNN3G5XCxbtoyOjg7fmNtuu41///vfbNy4kS1btnD06FG+9rWvjeKsJRKJZHAE8zuvJwkJCfzsZz9j69at7Nq1i1WrVrFq1Spef/11wJPxv2LFCg4ePMiLL77Ijh07yM7OZunSpb7jjh8/npqaGr+vX/3qV0RFRXHxxRf7nW/dunV+41asWDFs90MikUgk/TOmFpPW19eTkpLCli1bOO+882htbSU5OZkNGzb4Mqf379/P1KlT2bp1KwsWLBjlGUskEsng6fk7L1jmzJnDJZdcwt13382BAweYMmUKxcXFTJ8+HQDDMEhLS+O+++7jmmuuCXiM2bNnM2fOHB577DHfZ4qi8Pzzz0txLpFIJGOEMeVRb21tBTwVJIDt27fjcrlYunSpb0x+fj5ZWVl9CnWHw4HD4fB9bxgGTU1NJCYm9tnuXSKRnF4IIWhvbycjI8PX8CoUurq6cDqdQZ+r5++WsLAwwsLCBty35++8YM719ttvU1JSwm9/+1sA3+87b+MuAFVVCQsL44MPPggo1Ldv305RUREPPfRQr22rV6/mmmuuITc3l+9973usWrVK/u6USCSSUWLMCHXDMLj11ltZvHgxM2bMAKC2thaLxUJcXJzf2NTUVGprawMeZ+3atfzqV78a7ulKJJJTgMrKSsaNGxfSPl1dXWRZrdQHOT4qKgqbzeb32V133cUvf/nLfvcL9DuvL1pbW8nMzMThcKBpGg8//DAXXnghcKJ4cfvtt/Poo48SGRnJAw88QFVVFTU1NQGP99hjjzF16lQWLVrk9/mvf/1rLrjgAiIiInjjjTe44YYbsNls3HzzzQPcBYlEIpEMB2NGqK9evZri4mI++OCDkzrO7bffzpo1a3zft7a2kpWVxXtA1EnO8XQnb6g62l85+F33nZ8T0vhNhLZe4bkQx5c/17+ACsjfQt8FgK3lg9yxP/5vGI451Pz3MBzTBpxHdHR0yHs6nU7qIajfGTbgPJuNyspKYmJifJ8HU00P5XdedHQ0RUVF2Gw2Nm/ezJo1a8jNzWXJkiWYzWY2bdrE1VdfTUJCApqmsXTpUi6++GICORs7OzvZsGEDd955Z69t3T+bPXs2HR0d/P73v5dCXSKRSEaJMSHUb7zxRl5++WXee+89v+pXWloaTqeTlpYWv6p6XV0daWlpAY/V1yvnKKRQH4gY8xAd6GkgsC12QKJiQrMphDGwIOqOFupPQUTMwGN6Muj/qobjJ/S7wIZhOO5Q8M1hP8PJWDZC+Z0RExPjJ9QHoq/feX2hqioTJ04EoKCggH379rF27VqWLFkCwNy5cykqKqK1tRWn00lycjLz58+nsLCw17H+9a9/YbfbufLKgZ+o58+fz913343D4Qjq4UMikUgkQ8uopr4IIbjxxht5/vnnefvtt8nJ8a+mzp07F7PZzObNm32flZSUUFFRwcKFC0d6upIxyBU8O6zjJ1+xK6TxJ8W5k4bpwMMviENnLM5p+Bnod16wGIbhtxbHS2xsLMnJyZSWlvLZZ5/x//7f/+s15rHHHuPSSy8lOTl5wPMUFRURHx8vRbpEIpGMEqNaUV+9ejUbNmzgxRdfJDo62uc7j42NxWq1Ehsby9VXX82aNWtISEggJiaGm266iYULF8rEF8nYZTXQe43eKOMVxmOhun5minQY+HcewJVXXklmZiZr164FPOtuCgsLycvLw+Fw8Morr7B+/XoeeeQR33E3btxIcnIyWVlZ7N69m1tuuYUVK1awbNkyv/OXlZXx3nvv8corr/Sa27///W/q6upYsGAB4eHhvPnmm9x333388Ic/HK7bIZFIJJIBGFWh7v2Hxvv61su6detYuXIlAA888ACqqnLZZZfhcDhYvnw5Dz/88AjPVCIZIc6dBO+XDjxu0HyT0RXrZ65Ih+B+51VUVPgl1XR0dHDDDTdQVVWF1WolPz+fJ5980q9RV01NDWvWrKGuro709HSuvPLKgB70f/zjH4wbN66XgAcwm8089NBD3HbbbQghmDhxIvfffz/XXnvtEFy5RCKRSAbDmMpRHw7a2tqIjY3lc6RHfSAmfWMIDzZIjzrAngvyQhr/LKF1Fg11/IFnZ4U0Hji5ivqwCnUvoyHWR1Kk24A5tLa2huQdh9B+Z3jOwqDOI5FIJBLJQIyqR10ytih9erRnMDYZUZ86DKNXvTsjKZq/OcLnAxaG9rAnkUgkEslYRAp1ySnPcC8oHRSrh/8UJ89ICOhRsLqMyIOORCKRSCTDjxTqkuHh76M9gVOcERWbwyGmR6GKDlKkSyQSieS0YkzkqEskY53JV+wK3at+sukvw76wtDuBRHUoPvYze5GoRCKRSCTDgRTqkjOSK3g25EWlZx49xfeGPj4fI8hqukQikUhOM6T1RTLmmP52ecj7jIjvfDCcrFd9TInPUbKzBMOYuk8SiUQikQwNUqhLJEEy4ukvXqQI7R95fyQSiURymiKFukQikUgkEolEMgaRQl1yxjJidpmhiGqUVePAyPsikUhCQAiB2+2mo6MDh8OB2+3mNO/7KDnFkUJdMnychhGNo2Z/kfRGinSJRBIChmHgcrlwOBx0dXXR0dFBe3s7bW1tUrhLxiwy9UUiOVUY0bhGiUQiOT0QQvhEuhACRVEwmUwoigJ4BLzT6cTpdNLZ2YnD4SAlJQWTyYSmaWia5hsrkYw0UqhLJBKJRCI5LRFC4HA40HUdVVX9BLf3z5qm+ca2tbVRV1dHbGwsTqcTAFVVMZvNaJqGyWTqdRyJZDiRQl0ikUgkEslph7eK/vnnn5OQkEBOTg5An9YWRVFQVY8j2Gw2I4TwfXV1dfmNMZvNvoq7FO6S4UQKdYlEIpFIJKcNQgh0XcftdmMYRkhCumfFvXvVXQp3yWgghbpEIpEEIO9yiDH3P6bNBfxrRKYjkUiCQAiBy+VC13UAn2gOZYFofxX3YIS71yIjhbtkKJBCXSKRSCQSySmPd1Fozyp6KEI9FEHdl3A3DMMn3FVVRVVVKdwlg0YKdYlEIpFIJKcsXquLN9Ul0KLRUIT6YOMZ+xLuuq6j6zpdXV1SuEtCRgp1iUQikUgkpyR9WV2601N8u1wumpubiY2NxWQaPhnkFe7eBao9hbvD4fCzynj/t7vgl0ikUJdIRoLVwEOjPQmJRCI5ffBW0QdaMNpdqLe0tFBUVITb7UbXdWJiYoizWIhuasJSVUXXrl1Yy8qoiYjAsNkw7HYUiwVTRgamzExMWVlYpk3DWliIoobWM7Iv4e52u3G5XL7tPT3uUrif2UihLhmTTH+7nD0X5IW0zxU8y7NcMUwzkowpZFdSieSMxStu3W43ELiK3h1FUTAMg0OHDlFWVkZeXh7p6ek4nU7qfv97nI8/TpNheMYCGmA3mfyEuLOkBCUiAjUzE0dpKVpyMtHLlxP9pS8RPnfuoIR0KMLdm+PutcpIzhzk37bkjOYKnh25k60egmNIgSqRSM5gvAtGgxXp3n1qa2s5cuQI8+bNY8KECWAY2O65B+PJJzGZTFgsFsxms0+cu9xunE7nCVtNQgIiPh5Hqac7tF5fT8uTT1L5zW9y5Mtfxr5160lfm1e0m0wmnzBXFAW3243dbsdms1FeXk5jYyNdXV2+twmS0xsp1CWSEJl8xa7RncCZLtbP9OuXSM5AvN5up9OJrut+lej+aGpqora2FkVRWLx4MXFxcQiXi/pbbqF940a/sd5jKoriE+6qquJOSsLW0UHHoUM+4d7d8+4sLaXqqqs4evPNuI4eHbJrDiTcy8rKsNls2O122tvbaWtrw2azSeF+GiOFuuS0YkQr5INhKKrqcOaK1TP1uiWSMxjvglGn0xkw1aWvfcrLy9m+fTuxsbEkJSVhNpsxuro4et112N96q7+dAY9QDsvLw+x2E+5w+IS7YRg4j8/HddzrLoTA9tprHL7oIpr/8Y+hvHwf3mv2CnfvwlOXy+WruEvhfvohhbrkjGcw4n7Uq+pw5onWM+16JRKJn9Wle8W7PxwOB5999hnV1dXMnz+f2NhYAPSWFqq/+13sW7YEdW7zzJk4jh7FaG8HQO3mFw+zWHxC2TtHp9OJy2aj9r77qP7pTxHH7TlDiRDCLx++Z8UdPKk2nZ2dAYX7YKMnJaOHXEwqGV7+DlwzuF0Hs6D0lGAoE2DOnQTvlw7RwcYwUqRLJGcUXqtLTU0Nhw8fZt68eUEt2GxoaGDXrl0kJiYye/ZsTCYTtbW1iD17OHzNNdDVhTU/H+V4dRxVRRECcfycDrudjuZmTOPH07ljR7/nUlXVU+3UNM/+hoFhGOi6TtPTT9Owdy9hv/wlCePGERcXh8ViGZL70hfehafdxxqG4Xsb4V2c6k2U6Z4qIxm7SKEukQySyVfs4sCzs0Z7Gqe3WJcCXSI54+iejS6E8InM/jAMg7KyMo4cOcLUqVPJzMz07aP+5z+EP/ccVpsN0d6OaGrynMd7vm7HMZlMKImJUFxM1JQpiPBwHEeP4q6v7/f8CqAcb2bkPabYuxfxox9x5Ac/oDg8nKioKOLj44mPjycuLm5QGe7dK+oDEYxwV1W1V6qMFO5jCynUJX6UPg2TvjHaszg5BhPTOOLRjkOdq+4VtKeTYJciXSI54+iZje7t8NkfXV1d7Ny5E5fLxYIFC4iOjvZts61fj/n++z3Rh2Zz/ye3WHBnZKAdOOD5c0kJ4BFK4VOm4OzsxFlREdR1eIV7XIKJgs//ge37f6JZ12hubqasrIzOzk6io6N9wj02NtZPVPd77EEK6WCFe/dquxTuo48U6hLJSXBSVfXhaIJ0ulTXpUiXSM4o+spG79lVtCfHjh1j9+7dpKamMnXqVD8h2rFhA6133RXcBCwW9Oxs9OPivCfukhJURSFq+nQcTU24amr6P54C2V8pIMG2Gyp0Yh69CfMPnyQlJQXwPFw0NzfT3NzMvn37cDqdxMbG+oR7TExMwFSbUCrqA9FduHvvsddv7+2aKoX76COFumRMc9r61IeTU12sS5EukZxReKu63oSS7p04vSkrgfY5cOAAlZWVTJ8+nYyMDL/t9ueeo+XnP/cluPSHMJsROTm4+hDpJwYK3Hv2oKkqYQUF2HbtggBzM8VEMGl5NuH1Rb7P1MO7CPv7D3B870+gqoSHh5Oenk56ejpCCDo7O33CvaqqCl3XiYuL8wn36OjoAR9aTgbv/ZbCfewhhbrktGQk7S9jrqoOp6ZYlwJdIjmj6G698FaKe4q+QOLUbrezc+dODMNg0aJFREZG+m3vfPVVmn/84+BF+sSJOPftC37ihoG7qIioyZPprK1Fb2vzbYrOH0fOZBdafe/jmYreRPzrNzj/+45e1xgREUFERASZmZkIIejo6PAJ9yNHjgB4MuCFwG63Y7Vah1UgBxLu3i+Hw4HT6QSQwn0EkEJdIhlthlOsw6kh2KVIl0jOKLovGAUCinToXVGvra2luLiYjIwMpkyZ0svX3fnKKzTdckvASndPlJQU3FYr7lBEejfcBw4QlpyMOysLZ0UFGRfOJFWUQJuzz33Mbz2OkZyF+wvf7nteikJUVBRRUVGMHz8eIQTt7e20tLTQ0NBAcXExmqb5qu3x8fEjIty7i/eewj1Qxd1kMgUVpynpH5mjLhl+/j7aEwiewTZMGhO56n1x7qSxK4TH8tyGgbVr1zJv3jyio6NJSUlhxYoVlAzwun3Tpk0UFhYSFxdHZGQkBQUFrF+/3m9MXV0dK1euJCMjg4iICC666CJKS088oDU1NXHTTTcxZcoUrFYrWVlZ3HzzzbS2tvodx/uPcfevZ555ZuhugERCaNnoXqGu6zp79+6luLiYGTNmMG3aNP+FkS4XLXfdRdMtt2BJTyNy1nRi5hYQWzibyLOmEz5tEnHzZhNbWEDM3ALC5xXi1jTcx6vVPkIUlUZ9PVpDPbnfPIdU125w9y3SvYT931rUyuAfDhRFISYmhvHjxwMwf/58Zs2aRWRkJHV1dXzyySd89NFH7N27l5qaGrq6ukK6hsHQMzHGK8oNw+Ctt96isbGRtrY22trasNvtvo6yMsc9dGRFXTLmGaxPfcSTXE6G4aqqd2esVNjPIGHeky1btrB69WrmzZuH2+3mjjvuYNmyZezdu7fX63svCQkJ/OxnPyM/Px+LxcLLL7/MqlWrSElJYfny5QghWLFiBWazmRdffJGYmBjuv/9+li5d6jvu0aNHOXr0KP/zP//DtGnTOHLkCN/73vc4evQo//rXv/zOt27dOi666CLf93FxccN5SyRnEN5sdLfb7Ut1Gaja6m0otG3bNlRVZdGiRURERPgft60N149uw3pgP1aLgGNVnq/jqLqOYeiYzJ4ccyNvMq6ScqLcbpT0dIzkZFyGgb2kBJwDC+3umBJimHBOCuYjWzGyp6IeDUKA6y7CHvshnT97HszBZ6t7Ra6qqsTGxhIbG0tOTg66rtPa2kpzczPV1dXs37+f8PBwv4r7UGS490fPNyIWiwVVVRFC+B4cvItXu1tlZMV9YKRQl0iGiJPOVR8JsQ6jJ9jPYIHu5bXXXvP7/vHHHyclJYXt27dz3nnnBdxnyZIlft/fcsstPPHEE3zwwQcsX76c0tJStm3bRnFxMdOnTwfgkUceIS0tjaeffpprrrmGGTNm8Nxzz/mOkZeXx7333su3v/1t3G63X55zXFwcaWlpQ3TFEomHnlaXYAVafX09QggSExOZPHlyryQU0dWF+/vXILZ/Gtw8snPoPFgBx9NlRE0NSk0NFiAsPp6uzEya9+4NyjoTMXkc43McqPVlnmuqKMMYNwm1duDfrerRUiwv/AHnf90e1LzhhFDved80TSMhIYGEhAQA3G43LS0tPn/7nj17iIyM9MtwNw8UVTlIvDYlrwj3/tlrkzEMwyfc1eO581K494+0vkgkPRis/WVIWD2C5xop28kZYG/xvuL1fjkcjqD281pPvP/ADoQQgs2bN1NSUuIT9t5zhYeH+8apqkpYWBgffPBBv+eOiYnp1XRl9erVJCUlcfbZZ/OPf/xDvqqWnDSGYeBwOIKyunhxu93s3r2bsjKPCJ4yZUpvke524751NUYwIl2AkZZB59F6RGdn4CHNzVh27ybOMIgrKEDtUbnvTtzZk8nKaEJt69YISXeh1lRipOQMPB/A/ObjqCUfBzW2OwPdO5PJRFJSEpMmTeLss8/m3HPPJScnByEE5eXlvP/++3z66aeUlZXR2Njoi8QcCrxCveffVSCrjPdticPhwGaz0d7eTnt7u7TK9EBW1CWnNSNtfxmSbqUjVVn30lNED0Wl/XQQ5lcCgd0oJ+gA/oXPO+rlrrvu4pe//GW/uxqGwa233srixYuZMWNGv2NbW1vJzMzE4XCgaRoPP/wwF154IQD5+flkZWVx++238+ijjxIZGckDDzxAVVUVNX1kPTc0NHD33Xdz3XXX+X3+61//mgsuuICIiAjeeOMNbrjhBmw2GzfffHP/90EiCYDX6uJNdQm2Wtre3s7OnTsxm82cffbZfPTRRxiG0WvhqP6LOzDefTuouTijY1A6nAibzbOvrvvEY09UpxOlqIi4xEQ6MzPpLPX/nZi6/CwSbMXg0AOcqAul/hhG4njUxsoBZiUIX/dj7He9DNboAcb2XVEfCLPZTEpKii/D3eFw+BJlSkpKcDgcxMTE+GW4B9t8qSfdFwf3R0+rjLfirus6uq77LU71dk31ivszreIuhbpEIvGnu8gORbSfDuJ8kFRWVhITE+P7PiwsbMB9Vq9eTXFxcb9Vby/R0dEUFRVhs9nYvHkza9asITc3lyVLlmA2m9m0aRNXX301CQkJaJrG0qVLufjiiwNWo9ra2rjkkkuYNm1ar4eJO++80/fn2bNn09HRwe9//3sp1CUhYxgGzc3NqMczw4MR6UIIqqur2bdvH9nZ2UycONFXoe35s+z+4x/QN20Mai7CGoFdDSeiocEXB+mNfRSAelwQ9qrYNzYS3tREWEEBrXv3oqiQdfEUrLU7+z2f0tUBHVZEWBSKw9b/2KYawp65B8eq3w58HUNUXQ4LCyMtLc1nceue4X706FHcbrdf86Xo6OiADzSBCHbtQU+8Atx7nu7C3fsmJpDH/UwQ7lKoSyQSyUkSExPjJ9QH4sYbb+Tll1/mvffeY9y4cQOOV1WViRMnAlBQUMC+fftYu3atz78+d+5cioqKaG1txel0kpyczPz58yksLPQ7Tnt7OxdddBHR0dE8//zzA/pU58+fz913343D4Qjq4UMi6Z6NXlpaSmxsLLm5uQPu53a72bNnD42NjcyePZukpCTf8QC/iEb9mafQH/lzcPPRNOyJaZgOlOLWNHS325f33X2+3mQZ72e6rnsEJ6AUFZE0M5/YqRbMlcElfCmtDRhZU1Fq98EAOtK09Xlciy/DmHx2cMceYmFqtVqxWq1kZGT4ctq9wr2yshLDMPyaL0VFRfU5B69QP1n6Eu5ut9v3oOUV7h0dHezfv5/zzz//tBTtUqhLJBLJCCGE4KabbuL555/n3XffJScnOC9rT7y+zp7ExsYCUFpaymeffcbdd9/t29bW1sby5csJCwvjpZde8vO090VRURHx8fFSpEuCwiukvJ5n7yLCgWhra6OoqAir1crixYv9ft68Qs0r1I133sJ99y+CnpNr4jTYUeQR3243ZrPZT8x5xZ5XuOuGgft4l1RvJVfLTScxvgbtGBjJWaj1FUGdW63Yhz7pLLSK/ivwAGHP3ONJgenHcjJY60soKIpCZGQkkZGRjBs3DiEENpvNJ9wPHTqEoih+iTIRERG+OQ2VUA80r76E+44dO7juuuuoqAju7+VUQwp1iUQiGSFWr17Nhg0bePHFF4mOjqa2thbwCGyr1QrAlVdeSWZmJmvXrgU82euFhYXk5eXhcDh45ZVXWL9+PY888ojvuBs3biQ5OZmsrCx2797NLbfcwooVK1i2bBngEULLli3Dbrfz5JNP+ha9AiQnJ6NpGv/+97+pq6tjwYIFhIeH8+abb3Lffffxwx/+cCRvkeQUxVtF7+797tmsqCdCCCoqKjhw4AC5ubnk5uYG7EzqHWvs3oXrtptA731MJdIKqopwOD2JLobANX02js+2+x4cLBZLwE6n3VEVBRTF97ZJm5FNbGQNtNpwC4Fht2EkpBPeXI2qqANWy7XyYozMHNRjh/odp1btx/TBs7jP/2afY0ZjYaWiKERHRxMdHU1WVhaGYdDe3k5zczP19fWUlZVhMpl8oj2QhWi45uX9ObPb7URGRp6W1XSQQl0ikUhGDK+47hm5uG7dOlauXAlARUWF3z90HR0d3HDDDVRVVWG1WsnPz+fJJ5/kiitOLJKuqalhzZo11NXVkZ6ezpVXXunnN//888/5+GNPuoTXQuPl0KFDTJgwAbPZzEMPPcRtt92GEIKJEydy//33c+211w7lLZCcZvSXja6qqs9O0hOXy0VxcTEtLS3MnTu33+QjVVURRyvhj/cRNjsfVRMozk6Urg4Uuw3FbgP9eJLL8aAWd14B2oGDdOWkYYmIwulwYe504q6pC/raIhZNJUaUe5oYWSyeKq7uwt1YR2tcGpGNVSiqgqp4xKmiBhCKho7S1h6UX93ywoO4Cy+ByNiA20eioj4Q3TPcJ0yYgGEYvgz3mpoaXwFg3759PvE+3G/k7HZ7r2z90wkp1CUSiWSECKYi9u677/p9f88993DPPff0u8/NN9/c74LPJUuWDHjuiy66yK/RkUQyEANlo/dVUW9paWHnzp1ERUWxePHiAZvxmLvsRN15HabqI/2O8+IeNwnnpzsQTieJZo/Mcbt1LBYLYmoWzpgE7Ier0WuP9XVhRH1hJlH2PX556t4qrgUDi60Z14RpqFUlCMPA5fLeAwXleFXZey+U1gaM7ON+9X5QOlqwvPhHnN8MbO0ZC0K9J6qq+gQ5eLokHzx4ELPZTGVlJXv37iUiIsLPKjPUGe42m42oqKghPeZYQgp1iUQikUgkIWEYBk6ns9+UD03T/DK6hRAcPnyYsrIyJk6cyIQJEwYWnS4XZz3zJ9SqQ6AMbKlwJ6TSuacczeXCfNzq4nlYOC5yqyoI4whhAvSZedidCo6SMv+DLMwjqqMY+nu4dbswHzuKkZqN1lAFosfCVLcblBPVdvXwXvS8GWjVe/qdv/m9p3Gf/3WMzMkBt48lkd4XFovF9+bO5XL5mi8dOnSI4uJioqKi/Jov9ezlECodHR19dnY+HZBCXSKRSCQSSVCEko3evaLudDrZvXs3NpuNefPmERcXN/DJdB3Tb39M/KF9EEQVtit1Al1lVYQ5HZgsZgYykGuHy4kGrLOn0NHSietQBdEXnYWl5lPQgrBrOOwoXZGIiBgUe5tn4amqoaF5GiwJA3E8TcbtNnAfKcdkNmPSHX37uA0d84v/g+OGv/baJIQY80K952JSs9lMcnIyycnJgOfnwLswtbS0lK6uLqKjo33CPTY2NuQM946ODllRl0gkEolEcmYzkNWlJ16h3tTUxM6dO4mLi2PRokXBWR8aj2G6+xbUHduOn5w+dbdA0JoyGdOuPVhNGqopNGuFqayEWEXB+O9zMR3dTih9OpWWeoyMXBRHJ+iubhvwLDZVVTQAITA57bQnT8Jatw+E8FhkFNVnlxHhEXQtm0b7lw8Qpm3DpC/wv85ToEvnQKkvFouF1NRUUlNTAejq6vIJ93379uF0Ov0y3GNiYgZcnCor6hLJGGD62+XsuSBvxM430h1NezHS3Un74gxuYiSRSE7graKH0tBGURTa2trYvn07U6ZMYfz48cHtt/MTTL9cjdLU4Pm+n7FCCBoScojYvQez2YQSwB4TVA16yVlYyt7HiE3EFhdOQmdTMHsBoB49iJE3E/XI7r4HKQqqphBbdwhj3BSUuoMYhoEwBF2oNJ2dg/ENG2riAVRVxWE8GlCon2oV9YEIDw8nPT2d9PR0hBB+zZeqqqrQdd0vwz06OrrXPTjdhfrwZ+hIJAB/H+0JjByTrwiuIcaArB6aw5yRyKASiWRI8FbRnU7ngFaX7jgcDiorK+nq6mL+/PlkZWUFJ9LL92P66Xd9Ir0/DMPgWNx4okpKsVjMAUX6wCcE5YICTFVFAKitDUQ21+HOKyBIie/Zr3w3ek7BwAOFgdLlQlE9nTWZlo/toQmoNzejJjo83n+Xiy69iPKqp6itrfXrmXC6CfXuKIpCREQEmZmZzJgxg3POOYfCwkISExNpbW2lqKiI999/n127dlFZWYnNZkMIMaD1Ze3atcybN4/o6GhSUlJYsWIFJSUl/c5l06ZNFBYWEhcXR2RkJAUFBaxfv95vTF1dHStXriQjI4OIiAguuugiSkv9u3kvWbLEtwjZ+/W9730vpPsyqkL9vffe4ytf+QoZGRkoisILL7zgt33lypW9LlCmEkhC5QqeHdH9QIr1UUXeM4lkSPAuGPUuCA1WpDc0NPDhhx9iNptD69rbUIfpJ6tQ7B09NigIswkRE4OIikRERODSVBqiUog9UoXJbKJfUa3gXUvqh4iOQDl/Klplkf9wYWA6UISRMRFhDb5Sqx0sxkgeP+A4pb4KffxMHEvm0PDzFvSENl/jJbPZTJjFgslkInbcJiorK/jwww/5+OOPOXLkiK8R01jF29F1KFAUhaioKMaPH8+sWbM499xzKSgoIDY2lsbGRj777DOuu+46du7cyb59+ygrKwtoD9qyZQurV69m27ZtvPnmm7hcLpYtW0ZHR8+fsxMkJCTws5/9jK1bt7Jr1y5WrVrFqlWreP311wHPA+yKFSs4ePAgL774Ijt27CA7O5ulS5f2Ou61115LTU2N7+t3v/tdSPdhVK0vHR0dnHXWWXz3u9/la1/7WsAxF110EevWrfN9LzvkSc44xooN5lRAinSJ5KTxppeEanUxDIOysjKOHDnC1KlT0TSNw4cPB3fSLjva336NyE5HTEgFVyeKww5dHRgtjWiKC0VtO96N0kVndAKJzZ2o4xMQ0XEQHonQTIjWDsShQ+B09Xs6kTsOU5ILpbrvyES1shSRMg6hmVFsLQNfg+5Gcelgsniy1/vAyM5GfNlN6wIbaIFz5lVVJSyyioIF7dB1Hs3NzdTV1WEYBu+//z4xMTHEx8eTkJAQlI97pBiuzqTgEe7eB7/s7Gzfue6991727t3L9OnTefjhh7n66qv99nvttdf8vn/88cdJSUlh+/btnHfeeQHP1bPXxS233MITTzzBBx98wPLlyyktLWXbtm0UFxczffp0wNMnIy0tjaeffpprrrnGt29ERARpaWmDvu5R/Zu9+OKLueeee/jqV7/a55iwsDDS0tJ8X96sTsmZx/S3ywe97yldVQcpQAdiNfIeSSRDgBACp9OJw+EIyerS2dnJp59+yrFjx1iwYAHjxo1D07R+O5P60HVM99+I9tkrqId3oB7aiVp1AKW+CqW9GVV3e1JUDAOny4nbHEGUKxKtswOlpQm18iBq6W60/Tsw1RzAHAXazEmo82bD8bSR7nVWZdIETFEtKM0DNz9SjlWBFoaITRr4OgCl4Sj6+GkBtxnjs3DfPBXxqyMoZxUT7RhYzzgtf8Nk1khJSSE7OxuLxcKCBQtIT0+ns7OT3bt38/7777Nz504/O8hoMZxCvSeqqnLeeedhNpv58Y9/TEtLi18juL5obW0F6LfJVneEEGzevJmSkhKfsPfakcLDw/3mExYWxgcffOC3/1NPPUVSUhIzZszg9ttvx263B3VeL2N+Mem7775LSkoK8fHxXHDBBdxzzz0kJib2Od7hcPj5ubxdsiSS0WDyFbs48OysoTmYrKwHRgp0iWRI8FbRP/roI3Jzc4OuAh47dozdu3eTmprqq6RD/51Ju6Ot+xXq9ncGnJthGGgWC+bIHNSDpX0PdrtQj3i2a6qKa1Y+9rpmwo7Vo0zKRrM2gr2vLqG9H0qUpjpEbCJGQjpqU83A11O2EyNrMmr1AQBEbDz6d9JR5u6l+zOP2diJ2T0Zl6nvBwZDPYTb9CZm93LfYlKr1YrVaiUjI8Pn0W5qaqKpqYny8nJMJpOv2h4fH+8nJocbwzCGvKHRQHR0dBAdHY3Vah1wrGEY3HrrrSxevJgZM2b0O7a1tZXMzEwcDgeapvHwww9z4YUXApCfn09WVha33347jz76KJGRkTzwwANUVVVRU3PiZ+Sb3/wm2dnZZGRksGvXLn7yk59QUlLCpk2bgr6+MS3UL7roIr72ta+Rk5NDeXk5d9xxBxdffDFbt27tM2dz7dq1/OpXvxrhmUqC4u/ANQOOGnOMegJMd6RY90eKdInkpPFmo7vdbo8YDrISbhgGBw4coLKykunTp5ORkeG3PZjjqC88ivbq+j63CwRCeL60mCRUczpq+YHgLswzSUyH9hPrdKEtPhviTCgHDgeyrPeL0toIUbEYiZmojdX9DxYCpakeER6NyEjEuKkVJX5v72NiEOVQaB5AiTktf8PkXhqwUu71cUdFRZGVlYVhGLS2ttLc3Ex1dTX79+/HarX6hHtcXNywCumRrKh7sdvtREREBDV29erVFBcX96p6ByI6OpqioiJsNhubN29mzZo15ObmsmTJEsxmM5s2beLqq68mISEBTdNYunQpF198sd/f03XXXef788yZM0lPT+eLX/wi5eXl5OUFl2Q3poX617/+dd+fZ86cyaxZs8jLy+Pdd9/li1/8YsB9br/9dtasWeP7vq2tjfHjB17cITk1OJmYxtES3ENaVQcp1r1IkS6RnDSBstE1TRuwEm6329m5cyeGYbBo0aKA8XjdGx71wtGJ9tefo73bd2VRCE+FH0BPysXSYEdpCUGkd6MjNZn49nKUYzaMzIkIpxP1WEU/e/QObldsrWAyI6LiUWzN/Z5P6bTh/soCuHQbirlvv7xJ7CPMeRYOS99zMZRK3KbNCDFvQBuSqqq+KMPc3Fzcbrcv7rC8vJzOzk5fg6GEhARiY2OHVFiPtFD3vlGIjo4ecOyNN97Iyy+/zHvvvce4ceMGHK+qqq/DakFBAfv27WPt2rU+//rcuXMpKiqitbUVp9NJcnIy8+fPp7CwsM9jzp8/H4CysrLTQ6j3JDc3l6SkJMrKyvoU6mFhYXLBqWTIOVmRPyxiHc5cwS5FukRy0vSVjT6QUK+traW4uJiMjAymTJnS5xvuPoV6zWHMv70OpbJv+4q3wq9pGvaYTCLKqkMIS+xxrKzxWBxHUTqPVzorS3HpOh3pE4lqrsHs6gw62lFpaUCkZoGrCxydvQdoJvSF01AXHcUU9T5u1xQw9x8FGOlsxmFWQOm7zu80/xMhCkOOZzSZTH6dQR0OB01NTTQ3N7Nnzx7cbrcvpzwhIYGoqKiTioAcjYr6QPGMQghuuukmnn/+ed59911ycnIGdR7DMPys1V5iY2MBKC0t5bPPPuPuu+/u8xhFRUUApKenB33eU0qoV1VV0djYGNIFSiRjhSEX63DmVdelQJdIThpPcoobt9sdcMFoX0Jd13VKSko4evQoM2bMGNDDHtCj3tqI+Z6VKLVH+podLrcbQzc8DYziM7AcbAa3G0yhSxZjxjTUtkOYXZ0QFobbraPrOiaTRlxdOY6IWOxhkUQ013o6hAYh2JW6CoysKag1ZWDo3ovFOHs6yrm1aNEnggS0xhb0cAuK2ncKjEYFEc5C7GF9ByYYailK+CcoSlzQ1x6IsLAwvwZDdrvdJ9wPHz7sV5FPSEgIyvftN89Rsr70J9RXr17Nhg0bePHFF4mOjqa2thbwCGzv9V155ZVkZmaydu1awGOjLiwsJC8vD4fDwSuvvML69et55JFHfMfduHEjycnJZGVlsXv3bm655RZWrFjBsmXLACgvL2fDhg186UtfIjExkV27dnHbbbdx3nnnMWtW8FpgVIW6zWajrKzM9/2hQ4coKioiISGBhIQEfvWrX3HZZZeRlpZGeXk5P/7xj5k4cSLLly8fxVlLRpvRsr8MhXVm2MQ6nN6CXQp0iWRI8OZwd7e69KygBhLqHR0dFBUVoaoqixYtCsoTrKqqz1+uKAo4ujD95to+RbrXhgOeVvOERUKritbZAaFWeVUFY14B6pEdCMNTqXa53L7Fjt5rtnbZsGomnFNmo5Tt8r0BcDpdqKp6/Euhpw1GrSjBmDgL9fBujFn5cEEranzvzqSKqw6ltQDii/qdrtV1CLvFBErfGelK1P8B1/W5PVQURSEyMpLIyEjGjx+PYRi0t7fT1NREXV0dBw4cICwszKfJ4uPjB/S3j7RQ13Wdzs7OfjuTesV1z8jFdevWsXLlSgAqKir85t3R0cENN9xAVVUVVquV/Px8nnzySb9UmZqaGtasWUNdXR3p6elceeWV3Hnnnb7tFouFt956iwcffJCOjg7Gjx/PZZddxs9//vOQrlERg8jxaWlp4V//+hfl5eX86Ec/IiEhgc8//5zU1FQyMzODPs67777LF77whV6fX3XVVTzyyCOsWLGCHTt20NLSQkZGBsuWLePuu+8mNTU16HO0tbURGxvL50Dfz1uS7kz6xjCfYAgWlA5WqAMnLbaHwuc+5GLdy+ko1gcj0u1t8N1YWltbg2+2chzv74xtrTlExfT/D46tzWBB7KFBnUciGUm6Z6N7hXNfFof9+/cjhGDq1KkAHD16lD179jB+/HgmT54ctBBzOp28/fbbXHjhhWiKgvb0r1EOFoFJBQwQLhTdBboDd2cHjo42TCYTYWEWUE0IIx2ltRWbS0cxhxMRGQNuAU2tqFXV4OrD+60oGPNmoB7xCGfPdTtRVBWzyYyiQCDlo+dMRz16EFd7CyaTGUMYCMM4fr9OiHZv1d0onIhxTgqm5I/6vxGKGde4BFRz/3GQdtM8OsLL+txuGAaHt6/hrGnD/Y+0B7fbTWtrq6/ibrPZevnbe9qePvvsM7KyskhJSRmROba0tJCVlUVjY2PQcYunGiFX1Hft2sXSpUuJjY3l8OHDXHvttSQkJLBp0yYqKir45z//GfSxlixZ0m/ep7cDlEQylIypFJeh5nSqrssqukQyJPRcMNqfSAdPRd3hcOB2u9m3bx/Hjh3jrLPOCll8eQW9YRhYXlqLtu2JQLPD7dYxdB2ryYSma2DvxIg7C3XvTgDCXS4URUHtbn1J0hCJ4xBRSdBsRy0theOVc+PsmaiHPfYT3dBxuzxVao9I76NNKaAd2oNIzsTh0jEbDkyYQDuePGMYGIbA5dLpSo1FXJREVHgJmq0cI3Eiqtq3wEa40BpiEen9C/Vwdzkdov+qesL414GREeomk4nExERfJLbT6fSJ9n379uFyuYiNjfUJ9+jo6BGvqHu7gPZnfTnVCflurlmzhpUrV1JaWuqXzfmlL32J9957b0gnJ5H0xck0PzpZTqYJkpchbYYUiFO5AdCpPHeJZIxhGAZOpxO32+0Ru0E0MFJVla6uLrZt24bdbmfx4sWDqpB6BZv27j/Q3l3Xa7sQAufxxawWi9lXnTWSCnwiHfpwvRg6Sn0V6qEi1JYDiOwojPmz0C8457hIP+7Dd7kxeQV+EO4Zpb4aoWoYcSeuV0FBVTVMJhOmc6YTeblKVPhhT6Xe2UVXeSVdDmu/UZRq5wGErf/cbpUmIh0T+h0TkbgLXTk48IUMAxaLhbS0NKZOncqiRYs4++yzSU5Opr29naKiIt5//306OztpamrCbrePSOMlu91OeHj4ib/j05CQr+zTTz/l0Ucf7fV5Zmamz6AvkYx1xkJVfVj86j05lSrsUpxLJENGz2z0YDuMCiFob2+nsbGR3Nxc8vLyBl0hVRSFlOrPCCt6rNc2rw1HVVVMFhPKcRVtJE5F3b2z1/i+quC+c9nbEWEq2v4PMNLG0aqrWI8eJMxi9ih9N90SF/uuqgOE21tQwi0YKeNQj1V5PlQV9BVnoSXuAmGApvkeLExGJ/b68ajJbaC4AtpkALSmavSIMBS1d3KI79wDVNUVwGVZj+a4q9/7MdwoikJERAQRERGMGzfO93PjjSusrq7GYrH4vO0JCQmedQdDjM1mIyIi4qSSasY6IQv1sLCwgN0+Dxw44Iv/kUhOd4ZK6I+IWAd/ETzWRLsU6BLJkBIoGz0YIeN2u9mzZw8NDQ1ER0czadKkk5qHevAzzvr0r2BSwCdYBW5dR3frmEwmNE3FW+oWsdmoJYcCGMj7F9YARv5s1NIdngeAqnKiVBVTcioiNQuldDfQtzgOhNLeArqOkZED40woczrR3EUBp6GqKlGuanR9HmrEDj+bjGe7gqKqqK4mlNbZ/S4s9VTV+/equ0xvYHF+D1UEv15vuFEUhZiYGFRVZcqUKURGRvr87ZWVlezdu5eoqCg/f/tQVMFtNlu/C0lPB0J+TL700kv59a9/7VuZrSgKFRUV/OQnP+Gyyy4b8glKTkP+PjSHOVn7y8laWIbCAgMjYIPpyWhbS1b3+JJIJEOKy+UKyeoCnnbpH330EU6nk0mTJvWZjR4sSk0ppr9eg2q4fdq2+wOE2ey1uhwX6RGJUN0Gzq6Ax+vPReEV6d5ceE3TPNGO7U2oZUWQnEp7YvBBFz6PTEw4YnE0zHGhuKsG3Eur24nQ8302GYvFcjxhRsXQPQtaXXVFODqs6LrR5zWFu8tA9BaxJ4a7cZn/L4TrGTm8b280TSMhIYGJEycyb948zjnnHCZMmOCL+Hz//ff5/PPPOXTIsxg/mE64gfBmqMuKejf+8Ic/cPnll5OSkkJnZyfnn38+tbW1LFy4kHvvvXc45iiRnPaMWGW9OyNZZZeCXCIZMUIR6EIIKioqOHDgALm5ueTm5nLs2LEBO5P2S0stpkeuQrEff/suwBAGLrcLVVGwmC1+cxNmK9giUNoqQz6VMWU26oHPPdnrx6MXe1p1lIZqorsc6FPmoDXWobQ29ntMgcC1bBaWyFK0rl2I+miM5AxU99EBZiNQamoRmTEoiufaFUVB62aTMQwDW30GSsY+3O7uaTIqiuoxAKk0B1FVfwGL82oUBo7JHEn6WkxqsVhISUnxrXXwetmbm5upqqrCMAy//PZg7Sx2uz2oqNBTmZCFemxsLG+++SYffvghO3fuxGazMWfOHJYuXToc85NIhpWTtbAMpdd9VMS6l/6EdCgiXgpyiWTUGSjVxYvL5aK4uJiWlhbmzp3ri7cbqDNpv9hbMT98JUpzzfHJeMSbrutoJg1Ttyo6AKqK0LJRa/eHfCpjcgFK6ec4u2WvB77u4x1XD+9BCbNiTJqFciCQDx6IisC2II2EsF2ge/ZTnO3QaEEkJKLo/Yt8xdWK0ToNJW5vwO2qqhIjDuEmFyyVGIZx3K9/wqakqgphxgE6wsJACRxBKRQbLvO/sbjGToKZNwI0mDUNVquVzMxMMjMzEUJgs9loamqisbGR8vJyTCaTn7+9r47zNpvttE58gZNoeLR48WIWL148lHORSELmZJofDRWnjVjvCym+JZJTimBEektLC0VFRURHR7N48WK/hX6DFurOLkyPXoNSUwp4KtMIfFaXQALOiJnpl/ASkAAWdWPSLCjdgdPl9CxINZmCsz84u1AP7kKfNBOlohTFccJqY0zIQCkURLcdAfwb+yhdjYjWdERMDIrRe51ed9TmveiRM9DMxYEHCAO1KRKRdqLaLsDnbffYYo7hrJ2Bmlzrq7j3vAku87OYXf+FErqLeVjw2ldCXXysKArR0dFER0eTnZ2Nruu0tbXR1NREdXU1+/btIzIy0ifa4+LifP72jo4O6VHvyc0338z//u//9vr8z3/+M7feeutQzElyJjBEPvWhYCi85kPlV4dR8KxLJJIzBiEEhw4d4tNPPyU7O5s5c+b0SuNQVTV0oe7qRHv1bghzY0ybjWvKTBozsmnNykWfPhNmzkJMm46YNg0xbRrGtBnouQtAMzBmnYVx1myMWbMxZhRgTJqKyBiPiIoGeqcqGrkzMMp24nI5MZlMHj/6QCK9R5cj9eBuREw8Rup4MJvQLylAnVWP4qjp+xAdNYiOBFDC+xzjO37tIYRI7Hu7vQSjc/KJY8PxBw4Ni8WMxRJGsrUBYWi43W4cTge6W/d1egUwlGrc2tiJxR6sUO+JpmnEx8eTl5dHYWEh5557Lrm5uQghKCsr4/3332f79u1s3ryZQ4cO9Wt9Wbt2LfPmzSM6OpqUlBRWrFhBSUlJv+fftGkThYWFxMXFERkZSUFBAevXr/cbU1dXx8qVK8nIyCAiIoKLLrqI0tJSvzFdXV2sXr2axMREoqKiuOyyy6ir6z9LPxAhV9Sfe+45XnrppV6fL1q0iN/85jc8+OCDIU9CIjkZxkJVfajxivUxV12XSCSnLE6nk927d2Oz2Zg3bx5xcXEBx2maFtrivoZyzBtvQKk/AHgq6IbbTdzx42guDbXb4lRhiUPpSkat7KPi7MUEIi0KZ0QCXbpGrDUSIUzoJZ8j3K4+q/TBojbVoE+eiH7eHLSuTwYKlvHs03YYwzIVVd3Xby674u7AaM5EiW/sc5zW2InIVEDpfWJFAYupmVhRiD2s3Be36Y21BFBUFZf+DyK6Fvj1tRkthkqo98RsNpOcnOxLFuzq6qK5uZm3336bp59+mo6ODr70pS/x/e9/n6985St++27ZsoXVq1czb9483G43d9xxB8uWLWPv3r19VuITEhL42c9+Rn5+PhaLhZdffplVq1aRkpLC8uXLEUKwYsUKzGYzL774IjExMdx///0sXbrU77i33XYb//nPf9i4cSOxsbHceOONfO1rX+PDDz8M6fpDFuqNjY3Exsb2+jwmJoaGhoZQDzdi5F0Odf8a7VlIxipDYV8Zjmz2MWmFkUgkY5pA1eWmpiZ27txJXFwcixYtwmw2B9jTg9f6IoQYuDnSvtfQXvwBitMOwtNkSDcMzCYTqqbhdDr9xgtrOlR3obSX9nHEHtfSZcPS0Ypm6Og5hRgln+KKiyc8PQecLqguB1dgH3dPfDHqACYz+sLpaO27oLwMPWc2mnPH8ZP2HNzjmhv2oWcUoOlF/Z5PbT2AHnUWmiWwtUd1VuK2zUCJ7vuBxeo6it2ioCgn1h6YzWYMcbxbqqWYou3PgmsKCQkJvawhI4lhGL6FzMNJeHg46enp/OhHP+LYsWO0tbVx9tlnBzzva6+95vf9448/TkpKCtu3b+e8884LePwlS5b4fX/LLbfwxBNP8MEHH7B8+XJKS0vZtm0bxcXFTJ8+HYBHHnmEtLQ0nn76aa655hpaW1t57LHH2LBhAxdccAEA69atY+rUqWzbto0FCxYEfb0h382JEyf2unCAV199ldzc3FAPJ5GcVgylBcaLtMJIJJLBIoSgvLyc7du3k5eXR0FBQb8iHfBLKOkP5cBbmJ67EcVpP9FlVAgsFouvgt5d6wpLPNS6UdqbQ7sGUxjtsTkY+z5FUxSinO2YjuxGrdkPYSrGlJkY4ycGf7yscYgFqWhtRZ7mRYB2aAeGMhOU4ASudrQI3dx/p1EArWY/QvTdY0ZrqUcEiGL0onIUq3PCiQ+O31D1eJqM2Wxm1sIS8vLyEEJQWlrqiz48fPgwbW1tI9IhFPpOfBlO7HY72dnZ3HrrrVxyySUDjm9tbQXwLZweCCEEmzdvpqSkxCfsHQ5PJn/3txiqqhIWFsYHH3wAwPbt23G5XH5BK/n5+WRlZbF169bgLu44IT9yrVmzhhtvvJH6+nrfU8LmzZv5wx/+MOZtL5O+AaVPj/YsJD7+DlwzNIcaCvvLUFXEZWV9dJl8xS70Nhvl3x3tmUgko4vD4WDXrl10dnYyf/58YmJigtrPK9R1Xe8zT1058jHmjavB0DF0HZfbjXZ8USfdq/Beb7gaBu0xKC1HQroGYbLQaU4gqq4ck8ncez4uB+rh3Z6xaWmIuDSUinIUe3uASYOxaDZqZzG0O3ttVqt2Y6RMwk05Zgb26GtHD2BkZKG6KvoeZDgQzfEoCfUBNyuuOmifBTF9F2SsriY6faEn/mV+IaI4qkBscjxTjltD7HY7zc3NNDU1ceTIEVRV9S3ETEhIGDabzGgJ9WBTXwzD4NZbb2Xx4sXMmNH/Q1ZrayuZmZk4HA40TePhhx/mwgsvBE4I7ttvv51HH32UyMhIHnjgAaqqqqip8axxqK2txWKx9LKXpaamUltbG9I1hizUv/vd7+JwOLj33nu5++67AZgwYQKPPPIIV155ZaiHG3GkWJf0x3CI7KFC+tYHRr59kEg8FomGhgZ27dpFYmIis2fPDskK4RVbfS0oVWqKMT1zDbgdni6jurfLaGBRLxQVQ+SEHMEoVI02SxLhdYd8eeT9oTTXojTXIixWjKmzUSoPotg8FVRXZCTKgmwsbTsQeCw63mtVPb4Sz/fHSnFpcYSludDo6H+ChhOloQOREI+i9/2WQG09gBE9A7WPFBitpRI9yoKi9n54ANA4TJjzLOzaIQBq3Ev5WF/AZyKPj8QE3GhcpcCtxwvnERERREREkJmZiWEYtLe309jYyNGjRykpKSEiIsLPJnOyza28jIZQ9zY8CobVq1dTXFzsq3r3R3R0NEVFRdhsNjZv3syaNWvIzc1lyZIlmM1mNm3axNVXX01CQgKaprF06VIuvvjiYXl7MSgT0/e//32+//3vU19fj9VqPe0zLCWnBmNpUelwCn5ZXe+NFOgSyQna2trYsWMHU6dOJTMzM+SujV5RHEioK/WlmJ68ErraPfnlQmAxm1H6EWhdYjJRh0MT6QYKzWEpxNQfRjWZQkqhUZydKAd3gNmCMbUANDdwAFNrKQLFsxjzuOdbd7txC4GiqqjHmw9Znccw2rJRE0wo7tb+z9XViGHPRQlrg36q8ErtYcS4WBSl9/EUdzO0nQVxfcdURjg76bAqvNm6it9E9H4VvUkxuF4IrD0q7qqqEhsbS2xsLLm5ubhcLl+1vaSkBIfDQVxcnE+4n0yXz9EQ6jabLah4xhtvvJGXX36Z9957j3Hjxg04XlVVJk702KkKCgrYt28fa9eu9fnX586dS1FREa2trTidTpKTk5k/fz6FhYUApKWl4XQ6aWlp8auq19XVkZaWFtI1ntRqA+8K3FMNWVWX9MdYtsB4kdV1D1KgSyS9iYmJ4dxzzz0pi0PAiMamI5jWfxvR0YjL5fLECZrN/Qo7u2kqkQf3QwgVfV3XaYwcR0JjJSazGcMQBBXJ0hOXE6JAaTlEZ0Qq4XolutuBpqpo3eYjvAszfY2HBDRV4NQzMCfGoRot/Z5GbTmInn4WmtG30FbcNoy2GSixgYW/1noQPcaKonYCoBONk2R0wuhS4mhXEnm29Ub+bjmXQCsM2hH8WzH4b9F/ddxsNvs6hAohfB1Cm5qaOHz4MKqq+kR7f42GAjFa1pfo6Og+twshuOmmm3j++ed59913ycnJGdR5DMPwedO74w1XKS0t5bPPPvM5TebOnYvZbGbz5s1cdtllAJSUlFBRUcHChQtDOnfId7Suro7vfOc7ZGRk+F51df86VZj0jdGegQQY8jz16W+XD8lxhmpR6HAsLu3O5Ct2nZFi9VS97uHK9LXZbNx4442MGzcOq9XKtGnT+Mtf/uLbfvjwYV9iRM+vjRs3+sYF2v7MM88M7U2QDDuKopy0D7lnRKPSWIr27l10xMRRn5CFO3cW2tR5iEmzMSYWBPzSx5+DoijY86ZiTC3AyD8LY9J0jKxJiJQMRFSMv58dgdvtoik6m6SWquN2Hc/2kB0FZjNGwSzUuiIUh42Y2jI6bBEYcfmYTD2aGSkKqqZhMpuxhFng+M++2nKU9ioXdlc4utuN6GdxrVazE908rd8pqU3FGHp+wG2K3o7SOgWANmayOuIhvh71e74VdQ9XR/6QWyNWUWLJ7i8RkqcV3dNkKkgURSEiIoJx48Yxa9Yszj33XGbOnInVaqW6upoPP/yQjz/+mNLSUhobGwd8qzFa1pf+ctRXr17Nk08+yYYNG4iOjqa2tpba2lo6Ozt9Y6688kpuv/123/dr167lzTff5ODBg+zbt48//OEPrF+/nm9/+9u+MRs3buTdd9/l4MGDvPjii1x44YWsWLGCZcuWAR4Bf/XVV7NmzRreeecdtm/fzqpVq1i4cGFIiS8wiIr6ypUrqaio4M477yQ9PX3Qr0jGArKyLhkJRsL3fiZV2E9Fge5lODJ9wbPI/+233+bJJ59kwoQJvPHGG9xwww1kZGRw6aWXMn78eN8iJy9//etf+f3vf8/FF1/s9/m6deu46KKLfN/3lbUtOb3pbn1R97+A9vYduDtbMRuCZLMZtUOlLwu30KwIkYd2+AMi3G5AoLYFqAObgUQzIjoZ3RJNm82ByxlOotuOarKAMYjuqIBISIa0CNSaXd386IIoVxvaUTvGuKngrkPpauzzGKqqoppUYg0bzrZEnHEKmrsVBKiq4rHKqKqfBlJrjyBSUlH03k1tHHFTcEbEIoQFI6oQs96JZnShCieqcIFwIzoaqYj7Cj+N+jadAdJn6q0OMtrsHDMFXhR8GMGHCM7pV873jaqqxMXFERcX18sms3//fpxOZ782GV3XR1SoCyHo6Ojot6L+yCOPAL0jF9etW8fKlSsBqKio8Jt3R0cHN9xwA1VVVVitVvLz83nyySe54ooT/47X1NSwZs0a6urqSE9P58orr+TOO+/0O8cDDzyAqqpcdtllOBwOli9fzsMPPxzydSoiROd7dHQ077//PgUFBSGfbDRoa2sjNjaW1sshJsDvCSnUezPibxuGKPnFy1D61IdSYI/kItXTUbCHItD1NhvlsYtpbW0NOunCi/d3xrbWHKJi+v9Hx9ZmsCD20KDOA1BfX09KSgpbtmzpM9M3EHPmzOGSSy7xvWadMWMGV1xxhd8/FHPnzuXiiy/mnnvuCXiM2bNnM2fOHB577DHfZ4qi8Pzzz7NixYqQr0UytnA6nSe1sO2jjz4iLzeHjP2PoBQ9cdzqomAy9W91EWEp0GhCaToKgNvtRiAwm/qOhDQMg07DhG5KJ7q5CgUFNBMicRwiIg53px3XkQNEBqEBjbwpKO5qlC4bQghfcyAQmEwmVFU7Ps8I9MwctKbeCzydTufxsSdOaMRlosS0gqsdwzAwhIE4nhvuFe2qoiJislAia0GcWBjanH0On8/C52EQRgEfqIHFZbSeyzta4OhAt66T3B7Gx2F9R2EvECqPiP7jNwdDT5tMc3NzL5tMY2MjdXV1zJ49e8jP39ecJkyYwOuvv868efNG5JyjQciPPuPHjx+xTM6RQFpgxgBj1P4y1Ay3DaY7p3LVuTtei8tYv562tja/r0BexkAMRaYveDpDv/TSS1RXVyOE4J133uHAgQO+17A92b59O0VFRVx99dW9tq1evZqkpCTOPvts/vGPf5xWv+8lwaOpKjHb7oEdj+NyuXyZ3f2KdHMc1Cs+kQ6caB4UeA90XadNjcWkxxDjFekAuhvl2GHUw0WYavejaW5E9kSMyQWIxMCL8YxZBagdB1C6bBjCwOlyoqgKZouZXt2LHB1o5cUYkVMRYfF+mwJdodpSjehIQtEi0Eyee2GxhKFpnsq3261TH5lGs1mlIf4sWlNmY0ubQ+XMZXxegJ/aUtRdjDMCyy+7VkGc6Nti0xjpIFlx97l9m2JQTghdZYMkkE1mxowZfjaZgwcP0tnZGZRNZqgYyKN+OhCy9eXBBx/kpz/9KY8++igTJkwYhimNPNICcwL54OLPUNtWRjL+sbu4PZUq7GNFlG/ia4TR/0IqBw7gD4wfP97v87vuuotf/vKX/e47VJm+AH/605+47rrrGDdunK8S+Le//a3PKv1jjz3G1KlTWbRokd/nv/71r7nggguIiIjw2WdsNhs333xzv/OTnH7kHHoMa/UruIXAbDYPaGkQWgS0xaC0+GeK96XTvZYUuymeqE6BqauFvlqBKoBi6Cg1Zb4RYvwEhDUOpfogirMTY3o+ak0R4LFguN1uTCbv2rnjPvcAx1ar9yHCo9HTp6E17+33GtXGwxgpk1DNRwAnKKBqKqopgrbz8xG5ZTiNNgyjjgOtBbTG6KhqG6qhoqhqt6szmEQp1Uzs5SnXcTNHNPO2khhwDoYCM7VW3nYH3g7wlGLwCzG8FhRvNnt8fLzPJlNaWkpLSwv79+/H5XIRGxtLYmIiCQkJREZGDrlV2uVy4XA4TvvkwZCF+hVXXIHdbicvL4+IiIheHc6ampqGbHIjiRTrpxdDGdV4Kot1Lz3F71gU7mNFoA+GyspKP+tLMEkJQ5XpCx6hvm3bNl566SWys7N57733WL16NRkZGX6d8QA6OzvZsGFDLz8l4PfZ7Nmz6ejo4Pe//70U6qcgiqIM+m2I/tadJFf9BwFYLJaBBZZiAkcmSn1poI3Qo8LrtaQ4w+KJdppRu4LpVOp/LUrdYc9DQFwKxpTJ4GqD4+Jf142gHi58x+pqRzu0F31CAVprMRA4zxw8OetG+lRU8yGEJQIjIpa288y4k8tRUI4Ha8DExHJK3TOx0YFb1xFuN6qieHztqopbPcocPYvtWm+bik2tIFHE06gEnv8xczPR7nja+zBFvKLo3Cw04gbpVR8MZrOZiIgIhBBMmzYNu93us8kcOnQITdN8Fpn4+PiQ0mT6wmazAUih3pOx3n1UcooyhF1KTwVGu7HSWKi2n8rCvCcxMTEhedSHMtO3s7OTO+64g+eff97XQnvWrFkUFRXxP//zP72E+r/+9S/sdntQDermz5/P3XffjcPhGJJ/WCVjH/srP8W655+e1JMeiyUDo2CIyahH+65Gd5fYnghEF4Y1nkg9EsV2LIhZ+erodK+6Gxm5KK5m1IOfIYSg3ZqIMzqS+K5q1J72kSA0q3a4CCMpG4e5kQjRdnw/FSNrHCI9DiUOMNtQlBqcsVNozTsISkPgGSudTNSOsUeNR2AghDjubRcYLhcKYOETIvWF2Cyq3/QMdAqMRjZrPSKwj99IJwZzTa286/a37HhxABsVnWvFSSVwh4w39UVRFCIjI4mMjGT8+PEYhkFraytNTU1UVlayd+9eoqKifMI9NjZ2UKmBHR2e1czB5KifyoT8t3jVVVcNxzzGBLKqLumL0RbWpxunk0gPheHI9HW5XL5M6+70jNfz8thjj3HppZcG1QejqKhoyKpfkrGNYRg0v/ADEsqfxWw2oetB+JwFGOaZqAf7+e9ZOTHYrevobh01Ih4L8Sgt1YOf76SzUGv3gO7GEB7xH+6uI6rLBFEJGCnZqLXFoPft5w6E2nAEk6HRWTgXa74TxXQE1agAKryXAQIszS1EV8ylPftA38dSDzPJSOWA2uVrIuWVox7R7mJyWxnbmOB7MPJ2Sm3XKkkWidT3UVVvMTUT5o7F0UdV/VnF4CohsIxgVd0wjICCu7tNJi8vD6fT6UuT2bdvHy6Xyy9NJlibjN1uJyIi4pSKBh8Mg3rcKi8vZ926dZSXl/PHP/6RlJQUXn31VbKyspg+ffpQz1EikUhOC1avXs2GDRt48cUXfZm+4MnctVqtgCfTNzMzk7Vr1wKeTN/CwkLy8vJwOBy88sorrF+/3hc7FhMTw/nnn8+PfvQjrFYr2dnZbNmyhX/+85/cf//9fucvKyvjvffe45VXXuk1t3//+9/U1dWxYMECwsPDefPNN7nvvvv44Q9/OJy3RDJMhOIH7uzsZOfnn2GNKiTq8stRTVBx8ACq7mR8ZhroTtAdoLtAd6LoDtCdCD0M5VgdesIkFKcdnHboakext0Bnm+d/DR0EuFweQW2KiEPVklDqKgaaVreL8fyPt55u5M9GrdgBnPCja5qGyXTcj25rRrE1I6ITEWnjUWt2nzjAwDeOjmnjide3I2xzUGPsfQ4NP7Ydw1xIR0bfvRDC1Y9JNc6jTvVvdKSqKioQFV/HTPdE9qkn3jZ4t09xVnPMOt4/av74n+2Km7O1dt7XYwOetxHBq4rB/xugAdJQEmyOusViITU1ldTUVIQQfjaZgwcPYjKZ/NJkLBZLwOPYbDYiIiJO6ZjwYAhZqG/ZsoWLL76YxYsX895773HvvfeSkpLCzp07eeyxx/jXv/41HPOUSCSSU57hyvR95plnuP322/nWt75FU1MT2dnZ3HvvvXzve9/zO88//vEPxo0bFzANxmw289BDD3HbbbchhGDixIncf//9XHvttUN09ZKxSH19Pbt27SItLY38BYvQNA0BdHYm43K5yJxycsW3qtK9HN65jZQwwcSkSIS9A3FwN1hjofYgSlcfYeyB0CwYeVOOi3SB262j6zpm84nYxe4o7Y0o7Y2I2BQ6wsOJaT/U7+FFdAxiVgYxrbsBDa2yCCNhEkpaHYrSFnCfiOrtGObZdCYH8ud7SFV20Cam0al0Bdyeoe3hiDILh6p6CvbHbTLtpmqi2mNotkagqioCgSJOiNIuczOaHoPeR9X8SUUfcaFuCqEDLXBSNpmOjo7T3vYCgxDqP/3pT7nnnntYs2aNXyTOBRdcwJ///OchnZxEIpGcTgSzuO/dd9/1+/6ee+7pMwvdS1paGuvWrRvw2Pfddx/33XdfwG0XXXSRX6MjyemNYRiUlZVx5MgRpk+fTkZGht92TdPo6gosLIOltraWvYeqUOOymPTFL6IoCgZgfLHboJY6lMO7UQ/tRDm8E+XQLpSO1l7HcpmtmMaNR6sqRghPB1MhBBaLGaUPe4gXpfUYUS4nruQclAgLamM3wa6oGFOmQCKonaUo9v10DxZUm0oRnckY2VmoWqC3AIKoI7vQzVNxxh3uYwLt5BmNFCtRBCrr60oLhUYbH6rRnoSb451S0WC+2sGbarTHKnPcyibcAlVRaVGdzNNsbNMDxxOWIfgIg0WhJ3EPiqHoTBrIJuOttu/duxe3201cXBxms5n9+/f3W1Ffu3YtmzZtYv/+/VitVhYtWsRvf/tbpkyZ0uf5N23axH333UdZWRkul4tJkybxgx/8gO985zu+MTabjZ/+9Ke88MILNDY2kpOTw8033+xXGFmyZAlbtmzxO/b111/v1zE6WEIW6rt372bDhg29Pk9JSaGhIfCiColEIpFIJGMDh8PBzp07cTgcLFy4MGBqRvfOpKFiGAalpaVUVlaSl5dHZWVl3/aEuFREQSp6wYlFz0pVCcre91H3fYha8jGER+DWHajHyhF4EmMURcFsDiKRphvmxgrUVg0jexbY6zByUlDD61Ad+6BvhwtKZz3KAQt67gy0sN4NkhBuYsrLackfhzuypvd2QFXLmKgvokwL/AZBVXeRaZxDteov5NtMNUwwUqk0mXC5PX57RVHQDR237sbmqEBnMoqq9YiA9PBPRWfRMEc1ehkKod4Ti8VCWloaaWlpvk6kTU1NvPnmm9xxxx2oqsqqVau4/PLLfYvpvYxWJ2gv1157Lb/+9a9930dERAzqHoQs1OPi4qipqem1CGrHjh1kZmYOahISiUQikUiGjr4EbFNTEzt37iQhIYE5c+b0aVUYrFB3Op0UFRXhdDpZsGABuq5z+PDhkI4hxk1BjJuCsewacLtQDn5Gw3N/IqJpD6K13t+PHjTHE90FKPZ6RGoYhIHiqA9ud8OJVlaMPq4ALXYnveIiDTtxBxponhaPHhY4bjJC20aycQ71au83BmAwmTKO9spWF0yhlko8+kpRFEyaBl6LkslgRkszO7U4BPgiIL3pKx8rBqXCYNIIVNWHQ6h3R1EUoqKiiIqK4uqrr8YwDNavX09qaiq7du3qJdRfe+01v+8ff/xxUlJS2L59e589JnraEm+55RaeeOIJPvjgA59Q/+ijj7jqqqt8Y6+77joeffRRPvnkEz+hHhERQVpa4OZcoRDyHf3617/OT37yE2praz2vsQyDDz/8kB/+8IdBxX1JJBKJRCIZWYQQHDx4kO3bt5OXl8esWbP69RMPRqi3trby0UcfYTabWbBgAVFRUaiqGjB9KGhMZoxJC9g35yre+OJvaFr5F5QlVyEiAi+iHAgjbwrEtKG0HkE7vAujczxGWFbQ+2tVRRh1UxCid3VUcTcRV6KjuPryTRukKbsJF4FTlNzqUebqvbsat6g15Bq902sUPB1kE+IcWCwWLMez4w3DwOly4XQ6cbvd/LXLhtsdWvrNYNB1fViFek+cTifjxo3jN7/5DbfffvuA40e6E/RTTz1FUlISM2bM4Pbbb8du7+e1TT+EXFG/7777WL16NePHj0fXdaZNm4au63zzm9/k5z//+aAmIZFIJBKJZHhwuVzs3r2btrY2zj77bGJjBxa5qqqGJNSrqqrYt28fEydOZMKECb6Kfl8xocHidrspLvb40medVUBiejo6l6J/7U7UoldRtz6LWvYxDLD+w22NRJ84gaiuUjA8STGGEKgNB1GbTejjz0ITB8DoHHBOasN+RGcaRlYsqupvdVEd1cQfmEjTVCeorl77KkozeUY7e5TASSYR2g7ixUKaFf97lksNJaQH3Kde7WSW0skurMcbLnmq7eK4r/11TWHxx9vIskaQkJBAYmIiUVFRQ56WMtwV9Z7Y7fagmx2NdCfob37zm2RnZ5ORkcGuXbv4yU9+QklJCZs2bQr5OkMW6haLhb/97W/ceeedFBcXY7PZmD17NpMmTQr55BLJmYzMZpdIJMOFV4S1trZSVFREVFQUixYt6jPqrifBCmzDMNi7dy91dXXMmTOHxET/1vaqqiKEQAgRsjC02+3s2LEDk8mEyWTy9xWbwzDmrcCYtwLqD6O9/yTq1mdRumw9LwRjxiyUpt2Et+9FaJonAlGAqnmqz7rbAeWf4opIREnLRaXvuEUvSkctlEVi5OSjmvf7n9JeRlzpDFomV4DS+wFCU/eRayzmoGrrtU3g5CxRxbuK/+LeFrWOnI5oDkcEXjgaZ24C5wn7sQIoxy0wmODA/LnMq2uisbGRI0eO+HUK7S8CMRRGWqiHkvoy0p2gr7vuOt/xZs6cSXp6Ol/84hcpLy8nLy+0rumDbluVlZVFVlbwr4skkpFm+tvl7LkgtP8gRpqxINb7aj40VB1Lz9TmRhLJaCKEoLKykv3795Obm0tubm5IQjkY60tnZydFRUWAxw7g7QXQHa9w66sZTl80NjZSVFREeno6+fn5bNmype8Hh+QJ6F/7OfrFt6BufQZtyxMoTdUYEyaiRNpRW3ag6Z7qtsvpRFFUTBaT7zq98zO6mjEONtISM4HIqGOEaY5+u7Mqrg6U0gPo2QVokUV+28xtxcQenE1rXlnAfaPUbSQbiwP61XW1nFl6Krt63K9xVHOY/IDHq9U6yFcd7DcC22pesKhcn5lBZmamXwRiRUUFe/fuJSYmxldtj46OHpTgHmmhbrPZgqqoj2YnaC/z588HPL0shkWor1mzhrvvvpvIyEjWrFnT79ieDTZONWR30tOLoRTrwyWqx4JYD4QU2BLJqUtjYyOlpaUBq9zBMJBQb2xsZOfOnaSkpDB16tQ+RbhXuOm6HpRQF0JQUVHBgQMHyM/PZ/z48YDnDcGA8abWaIwLrsVY8l2UvW9h+uxBlIajvuMahkAzaZ7FmPgvB/UuwASIaz+C7oihPTGNCHc5dO8a2lOICgPtcBFG6gzUpAOA07fJ0rSDaPNc2rMCdS/VSVd20S6m0BUgXz1e3UGMmEdbt4p8p7WdfIeNsj78+WmmRvY7MwJu6wQ2KDrfF6ZeEYgOh8MXgbhr1y6EEL5Ke2JiYtCdiUejop6UlNTn9rHQCdqL94E2PT2wfak/ghLqO3bs8HXL2rFjR8gnOdWQYn2U+DtwzWhPon/ONLEukUhOTZKSkjj33HMxm82D2r8voS6E4PDhw5SVlfkJ6b7oXlEfCMMw2LNnD/X19RQWFhIfH+93nKC97qqGmLEc1/RlKKVv4Hr392jH9qCq2okFtAOIfovbRnhDJ3rabIRyBPRW34JMpUeyCoB6bA/ucfNpT7WiGF2Et9YS3naI8LrtGKY+upcqLUw0GtmjRPVIegFD6WSOUcO7in9qSIpaTRmBhfpRzdZvVf1pxeBKIYjskZYTFhZGeno66enpCCFob2+nsbGRo0ePUlJSQkREBImJiSQkJBAXF9enGB9rHvXR6gRdXl7Ohg0b+NKXvkRiYiK7du3itttu47zzzmPWrNDfVAcl1N95552Afz6dkWL99GGoLTBSrEskkrGOJ2d8cCIdTgj17t5y78LOlpYW5s2bR1xc3IDH8YrZgUR2V1cXO3bsQAjBokWLCA8P73WcUBelGkKwzzWOuol3kJ1VyvjD/4fZdhDEcVnsFev9WIK02r2IsBiMzAIsXcW+rqEeb7vbU+m3hCMKcgnTthHXFEVDxjQa0lxoxgysHYnEHKvDWj+pV/dSh0igifFM1Dsp1XovYtXVUqbrqezRTsyv09zOPL2TT7XeNiOAVFMD+52Bo7LbEfyfYrCqn26liqIQExNDTEwMOTk5uFwuv4ZDuq4THx/vq7h3zwYfjYp6f0J9tDpBWywW3nrrLR588EE6OjoYP348l1122aADV0L2qH/3u9/lj3/8o19XUu/F3XTTTfzjH/8Y1ETGIlKsS/piOMU6IAW7RCIZVbp7tzVNo6Ojgx07dmCxWFi4cGHQdggYWGS3tLSwY8cOEhMTmT59ekCLTFDWl25489xdLhcLFy7k0KE0DuUsIZ+DaB/ej9JY6hHoQvhX14+L9u5nUhxtaAeLcecVoowXEKGjagZCF7gcbgxzA2axF6cTVKWZhCPbsCQuoD79KLboFmzRYHJHgutcws2foOHAJnJ5lwtoU+2kGlGM0xtxaCf87KpIYo9xPtOVIqJEJjbFkwGPAuHqIcxMo3emDNRoHUxTu9hrhAfYCk8pOt8UKmFBZtCbzWZSU1NJTU31NRxqbGykvr6e0tJSwsPDfdX2kY5nHGgx6Wh1gh4/fnyvrqQnQ8h39IknnqCzs/eTX2dnJ//85z+HZFJjiUnfGO0ZnGH8fXgOO/3t8uE58DDhFewSiUQyGE42eq+7t/zYsWNs3bqVpKQkCgsLQxLp3mP1JdSrqqr49NNPycnJYebMmf163YOtqNtsNrZt24bJZGL+/PlYrVaf0HflXYj9W//Gufz3iNjxHmHe7cubUAP4CXgjIw/NXIJaux/FpaNpuzBZdmON3kdkeD0WiwWz2YyiqhiGjrXufeJ2gdGpIYSB21SH27yXvfrlFOvf4g3Op03x5GrXqTaKtCga3RejikgUI5v1/BdvaOP4s/olzPpENEx4lXqnYmeB3tbn9SeZGvvc1ojgeWVwcZnehkPZ2dnMnj2bc889l0mTJiGE4MCBAxiGQUlJCRUVFdhstpAerAaDzWbrVTQ+HQm6ot7W1ub7AW5vb/d7LaXrOq+88gopKSnDMsnRRlbWJYEYbquKrK5LJJLRwiuYy8vLqaqqYubMmYPushgok90r6o4ePcrs2bP7XRQIwVfU6+vr2blzJ1lZWUyaNMnvgaWjowOHw0FYWBjG9K/hyP8K2q4NmD/+M9ibPELe5UJVVLTjDypCNaHn5KMp+1BcOiigHNqNET8ZJa0ZRTvR2VRRFF+OOUKQICqILI2hMiEdV0orquoiU3mVA2IZXYp/YyMdF01aMx+Ib3NMNWPHc/9dqGw2RZN1bBnxYiske0S4Wz1MjJhJW4AHslqtgxlqF8XHq+phAlSh0Kl67t/jis5lQsUcUmfX3phMJpKSkkhKSsIwDN59910SEhJobm7m4MGDmM1m34LU+Pj4k7Ji9UQIgd1u97PenK4ELdTj4uJQFAVFUZg8eXKv7Yqi8Ktf/WpIJzeWOBPE+un+9mA44hpHwlcuvesSiWQwhGoX6Y43QOLYsWMsWLDgpCqXPRMxvLYUp9PJwoULgxJbA1XUhRAcOXKE0tJSpk+fTkZGhu9zIQTx8fE0NjbywQcfEBMTQ3JyMklJSUQVXIk+/TKcW/6Iecc6LJqGMm4SRlIsCs0oXVWYRPFxL4zweWLUphJEqxV93Flo0buhZ5VaUVAVBatqY3JbOS1iNnVpNRiiixz3f2i3LaEmOsKzKPW42HYo7cwUpbxG74Y8dcnH+OCj5UxrrOesKZ/RqbVSaDTytuJ5wEmyWwlrjODYuGZcikGCqRGcmSS6FPRbo6jeZiYqzcBkFVTVq/zfaiffunzoupV6f87GjRuH2WxG13VaW1tpbGzk0KFD7Nmzp1cE5Mm+9eno6JAV9e688847CCG44IILeO655/xasFosFl8HptOZM0GsjwlOgfSX7oyUWAdZXZdIJMNPW1sbO3bsQFEUZs6cedJiqLvIbm9v5/PPPycmJoY5c+acSGEZgP4eOrxNl44dO+a3yFUI4VsQm5iYSHJyMl1dXTQ0NNDQ0MChQ4cwmUxYrVZalflM/+qXGd/1GtqRf0BnDxGr+P4fxw+OoneiHSlCj8qCTBXNcqSP2RvEtW8nypnH0XHhOK0tzDVv5XP7OVSGmfyaE3WodSw3onlZneB3BIdikD9tP+/vnM/WxslcPnE31pQi0kUCojWW9+7Jp6NNIzrexdzljWjTWpnvcrPrlkQa9nuq87baE27nhx+z8NVL3EQEXpMaMt6/X69lqntDJfAsFm5q8jRc8i7g9Ir2wTZcCqXh0amMIkJ83D5y5Ajjx48f0QUDJ0NbWxuxsbG0Xg4xQ/TW5XQV62Oqoj6MQn24miCNlIiWYn1g9DYb5bGLaW1tJSYmJqR9vb8z8lo/RIvpv5nGyZxHIhlunE5nyBX16upq9u7dS25uLhUVFRQUFPjFJA6Gjz76iLy8PIQQ7N69m5ycHPLy8kKqqG7fvp3k5ORejRadTic7duzA7XYzZ84cX+yeN53Fu8Ax0Ll0XWf37t00NjZiNptxuVzEx8eTHmUns/FxLPVBptwJQFFwp85ESyxFUex9JskINYLWxLNoSKpEUcIo0b9IiYovScabsuPumsZHUeNRlBNay+VykdqQwpsHpgIQpuksTarjjT+n4XL21mTZ8QZHXlahjx+BW77nZPXVgZakho7D4eDDDz9kyZIlA+pDwzBoa2ujsbGRpqYm2tvbiY6O9gn3mJiYAY8hhCApKYni4uKALo/TiZBTX7KzswFPfmVFRQVOp9Nv+2AyIk81ZGX91Ga4OpaOlEWl+0JTKdoDcxmb+N1oT0IiGWVCsb4YhsH+/fupqamhoKCA5ORkjh49OmB30mDnUV1dTWNjI7NmzSI1NTXkYwSyvthsNrZv305MTAxz5871Vee9lXRvXGAgke52u9m9ezednZ0sXLgQq9WK3W6noaGBow2CPR1fJy1mMVO6/o+orv0o/QlHBUBgqtuFaI7HnZGHKWL3iQJ8t/Mrhp24+q1EtU+iNiOcyeFvEK4vZbemgaYhBBjCQAnfx9RGg10xmccz2xVA0JDayFxbE9uPJuDQNf5Tl8GUWQYln/We1pFmlZlLdHa/E3iB7mNPWvjGZS4S4vq+tGAxDMOXLz8QqqoSFxdHXFwceXl5OJ1OX7V99+7dPquSt9reM6oTPA9oLpcrqM6kpzohC/X6+npWrVrFq6++GnD7UPxHfSpwuon1MVVNh1PO/uJlpP3k0hJzgu4PMI5+xkkkEn+6urooKipC13U/z/hA3UmDwe12Y7fb6ezsPCmve8+HDu+i0ezsbCZOnOgT497KdH8i3ZvZbrFYmDdvnm+RY2RkJJGRkWRnZ+N2u2lsbORAw9lQ/Tq5Hc8SbdSe6E7ax8sAxdmM6XAzRnQOIh00y+HezZUUBVNXKeMOmWlLmgdJbxGuL+FTLQxFAe34YtZxSYcId8SxXYn2WXh03Y01ax9JTXNo6PK8PWiZpmDZDc4Av/iqLSoWKzh7h/Vhs8Ej/7DwszXO3htD5GQy1C0WC2lpaaSlpfkCS5qamqipqfE1XPJW22NjY9E0DZvNBnBGCPWQ7+qtt95KS0sLH3/8MVarlddee40nnniCSZMm8dJLLw3HHMcsY07cSoJmOOMaRyNa8QqePWMjHc/ka5dITpbm5ma2bt1KREQECxYs8FvYebJCvaOjg61btwKQk5NzUl53b0Xd2xm1qKiIadOm+ZJdultdhBB9ivTW1lY+/vhjYmNjmT17dp9JJCaTidTUVKZPn860C2/DdcFr1Gb9GLsSh9PpwOVy+c4VcL7th9EOHEYcm4GujkMo2onK+vHsdl21YAmvIbPLQY5eyULdX00LDJLDipitODGbLccDPVQ6NDeT8z5BuOy43W5qXIL8CwMvDG3qUJh+Qd9/hxv+Zabq6Mkt6oSha3bkbbg0YcIE5s6dyznnnENOTg5ut5t9+/bx/vvvs337dv73f/+X+Ph4n9WpJ2vXrmXevHlER0eTkpLCihUrKCkJ0B22G5s2baKwsJC4uDgiIyMpKChg/fr1fmNsNhs33ngj48aNw2q1Mm3aNP7yl7/4jenq6mL16tUkJiYSFRXFZZddRl1d3aDvSch39e233+b++++nsLAQVVXJzs7m29/+Nr/73e98LVjPJKRYP3U53cS697xnimg9k65VIhkM/XnAvSkpn332Gbm5uQEzzAfTDdRLfX09W7duJSUlhfj4+JNO+PB2N92zZw+HDh1i3rx5fskuuq77Hiq8CXU9qaurY/v27WRnZzN16tSghaWiKMTExpM0bzWmr2zDOOsXEJbki3N0Op243e6A90pYzWjt9RiWApwZ+TgzC3BHT0QPT8U1LhrFdBCVoyTobzHN8THLHDYs4sTcDXTS1E+ZanhEvKqqmExmHElmLp5bBgq4dZ0d4W5iEm0BHx722jUSUgM/ULhc8OBfQl/I2ZPh6kpqNptJSUlh6tSpLFq0iMLCQhRF4Z133qGlpYX8/Hx++MMf9tpvy5YtrF69mm3btvHmm2/icrlYtmwZHR0dfZ4rISGBn/3sZ2zdupVdu3axatUqVq1axeuvv+4bs2bNGl577TWefPJJ9u3bx6233sqNN97oV6i+7bbb+Pe//83GjRvZsmULR48e5Wtf+9qg70HId7Wjo8OXlx4fH099vSdDdObMmXz++eeDnsipzKku1sfs/Iep+dFIMZoi8nQVsd7rOh2vTSIZKbyLKA8ePEhhYSHZ2dkBha2mabjdoUX4CSE4ePCgr+I9ZcqUXvGMg0EIQXV1NW1tbSxcuLBXskt3j3TPaxFC+CICZ8yYwYQJEwb/4KCFweTr0C/6AGbejiUyGbPJk9yiu904Hd5qu4EreyYqO0A40Ro/x1J6GK1JxUg4hp5Rj6rVohz/P1AwK/vJNZ7iCvt2JrgbfWtAdVxkKZ+RbW/1m0p9vI2vzKzGYjajWsKI/4KGIQzPw4PLiVv3PDw4XJC5sO+1Ci+/bmLP/pMT2SPRldTbcGnOnDn84Q9/ICkpiT/+8Y/k5ub2Gvvaa6+xcuVKpk+fzllnncXjjz9ORUUF27dv7/P4S5Ys4atf/SpTp04lLy+PW265hVmzZvHBBx/4xnz00UdcddVVLFmyhAkTJnDddddx1lln8cknnwCeNzaPPfYY999/PxdccAFz585l3bp1fPTRR2zbtm1Q1x3yXZ0yZYrv9cFZZ53Fo48+SnV1NX/5y19IT08f1CROByZ9YwwLXkmfDHfH0tEWlN2F7WjPZbCc6vOXSMYSdrudbdu2+RZR9pfoEqrA1nWdnTt3UlFRwdlnn+2reAdqeBQK7e3t1NXVoWka8+fP9y0uDGbRqDe6sbKyksLCwqFrzGiKwD3pe3Qt3YJ75k9Qpp6DadokTFNSISce17hwhGO7f7Vd70Kr34Fln4FWUwCuBI5rdE9j1OOSPUr9lOWuZ/mq41my9T0IBC7FwcSwzylw9RDrydUszjqGoigcCbMye4mKxWLxLax1625PMk6tTlpuV0CrjmHAz+4N42SWIwxXRb0vOjo6iIqK4pJLLuGGG24YcHxrq+e+dY8W7w8hBJs3b6akpITzzjvP9/miRYt46aWXqK6uRgjBO++8w4EDB1i2bBngSSdyuVwsXbrUt09+fj5ZWVk+G1iohHxXb7nlFmpqagC46667ePXVV8nKyuJ///d/ue+++0I61nvvvcdXvvIVMjIyUBSFF154wW+7EIJf/OIXpKenY7VaWbp0KaWlpaFOeUSRYn2IGYGq+uku1rtzKoje0+HhQiIZC/QUrl47SkJCAvPmzQuYptGdUDzqnZ2dfPzxxzgcDhYuXEhsbKxv28lYaI4dO8bHH39MVFQUiYmJPnuO14/en0h3uVx8/vnntLe3c/bZZw9PhKo5Gj3vezgnP4qedAWqpmHWbIRbnP6C2e0RzG6XC8PVhnbscyz72tAqZqF0jvMcSznxpSoa6UYLS11vcLnzUc5yv0eY0kqi0cAkvRPw3E8B6BMOMj25DYDqXJXoWIGqqJg0ExazBbPZjKKq6BNcuHSnp9rew6qzd7/KP54afIb1SAt1m81GZGRkUG9GDMPg1ltvZfHixcyY0buZVHdaW1uJiorCYrFwySWX8Kc//YkLL7zQt/1Pf/oT06ZNY9y4cVgsFi666CIeeughn5ivra3FYrH43vh4SU1Npba2NvQLZRBC/dvf/jYrV64EYO7cuRw5coRPP/2UyspKrrgitOSJjo4OzjrrLB566KGA23/3u9/xv//7v/zlL3/h448/JjIykuXLl9PV1RXqtEeUU0msn0pzPZUZi4JTzkkiOTMQQlBeXk5RURFTp04N2p8drFBvamrio48+IjY2lnnz5hEWFua3fTBC3WtX2blzJ9OnTychIcHXZTSYRaMdHR188sknmEymoB5KThotCnfK9XRNfQ9Xxi8Q5nSP4FZVTCYTFstxwayo6LrhiRd0dEL9Dkz7KzGVT0ZpngFGN7GsgIUIYnUXc9zbuFL8naWm3zOD/2OGqw3QAYFL0YmdupeZKa006wrjLvGvmiuKgqZq1DujmfdlDZPm//DgcnsWxv7xUTNHKgdnCRppoW6324NudrR69WqKi4t55plnBhwbHR1NUVERn376Kffeey9r1qzh3Xff9W3/05/+xLZt23jppZfYvn07f/jDH1i9ejVvvfXWYC9lQEKOZ+yOEAKr1cqcOXMGtf/FF1/MxRdf3OexH3zwQX7+85/z//7f/wPgn//8J6mpqbzwwgt8/etfH/S8JRKJRCI5E3C5XOzatQubzcb8+fNDqiprmobL1XdDHCEElZWVlJSUkJ+fz/jx4wd1nJ54F402NDRw9tlnExsbi81m84tehL4XjTY1NbFr1y4yMzP9ohtHBDUcPfkq9KRvobW8hqn+7yiduz3zVT2CWUMDcSJK0uVyQWMxarOKYoqBxGmI5EZEeBWGIVBcoJkiQDPI1g8TqzSxzPQCDcZ4dinT+YxzOKRMJSH3IBOcM9jXYmbWF3V2be6dn76308T4SQbV5Scy573zaLfprP6hjQfuOUpiYiJxcXFBi+/RqqgPxI033sjLL7/Me++9x7hx4wYcr6oqEydOBKCgoIB9+/axdu1alixZQmdnJ3fccQfPP/88l1xyCeDpHVRUVMT//M//sHTpUtLS0nA6nbS0tPhV1evq6khLSxvUtQ5KqD/22GM88MADPhvKpEmTuPXWW7nmmqELvj506BC1tbV+Pp/Y2Fjmz5/P1q1b+xTqDocDh+NEmGhbW9uQzUkikUgkklMFm83GJ598QkREBAsXLgy5TbumaX2+wfZ6v48dO0ZhYWG/XvdQKuoOh8Mv091bCfemvui63m9jnerqavbv38+UKVOCEmbDhmJCj/8yevyXUW2fYmr4B2rrZjxVcDzVdk1F1TzXIYzjgtnVivtoEY7mcZgtSbQQgzU9moi4NlRxCKc6lwh1FwInmUoZGZSzjJdxCCtH1InsnTSDyqazeTVsGWnZydQe8RfrLh3M00E9DIZ+vNquaT5L0f6yJF7dbGPOjL3ouu7LL09MTOz1pqQ7hmH0Sg0aTrwe9b4QQnDTTTfx/PPP8+6775KTkzOo8xiG4dOULpcLl8vV62ev+1qOuXPnYjab2bx5M5dddhkAJSUlVFRUsHDhwkHNIWSh/otf/IL777+fm266yXfSrVu3ctttt1FRUcGvf/3rQU2kJ14vT88OZgP5fNauXcuvfvWrIZmDRCKRSCSnKm63m/T09EFXlftaBOpwONixYweGYfi6eg7mOD1pb29n+/btxMXF+cVFCiGwWCyUl5fjcDhITk4mKSnJL/NdCEFZWRlVVVXMnj076EWDI4ERNQ9n1Dxw1mBqehZT47PgPuY3xldt1+JQIxIxd5VhuHWSOQqV4K5Jwx1bgJpoJzzSiiAMJ10IxYmGjpVOpmi7yDfthMynuCUDbIUxNLQlU9OSSVXDBPYems3mzy7lcFMCBct1il7pLaxVVWX9xhy+flkq1vB2GhsbfY2HIiMjfaI9JibGT7COhvWlP6G+evVqNmzYwIsvvkh0dLRPN8bGxvp+Xq+88koyMzN90eJr166lsLCQvLw8HA4Hr7zyCuvXr+eRRx4BICYmhvPPP58f/ehHWK1WsrOz2bJlC//85z+5//77fce/+uqrWbNmDQkJCcTExPj08oIFCwZ1rSEL9UceeYS//e1vfOMbJ8zNl156KbNmzeKmm24aMqE+WG6//XbWrFnj+76tra3P13ESiUQikZyuxMfHn1TnxkCpL62trXz++eckJiYyffr0oKqowVTUjx07xs6dO8nJySEvL8/3YOFNdklLSyMuLo7Gxkbq6+s5cOAAERERJCcnk5CQQGVlJTabjbPPPjto7/KIY0nHnXYr7tQbUVvfQm1/C1U/jIIdT6VdBaMJHOUYhuHztAthoBrHMJpqoREMNRK3NRtrQgQipgFn2FF0xQmKDkIFxQAFotQ2ouPamBBbjiPrY1KnHaHw4rdpakym/MBMVH0hn78+mZ5tVlvbFG76qZUn/wITJkQzYcIEXC4XTU1NNDY2snv3boQQvmp7QkLCmLO+eMX1kiVL/D5ft26db51lRUWF35w7Ojq44YYbqKqqwmq1kp+fz5NPPum3/vKZZ57h9ttv51vf+hZNTU1kZ2dz77338r3vfc835oEHHkBVVS677DIcDgfLly/n4YcfHvS1hizUXS4XhYWFvT6fO3duyHmr/eH18tTV1fnFPtbV1VFQUNDnfmFhYf2+npFIJBKJRDIwPReTVldXs3fvXiZOnBhSFnl/Qt27aLS8vJyZM2f6/u3vvnDUKwIjIyOJjIwkKysLl8tFY2MjdXV1HDlyBICUlBRsNhthYWG+tJUxiWLCiLsII+4icNdhansBrX0TivOAJ41FPy7SVc/9VRQV03FB6bknXWj2fYgOT3a8SUtERGaixIbTFtNIu8WOExcaDiKxoWPiU6OQdsOzPiEhsZ6EhW+zYNFmvrAyjS1PfYkdr5+D7jqxkHXHLoUfvVnNnZfEkygiMJvNpKamkpqaihCC9nZPtb26upp9+/ZhsViwWCy0trYSExMz7OsCOjo6+u1021fH2O50XyQKcM8993DPPff0u09aWhrr1q3rd0x4eDgPPfRQn0EpoRLyT/J3vvMdHnnkEV+Z38tf//pXvvWtbw3JpMDTbjgtLY3Nmzf7hHlbWxsff/wx3//+94fsPBKJRCKRnI6crFjyCnXDMCgpKeHo0aPMnj2bpKSkkI8TSKgbhkFxcTGNjY2+RaPgv8ARCJjsYjabiYyMpLW1ldTUVDIyMmhsbKS8vJzdu3cTHx9PcnIyycnJA1pzRhVTKu6E63HGXcvB4k1Eut4kO24nilEfcLifp/z4glTFaMZobaSlYRIV6n0kJE9g87ijfBR2BKseRkNTGOmxh+koSyDc0oVJ6Gjo6GiEh6skX3qYBcubOfBGAcf+MwGEQs7NRTR+oZxf6CqXmWdxvjsN7fjfQSXwm+hIbomOpjAnB6fTyb59+7Db7ezcuRNFUfyq7aGujQiGjo6OM6Z3z6AXk77xxhs+v83HH39MRUUFV155pZ/tpKeY74nNZqOsrMz3/aFDhygqKiIhIYGsrCxuvfVW7rnnHiZNmkROTg533nknGRkZrFixYjDTlkgkEolEEiTezqTbt2/H4XCwYMGCQdlKAlXUvT53IYTfolGv1cVbEe3LTlFfX8/u3bvJycnxVfcTExOZPHkydrud+vp6jh07xoEDB4iMjCQpKYnk5GRiY2NHNgUmCNxuNzt37sTlGkfWnD/hNJtRuz5Da/8Pmu1V0BsC79htQaoRcT4i8j6sjR1UVlaStacNkR/HNFKZFj2eb224mLLWZmIn1BOV047F7CQmzIFucWCNBdsxM4mXHcFU2EHLsQRaJ4ZTVTKf9sRINqdoFJp17kVDB65Fpx7YZeh8v87M19MsWK1WIiMjycvLo62tjcbGRiorK9m3bx/R0dE+b3t0dPSQ3H+73e63RuF0JmShXlxc7ItjLC/3NIpJSkoiKSmJ4uJi37hg/iI+++wzvvCFL/i+94r8q666iscff5wf//jHdHR0cN1119HS0sI555zDa6+9Nvx5qBKJRCKRnOE4HA5fXvWCBQsGbSfpKdTb2tr4/PPPAy4a9Yr0vqIXhRBUVFRQXl7O9OnTewVOAERERJCdnU12drbPIlNfX8+OHTtQFMW3GDUxMXHULTJOp5PPP/8cs9lMYWGhbz6GdR6GdR6u5F+gdu1Atb2B1vEGiqsCAGFKx4g4FyNsKsIyEcM6j1jFTGwcvsWQjY2NNDQ0sKPsc36crrJeFPCvl6bBFQ4sZzkQdQqW1nC6ohSiIjuxRwtIBrPmQtctaJoKCnR0GHweBZebBAmGQnKLSlSphdJiC79yKbyYZnBtlom8BI/2i42NJTY2ltzcXN88GhsbqaioQNM0X7V969ZoqqsVIiMVWloEX/6yhYkTg0uOGSj15XRCEcEYeU5h2traiI2NpfVyiBl8062QKX165M51MpwSDY+GLvWzX/ZckDfs53iW0JqCjTQjPb/hanDkaHPwu9g/+PySoeD9nZHX+iFaTP//EOhtNspjFwd9nrVr17Jp0yb279+P1Wpl0aJF/Pa3v2XKlCl97rNp0ybuu+8+ysrKcLlcTJo0iR/84Ad85zvf8Y2x2Wz89Kc/5YUXXqCxsZGcnBxuvvlm3wKnpqYm7rrrLt544w0qKipITk5mxYoV3H333X4dJAMJo6efflr2rTiF6R5XHAq1tbXs3u3J/166dOlJVUHr6+vZv38/5557LnV1dezatYvc3Fxyc3N7LRrtT6QbhsH+/fupr6+noKDA72c3GAzDoKWlhYaGBurr6+ns7CQhIcEn3EfaItPZ2cn27duJiYlhxowZQS3GVBz7ARBh+UGfp/t1b9yh8uCbU3BcaSC2mVCrNczpgtgpOnpeF8Jsp9Pu8rXDVOp1RK1AbTeTER9PW0sYhn5inr6/JcPFtyc38dMvRmHpprVr6hT+tsHMVy50M2uqm7a2VhobG1m/3sXjj8ejqgp5efC731mZPTv4avvy5cu57rrrfAtDT2fG8GqLU5tJ3zh1xPqY5++MmFgfbq7g2TEt1vsTzoOdt+w2eoItW7awevVq5s2bh9vt5o477mDZsmXs3bu3T0tBQkICP/vZz8jPz8disfDyyy+zatUqUlJSWL58OeB5G/n222/z5JNPMmHCBN544w1uuOEGMjIy/n979x1XZfk+cPxzDntvBBUFXDhBwF2aZY4c4Nf6OTJHZuVq0B6mZqa5sszsmzvN3LPUnLhHKqgIoiIuZO89znl+f/g9TyBDQOAc8H6/XudVPDzjvg9HuJ77ue7rZtCgQTx48IAHDx4wf/58WrVqxZ07d3j77bd58OABW7ZsKXK9VatW0bdvX/nrR5fCFmoXhUJRrol1Gpoyh7dv36ZZs2bcuHHjiVMVNOUZIyIiuHXr1mMnjZZ0Pc3CTXl5eXTs2LFSQbVSqcTW1hZbW1uaN29OZmYm8fHxxMbGyuUHNXnt1T0hMj09nYsXL1KvXj1atGhR7mtVJEDXKNzvL5pDf88s/Gabk6jQRwWoUhXkXlOiJ+lj6GJAdilNuRGrwMJcovBbr/lkFahgTbg9x+IVBHTMpW9TNdGxCl57x4T7DxSs22pAo4YSHb2MsTEw4Y8/sjAygv/7vzwGD44jPT2ZU6f0sbW1xd7eHhsbmzKfdogR9TpEWyPqhelqwF4rRtM16tCoOuj+yHptp6sj6o+Kj4/H0dGRo0eP0r1793If5+3tTf/+/Zk5cyYAbdq0YejQoUydOlXex8fHh379+pVaxWDz5s2MHDmSzMxM+Q+iQqFg+/btYh5QHZKXl1fuQL2goEBexbR9+/bo6elx/Phxevfu/URBa1JSEufPn8fQ0BBvb2/538qjk0ZLG0nPysoiODgYExMT2rZtWy3pKvn5+fJIe2JiIkqlUs5rt7Ozq9LFfJKSkrh06RKurq4Vqp5TlbJyYOAXRpxLUsrRtgQoVBLGLnnk6JX+mTEx1cPCXP/hcLoEKpUKlUqFvoE+CsXD0fZednmEbtInOvbf0XcXZxWKjGTuRmTj46PPBx+Y4Ov7MDDTjPpr0mSys7OxtraWc9tNTU2LPH3x8fHhxx9/LHV1+7qk5opePsV0MSDWxTaVaXnNXKb14Ygauc5QNoqR5jokLS2tyKu86QapqakA5V6cRZIkDh06RHh4eJHAvmvXruzatYuoqCgkSeLIkSNcv36d3r17l3ltS0vLYkHPpEmTsLe3p2PHjqxcubJCo7FC7ZWZmcnp06dRqVR07twZCwsL9PT05BHvysrNzSU0NBRJkujcuXORIF1TUQZKruwCkJKSwrlz57Czs8PLy6vacsoNDAxwdnamXbt29OjRQ74huH79OoGBgQQFBXHv3r1SV2otr9jYWIKCgmjevDlubm5am9hqagyHFuQysUPBw/QVBSgUgJ6C3HtGGOf/b95ACcdmZ6lISsonJ0ctB+kGBgYoFUrcTdU0u6Xi4GJDHsQqkQAjQ4m2buncv/yA+g75rF1rwfr1FnKQDv+O+jdr1ozOnTvTuXNnHBwcSE5O5p9//uH06dOEh4eTkJBAXl4eGRkZpZZnnD17Nh06dMDCwgJHR0f8/f0JDw8v8/3Ytm0bvr6+WFtbY2ZmhpeXF2vXri2yj+ZG8tHXvHnz5H00N16FX3PmzCnHT6R0IvWlhmgCY10dXRf+1fpwRI2NrOt6KszTLGJrGzB9zCh5VhpAsUXVpk2bxvTp08s8VK1W895779GtWzfatGlT5r6pqak0aNCA3Nxc9PT0+Pnnn3nxxRfl7y9evJg333yThg0boq+vj1KpZNmyZaWO0ickJDBz5kzefPPNItu//vprnn/+eUxNTeX0mYyMDN55550y2yfUbvHx8Vy6dImGDRvSvHlzOVdaM4qsUqkqtZiNZtKohYUFWVlZxSq7lJXqAhAdHU1oaCjNmzev0YULH02R0VSRiYmJITw8HHNzczmvvSIpMvfu3ePGjRu0bdsWR0fHau5F+Xw3MZ8hPVR8usKA80lKJAVI+pATbYCpox65Zg8D8YcBuwJQoEBNQYGatFQ1CiWYmurRxALMItWEHVU+3EsBRobg0TgbI1UajRtKfDTJBG9vPRSK/5WVVChK/VyZmJjQsGFDGjZsiEqlkkfbw8PDGTduHEqlkl27dlGvXj2aNWtW5NjqSjGMjo4ucszevXsZN24cQ4YMKbL966+/Zvz48fLXZdV7Lw+R+qIF2g7Wa91oemE1mKteU8E6iFSYqlYVqS+sTC1foP66Fffu3StynfIsvDZhwgT27t3LiRMnaNiwYZn7qtVqbt26RUZGBocOHWLmzJns2LFDXnVv/vz5LFu2jPnz59O4cWOOHTvGZ599xvbt2+nVq1ex/r344ovY2tqya9cuDAxK/8X41VdfsWrVKu7du1f2+yDorPz8/DIXG7p9+zY3b96kdevW1K9fv9j3//77b5577rkKV1vTTEZ1d3fHycmJ48ePywHP44J0SZK4desWd+/epW3bthWu216d8vLy5CoymhSZwlVkSkqRKdyf9u3b6+y8j7BI+OhXQ0480EOlBNSgbwxSfVAoCsjL/9/YrqRGQR7KlCyUd3PRjzEnL/lhaoqBPtjbqHj3TTVeLfJo20aJufnDqj+Fb9AKh55KpVIO2B93Q6hWq7ly5Qr+/v54eHhw6dIlHjx4UGYwXFUpho/y9/cnPT2dQ4cOydtcXV157733eO+998p9nccRI+paoM3R9VodpNdhmjQYEbDXTpaWlhW6IZg8eTJ//vknx44de2yQDg//eDVt2hQALy8vwsLCmD17Ns899xzZ2dl8/vnnbN++nf79+wPQrl07goODmT9/fpFAPT09nb59+2JhYcH27dvLDNIBOnXqxMyZM8nNzRUrPtcxKpWKkJAQkpOTiyw2VJhmxLPw6qSPowlKb926Rbt27ahXr56cLqI5T1lBukql4urVq6SmptKhQwedmzBoaGiIs7Mzzs7OqNVqkpOTSUhI4Pr16+Tm5hapImNsbIwkSXKlGl3sT2Et3eDP2XmkZkDgBSVnw/S4cldBTIYCha0SVXYBKffzyU3IQy8uhdx0ffIU1hgZqmnglEgzt3ye6azH26+bYWysT+EQ89GnNGq1ukjQrlnZXvOZK220XalU0qxZMxITE9myZQs2NjaP/d1UmRTDw4cPEx4eznfffVfiPrGxsfz111+sWbOm2PfmzJnDzJkzadSoESNGjOD9999/opStSh2pVCpp2bIlV69elbe1bNmS69evV+gf9NNOpMPotppMgdEQqTB1myRJTJkyhe3btxMYGIibm1ulzqNWq+U8+Pz8fPLz84v9UXt0Nci0tDT69OmDkZERu3btKtcIaXBwcLn+EAq1S3Z2NkFBQSiVSrp06VLmz1ezOml5FA7+O3XqJN+8aj6beXl5D3OZSwnS8/LyCA4OBh7eJFbHipZVSalUypMdC1eRiY6O5tq1a5ibm8vBqK+vb61ZoMfKHPx6qPHrUfRJjCRJ3Lhxg+joaHx9feU0EpVKIiUlj/j4eBISEjh5MhcbGxt5Mm5JFXoKj6JrJhRrXoU/b5r9Cv9+y8zMBMDc3Pyxv5uqMsWwsDVr1mBhYcF//vOfItvfeecdvL29sbW15dSpU3z22WdER0c/dgHQslQqUF+5cmWxRzezZ8+W71qEiqmpUo51YjS9hks1aitYBzG6XhdNmjSJ9evXs3PnTiwsLIiJiQHAyspK/mM2atQoGjRowOzZs4GHv1t9fX3lRUz27NnD2rVrWbp0KfBwNL9Hjx589NFHmJiY0LhxY44ePcpvv/0m/3FIS0ujd+/eZGVlsW7dOnnSK4CDgwN6enrs3r2b2NhYOnfujLGxMQcOHODbb7/lww8/rOm3SahCjwbESUlJBAcH4+joSKtWrR6balDeQD0nJ0deUKhw8K9JcTA2NubUqVNy8GZvb19klDEjI4OgoCCsra1p1apVlVZZqQkKhQJzc3PMzc1xc3MjMzOT4OBguerO+fPn5b7b2trWuv5JkkR4eDhxcXFFgnR4+BnR3LBIkkRWVpZcQef69euYmprKC2NaW1sX+8w9GrQXrgZU0mh7RkYGSqWyXCU6J02aREhICCdOnHjsvhYWFgQHB8sphgEBAbi7u8sphoWtXLmSV199tdiAh2bhTnj4ZNPQ0JC33nqL2bNnV3rAo1KBekkF5kU5rydTOIiujqC9TgTpWqKNYB1EwF4XaYLrR3/xr1q1Sv69evfu3WKjRxMnTuT+/fuYmJjg4eHBunXrGDr038/Fhg0b+Oyzz3j11VdJSkqicePGzJo1S17w6OLFi5w9exZATqHRiIyMxNXVFQMDA5YsWcL777+PJEk0bdqUhQsXFpkUJdRud+/eJTw8nBYtWtCoUaNyHfPoqqIlSU1NJSgoCFtbW1q3bl1kpVHNsd26dSM9PZ34+Hhu3bpFSEiInCaip6dHeHg4jRo1KrIIUm2Vm5vL5cuXMTExoXPnzigUCpKTk+WFn/Ly8uS+Ozg46PwTK0mSCAsLIzExkQ4dOpQZICsUCszMzDAzM6Nx48YUFBTIK6ReuXIFtVot993Ozq5Y30tKkXl0tP3u3bvo6+ujVqvLvOGpyhTDwo4fP054eDgbNz6+clunTp0oKCjg9u3bZS5sV5YnnkwaGBhIp06danxFr/LSxcmkFVEVQXudDNK1sACSNoJ1DRGsV0xNTyatbB11QahuBQUF5OfnExoaSlxcHF5eXuXO1QU4efIkzZo1K7VKiWbSaJMmTYqUG3xcZZesrCzi4uK4f/8+2dnZmJiYUL9+fRwdHTEzM6u1wXpmZiYXL17ExsamxCcWkiTJKTLx8fGkpaVhYWEhj7ZbWJR/dc6aIEkSoaGhJCcn4+Pj80SxniRJpKWlkZCQQEJCAmlpaVhaWsqj7Y+roKNWq0lISJAnJYeEhJQ4z+bRFMNHq8KU1+uvv86tW7cIDAwssn3MmDGEhIRw/vz5x57j999/Z9SoUSQkJGBjY1OpdjzxZNLevXtz6dIlWrZs+aSnEkpQmZH2OhmY6wBtjayDGF0XBKFy8vLy+Oeff1Cr1XTp0qXCgVZpqS+SJBEREUFkZKQ8aVSj8AhoafnoJiYm5OTkUFBQgJeXF/n5+cTFxREZGYmRkZE82lxSqoSu0jxZqF+/Ps2aNSux34+myOTl5clpInfu3EFfX1/uu42NjVZTZNRqNVevXiUtLQ1fX98KV/55lEKhwMrK6uGCcv9L5dNU0NE8SdQE7XZ2dsUmYKampjJ48GA8PDzYvHlzqZPhqyPFUCMtLY3NmzezYMGCYtc9ffo0Z8+epWfPnlhYWHD69Gnef/99Ro4cWekgHSoQqHt7e5e4vaCggCFDhsg/wIsXL1a6MULZRABeSA3nqmtoM1gHEbALglAxmpSpNm3aVCroKylQV6lUXLlyhZSUFHlxJEBeHEmzf2lBekFBAVeuXCE7O5uOHTvKkyzr16+PSqWSg7fLly8DYG9vj6OjY5WvEFqVEhMTuXTpEu7u7ri6upb7OENDQ+rXr0/9+vVRq9UkJSWRkJBAWFgY+fn5RarI1GSKjFqtJiQkhIyMDHx9favl2kZGRkX6npKSQkJCAhEREVy5ckWekKqvr4+pqSn+/v44OTmxadOmMicaV1eKITxMM5QkieHDiwdkRkZGbNiwgenTp5Obm4ubmxvvv/9+kbz1yih36ouBgQG9evWic+fO8jZJkpg5cyZvv/22/Fhs2rRpT9SgqlbbU1+Ex9BCsA7aTYN5lAjaixOpL4LwUEFBAQUFBZVOp7h48SJ2dnY0btwYKDpptH379kUmjapUKnnyqGZVxkdlZ2cTHByMoaEh7dq1K7NEqCRJpKSkyGkiOTk5OpnbHRMTw9WrV2nVqhXOzs5Vck5JksjIyJArqRROE3FwcMDc3LzaUmTUajWXL18mOzsbHx8frVTfyc7Olvv++uuvk5SUhImJCT///DN9+vTR+YpAVancI+qBgYGMHj2ajh07Mm3aNPlOZNasWUyaNIlWrVpVWyMFQddoe2S9MDHKLghCacpa+bM8Co+op6amyoF7mzZt5DigcJWOsq6XmpoqV5xp0aLFY1NaFAoFNjY22NjY0KxZMzm3+8GDB1y7dg1LS0scHR1xcHAodcXJ6nb37l1u3ryJp6dnlS7MpFAosLCwwMLCAnd3d3Jzc+UUmcjISAwNDeWRdltb2ypLD1KpVFy+fJnc3Fx8fX0fu9ZCdTExMaFRo0bY2dnh7OyMjY0Nbdq0YdKkSZw6dapck0PrinIH6t26dePChQu8/fbbdO3ald9//50mTXQjUBGeYlpKgQHdCtZBBOyCIFQ9TaAeHR1NSEgITZs2xdXVtdyTRjViY2O5evUqTZo0oVGjRhW+eXg0tzs3N1ceaY+IiMDY2FgO2q2srKp9QqYkSdy8eZOoqCh8fHxKXDCqKhkZGdGgQQMaNGiASqWSq8iEhoZSUFCAnZ2dHLhXdrRZpVJx6dIlCgoK8PHx0VqQrpGdnc3QoUNRqVQcPHgQCwsLJEnSqcm2NaFCk0mtrKz4448/WLVqFc888wwzZsx46t4wQShM14J1+Ddgh6czaB/KRjJQM1fbDRGEOkChUJCYmMjt27fx9PQsUv2lPJNGJUni9u3bREZG0rZtWxwcHKqkXUZGRjRs2JCGDRvKJQDj4+PlhZw06THVUbNcrVYTFhZGUlISHTp0qPHRfD09PXnSpYeHh5wic+/ePUJDQ7G0tJT7X94KOiqViqCgICRJwtvb+4lW0qwKOTk5jBgxgqysLP7++295HsTTGHNW6icxduxYnnnmGV599VW5EL0gaI0WR9VBN4N1jaclaC/cT0EQ/vUkgY1KpSIpKYmcnJxKTRpVq9WEhobKAa3m+Kqmr69PvXr1qFevnjwpsXDN8sKLLD1pbrMmNSQnJ4cOHTo8cSWUJ1VSiowmt/vWrVtyioymikxJKTIFBQVF5h1oO0jPy8uTSxoePHiw2p9W6LonqqOuVqtJT09/bO1LbRKTSZ8SWgzUNXQ1WC9JbQ/aHxeYZ6Sp6WwVKSaTCk89SZLIy8ur8HE5OTlcvHiRvLw8rK2t8fLyks9XnkmjeXl5XLp0CbVajZeXl1YmfmomZMbFxREfH09GRgbW1tZy4KqpNlNe+fn5BAcHAw8XxNF2asjjaG60NIF7SSky+fn5BAUFoaenh5eXl9ar6uTn5zN69GgiIyM5dOhQleb911YVvm06cuQIPXv2BB7eRRe+0/nvf//LW2+9VXWtE4Ty0vKoOuj2yPqjHg10dT1wFyPmglBzNJNG7e3tMTU1JT09HSiaj65Zzr0kmZmZBAUFYWFhUemykFWh8GhzkyZNyMnJIT4+nri4OG7cuIGZmZkctD9uwFFz42Jqakrbtm21HtCWh56entw/SZLklWHv3r1LaGgoFhYW5OTkYGpqiqenp9b7VFBQwPjx47lx4wZHjhwRQfr/VHhE3cjIiHfeeYdvv/1WvptMSEhg7NixnDhxguTk5GppaGWJEfWnjBhZrzLaCt6rIigXI+qC8FBFR9QfnTR679494uPj8fb2Ltek0aSkJC5dukTDhg1p2rSpzj5tz8/Pl6uoJCQkyAsNOTo6FksRycjIICgoCDs7Ozw8PGrNAkxlSU9Pl3PSCwoK5EWm7O3tS02RqU4qlYoJEyZw/vx5jhw5UmVlLuuCSo2ojxo1igMHDrB+/XoiIyMZN24cLVq0kB8JCcLTrPXhCKD2B+zlCZgrGsyLkXFBqFnlDZQ1VUzu3LmDl5eXPOlTU/WlPEF6VFQU165dw8PDgwYNGlRZH6qDgYEBzs7OODs7o1arSU5OJi4ujqtXr6JSqbCzs8PR0RF9fX1CQkJo2LAhTZo00dkbj4rIzc3lypUrWFtb06ZNGyRJklNkQkJCUKvVcoqMnZ1dtdcsV6lUTJkyhTNnzoggvQQVDtS7du1KcHAwb7/9Nt7e3qjVambOnMnHH39cJz7AQi2nAykwGrUpFaayROAtCLpPoVBQ1sNzzUqhaWlpdOrUqcikUaVSSUZGBlFRUaUuMiRJEjdu3ODBgwe0b98eW1vbautLdVAqldjZ2ckj5mlpacTHx3Pjxg05NcTIyIjc3FytTx59Ujk5OVy4cAFLS0tat24tj5wXTpFJS0sjISGBO3fucPXqVaysrIrk9VdlrKdWq/nggw84evQoR44cwcXFpcrOXVdUamrv9evXOX/+PA0bNuTBgweEh4eTlZWltQUHBKEIEawLgiCUiyb3Wk9Pjy5dusijp5pFjGxtbXFxcZFHy21sbOR65cbGxqhUKq5cuUJmZqZWShVWNYVCgZWVFZmZmeTl5dGiRQskSSI2Npbw8HDMzc3lFJnqXB20OmRnZ3PhwgVsbGxo1apViW3X9N/KyqpIXn9CQgIRERFyioyDgwPW1tZPlCKjVqv59NNP2bt3L4GBgbi6uj5B7+quCgfqc+bMYdq0abz55pvMmzePmzdv8tprr9GuXTvWrVtHly5dqqOdglBriWBdEARdlJKSQlBQEA4ODrRq1arISqOayi5KpRJ3d3fc3d3lZd0LB62aUeaOHTvqfBWU8tLUfffy8sLOzg6Axo0bk5eXJ+e13759G0NDQ/mm5UmD1uqWnZ3N+fPnsbOzo2XLluW+wTA2NsbFxQUXFxdUKpVcr/7KlStFUmTs7e0r9PNXq9V89dVXbNu2jcDAQLGAZhkqPJnU2dmZlStX0q9fP3lbfn4+n3/+OT/++CO5ublV3sgnISaTPsV0ZFS9MBGw14wqmUzaJRX0H3NsQRqcFpNJBd2Wn5+PWq0usu3BgwdcvXqVZs2a0bhx4wqvNJqYmMjly5fR09MjLy8PU1NTHB0dcXR0xMLColaNNGtoUniio6Np3759mf+mC5c+jI+PR5IkuV67nZ2d1muRF5aVlcWFCxdwcHCgRYsWVfKz0aTIaPqfmZmJtbW1/B6U9WRFkiS++eYbVq5cyZEjR2jVqtUTt6cuq3CgnpCQUGrJnKNHj9KjR48qaVhVEYH6U0wHA3UQwXpNEIG6IPyrcKCuCUbv3r2Lp6dnkZVCyxukx8XFERISgpubG66urqhUKhISEoiLiyMhIQEDAwM5aLe2tq4VQbtmcaaUlBS8vb0rVGNdkiRSU1Pl0o85OTnY2trKKSLaqCGvkZmZyfnz53F2dqZZs2bV9rPIzs6WnzYkJSVhYmIij7QXftogSRJz585lyZIlHD58mHbt2lVLe+qSJ1rwqDYQgfpTTkeDdRABe3USgbog/EsTqBeeNOrj44O5uTnw70qjarW6zCBdkiTu3LnDrVu3aN26NfXq1Su2j2akWbPIkEKhkHO6bW1tdTI9pKCggMuXL5OXl0f79u2fOLDOzMyUg/a0tDQsLS3loN3MzKzGblwyMjK4cOECDRo0qNGKNQUFBUUWWlKr1VhZWXHx4kUSExNZvHgxBw4cwMfHp0baU9vpzrMZQagOOjSx9FEid10QhJqSnZ3NxYsXMTAwKHHSqGbEvbQgXa1Wc+3aNeLj4/Hx8Sl1WffCi+yo1WpSUlKIi4sjLCyMgoIC7O3tcXR0xN7eXusL7MDDFVQ1K3P6+vpWScqKmZkZZmZmuLq6kpubK6eH3Lp1C2NjY/nGxcrKqtqC5/T0dC5cuICLiwvu7u41+lRDX19ffqKiedoQHBzMggULuHfvHt7e3pw9e1YE6uUkAnWh7tPxYB3E6LogCNUnJSWF8+fP4+joWOqkUaDU0e78/Hx5xLlTp07lLlGoVCqxtbXF1taWFi1ayDnNERERhISEyLXKHRwctDIRVXPzYm5uXm0rqBoZGdGwYUMaNmwoT8aMi4uT153R3NTY2dlV2fU1K8u6urri5uZWJeesLE0VmRs3bpCSksKmTZuIiYkhOjpaq+2qTUSgLgg6QIyuC4JQXWJjY3F3d6/UpNGsrCyCgoIwNTWlQ4cOlR5xLlz2r2nTpmRkZBRZzv7Rso/VTbMyp4ODAx4eHjUy4qynpyePNGueNsTHx3P9+nVyc3PlGxd7e/tKLzKkqeSj+XlrmyRJrFmzhqlTp7J7926dm8dYG4gcdeHpoaOj6o8SAfuTEznqgvCvgoICVCqV/LVm2Xh4GECXFqQmJydz6dIlnJ2dad68ebVORNTkdKekpGBpaSkHtBWZ1FleycnJBAcH07hxY9zc3LQ+2VWSJDIzM+W8/vT0dKysrOQbl/K+B8nJyQQFBdG0aVMaNWpUza1+PEmSWL9+PQEBAezYsYMXXnhB202qlcSIuvD00OEUmMJEOowgCFWp8Ci6JiddUyO9tCD1wYMHhIWF0aJFCxo2bFit7TMxMaFRo0Y0atSIvLw8OWi/efMmZmZmctBeFQsMaSrWNG/evNr7VV4KhQJzc3PMzc1xd3eXFxnSrI6qKX3p4OCApaVlie9BUlISwcHBOtWvLVu28P7777NlyxYRpD8B3Zt+LQjVabm2G1B+rQ9HyEG7IAjCk9AE6IUXMiqtssvNmzcJDw/Hy8urxoM+Q0NDGjRoQPv27Xnuuedwc3MjMzOTf/75h5MnTxIeHk5KSgqVSQa4f/8+ISEhtGnTRmeC2ZJoFhny9vamR48e8mJTFy9e5Pjx44SFhcnVVOBhTfvg4GA8PDx0pl87duxg4sSJ/PHHH/Tt27fGrjt79mw6dOiAhYUFjo6O+Pv7Ex4eXmSfnJwcJk2ahJ2dHebm5gwZMoTY2Ngaa2NFidQX4elTC0bVSyJG2MtPpL4Iwr8KCgrIzc197KRRlUrF1atXSUtLw8vLSy7fqAtKK/tYr149bGxsyiz7KEkSkZGR3LlzBy8vL2xsbGqw5VVHrVaTnJwsP3EoKCjAwsKC1NRUnQrS//zzT8aOHcvatWv5z3/+U6PX7tu3L8OGDaNDhw4UFBTw+eefExISQmhoqLwI04QJE/jrr79YvXo1VlZWTJ48GaVSycmTJ2u0reUlAnXh6VQLg3URqJefCNQF4V8jR47Ezs4Of39/OnToUGJQm5ubS3BwMEqlEk9Pz0pPZqwJhcs+xsXFoVKpSi37KEkS4eHhxMbG4u3tjYWFhRZbXnU0Ne1v3LiBsbExubm52NjYyFVkTExMtNKu/fv3M3LkSJYvX86wYcO00obC4uPjcXR05OjRo3Tv3p3U1FQcHBxYv349L7/8MgDXrl2jZcuWnD59ms6dO2u5xcWJHHVBEARBqMNefvllNm/ezODBg7G0tGTQoEH4+fnRuXNn9PT0SEhIICwsDGtra1q1aqUT9c3LUlLZR01Oe+Gyj3Z2doSHh5Oenk7Hjh21FrxWh9jYWCIiIvD09MTR0bHIhNzr169jbm4u12uvitz+8jhy5AgjR47k559/ZujQodV+vfJITU0FwNbWFoALFy6Qn59Pr1695H08PDxo1KiRCNQFQRAEQah5/v7++Pv7k52dzYEDB9i2bRtDhw7FyMiIbt26cfToUbZu3UqbNm20XgGloh4t+6ipnnLnzh2uXr2Knp4e7u7uOrkiamVFR0cTGhpKu3btcHBwAIpOyM3PzychIUF+HwwMDOSR9selCVXW8ePHGTZsGD/88AOvvfaaTnyO1Go17733Ht26daNNmzYAxMTEYGhoiLW1dZF969WrR0xMjBZa+XgiUBcEQRCEp4CJiQmDBg1i0KBB5OXl8d5777Fs2TKaNWvGyy+/TP/+/Rk8eDDdu3fX6dSX0miqpxgYGBAXF4e1tTX29vbEx8dz8+bNai/7WBOioqLkib52dnYl7mNgYICzszPOzs5ybn98fDwhISGo1Wo5TcjOzq5KVmI9ffo0r7zyCt999x2vv/66TgTpAJMmTSIkJIQTJ05ouylPRATqgiAIgvCU0dPTIykpiWPHjtGhQweOHTvG5s2beeutt8jNzaV///74+/vTs2fPGlmAqKpkZWVx8eJFrKysaN26NUqlEjc3N/Ly8uSc9uoo+1gT7t+/z/Xr1/Hy8pJTOR5HT09PHk2XJInU1FR5ddgrV65ga2srl340MjKqcJvOnz/PkCFDmDlzJhMmTNCZ93Hy5Mn8+eefHDt2rMgkWycnJ/Ly8khJSSkyqh4bG4uTk5MWWvp4YjKp8HQSk0nrNDGZVBAqR6VScfLkSbZs2cKOHTtITU2lX79++Pv706tXL50eiU5LSyMoKAgnJ6cyF2jSpIbEx8eTkJCAoaGhHLRbWVnpTLBZ2N27d4mIiKB9+/bF0jYqKzMzU67XnpqaKpc0dHBwwMzM7LHvQ3BwMP379+fzzz/nww8/1In3TZIkpkyZwvbt2wkMDKRZs2ZFvq+ZTPrHH38wZMgQAMLDw/Hw8NDZHHURqAtPJxGo12kiUBeEJ6dWqzl79qwctMfGxtKnTx/8/Pzo27evTpVvTEpK4tKlS7i6uuLq6lruoLGkso+aoL268rkr6vbt20RGRuLt7f3wd1M10Cw0FR8fT2JiIkZGRnLQbm1tXez9DAkJoV+/fgQEBPD555/rRJAOMHHiRNavX8/OnTtp0aKFvN3KykqeTDxhwgT27NnD6tWrsbS0ZMqUKQCcOnVKK21+HO1/AgVBEJ4S5VmM41Hbtm3D19cXa2trzMzM8PLyYu3atUX20SwD/+hr3rx5AAQGBpa6zz///AM8DAZK+v6ZM2eq580QdJ5SqaRLly4sWLCAGzduEBgYSPPmzfnmm29wdXVl2LBh/PHHH6SmplZqAaKqEhsbS1BQEC1atMDNza1CQaMmNaR169Z0796dtm3bolAouHr1KkePHiUkJEQuAakNkZGR3L59Gx8fn2oL0uHfhaa8vLx47rnnaN68Ofn5+Vy6dImjR49y9epV4uLiyMjIICwsjAEDBjB58mSdCtIBli5dSmpqKs8995ycp+/s7MzGjRvlfb7//nsGDBjAkCFD6N69O05OTmzbtk2LrS6bGFEXnk5iRL1O09UR9fIsxvGowMBAkpOT8fDwwNDQkD///JMPPviAv/76iz59+gAUq1awd+9exo0bx82bN3F3dycvL4+kpKQi+0ydOpVDhw4RERGBQqHg9u3buLm5cfDgQVq3bi3vZ2dnh4GB+OUp/EutVhMSEsKWLVvYtm0bN27c4IUXXmDQoEEMGDAAGxubGgve7t27x40bN2jbtq1cAaUqSJIkl32Mi4sjJyenSK326v43IUkSt27d4t69e/j4+Git/rskSaSkpBAfH8+lS5d48803sbGxwdvbm1WrVlGvXj2ttOtpIgJ14elVC4N1EAF7eehqoP6oRxfjKC9vb2/69+/PzJkzS/y+v78/6enpHDp0qMTv5+fn06BBA6ZMmcLUqVMB5EA9KCgILy+vCvdFeDpJksS1a9fkoP3q1at0794df39/Bg4ciL29fbUE7ZIkERERwb1796o0b7u0a2nKPmpGlW1sbOQUmcpMwnzc9W7evMmDBw/w8fHRmRSjmzdvMmLECOzs7MjNzSUmJobIyEidGlGvi0TqiyDUMq0PR9D6cIS2myEUkpaWVuSVm5tbruMeXYzjcSRJ4tChQ4SHh5ca2MfGxvLXX38xbty4Us+za9cuEhMTGTt2bLHvDRo0CEdHR5555hl27dpVrnYJTy+FQkHLli2ZOnUqFy9eJDQ0lF69evHbb7/RtGlTXnrpJf773/8SHR1dZekxkiQRFhbGgwcP6NChQ7UG6fBv2Ud3d3c6d+5Mt27dsLe3JyYmhuPHj3Pu3Dlu375NVlbWE19LkiSuX79OdHQ0vr6+OhOk37lzh4EDB/Lcc89x5MgRzpw5w9WrV0WQXgPEiLrwdKulo+qPEqPsRVXJiDoXgcf9kcwAvIttnTZtGtOnTy/zSLVazaBBg0hJSXlsnd/U1FQaNGhAbm4uenp6/Pzzz7z++usl7jt37lzmzJnDgwcPSi2r99JLLwGwZ88eeVtCQgK//fYb3bp1Q6lUsnXrVubOncuOHTsYNGhQme0ThEdplrjfunUr27Zt4+zZs3Tq1Ak/Pz/8/Pxo2LBhpYI8lUpFSEgImZmZeHt7a710ZG5urrwiaFJS0hOVfZQkifDwcOLj4/Hx8dGZCjtRUVH06dOHXr168csvv+jEBNuniQjUBaGOBOsgAnaNmg7U7927V+Q6RkZGj30cPmHCBPbu3cuJEyeK1PktiVqt5tatW2RkZHDo0CFmzpzJjh07eO6554rt6+HhwYsvvsjixYtLPNf9+/dp3LgxmzZtksuTlWbUqFFERkZy/PjxMvcThLJIkkRUVBTbtm1j27ZtnDx5kvbt28tBe3kngObn5xMcHIwkSbRv317n5k4UXhE0ISFBrpxSnrKPmqcESUlJ+Pj4yBVKtC0mJoY+ffrQrVs3VqxYgZ6enrabpHVqtbpGb1bEbZEgLNd2A6qOSIvRDktLyyKvxwXpmsU4jhw58tggHR5W32jatCleXl588MEHvPzyy8yePbvYfsePHyc8PJw33ij97nPVqlXY2dmVa5S8U6dO3Lx587H7CUJZFAoFDRs25J133uHIkSPcu3ePsWPHEhgYSPv27XnmmWeYO3cu169fLzU9Jicnh/Pnz6Ovr4+Pj4/OBenw74qgnp6ecuWUvLw8goKCOHbsGGFhYSQmJqJWq4scJ0kSV69eJTk5GV9fX50J0uPi4ujfvz8dO3Zk+fLlNRqkHzt2jIEDB1K/fn0UCgU7duwo8v0xY8YUq1DVt2/fam+XSqVCqVSSmJjIhQsX2LVrF1lZWdVaFUinA/Xp06cX+0F4eHhou1lCXVSHgnX4N2AXQbtukSSJyZMns337dg4fPoybm1ulzqNWq0vMg1+xYgU+Pj54enqWev1Vq1YxatSocgU6wcHBODs7V6qNglAShUKBk5MTEyZMYP/+/URHRzN58mTOnTtHp06d6Ny5M7NmzSI0NFQO2tPS0vjnn3+wsLDA09OzVozq6unp4ejoSJs2bejRowdt2rQBKFb2MT8/n5CQENLS0vDx8dF6Ko9GQkICAwcOpE2bNqxevRp9/ZpdyD4zMxNPT0+WLFlS6j59+/YlOjpafv3xxx/V2ia1Wo2enh7379/n2WefZfLkybz++uv069ePn376ifz8/Gq5bs2+85XQunVrDh48KH9d0x8W4SmynDqVBqPxaLAu0mO0Z9KkSfJiHBYWFnJZxcKLcYwaNYoGDRrII+azZ8/G19eXJk2akJuby549e1i7di1Lly4tcu60tDQ2b97MggULSr3+4cOHiYyMLHHEfc2aNRgaGtK+fXvgYf32lStXsnx5HbuLFXSGQqHA3t6ecePG8frrr5OamsquXbvYunUrCxcupFGjRjz77LPs27eP3377jdatW9fKyYtKpRI7Ozvs7Ozw8PAgNTWV+Ph4rl+/TnZ2Nnp6ejRt2lRnbkCSk5Px8/PD3d2d33//XStPL/r160e/fv3K3MfIyAgnJ6caatHDn2Nqaip9+vShR48e/PjjjxQUFMjrW1RXJrnOR736+vo1+oMQnnJ1NFgvrHDgLoL2mqUJrh/NLV+1ahVjxowBHi4VXjj/MTMzk4kTJ3L//n1MTEzw8PBg3bp1DB06tMg5NmzYgCRJDB8+vNTrr1ixgq5du5b6ZHLmzJncuXMHfX19PDw82LhxIy+//HIleioIFaNQKLC2tmbUqFGMGjWKtLQ0Zs+ezfz583F3d+eNN97Az88Pf39/fHx8au2ERk0/LS0tycjIQKFQ4ODgwIMHD7h+/Tq2trbyiqBVXfaxPFJTU/Hz88PZ2ZlNmzZhaGhY420or8DAQHkF2eeff55vvvkGOzu7ar1mUFAQJiYmLFq0CAMDA/z9/encuTPTp0/H0NCQuLg4HBwcqvSGUqcnk06fPp158+ZhZWWFsbExXbp0Yfbs2TRq1KjUY3Jzc4s8Ek5LS8PFxUVMJhUqpo4H66WpK4F7TU8mrWwddUEQSiZJEv3792fkyJH4+fmxd+9etm7dyp49e7C2tmbQoEH4+fnRqVMnnRmJLi+VSsXly5fJy8vD29tbHrHOzs6Wa7WnpqZiZWUlT0atibz19PR0/P39MTc3Z/fu3TqThqNQKNi+fTv+/v7ytg0bNmBqaoqbmxsRERF8/vnnmJubc/r06Sr9PEiSVCTo3rVrF9999x0nT56kX79+pKSksHv3buzt7Tl37hz79+9n4sSJ5S65Wx46Hajv3buXjIwMWrRoQXR0NDNmzCAqKoqQkJBSV+maPn06M2bMKLZdBOpChT2lwXphtTVwF4G6INR+jwZJ8DCY3b9/P9u2bZODyYEDBzJ48GC6du2q8+mxKpWK4OBgVCpVmZVrHi37aG5ujoODA/Xq1cPMzKzKU4AyMzMZMmQISqWSv/76q9SVkrWhpED9Ubdu3aJJkyYcPHiQF154oUquW1BQgL6+PgUFBSQlJeHo6Mjdu3fp0KGDXIbzr7/+kkfxly5dyvr161m3bh2NGzeukjaAjgfqj0pJSaFx48YsXLiw1MU8xIi6UKVEsF6MLgfvmrSetEywGoQI1AWhDsvLy+PgwYNs27aNnTt3olAoGDBgAIMHD6Z79+46VxmmoKCgSHnJ8t5UPEnZx/LIzs7mlVdeIS8vj71795Y6EKot5QnUARwcHPjmm2946623nviaKpUKPT098vLyePnll3F2dmbq1Kk0bNiQRYsWMW/ePMaOHcs333xDYmIix44dY9SoUfz6669lph9Whm7fej7C2tqa5s2bl1kurDz1iwWh3J6CnPWKelwlmeoM5EUVG0EQNAwNDXnppZd46aWXWLp0KceOHWPz5s2MHz+e/Px8+vfvj7+/Pz179tR6XFBQUEBQUBBKpZL27dtXKD1DU/bR2dkZlUpFYmIicXFxBAUFoaenh4ODg5yrXdHc/ZycHEaMGEFWVhZ///23zgXp5XX//n0SExOrrEqVnp4eKpUKX19f3NzceOONN3BwcABg8ODBxMXF8cMPP7B9+3ZMTU2Ji4tj7ty5VR6kQy0bUc/IyKBRo0ZMnz6dd955p1zHiAWPhCohgvVaRYyoC8LTS6VSceLECbZs2cKOHTtIT0+nX79++Pv706tXrxqvU56fn8/FixcxMDCo0vKSarWa5ORkOa9drVbLQbudnd1jr5OXl8fIkSOJiYnhwIED2NjYVEm7qkJGRoY8KNu+fXsWLlxIz549sbW1xdbWlhkzZjBkyBCcnJyIiIjg448/Jj09nStXrlTZTdmiRYvYvHkze/bs+d/fhH8XO0pLS+PWrVvs2LGDli1b4uLiQteuXYGSU7aehE4H6h9++CEDBw6kcePGPHjwgGnTphEcHExoaKh8Z/M4IlAXqowI1msNEagLggAPA6szZ87IQXt8fDx9+vTBz8+PPn36YG7+uH/jTyYvL4+LFy9iZGREu3btqm3iqyRJpKamykF7bm4u9vb2ODo6Ym9vXywNKD8/n9GjRxMZGcnhw4ervVpKRQUGBtKzZ89i20ePHs3SpUvx9/cnKCiIlJQU6tevT+/evZk5cyb16tWrsjZMmTKFsLCwIiXCNdLS0kr8nV/VQTroeKA+bNgwjh07RmJiIg4ODjzzzDPMmjWLJk3K/2hdBOpClRLBeq0gAnVBEB6lVqu5cOECW7ZsYfv27dy/f58XX3wRPz8/+vXrJ4+aVpW8vDwuXLiAqakpbdu2rbGSkpIkkZGRIQftmZmZctlHa2trjI2NGTduHKGhoRw5cgRHR8caaVdtoRk1nzp1KidOnGDbtm1YW1ujUChQq9VkZ2fz/fffM2jQINq1a1ft7dHpQL0qiEBdqHIiWNd5IlAXBKEsarWay5cvs3XrVrZt20ZERATPP/88fn5+DBgwQA7MKis3N5cLFy5gbm5OmzZttFr3PSsrSw7aJ0yYQF5eHunp6fz555907NhRa+3SFZqJo4/at28fAwYMYNasWUyZMgVTU1MAzp07x+jRo/nhhx/o3bt3tbdPBOqCUBkiWNdpIlAXBKG8JEkiLCyMLVu2sG3bNkJDQ+nRowf+/v4MGDAAe3v7CgXtOTk5XLhwASsrK1q1aqUzizOpVComTpzI+fPnqVevHqdOnWLPnj306tVL203TGs3oOcAXX3xBeno6FhYWfPbZZ5ibm7No0SICAgJ4/fXXcXd3x8LCgunTp/Pmm2/Kq0dXNxGoC0JliWBdZ4lAXRCEypAkiZs3b8pBe3BwMN26dcPf359BgwZRr169MoP27OxsLly4gI2NDa1ataryfOXKUqvVBAQEcODAAQIDA2ncuDHJycmYmppqvSKOthQO0vv168edO3do1KgR9+/fR6VScfLkSWxtbdm6dSvLly8nIiKCpk2b0qNHDz755JNi56guunGbJwiCIAhCuS1ZsgRXV1eMjY3p1KkT586dK3P/zZs34+HhgbGxMW3btmXPnj011NLaRaFQ0KxZMz777DPOnTvH9evXGTBgAJs2baJ58+b06dOHJUuWcP/+fR4d58zKyuL8+fPY2dnpXJD+6aefsm/fPg4ePCgvxmNjY/PUBumAHGBHRUXh5OTEmTNn2L17N7/99htWVlZ4enoSExPDkCFD2LBhA8HBwWzYsKFGg3QQgbogCIIg1CobN24kICCAadOmcfHiRTw9PenTpw9xcXEl7n/q1CmGDx/OuHHjCAoKwt/fH39/f0JCQmq45bWLQqHAzc2NDz/8kJMnTxIZGckrr7zCn3/+SatWrXj++edZtGgRkZGRXLlyha1bt+Lo6IiHh4dOBelfffUV27dv5+DBgxUqxvE0mDZtGu3atSMqKgp9fX0MDAxo3749y5cvx9XVlQ4dOhAVFYWVlRWmpqbyk1NJkmospUkE6oIgCIJQiyxcuJDx48czduxYWrVqxS+//IKpqSkrV64scf8ffviBvn378tFHH9GyZUtmzpyJt7c3P/30Uw23vPZSKBS4uLjw7rvvEhgYyL179xg9ejSHDx/G09OTF198kb1792q7mUVIksSsWbNYv349Bw4coHnz5jV6/WPHjjFw4EDq16+PQqFgx44dxdr31Vdf4ezsjImJCb169eLGjRs11j6VSkW7du1o0aIFoaGh8kqxCoWCNm3a8Ouvv9KkSRNcXFxISUkpcmxN3oiJQF0QBEEQaglNyb/CEwCVSiW9evXi9OnTJR5z+vTpYhMG+/TpU+r+QtkUCgXOzs5MnDiRxYsXY2NjQ/fu3cnJyaFz58507tyZb7/9ltDQ0GLpMTVFkiTmzp3L8uXLOXDgAK1atarxNmRmZuLp6cmSJUtK/P7cuXP58ccf+eWXXzh79ixmZmb06dOHnJycammPWq0u8rWenh4DBw7k66+/xsjIiO7du5OXlyd/v2XLlixZsoTFixdjbW1dLW0qD32tXVkQBEEQhApJSEhApVIVW9ilXr16XLt2rcRjYmJiStw/Jiam2tr5tKhfvz5z5sxh3LhxSJJESkoKu3btYuvWrSxYsIDGjRvj5+fH4MGDa6xMoyRJLFq0iMWLF3Pw4EHatm1b7dcsSb9+/ejXr1+J39O08csvv8TPzw+A3377jXr16rFjxw6GDRtWpW0pnE++e/du7t69i42NDZ06daJXr16sWLGCd999l2effZYjR47IpRhbt25N69atgdLLOFY3EagLgiCUaBNg/Jh9qmfkRxCE2sHKyopx48YBD0fabWxsGD16NKNHjyYtLY0///yTrVu38sILL+Dk5ISfnx/+/v54e3tXS9AuSRJLlixh/vz5/P3333h7e1f5NapCZGQkMTExRZ70WFlZ0alTJ06fPl3lgbrmvZ4yZQq7d+/Gw8OD6OhoDA0NmTp1KoMGDeL777/n008/pXv37hw8eLDYKLo2gnQQqS+CIAiCUGvY29ujp6dHbGxske2xsbE4OTmVeIyTk1OF9heqhqWlJSNGjGDr1q3ExsYyZ84cHjx4wIABA2jdujWffPIJp0+fRqVSVcn1JEli2bJlzJo1i7/++kunFzPSPM2p7ic9hVOPli1bxs6dO9m1axf79u3jlVde4fr161hYWADQs2dPFixYQGJiIvPmzauyNjwpEagLgiAIQi1haGiIj48Phw4dkrep1WoOHTpEly5dSjymS5cuRfYHOHDgQKn7C1XP3NycV155hQ0bNhATE8MPP/xASkoKL7/8Mh4eHgQEBHDs2DEKCgoqdX5JklizZg1fffUVu3fvpmvXrlXcg9pF83kvPOkzNDSUQYMG0a5dO9asWcO8efNYunQpPXv2JDExkTt37vDss8+yd+9eZs2apa2mFyMCdUGorOXaboAgCE+jgIAAli1bxpo1awgLC2PChAlkZmYyduxYAEaNGsVnn30m7//uu++yb98+FixYwLVr15g+fTrnz59n8uTJ2urCU83U1BR/f3/Wrl1LdHQ0v/76K/n5+YwcOZJmzZoxZcoUDh8+TH5+frnOJ0kS69ev55NPPmHHjh107969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",
+                        "image/png": "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2LGDe++9l6VLl/Lf//3f5/6DUSgUCkVE+qwws7W1FZfLxerVq7nhhhtCxydMmMD111/PI4880hfbUigUil7h9OnT5Ofns3btWqZPn57weVdccQU33HADDz/8MHv37mXEiBFUVFQwevRoACzLoqCggEcffZSbb7454hzjx4/niiuu4Omnn466zsKFC9m1axfvvvtu9y5MoVAoFL1Cn+WEG4aBaZqhZipBkpOTWbduXcRzvF4vXq839NqyLGpra8nJyYnaYlyhUFxaSClpamqif//+oWZN3cXj8eDz+RJaq/PvFqfTidPpjHtuQ0MDEIh2J4KUknfffZc9e/bw2GOPAYR+33X8PalpGk6nk3Xr1kUU4Zs2baK8vJxf/epXcfeX6N4UCoVCcQ7oK4NyKaWcMmWKvPrqq+Xx48elYRhyxYoVUtM0OXz48Ijjg81e1Jf6Ul/q6+jRoz36vdPa2ioLHImtkZaW1uVYxwZU0TBNU95www1y2rRpccfW19fL1NRUabPZpNPplE8//XToPZ/PJ0tKSuQ3v/lNWVtbK71er/zlL38pATl79uyI8/3TP/2THDlyZMw1P/roI2mz2eSbb74Zd38KhUKhODf0qU/4/v37+eEPf8gHH3yArutcccUVDB8+nE2bNrFr164u4ztHwhsaGigpKeHoTyA9fmCq9/jCeVxLEZeaaal9vYWE+ITJfb2F885kPun1OZsaJWOL3dTX15ORkdHt8xsbG8nIyODoVZCuxxhnQvEGOHr0KOnp6aHjiUTC/+mf/ok33niDdevWMWDAgJhjLcviwIEDNDc388477/Dwww/z5z//mRkzZgCByPZNN93E1q1b0XWdmTNnomkaUkreeOONsLlaW1spLCzk/vvv5yc/+UnE9SoqKrjmmmtYvHgx9913X8y9KRQKheLc0acWhaWlpaxdu5aWlhYaGxspLCzk29/+NkOGDIk4Pto/fulOSE+KcMK54uLQfJ8bfOkXRypSyufQEdTFufvenG0KWroO6Ql8S9LT08NEeDxuv/12XnvtNT744IO4AhwC6SVDhw4FYNy4cezatYtly5aFRPiECRMoLy+noaEBn89HXl4ekydPZuLEiV3m+tOf/oTb7WbevHkR19q5cyfXXnstP/rRj5QAVygUij6mT91RgqSmplJYWEhdXR1vvvkmX/3qV/t6SwqFQtEtpJTc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",
                         "text/plain": [
                             "<Figure size 900x600 with 3 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAu4AAAEnCAYAAAD2EsYrAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAADvFElEQVR4nOydd3wc1dm2r5nZot67bMvdcpd7o5jgEkIAp8FLEsAONZhmJ1/AIYQSwCFvAiSElkIJJRCICbxAIMSAaTZgW7ItF0mW3GSrWr3t7syc74/VrrXSVlmunOv3E2ZnzzlzzqzKPc/c53kUIYRAIpFIJBKJRCKRnNSoJ3oCEolEIpFIJBKJJDRSuEskEolEIpFIJKcAUrhLJBKJRCKRSCSnAFK4SyQSiUQikUgkpwBSuEskEolEIpFIJKcAUrhLJBKJRCKRSCSnAFK4SyQSiUQikUgkpwBSuEskEolEIpFIJKcAUrhLJBKJRCKRSCSnAFK4SyQSiUQikUgkpwBSuEsGnG3btvHd736XvLw8oqKiyM3NZeHChTzyyCMnemrHnLfffpu77rrrRE9DIpFIJBLJaYgihBAnehKS04fPPvuMc845hyFDhnDFFVeQlZXFgQMH2LBhA+Xl5ezevftET/GYcsMNN/Doo48if6wkEolEIpEMNJYTPQHJ6cV9991HYmIiX375JUlJST7v1dbWDsg52tvbiY2N7XNcCEFXVxfR0dEDch6JRCKRSCSSkwlplZEMKOXl5YwfP76PaAfIyMgAYO/evSiKwjPPPNOnjaIoPlaTu+66C0VR2LFjB9///vdJTk7mjDPOAGDo0KF885vf5N1332X69OlER0fz5JNPAlBRUcH3vvc9UlJSiImJYfbs2bz11lt9zrdv3z4uvPBCYmNjycjIYMWKFbz77rsoisKHH37obffxxx/zve99jyFDhmC32xk8eDArVqygs7PT22bp0qU8+uij3nV4vjyYpsnDDz/M+PHjiYqKIjMzk2uvvZbGxsawr69EIpFIJJKvLjLiLhlQ8vLyWL9+PcXFxUyYMGHAxv3e977HqFGjuP/++31sKCUlJVx66aVce+21XH311YwZM4aamhrmzp1LR0cHN910E6mpqTz77LNceOGFvPrqq3zrW98C3JH7r33ta1RVVXHzzTeTlZXFiy++yAcffNDn/K+88godHR38+Mc/JjU1lS+++IJHHnmEyspKXnnlFQCuvfZaDh06xHvvvcdzzz3XZ4xrr72WZ555hmXLlnHTTTexZ88e/vjHP1JYWMinn36K1WodsOslkUgkEonkNERIJAPIf/7zH6FpmtA0TcyZM0f87Gc/E++++65wOp3eNnv27BGAePrpp/v0B8Sdd97pfX3nnXcKQFx66aV92ubl5QlAvPPOOz7Hb7nlFgGIjz/+2HustbVVDBs2TAwdOlQYhiGEEOJ3v/udAMS//vUvb7vOzk6Rn58vAPHBBx94j3d0dPQ5/+rVq4WiKGLfvn3eY8uXLxf+fqw+/vhjAYgXXnjB5/g777zj97hEIpFIJBJJb6RVRjKgLFy4kPXr13PhhReyZcsWfvOb37B48WJyc3N54403+j3udddd5/f4sGHDWLx4sc+xt99+m5kzZ3otNQBxcXFcc8017N27lx07dgDwzjvvkJuby4UXXuhtFxUVxdVXX93nPD198+3t7dTX1zN37lyEEBQWFoac/yuvvEJiYiILFy6kvr7e+zVt2jTi4uL8RvklEolEIpFIeiKFu2TAmTFjBmvWrKGxsZEvvviCVatW0drayne/+12vaI6UYcOGhX183759jBkzps/xsWPHet/3/DtixAgfHzrAyJEj+/Tdv38/S5cuJSUlhbi4ONLT0zn77LMBaG5uDjn/srIympubycjIID093eerra1twDbuSiQSiUQiOX2RHnfJMcNmszFjxgxmzJjB6NGjWbZsGa+88gpLly71294wjIBjBcoUczwyyBiGwcKFC2loaODWW28lPz+f2NhYDh48yNKlSzFNM+QYpmmSkZHBCy+84Pf99PT0gZ62RCKRSCSS0wwp3CXHhenTpwNQVVVFcnIyAE1NTT5tPJHwoyUvL4+SkpI+x3ft2uV93/Pvjh07EEL4RN1755rftm0bpaWlPPvss1x++eXe4++9916fc/SO3nsYMWIE//3vf5k3b55MVymRSCQSiaRfSKuMZED54IMP/BYfevvttwEYM2YMCQkJpKWl8dFHH/m0eeyxxwZkDt/4xjf44osvWL9+vfdYe3s7f/rTnxg6dCjjxo0DYPHixRw8eNDHe9/V1cWf//xnn/E0TQPwWZcQgt///vd9zu3JL9/7puTiiy/GMAx+9atf9emj63qf9hKJRCKRSCS9kRF3yYBy44030tHRwbe+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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAuAAAAEnCAYAAADo2/aYAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/bCgiHAAAACXBIWXMAAA9hAAAPYQGoP6dpAADNpUlEQVR4nOydeXxU5d32v/c5s2TfExLCvgYBZRWFxx1BuihdrbVFrFpbURAe24q+fV3btE9btYv62MWlWvV5bbG0PtaluFKlyhIgAiFAWAIh+zqTzMw5537/mMwwk8xMZkIggPfXTz4yZ865z31OErjOb677+gkppUShUCgUCoVCoVCcFLTBnoBCoVAoFAqFQvFpQglwhUKhUCgUCoXiJKIEuEKhUCgUCoVCcRJRAlyhUCgUCoVCoTiJKAGuUCgUCoVCoVCcRJQAVygUCoVCoVAoTiJKgCsUCoVCoVAoFCcRJcAVCoVCoVAoFIqTiBLgCoVCoVAoFArFSUQJcIVCoVAoFAqF4iSiBLgiJtu3b+fLX/4yI0eOJCkpieLiYi6//HJ+/etfD/bUTjivvvoq995772BPQ6FQKBQKxRmGkFLKwZ6E4tTkgw8+4JJLLmHEiBFcd911FBYWcujQITZs2MDevXvZs2fPYE/xhHLrrbfy6KOPon5FFAqFQqFQDCS2wZ6A4tTlRz/6EZmZmXz88cdkZWWFvVdXVzcg53C5XKSmpvbaLqWkq6uL5OTkATmPQqFQKBQKxamCsqAoorJ3714mT57cS3wDFBQUALB//36EEDz99NO99hFChFk47r33XoQQ7Nixg69//etkZ2fzH//xHwCMGjWKz33uc7z++uvMmjWL5ORknnjiCQD27dvHV77yFXJyckhJSeG8887jf//3f3ud78CBA1x55ZWkpqZSUFDAypUref311xFC8M477wT3e//99/nKV77CiBEjcDqdDB8+nJUrV9LZ2RncZ+nSpTz66KPB6wh8BbAsi0ceeYTJkyeTlJTEkCFDuPnmm2lubo77/ioUCoVCofh0oirgiqiMHDmSDz/8kPLycqZMmTJg437lK19h/Pjx/PjHPw6zd1RUVHDNNddw8803c9NNNzFx4kRqa2uZO3cubreb5cuXk5ubyzPPPMOVV17Jn//8Z77whS8A/kr6pZdeSk1NDStWrKCwsJDnn3+et99+u9f5X3rpJdxuN9/97nfJzc3lo48+4te//jXV1dW89NJLANx8880cOXKEN998k2effbbXGDfffDNPP/00119/PcuXL6eqqorf/OY3bNmyhX/961/Y7fYBu18KhUKhUCjOMKRCEYU33nhD6roudV2X559/vvz+978vX3/9den1eoP7VFVVSUA+9dRTvY4H5D333BN8fc8990hAXnPNNb32HTlypATka6+9Frb99ttvl4B8//33g9va29vl6NGj5ahRo6RpmlJKKX/xi19IQP71r38N7tfZ2SlLSkokIN9+++3gdrfb3ev8paWlUgghDxw4ENy2bNkyGelX5P3335eA/NOf/hS2/bXXXou4XaFQKBQKhSIUZUFRROXyyy/nww8/5Morr2Tr1q3813/9FwsXLqS4uJi//e1v/R73O9/5TsTto0ePZuHChWHbXn31Vc4999ygVQUgLS2Nb3/72+zfv58dO3YA8Nprr1FcXMyVV14Z3C8pKYmbbrqp13lCfeUul4uGhgbmzp2LlJItW7b0Of+XXnqJzMxMLr/8choaGoJfM2fOJC0tLWLVXaFQKBQKhSKAEuCKmMyePZs1a9bQ3NzMRx99xOrVq2lvb+fLX/5yUPwmyujRo+PefuDAASZOnNhr+6RJk4LvB/4/duzYMJ82wLhx43ode/DgQZYuXUpOTg5paWnk5+dz0UUXAdDa2trn/CsrK2ltbaWgoID8/Pywr46OjgFboKpQKBQKheLMRHnAFXHhcDiYPXs2s2fPZsKECVx//fW89NJLLF26NOL+pmlGHStassnJSDwxTZPLL7+cpqYmfvCDH1BSUkJqaiqHDx9m6dKlWJbV5xiWZVFQUMCf/vSniO/n5+cP9LQVCoVCoVCcQSgBrkiYWbNmAVBTU0N2djYALS0tYfsEKtPHy8iRI6moqOi1fdeuXcH3A//fsWMHUsqwKnjPrPLt27eze/dunnnmGZYsWRLc/uabb/Y6R89qeoCxY8fyz3/+k3nz5qmYRIVCoVAoFAmjLCiKqLz99tsRm9C8+uqrAEycOJGMjAzy8vJ47733wvZ57LHHBmQOn/nMZ/joo4/48MMPg9tcLhe//e1vGTVqFGeddRYACxcu5PDhw2He9K6uLn73u9+FjafrOkDYdUkp+eUvf9nr3IF88p4PF1/96lcxTZMHHnig1zGGYfTaX6FQKBQKhSIUVQFXROW2227D7XbzhS98gZKSErxeLx988AH/8z//w6hRo7j++usBuPHGG/nJT37CjTfeyKxZs3jvvffYvXv3gMzhzjvv5IUXXmDRokUsX76cnJwcnnnmGaqqqvjLX/6CpvmfIW+++WZ+85vfcM0117BixQqKior405/+RFJSEnCsml1SUsLYsWO54447OHz4MBkZGfzlL3+JmN89c+ZMAJYvX87ChQvRdZ2vfe1rXHTRRdx8882UlpZSVlbGggULsNvtVFZW8tJLL/HLX/6SL3/5ywNy/QqFQqFQKM5ABjWDRXFK849//EN+61vfkiUlJTItLU06HA45btw4edttt8na2trgfm63W95www0yMzNTpqeny69+9auyrq4uagxhfX19r3ONHDlSfvazn404j71798ovf/nLMisrSyYlJclzzz1XvvLKK73227dvn/zsZz8rk5OTZX5+vvzP//xP+Ze//EUCcsOGDcH9duzYIefPny/T0tJkXl6evOmmm+TWrVt7xSkahiFvu+02mZ+fL4UQvSIJf/vb38qZM2fK5ORkmZ6eLqdOnSq///3vyyNHjsR7ixUKhUKhUHwKEVJG8BgoFGcIjzzyCCtXrqS6upri4uLBno5CoVAoFAoFSoArzhg6OzvDFkV2dXUxffp0TNMcMEuMQqFQKBQKxfGiPOCKM4YvfvGLjBgxgmnTptHa2spzzz3Hrl27osYFKhQKhUKhUAwGSoArzhgWLlzI73//e/70pz9hmiZnnXUWL774IldfffVgT02hUCgUCoUiyKBbUA4fPswPfvAD/vGPf+B2uxk3bhxPPfVUMGtaoVAoFAqFQqE4kxjUCnhzczPz5s3jkksu4R//+Af5+flUVlYGm7soFAqFQqFQKBRnGoNaAb/zzjv517/+xfvvvz9YU1AoFAqFQqFQKE4qgyrAzzrrLBYuXEh1dTXvvvsuxcXF3HLLLdx0000R9/d4PHg8nuBry7JoamoiNzc3attwhUJxZiGlpL29naFDhwYbMSVKV1cXXq+3z/0cDkewmZNCoVAoFAPFoArwwD9sq1at4itf+Qoff/wxK1as4L//+7+57rrreu1/7733ct99953saSoUilOQQ4cOMWzYsISP6+rqojA5mdY49i0sLKSqqkqJcIVCoVAMKIMqwB0OB7NmzeKDDz4Iblu+fDkff/wxH374Ya/9e1bA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",
                         "text/plain": [
                             "<Figure size 900x600 with 3 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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OX/88ccLHUuv1zNx4kR8fHywsLCgevXqrFu3zvB8epnJtm3bqFatGubm5tStW5eLFy9m2s/69eupXLkyZmZmeHt7M23atEzPp6Sk8Omnn+Lh4YGZmRlly5Zl0aJFmdY5deoUtWvXxtLSkvr163P16lXDc+fOnaNJkyZYW1tjY2NDrVq1OHny5AudqyRJkpQ36eNqCyEMLenpo7TIpFwqimRiLj2Xk5MTP/30E+PGjePkyZMkJCTw7rvvMmjQIN56662nbnPmzBmOHDlCo0aNDMuWLFny3C/KiRMnsmzZMubOnctff/3FsGHD6NGjBwcOHMi03siRI5k2bRonTpzAycmJNm3akJqaCqQl1J06daJLly5cuHCBcePGMWbMGJYsWWLYvmfPnqxatYoffviBy5cvM2/ePEqUKJHpGKNHj2batGmcPHkStVpN3759Dc91794dd3d3Tpw4walTp/jss88M00hLkiRJBUuhUGRqSZekIktIUg4NHDhQlC9fXnTr1k1UrVpVJCcnZ1mndOnSwtTUVCiVSvH1119nem7Dhg3C19f3mftPTk4WlpaW4siRI5mWv/fee6Jr165CCCH27dsnALF69WrD8w8ePBAWFhZizZo1QgghunXrJpo2bZppHyNHjhSVKlUSQghx9epVAYjdu3c/NY70Y+zZs8ewbNu2bQIQSUlJQgghrK2txZIlS555LpIkSZIkSS9KtphLOTZ16lS0Wi1r167l559/xszMLMs6f/zxBydPnmTu3LnMmDGDVatWGZ5r3749V65ceeb+w8LCePz4MU2bNqVEiRKGn2XLlnH9+vVM69arV8/wu729Pb6+vobpmy9fvkxAQECm9QMCAggNDUWn03H27FlUKlWm1vynqVatmuF3V1dXAMNMdMOHD6dfv34EBgYyadKkLPFJkiRJkiS9KNn5U8qx69ev888//6DX67l58yZVq1bNso6Pjw8AVatWJTIyknHjxtG1a9cc7T8xMRGAbdu2ZelN/7SLgNyysLDI0XoZS1PSS3D0ej2QNm5ut27d2LZtGzt27GDs2LGsXr2a9u3b51uckiRJkiS9WmSLuZQjGo2GHj160LlzZ8aPH0+/fv0MrcfPotfrSUlJyfExKlWqhJmZGbdv36Zs2bKZfjw8PDKte+zYMcPvMTExXLt2jYoVKwJQsWJFDh8+nGn9w4cPU758eVQqFVWrVkWv12epW39R5cuXZ9iwYfz222+8/fbbLF68OE/7kyRJkiTp1SZbzKUcGT16NHFxcfzwww+UKFGC7du307dvX7Zu3QrAjz/+iKenJxUqVADg4MGDTJ06lSFDhhj2sXHjRkaNGvXMchZra2tGjBjBsGHD0Ov1NGjQgLi4OA4fPoyNjQ29evUyrPv111/j4OCAi4sLo0ePxtHRkeDgYAA+/vhj6tSpw/jx4+ncuTNHjx5l1qxZzJ49GwBvb2969epF3759+eGHH6hevTq3bt0iKiqKTp06Pfe1SEpKYuTIkXTo0AEfHx/u3LnDiRMneOedd3L12kqSJEmSJAGy86f0fPv27RNqtVr88ccfhmXh4eHCxsZGzJ49WwghxA8//CAqV64sLC0thY2NjahZs6aYPXu20Ol0hm0WL14snveR0+v1YsaMGcLX11eYmJgIJycn0bx5c3HgwAFDLIDYsmWLqFy5sjA1NRX+/v7i3Llzmfazbt06UalSJWFiYiI8PT3FlClTMj2flJQkhg0bJlxdXYWpqakoW7as+OmnnzIdIyYmxrD+mTNnBCDCw8NFSkqK6NKli/Dw8BCmpqbCzc1NDBo0yNAxVJIkSZIkKTcUQjwx160kFWL79++nSZMmxMTEYGdnZ+xwJEmSJEmS8o2sMZckSZIkSZKkQkAm5pIkSZIkSZJUCMhSFkmSJEmSJEkqBGSLuSRJkiRJkiQVAjIxlyRJkiRJkqRCQCbmkiRJkiRJklQIyMRckiRJkiRJkgoBmZhLkiRJkiRJUiEgE3NJkiRJkiRJKgRkYi5JkiRJkiRJhYBMzCVJkiRJkiSpEPg/kNgQJfE1qzQAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 900x600 with 3 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -2561,15 +2095,15 @@
             "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "14-torch_bartz09_60min_20init_2023-06-01_01-36-22\n"
+                        "14-torch_maans05_60min_20init_2023-06-01_10-10-59\n"
                     ]
                 }
             ],
             "source": [
                 "#| echo: false\n",
                 "import os\n",
                 "import copy\n",
@@ -2679,21 +2213,21 @@
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "ImportError",
-                    "evalue": "cannot import name 'CSVDataset' from 'spotPython.torch.dataframedataset' (/Users/bartz/miniforge3/envs/spotCondaEnv/lib/python3.10/site-packages/spotPython/torch/dataframedataset.py)",
+                    "evalue": "cannot import name 'CSVDataset' from 'spotPython.torch.dataframedataset' (/Users/bartz/.venv/lib/python3.10/site-packages/spotPython/torch/dataframedataset.py)",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[0;31mImportError\u001b[0m                               Traceback (most recent call last)",
                         "Cell \u001b[0;32mIn[24], line 2\u001b[0m\n\u001b[1;32m      1\u001b[0m \u001b[39mfrom\u001b[39;00m \u001b[39mtorch\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mutils\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mdata\u001b[39;00m \u001b[39mimport\u001b[39;00m DataLoader\n\u001b[0;32m----> 2\u001b[0m \u001b[39mfrom\u001b[39;00m \u001b[39mspotPython\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mtorch\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mdataframedataset\u001b[39;00m \u001b[39mimport\u001b[39;00m CSVDataset\n\u001b[1;32m      3\u001b[0m \u001b[39mfrom\u001b[39;00m \u001b[39msklearn\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mpreprocessing\u001b[39;00m \u001b[39mimport\u001b[39;00m OrdinalEncoder\n\u001b[1;32m      4\u001b[0m \u001b[39mfrom\u001b[39;00m \u001b[39msklearn\u001b[39;00m\u001b[39m.\u001b[39;00m\u001b[39mmodel_selection\u001b[39;00m \u001b[39mimport\u001b[39;00m train_test_split\n",
-                        "\u001b[0;31mImportError\u001b[0m: cannot import name 'CSVDataset' from 'spotPython.torch.dataframedataset' (/Users/bartz/miniforge3/envs/spotCondaEnv/lib/python3.10/site-packages/spotPython/torch/dataframedataset.py)"
+                        "\u001b[0;31mImportError\u001b[0m: cannot import name 'CSVDataset' from 'spotPython.torch.dataframedataset' (/Users/bartz/.venv/lib/python3.10/site-packages/spotPython/torch/dataframedataset.py)"
                     ]
                 }
             ],
             "source": [
                 "from torch.utils.data import DataLoader\n",
                 "from spotPython.torch.dataframedataset import CSVDataset\n",
                 "from sklearn.preprocessing import OrdinalEncoder\n",
@@ -4520,13 +4054,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `spotPython-0.2.7/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.2.9/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png` & `spotPython-0.2.9/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/spotModel.graffle` & `spotPython-0.2.9/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/spotModel.pdf` & `spotPython-0.2.9/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures/spotModel.png` & `spotPython-0.2.9/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_2880min_20init_2023-05-21_00-34-43_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_contour_0_2.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png` & `spotPython-0.2.9/notebooks/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/pyproject.toml` & `spotPython-0.2.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.2.7"
+version = "0.2.9"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
@@ -27,14 +27,17 @@
   "matplotlib",
   "numpy",
   "pandas",
   "plotly",
   "tabulate",
   "scikit-learn",
   "scipy",
+  "river",
+  "torch",
+  "torchmetrics"
 ]
 # dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://www.spotseven.de"
 Issues = "https://github.com/sequential-parameter-optimization/spotPython/issues"
 Repository = "https://github.com/sequential-parameter-optimization/spotPython"
```

### Comparing `spotPython-0.2.7/src/spotPython/budget/ocba.py` & `spotPython-0.2.9/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/build/kriging.py` & `spotPython-0.2.9/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/data/base.py` & `spotPython-0.2.9/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.2.9/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/data/torch_hyper_dict.json` & `spotPython-0.2.9/src/spotPython/data/torch_hyper_dict.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.789%*

 * *Differences: {"'Net_lin_reg'": "OrderedDict([('_L0', OrderedDict([('type', 'int'), ('default', 10), "*

 * *                  "('transform', 'None'), ('lower', 10), ('upper', 10)])), ('l1', "*

 * *                  "OrderedDict([('type', 'int'), ('default', 3), ('transform', "*

 * *                  "'transform_power_2_int'), ('lower', 3), ('upper', 8)])), ('dropout_prob', "*

 * *                  "OrderedDict([('type', 'float'), ('default', 0.01), ('transform', 'None'), "*

 * *                  "('lower', 0.0), ('upper', 0.9)])), ('lr_mult', Or […]*

```diff
@@ -156,15 +156,110 @@
             "default": 0.0,
             "lower": 0.0,
             "transform": "None",
             "type": "float",
             "upper": 1.0
         }
     },
+    "Net_lin_reg": {
+        "_L0": {
+            "default": 10,
+            "lower": 10,
+            "transform": "None",
+            "type": "int",
+            "upper": 10
+        },
+        "batch_size": {
+            "default": 4,
+            "lower": 1,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 4
+        },
+        "dropout_prob": {
+            "default": 0.01,
+            "lower": 0.0,
+            "transform": "None",
+            "type": "float",
+            "upper": 0.9
+        },
+        "epochs": {
+            "default": 4,
+            "lower": 4,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 9
+        },
+        "k_folds": {
+            "default": 1,
+            "lower": 1,
+            "transform": "None",
+            "type": "int",
+            "upper": 1
+        },
+        "l1": {
+            "default": 3,
+            "lower": 3,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 8
+        },
+        "lr_mult": {
+            "default": 1.0,
+            "lower": 0.1,
+            "transform": "None",
+            "type": "float",
+            "upper": 10.0
+        },
+        "optimizer": {
+            "class_name": "torch.optim",
+            "core_model_parameter_type": "str",
+            "default": "SGD",
+            "levels": [
+                "Adadelta",
+                "Adagrad",
+                "Adam",
+                "AdamW",
+                "SparseAdam",
+                "Adamax",
+                "ASGD",
+                "NAdam",
+                "RAdam",
+                "RMSprop",
+                "Rprop",
+                "SGD"
+            ],
+            "lower": 0,
+            "transform": "None",
+            "type": "factor",
+            "upper": 12
+        },
+        "patience": {
+            "default": 2,
+            "lower": 1,
+            "transform": "transform_power_2_int",
+            "type": "int",
+            "upper": 5
+        },
+        "sgd_momentum": {
+            "default": 0.0,
+            "lower": 0.0,
+            "transform": "None",
+            "type": "float",
+            "upper": 1.0
+        }
+    },
     "Net_vbdp": {
+        "_L0": {
+            "default": 64,
+            "lower": 64,
+            "transform": "None",
+            "type": "int",
+            "upper": 64
+        },
         "batch_size": {
             "default": 4,
             "lower": 1,
             "transform": "transform_power_2_int",
             "type": "int",
             "upper": 4
         },
@@ -190,15 +285,15 @@
             "upper": 1
         },
         "l1": {
             "default": 8,
             "lower": 8,
             "transform": "transform_power_2_int",
             "type": "int",
-            "upper": 13
+            "upper": 16
         },
         "lr_mult": {
             "default": 1.0,
             "lower": 0.1,
             "transform": "None",
             "type": "float",
             "upper": 10.0
@@ -227,15 +322,15 @@
             "upper": 12
         },
         "patience": {
             "default": 2,
             "lower": 1,
             "transform": "transform_power_2_int",
             "type": "int",
-            "upper": 9
+            "upper": 5
         },
         "sgd_momentum": {
             "default": 0.0,
             "lower": 0.0,
             "transform": "None",
             "type": "float",
             "upper": 1.0
```

### Comparing `spotPython-0.2.7/src/spotPython/design/spacefilling.py` & `spotPython-0.2.9/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/fun/hypersklearn.py` & `spotPython-0.2.9/src/spotPython/fun/hypersklearn.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/fun/hypertorch.py` & `spotPython-0.2.9/src/spotPython/fun/hypertorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,57 +60,76 @@
         z_res = np.array([], dtype=float)
         self.fun_control.update(fun_control)
         self.check_X_shape(X)
         var_dict = assign_values(X, self.fun_control["var_name"])
         # type information and transformations are considered in generate_one_config_from_var_dict:
         for config in generate_one_config_from_var_dict(var_dict, self.fun_control):
             print(f"\nconfig: {config}")
+            config_id = ''
+            for key in config:
+                config_id += str(config[key]) + "_"
+            config_id = config_id[:-1]
             if self.fun_control["prep_model"] is not None:
                 model = make_pipeline(self.fun_control["prep_model"], self.fun_control["core_model"](**config))
             else:
                 model = self.fun_control["core_model"](**config)
             try:
                 if self.fun_control["eval"] == "train_cv":
                     df_eval, _ = evaluate_cv(
                         model,
                         dataset=fun_control["train"],
                         shuffle=self.fun_control["shuffle"],
                         device=self.fun_control["device"],
                         show_batch_interval=self.fun_control["show_batch_interval"],
+                        task=self.fun_control["task"],
+                        writer=self.fun_control["writer"],
                     )
                 elif self.fun_control["eval"] == "test_cv":
                     df_eval, _ = evaluate_cv(
                         model,
                         dataset=fun_control["test"],
                         shuffle=self.fun_control["shuffle"],
                         device=self.fun_control["device"],
                         show_batch_interval=self.fun_control["show_batch_interval"],
+                        task=self.fun_control["task"],
+                        writer=self.fun_control["writer"],
                     )
                 elif self.fun_control["eval"] == "test_hold_out":
                     df_eval, _ = evaluate_hold_out(
                         model,
                         train_dataset=fun_control["train"],
                         shuffle=self.fun_control["shuffle"],
                         loss_function=self.fun_control["loss_function"],
                         metric=self.fun_control["metric_torch"],
                         test_dataset=fun_control["test"],
                         device=self.fun_control["device"],
                         show_batch_interval=self.fun_control["show_batch_interval"],
                         path=self.fun_control["path"],
+                        task=self.fun_control["task"],
+                        writer=self.fun_control["writer"],
+                        writerId=config_id,
                     )
                 else:  # eval == "train_hold_out"
                     df_eval, _ = evaluate_hold_out(
                         model,
                         train_dataset=fun_control["train"],
                         shuffle=self.fun_control["shuffle"],
                         loss_function=self.fun_control["loss_function"],
                         metric=self.fun_control["metric_torch"],
                         device=self.fun_control["device"],
                         show_batch_interval=self.fun_control["show_batch_interval"],
                         path=self.fun_control["path"],
+                        task=self.fun_control["task"],
+                        writer=self.fun_control["writer"],
+                        writerId=config_id,
                     )
             except Exception as err:
                 print(f"Error in fun_torch(). Call to evaluate_model failed. {err=}, {type(err)=}")
                 print("Setting df_eval to np.nan")
                 df_eval = np.nan
-            z_res = np.append(z_res, fun_control["weights"] * df_eval)
+            z_val = fun_control["weights"] * df_eval
+            if self.fun_control["writer"] is not None:
+                writer = self.fun_control["writer"]
+                writer.add_hparams(config, {"fun_torch: loss": z_val})
+                writer.flush()
+            z_res = np.append(z_res, z_val)
         return z_res
```

### Comparing `spotPython-0.2.7/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.2.9/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.2.9/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.2.9/src/spotPython/hyperparameters/optimizer.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/hyperparameters/values.py` & `spotPython-0.2.9/src/spotPython/hyperparameters/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,15 +595,15 @@
                 hyper_dict=RiverHyperDict,
                 filename=None)
     """
     fun_control.update({"core_model": core_model})
     if filename is None:
         new_hyper_dict = hyper_dict().load()
     else:
-        with open("river_hyper_dict.json", "r") as f:
+        with open(filename, "r") as f:
             new_hyper_dict = json.load(f)
     hyper_dict().load()
     fun_control.update({"core_model_hyper_dict": new_hyper_dict[core_model.__name__]})
     return fun_control
 
 
 def get_one_core_model_from_X(X, fun_control=None):
```

### Comparing `spotPython-0.2.7/src/spotPython/plot/contour.py` & `spotPython-0.2.9/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/plot/validation.py` & `spotPython-0.2.9/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/sklearn/traintest.py` & `spotPython-0.2.9/src/spotPython/sklearn/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/spot/spot.py` & `spotPython-0.2.9/src/spotPython/spot/spot.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,17 +385,17 @@
         if self.show_models:
             self.plot_model()
 
     def show_progress_if_needed(self, timeout_start):
         if not self.show_progress:
             return
         if isfinite(self.fun_evals):
-            progress_bar(progress=self.counter / self.fun_evals)
+            progress_bar(progress=self.counter / self.fun_evals, y=self.min_y)
         else:
-            progress_bar(progress=(time.time() - timeout_start) / (self.max_time * 60))
+            progress_bar(progress=(time.time() - timeout_start) / (self.max_time * 60), y=self.min_y)
 
     def generate_design(self, size, repeats, lower, upper):
         return self.design.scipy_lhd(n=size, repeats=repeats, lower=lower, upper=upper)
 
     def update_stats(self):
         """
         Update the following stats: 1. `min_y` 2. `min_X` 3. `counter`
```

### Comparing `spotPython-0.2.7/src/spotPython/torch/dataframedataset.py` & `spotPython-0.2.9/src/spotPython/torch/dataframedataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/torch/mapk.py` & `spotPython-0.2.9/src/spotPython/torch/mapk.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/torch/netcifar10.py` & `spotPython-0.2.9/src/spotPython/torch/netcifar10.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.2.9/src/spotPython/torch/netfashionMNIST.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/torch/netvbdp.py` & `spotPython-0.2.9/src/spotPython/torch/netvbdp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from torch import nn
 import spotPython.torch.netcore as netcore
 
 
 class Net_vbdp(netcore.Net_Core):
-    def __init__(self, l1, dropout_prob, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):
+    def __init__(self, _L0, l1, dropout_prob, lr_mult, batch_size, epochs, k_folds, patience, optimizer, sgd_momentum):
         super(Net_vbdp, self).__init__(
             lr_mult=lr_mult,
             batch_size=batch_size,
             epochs=epochs,
             k_folds=k_folds,
             patience=patience,
             optimizer=optimizer,
@@ -16,15 +16,17 @@
         # min 160 (= 2*2*2*20) neurons in first layer
         # min 80 (= 2*2*2*10) neurons in second layer
         # min 40 (= 2*2*2*5) neurons in third layer
         # min 20 (= 2*2*2*2*2) neurons in fourth layer
         l2 = l1 // 2
         l3 = l2 // 2
         l4 = l3 // 2
-        self.fc1 = nn.Linear(6112, l1)
+        # self.fc1 = nn.Linear(6112, l1)
+        # self.fc1 = nn.Linear(196, l1)
+        self.fc1 = nn.Linear(_L0, l1)
         self.fc2 = nn.Linear(l1, l2)
         self.fc3 = nn.Linear(l2, l3)
         self.fc4 = nn.Linear(l3, l4)
         self.fc5 = nn.Linear(l4, 11)
         self.relu = nn.ReLU()
         self.softmax = nn.Softmax(dim=1)
         self.dropout1 = nn.Dropout(p=dropout_prob)
```

### Comparing `spotPython-0.2.7/src/spotPython/torch/traintest.py` & `spotPython-0.2.9/src/spotPython/torch/traintest.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,82 +34,86 @@
     for attr in removed_attributes:
         attributes[attr] = getattr(net, attr)
     # 3. Remove the attributes:
     net = remove_attributes(net, removed_attributes)
     return attributes, net
 
 
-def train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval=10_000):
+def train_fold(net, trainloader, epochs, loss_function, optimizer, device, show_batch_interval=10_000, writer=None):
     for epoch in range(epochs):
         print(f"Epoch: {epoch + 1}")
         running_loss = 0.0
         epoch_steps = 0
         for i, data in enumerate(trainloader, 0):
-            inputs, labels = data
-            inputs, labels = inputs.to(device), labels.to(device)
+            input, target = data
+            input, target = input.to(device), target.to(device)
             optimizer.zero_grad()
-            outputs = net(inputs)
-            loss = loss_function(outputs, labels)
+            output = net(input)
+            loss = loss_function(output, target)
             loss.backward()
             torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
             optimizer.step()
             # print statistics
             running_loss += loss.item()
             epoch_steps += 1
             if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches
                 print("Batch: %5d. Training Loss (running): %.3f" % (i + 1, running_loss / epoch_steps))
+                # Log the running loss averaged per batch
+                if writer is not None:
+                    writer.add_scalars(
+                        "Validation Loss", {"Validation": running_loss / epoch_steps}, epoch * len(trainloader) + i
+                    )
                 running_loss = 0.0
 
 
-def validate_fold_or_hold_out(net, valloader, loss_function, metric, device):
+def validate_fold_or_hold_out(net, valloader, loss_function, metric, device, task):
     val_loss = 0.0
     val_steps = 0
     total = 0
     correct = 0
     metric.reset()
     for i, data in enumerate(valloader, 0):
+        # get batches
         with torch.no_grad():
-            inputs, labels = data
-            inputs, labels = inputs.to(device), labels.to(device)
-            outputs = net(inputs)
-            # print(f"outputs: {outputs}")
-            # print(f"labels: {labels}")
-            metric_value = metric.update(outputs, labels)
-            _, predicted = torch.max(outputs.data, 1)
-            # print(f"predicted: {predicted}")
-            total += labels.size(0)
-            # print(f"total: {total}")
-            correct += (predicted == labels).sum().item()
-            # print(f"correct: {correct}")
-            #
-            # print(f"predicted: {predicted}")
-            # print(f"labels: {labels}")
-            # metric_value = metric.update(predicted, labels).to(device)
-            # print(f"Accuracy on batch {i}: {acc}")
-            #
-            loss = loss_function(outputs, labels)
+            input, target = data
+            input, target = input.to(device), target.to(device)
+            output = net(input)
+            # print(f"target: {target}")
+            # print(f"output: {output}")
+            if task == "regression":
+                target = target.unsqueeze(1)
+                if target.shape == output.shape:
+                    loss = loss_function(output, target)
+                else:
+                    raise ValueError(f"Shapes of target and output do not match: {target.shape} vs {output.shape}")
+                metric_value = metric.update(output, target)
+            elif task == "classification":
+                loss = loss_function(output, target)
+                metric_value = metric.update(output, target)
+                _, predicted = torch.max(output.data, 1)
+                total += target.size(0)
+                correct += (predicted == target).sum().item()
+            else:
+                raise ValueError(f"Unknown task: {task}")
             val_loss += loss.cpu().numpy()
             val_steps += 1
-    accuracy = correct / total
     loss = val_loss / val_steps
     print(f"Loss on hold-out set: {loss}")
-    print(f"Accuracy on hold-out set: {accuracy}")
+    if task == "classification":
+        accuracy = correct / total
+        print(f"Accuracy on hold-out set: {accuracy}")
     # metric on all batches using custom accumulation
     metric_value = metric.compute()
-    print(f"Metric value on hold-out data: {metric_value}")
+    metric_name = type(metric).__name__
+    print(f"{metric_name} value on hold-out data: {metric_value}")
     return metric_value, loss
 
 
 def evaluate_cv(
-    net,
-    dataset,
-    shuffle=False,
-    num_workers=0,
-    device=None,
-    show_batch_interval=10_000,
+    net, dataset, shuffle=False, num_workers=0, device=None, show_batch_interval=10_000, task=None, writer=None
 ):
     lr_mult_instance = net.lr_mult
     epochs_instance = net.epochs
     batch_size_instance = net.batch_size
     k_folds_instance = net.k_folds
     loss_function_instance = net.loss_function
     optimizer_instance = net.optimizer
@@ -149,37 +153,45 @@
                 net,
                 trainloader,
                 epochs_instance,
                 loss_function,
                 optimizer,
                 device,
                 show_batch_interval=show_batch_interval,
+                writer=writer,
             )
             # Validate fold: use only loss for tuning
-            metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(net, valloader, loss_function, device)
+            metric_values[fold], loss_values[fold] = validate_fold_or_hold_out(
+                net, valloader, loss_function, device, task
+            )
         df_eval = sum(loss_values.values()) / len(loss_values.values())
         df_preds = np.nan
     except Exception as err:
         print(f"Error in Net_Core. Call to evaluate_cv() failed. {err=}, {type(err)=}")
         df_eval = np.nan
         df_preds = np.nan
     add_attributes(net, removed_attributes)
+    if writer is not None:
+        writer.flush()
     return df_eval, df_preds
 
 
 def evaluate_hold_out(
     net,
     train_dataset,
     shuffle,
     test_dataset=None,
     loss_function=None,
     metric=None,
     device=None,
     show_batch_interval=10_000,
     path=None,
+    task=None,
+    writer=None,
+    writerId=None,
 ):
     lr_mult_instance = net.lr_mult
     epochs_instance = net.epochs
     batch_size_instance = net.batch_size
     optimizer_instance = net.optimizer
     patience_instance = net.patience
     sgd_momentum_instance = net.sgd_momentum
@@ -214,28 +226,42 @@
         best_val_loss = float("inf")
         counter = 0
         # We only have "one fold" which is trained for several epochs
         # (we do not have to reset the weights for each fold):
         for epoch in range(epochs_instance):
             print(f"Epoch: {epoch + 1}")
             # training loss from one epoch:
-            _ = train_hold_out(
+            training_loss = train_hold_out(
                 net=net,
                 trainloader=trainloader,
                 batch_size=batch_size_instance,
                 loss_function=loss_function,
                 optimizer=optimizer,
                 device=device,
                 show_batch_interval=show_batch_interval,
+                task=task,
+                writer=writer,
             )
             # TODO: scheduler.step()
             # Early stopping check. Calculate validation loss from one epoch:
-            val_accuracy, val_loss = validate_fold_or_hold_out(
-                net, valloader=valloader, loss_function=loss_function, metric=metric, device=device
+            metric_val, val_loss = validate_fold_or_hold_out(
+                net, valloader=valloader, loss_function=loss_function, metric=metric, device=device, task=task
             )
+            # Log the running loss averaged per batch
+            metric_name = "Metric"
+            if metric is None:
+                metric_name = type(metric).__name__
+                print(f"{metric_name} value on hold-out data: {metric_val}")
+            if writer is not None:
+                writer.add_scalars(
+                    "evaluate_hold_out: Train & Val Loss and Val Metric" + writerId,
+                    {"Train loss": training_loss, "Val loss": val_loss, metric_name: metric_val},
+                    epoch + 1,
+                )
+                writer.flush()
             if val_loss < best_val_loss:
                 best_val_loss = val_loss
                 counter = 0
                 # save model:
                 if path is not None:
                     torch.save(net.state_dict(), path)
             else:
@@ -246,14 +272,16 @@
         df_eval = val_loss
         df_preds = np.nan
     except Exception as err:
         print(f"Error in Net_Core. Call to evaluate_hold_out() failed. {err=}, {type(err)=}")
         df_eval = np.nan
         df_preds = np.nan
     add_attributes(net, removed_attributes)
+    if writer is not None:
+        writer.flush()
     print(f"Returned to Spot: Validation loss: {df_eval}")
     print("----------------------------------------------")
     return df_eval, df_preds
 
 
 def create_train_val_data_loaders(dataset, batch_size, shuffle, num_workers=0):
     test_abs = int(len(dataset) * 0.6)
@@ -273,52 +301,91 @@
     )
     testloader = torch.utils.data.DataLoader(
         test_dataset, batch_size=int(batch_size), shuffle=shuffle, num_workers=num_workers
     )
     return trainloader, testloader
 
 
-def train_hold_out(net, trainloader, batch_size, loss_function, optimizer, device, show_batch_interval=10_000):
+def train_hold_out(
+    net,
+    trainloader,
+    batch_size,
+    loss_function,
+    optimizer,
+    device,
+    show_batch_interval=10_000,
+    task=None,
+    writer=None,
+):
     running_loss = 0.0
     epoch_steps = 0
-    for i, data in enumerate(trainloader, 0):
-        inputs, labels = data
-        inputs, labels = inputs.to(device), labels.to(device)
+    for batch_nr, data in enumerate(trainloader, 0):
+        input, target = data
+        input, target = input.to(device), target.to(device)
         optimizer.zero_grad()
-        outputs = net(inputs)
-        loss = loss_function(outputs, labels)
+        output = net(input)
+        if task == "regression":
+            target = target.unsqueeze(1)
+            if target.shape == output.shape:
+                loss = loss_function(output, target)
+            else:
+                raise ValueError(f"Shapes of target and output do not match: {target.shape} vs {output.shape}")
+        elif task == "classification":
+            loss = loss_function(output, target)
+        else:
+            raise ValueError(f"Unknown task: {task}")
         loss.backward()
         torch.nn.utils.clip_grad_norm_(net.parameters(), max_norm=1.0)
         optimizer.step()
         running_loss += loss.item()
         epoch_steps += 1
-        if i % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches
+        if batch_nr % show_batch_interval == (show_batch_interval - 1):  # print every show_batch_interval mini-batches
             print(
                 "Batch: %5d. Batch Size: %d. Training Loss (running): %.3f"
-                % (i + 1, int(batch_size), running_loss / epoch_steps)
+                % (batch_nr + 1, int(batch_size), running_loss / epoch_steps)
             )
+            # Log the running loss averaged per batch
+            if writer is not None:
+                writer.add_scalars(
+                    "Training Loss (running)", {"Training Loss (running)": running_loss / epoch_steps}, batch_nr + 1
+                )
             running_loss = 0.0
+    # if writer is not None:
+    #     writer.flush()
     return loss.item()
 
 
-def train_tuned(net, train_dataset, shuffle, loss_function, metric, device=None, show_batch_interval=10_000, path=None):
+def train_tuned(
+    net,
+    train_dataset,
+    shuffle,
+    loss_function,
+    metric,
+    device=None,
+    show_batch_interval=10_000,
+    path=None,
+    task=None,
+    writer=None,
+):
     evaluate_hold_out(
         net=net,
         train_dataset=train_dataset,
         shuffle=shuffle,
         test_dataset=None,
         loss_function=loss_function,
         metric=metric,
         device=device,
         show_batch_interval=show_batch_interval,
         path=path,
+        task=task,
+        writer=writer,
     )
 
 
-def test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None, path=None):
+def test_tuned(net, shuffle, test_dataset=None, loss_function=None, metric=None, device=None, path=None, task=None):
     batch_size_instance = net.batch_size
     removed_attributes, net = get_removed_attributes_and_base_net(net)
     if path is not None:
         net.load_state_dict(torch.load(path))
         net.eval()
     try:
         device = getDevice(device=device)
@@ -328,15 +395,15 @@
                 print("We will use", torch.cuda.device_count(), "GPUs!")
                 net = nn.DataParallel(net)
         net.to(device)
         valloader = torch.utils.data.DataLoader(
             test_dataset, batch_size=int(batch_size_instance), shuffle=shuffle, num_workers=0
         )
         metric_value, loss = validate_fold_or_hold_out(
-            net, valloader=valloader, loss_function=loss_function, metric=metric, device=device
+            net, valloader=valloader, loss_function=loss_function, metric=metric, device=device, task=task
         )
         df_eval = loss
         df_metric = metric_value
         df_preds = np.nan
     except Exception as err:
         print(f"Error in Net_Core. Call to test_tuned() failed. {err=}, {type(err)=}")
         df_eval = np.nan
```

### Comparing `spotPython-0.2.7/src/spotPython/utils/aggregate.py` & `spotPython-0.2.9/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/utils/compare.py` & `spotPython-0.2.9/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/utils/convert.py` & `spotPython-0.2.9/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/utils/device.py` & `spotPython-0.2.9/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/utils/eda.py` & `spotPython-0.2.9/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/utils/metrics.py` & `spotPython-0.2.9/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/utils/progress.py` & `spotPython-0.2.9/src/spotPython/utils/progress.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from sys import stdout
 
 
-def progress_bar(progress: float, bar_length: int = 10, message: str = "spotPython tuning:") -> None:
+def progress_bar(progress: float, bar_length: int = 10, message: str = "spotPython tuning:", y=None) -> None:
     """
     Displays or updates a console progress bar.
 
     Args:
         progress (float): a float between 0 and 1. Any int will be converted to a float.
             A value under 0 represents a halt.
             A value at 1 or bigger represents 100%.
         bar_length (int): length of the progress bar
         message (str): message text to display
     """
     status = ""
+    if y is not None:
+        message = f"{message} {y}"
     if progress < 0:
         progress = 0
         status = "Halt...\r\n"
     elif progress >= 1:
         progress = 1
         status = "Done...\r\n"
     block = int(round(bar_length * progress))
-    text = f"{message} [{'#' * block + '-' * (bar_length - block)}] {progress * 100:.2f}% {status}\r"
+    text = f"{message} [{'#' * block + '-' * (bar_length - block)}] {progress * 100:.2f}% {status}\r\n"
     stdout.write(text)
     stdout.flush()
```

### Comparing `spotPython-0.2.7/src/spotPython/utils/repair.py` & `spotPython-0.2.9/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython/utils/transform.py` & `spotPython-0.2.9/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.2.9/src/spotPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.2.7
+Version: 0.2.9
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.2.7/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.2.9/src/spotPython.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,20 @@
 notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
 notebooks/15_spot_hpt_sklearn_regression.ipynb
 notebooks/16_spot_hpt_sklearn_multiclass_classification_randomforest.ipynb
 notebooks/17_spot_hpt_sklearn_multiclass_classification_xgb.ipynb
 notebooks/18_spot_hpt_sklearn_multiclass_classification_svc.ipynb
 notebooks/19_spot_hpt_sklearn_multiclass_classification_knn.ipynb
 notebooks/20_spot_torch_vbdp.ipynb
+notebooks/20_spot_torch_vbdp_big_09.ipynb
+notebooks/20_spot_torch_vbdp_maans03.ipynb
+notebooks/21_spot_torch_vbdp.ipynb
+notebooks/22_spot_torch_vbdp.ipynb
+notebooks/23_spot_torch_vbdp.ipynb
+notebooks/24_spot_torch_regression.ipynb
 notebooks/data.json
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_1.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_2.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_0_4.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_2.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_1_4.pdf
 notebooks/figures14-torch_maans03_1440min_20init_2023-05-19_22-36-49_contour_2_4.pdf
@@ -148,14 +154,15 @@
 src/spotPython/data/__init__.py
 src/spotPython/data/base.py
 src/spotPython/data/sklearn_hyper_dict.json
 src/spotPython/data/sklearn_hyper_dict.py
 src/spotPython/data/torch_hyper_dict.json
 src/spotPython/data/torch_hyper_dict.py
 src/spotPython/data/torchdata.py
+src/spotPython/data/vbdp.py
 src/spotPython/design/designs.py
 src/spotPython/design/factorial.py
 src/spotPython/design/spacefilling.py
 src/spotPython/fun/hypersklearn.py
 src/spotPython/fun/hypertorch.py
 src/spotPython/fun/objectivefunctions.py
 src/spotPython/hyperparameters/categorical.py
@@ -166,14 +173,15 @@
 src/spotPython/sklearn/traintest.py
 src/spotPython/spot/spot.py
 src/spotPython/torch/dataframedataset.py
 src/spotPython/torch/mapk.py
 src/spotPython/torch/netcifar10.py
 src/spotPython/torch/netcore.py
 src/spotPython/torch/netfashionMNIST.py
+src/spotPython/torch/netregression.py
 src/spotPython/torch/netvbdp.py
 src/spotPython/torch/traintest.py
 src/spotPython/utils/aggregate.py
 src/spotPython/utils/classes.py
 src/spotPython/utils/compare.py
 src/spotPython/utils/convert.py
 src/spotPython/utils/device.py
```

### Comparing `spotPython-0.2.7/test/test_aggregate_mean_var.py` & `spotPython-0.2.9/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_build_Psi.py` & `spotPython-0.2.9/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_build_U.py` & `spotPython-0.2.9/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_build_psi_vec.py` & `spotPython-0.2.9/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_evaluate_new_X.py` & `spotPython-0.2.9/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_evaluate_new_solutions.py` & `spotPython-0.2.9/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_extract_from_bounds.py` & `spotPython-0.2.9/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_generate_design.py` & `spotPython-0.2.9/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_infill.py` & `spotPython-0.2.9/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_nat_to_cod.py` & `spotPython-0.2.9/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_nat_to_cod_init.py` & `spotPython-0.2.9/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_ocba.py` & `spotPython-0.2.9/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_repair_non_numeric.py` & `spotPython-0.2.9/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_set_de_bounds.py` & `spotPython-0.2.9/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_show_progress.py` & `spotPython-0.2.9/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_suggest_new_X.py` & `spotPython-0.2.9/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.2.7/test/test_update_surrogate.py` & `spotPython-0.2.9/test/test_update_surrogate.py`

 * *Files identical despite different names*

