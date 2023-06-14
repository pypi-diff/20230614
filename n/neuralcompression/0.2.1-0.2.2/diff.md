# Comparing `tmp/neuralcompression-0.2.1.tar.gz` & `tmp/neuralcompression-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralcompression-0.2.1.tar", last modified: Wed Jan 12 14:55:10 2022, max compression
+gzip compressed data, was "neuralcompression-0.2.2.tar", last modified: Wed Jun 14 14:01:37 2023, max compression
```

## Comparing `neuralcompression-0.2.1.tar` & `neuralcompression-0.2.2.tar`

### file list

```diff
@@ -1,237 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.478005 neuralcompression-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.454003 neuralcompression-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.454003 neuralcompression-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/ISSUE_TEMPLATE/bug_template.md
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/ISSUE_TEMPLATE/enhancement_template.md
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.454003 neuralcompression-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.github/workflows/publish-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     6604 2022-01-12 14:55:10.478005 neuralcompression-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5812 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.454003 neuralcompression-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.454003 neuralcompression-0.2.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)   612582 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/examples/image.png
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/examples/plot_image_compression.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/data.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/distributions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/entropy_coders.rst
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/functional.rst
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/layers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/docs/source/models.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/neuralcompression/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/neuralcompression/data/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/data/_clic_2020_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     6510 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/data/_clic_2020_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     3561 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/data/_kodak.py
--rw-r--r--   0 runner    (1001) docker     (121)     5755 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/data/_vimeo_90k_septuplet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/neuralcompression/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/distributions/_noisy_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/distributions/_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/neuralcompression/entropy_coders/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/entropy_coders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13494 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)    11539 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/codecs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11849 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/coder.py
--rw-r--r--   0 runner    (1001) docker     (121)    21304 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/entropy_coders/jax_arithemetic_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/neuralcompression/ext/
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/ext/_extension_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/ext/pmf_to_quantized_cdf_py.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.462004 neuralcompression-0.2.1/neuralcompression/functional/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6625 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_count_flops.py
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_dense_image_warp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_estimate_tails.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_hsv_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_information_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_log_cdf.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_log_expm1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_log_ndtr.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_log_survival_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_lower_bound.py
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_lower_tail.py
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_lpips.py
--rw-r--r--   0 runner    (1001) docker     (121)     8945 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_multiscale_structural_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_ndtr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_optical_flow_to_color.py
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_pmf_to_quantized_cdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_quantization_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_soft_round.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_soft_round_conditional_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_soft_round_inverse.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_survival_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/functional/_upper_tail.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.466004 neuralcompression-0.2.1/neuralcompression/layers/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_analysis_transformation_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)    14907 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_continuous_entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)     8481 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_generalized_divisive_normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_hyper_analysis_transformation_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_hyper_synthesis_transformation_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     3485 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_non_negative_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_rate_mse_distortion_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/_synthesis_transformation_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     4045 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/layers/gdn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.466004 neuralcompression-0.2.1/neuralcompression/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6594 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/metrics/distortion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.466004 neuralcompression-0.2.1/neuralcompression/models/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_factorized_prior_autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.466004 neuralcompression-0.2.1/neuralcompression/models/_hific/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/_channel_norm_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/_hific_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/_hific_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4067 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/_hific_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/_least_squares_adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/_non_saturating_adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hific/_weighted_rate_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6132 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_mean_scale_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_prior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/_scale_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)    26738 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/deep_video_compression.py
--rw-r--r--   0 runner    (1001) docker     (121)    22525 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/neuralcompression/models/scale_hyperprior.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-12 14:55:10.000000 neuralcompression-0.2.1/neuralcompression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.458004 neuralcompression-0.2.1/neuralcompression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6604 2022-01-12 14:55:10.000000 neuralcompression-0.2.1/neuralcompression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8641 2022-01-12 14:55:10.000000 neuralcompression-0.2.1/neuralcompression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 14:55:10.000000 neuralcompression-0.2.1/neuralcompression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-01-12 14:55:10.000000 neuralcompression-0.2.1/neuralcompression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-12 14:55:10.000000 neuralcompression-0.2.1/neuralcompression.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.466004 neuralcompression-0.2.1/projects/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.466004 neuralcompression-0.2.1/projects/deep_video_compression/
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.466004 neuralcompression-0.2.1/projects/deep_video_compression/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/deep_video_compression/config/mode/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/mode/submitit_multi_node.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/mode/submitit_single_node.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/deep_video_compression/config/training_stages/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/training_stages/s1_motion_estimation.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/training_stages/s2_motion_compression.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/training_stages/s3_motion_compensation.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/training_stages/s4_total_2frame.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/config/training_stages/s5_total.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/data_module.py
--rw-r--r--   0 runner    (1001) docker     (121)    12180 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/dvc_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5761 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/deep_video_compression/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/config/base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/config/mode/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/config/mode/submitit_multi_node.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/config/mode/submitit_single_node.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5047 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/scale_hyperprior.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/tests/test_scale_hyperprior_lightning.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/train.py
--rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/scale_hyperprior_lightning/vimeo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.450003 neuralcompression-0.2.1/projects/variational_image_compression/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/variational_image_compression/lightning/
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/lightning/_factorized_prior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/lightning/_mean_scale_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/lightning/_prior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/lightning/_scale_hyperprior_autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/projects/variational_image_compression/test/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/test/test_factorized_prior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/test/test_mean_scale_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/projects/variational_image_compression/test/test_scale_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-01-12 14:55:10.478005 neuralcompression-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.470004 neuralcompression-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/data/test_clic_2020_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/data/test_clic_2020_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/data/test_kodak.py
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/data/test_vimeo_90k_septuplet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.474005 neuralcompression-0.2.1/tests/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/distributions/test_noisy_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/distributions/test_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.474005 neuralcompression-0.2.1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5189 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_count_flops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_dense_image_warp.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_estimate_tails.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_hsv_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_information_content.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_log_cdf.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_log_expm1.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_log_ndtr.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_log_survival_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_lower_bound.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_lower_tail.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_lpips.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_multiscale_structural_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_ndtr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_optical_flow_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_pmf_to_quantized_cdf.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_quantization_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_soft_round.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_soft_round_conditional_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_soft_round_inverse.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_survival_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/functional/test_upper_tail.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.474005 neuralcompression-0.2.1/tests/layers/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_analysis_transformation_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     7330 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_continuous_entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_generalized_divisive_normalization.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_hyper_analysis_transformation_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_hyper_synthesis_transformation_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_non_negative_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_rate_mse_distortion_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/layers/test_synthesis_transformation_2d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.478005 neuralcompression-0.2.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.478005 neuralcompression-0.2.1/tests/models/_hific/
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/_hific/test_hific_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/_hific/test_hific_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/_hific/test_hific_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/test_factorized_prior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/test_mean_scale_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/test_prior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/models/test_scale_hyperprior_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)    16286 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/test_entropy_coders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/test_layers_gdn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/test_scale_hyperprior.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 14:55:10.478005 neuralcompression-0.2.1/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)    12503 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tutorials/Flop_Count_Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    83884 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tutorials/Metrics_Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  1191300 2022-01-12 14:54:58.000000 neuralcompression-0.2.1/tutorials/image_compression.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.215824 neuralcompression-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.183824 neuralcompression-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.183824 neuralcompression-0.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/ISSUE_TEMPLATE/bug_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/ISSUE_TEMPLATE/enhancement_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.183824 neuralcompression-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.github/workflows/publish-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-14 14:01:37.215824 neuralcompression-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.183824 neuralcompression-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.187824 neuralcompression-0.2.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   612582 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/examples/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/examples/plot_image_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.187824 neuralcompression-0.2.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/distributions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/entropy_coders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/layers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/docs/source/models.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.187824 neuralcompression-0.2.2/neuralcompression/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.187824 neuralcompression-0.2.2/neuralcompression/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/data/_clic_2020_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/data/_clic_2020_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/data/_kodak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/data/_vimeo_90k_septuplet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.187824 neuralcompression-0.2.2/neuralcompression/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/distributions/_noisy_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/distributions/_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.191824 neuralcompression-0.2.2/neuralcompression/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_count_flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_dense_image_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_estimate_tails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_hsv_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_information_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_log_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_log_expm1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_log_ndtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_log_survival_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_lower_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_lower_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_multiscale_structural_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_ndtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_optical_flow_to_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_quantization_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_soft_round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_soft_round_conditional_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_soft_round_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_survival_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/functional/_upper_tail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.191824 neuralcompression-0.2.2/neuralcompression/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_analysis_transformation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_continuous_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_generalized_divisive_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_hyper_analysis_transformation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_hyper_synthesis_transformation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_non_negative_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_rate_mse_distortion_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/_synthesis_transformation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/layers/gdn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/neuralcompression/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/metrics/distortion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/neuralcompression/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_factorized_prior_autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/neuralcompression/models/_hific/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/_channel_norm_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/_hific_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/_hific_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/_hific_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/_least_squares_adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/_non_saturating_adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hific/_weighted_rate_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_mean_scale_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_prior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/_scale_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26738 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/deep_video_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/neuralcompression/models/scale_hyperprior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 14:01:37.000000 neuralcompression-0.2.2/neuralcompression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.187824 neuralcompression-0.2.2/neuralcompression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-14 14:01:37.000000 neuralcompression-0.2.2/neuralcompression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-06-14 14:01:37.000000 neuralcompression-0.2.2/neuralcompression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:01:37.000000 neuralcompression-0.2.2/neuralcompression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-14 14:01:37.000000 neuralcompression-0.2.2/neuralcompression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 14:01:37.000000 neuralcompression-0.2.2/neuralcompression.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/projects/bits_back_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/projects/bits_back_diffusion/bits_back_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/bits_back_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26243 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/bits_back_diffusion/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/bits_back_diffusion/script_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/compute_vlb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/projects/bits_back_diffusion/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/compute_vlb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.195824 neuralcompression-0.2.2/projects/bits_back_diffusion/config/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/data/cifar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/data/imagenet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/bits_back_diffusion/config/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/diffusion/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/diffusion/respaced.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/encode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/bits_back_diffusion/config/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/evaluator/cifar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/evaluator/imagenet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/bits_back_diffusion/config/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/mode/submitit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/bits_back_diffusion/config/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/model/cifar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/model/imagenet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/config/train.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/bits_back_diffusion/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/bits_back_diffusion/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/deep_video_compression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/deep_video_compression/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/deep_video_compression/config/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/mode/submitit_multi_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/mode/submitit_single_node.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/deep_video_compression/config/training_stages/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/training_stages/s1_motion_estimation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/training_stages/s2_motion_compression.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/training_stages/s3_motion_compensation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/training_stages/s4_total_2frame.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/config/training_stages/s5_total.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/dvc_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/deep_video_compression/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/jax_entropy_coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21306 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/jax_arithmetic_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/jax_entropy_coders/test_entropy_coders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.199824 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/config/base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/config/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/config/mode/submitit_multi_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/config/mode/submitit_single_node.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/scale_hyperprior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/tests/test_scale_hyperprior_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/scale_hyperprior_lightning/vimeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/analysis_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/analysis_transform/elic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/analysis_transform/gdn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/datamodule/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/datamodule/kinetics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/datamodule/vimeo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/mode/submitit_multi_node.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/optim/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/optim/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/optim/lion.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/scheduler/cosine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/scheduler/linearrampcosine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/scheduler/linearramplinear.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/scheduler/linearwarmupcosine.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/synthesis_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/synthesis_transform/elic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/synthesis_transform/gdn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/config/test_datamodule/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/test_datamodule/uvg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/config/train_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/datamodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/datamodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/datamodules/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/datamodules/uvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/datamodules/video_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/datamodules/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.203824 neuralcompression-0.2.2/projects/torch_vct/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)   120010 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/fig/vct_rd.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/model_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/model_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/model_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.207824 neuralcompression-0.2.2/projects/torch_vct/neural/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/neural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/neural/bottlenecks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29693 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/neural/entropy_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/neural/entropy_model_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/neural/layers_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/neural/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/neural/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.207824 neuralcompression-0.2.2/projects/torch_vct/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.207824 neuralcompression-0.2.2/projects/torch_vct/tests/neural/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/tests/neural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/tests/neural/test_entropy_model_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/tests/neural/test_layers_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/tests/neural/test_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.207824 neuralcompression-0.2.2/projects/torch_vct/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/utils/checkpoint_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/utils/datavis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/utils/hydra_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/torch_vct/utils/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.183824 neuralcompression-0.2.2/projects/variational_image_compression/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.207824 neuralcompression-0.2.2/projects/variational_image_compression/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/lightning/_factorized_prior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/lightning/_mean_scale_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/lightning/_prior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/lightning/_scale_hyperprior_autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.207824 neuralcompression-0.2.2/projects/variational_image_compression/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/test/test_factorized_prior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/test/test_mean_scale_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/projects/variational_image_compression/test/test_scale_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 14:01:37.215824 neuralcompression-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.207824 neuralcompression-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.211824 neuralcompression-0.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/data/test_clic_2020_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/data/test_clic_2020_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/data/test_kodak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/data/test_vimeo_90k_septuplet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.211824 neuralcompression-0.2.2/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/distributions/test_noisy_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/distributions/test_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.211824 neuralcompression-0.2.2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_count_flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_dense_image_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_estimate_tails.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_hsv_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_information_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_log_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_log_expm1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_log_ndtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_log_survival_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_lower_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_lower_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_multiscale_structural_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_ndtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_optical_flow_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_quantization_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_soft_round.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_soft_round_conditional_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_soft_round_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_survival_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/functional/test_upper_tail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.215824 neuralcompression-0.2.2/tests/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_analysis_transformation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_continuous_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_generalized_divisive_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_hyper_analysis_transformation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_hyper_synthesis_transformation_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_non_negative_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_rate_mse_distortion_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/layers/test_synthesis_transformation_2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.215824 neuralcompression-0.2.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.215824 neuralcompression-0.2.2/tests/models/_hific/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/_hific/test_hific_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/_hific/test_hific_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/_hific/test_hific_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/test_factorized_prior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/test_mean_scale_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/test_prior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/models/test_scale_hyperprior_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/test_layers_gdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/test_scale_hyperprior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:37.215824 neuralcompression-0.2.2/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tutorials/Flop_Count_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    83884 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tutorials/Metrics_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1191300 2023-06-14 14:01:26.000000 neuralcompression-0.2.2/tutorials/image_compression.ipynb
```

### Comparing `neuralcompression-0.2.1/.github/CODE_OF_CONDUCT.md` & `neuralcompression-0.2.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/.github/CONTRIBUTING.md` & `neuralcompression-0.2.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/.github/workflows/build-and-test.yml` & `neuralcompression-0.2.2/.github/workflows/build-and-test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
     name: Build
     strategy:
       max-parallel: 4
       matrix:
         platform: [ubuntu-latest]
-        python-version: [3.8]
+        python-version: ["3.10"]
 
     runs-on: ${{ matrix.platform }}
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
@@ -38,15 +38,15 @@
 
   lint-and-test:
     name: Lint and Test
     strategy:
       max-parallel: 4
       matrix:
         platform: [ubuntu-latest]
-        python-version: [3.8]
+        python-version: ["3.10"]
 
     runs-on: ${{ matrix.platform }}
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
@@ -63,27 +63,27 @@
           key: ${{ runner.os }}-pip-py${{ matrix.python-version }}-${{ hashFiles('**/requirements.txt') }}
           restore-keys: |
             ${{ runner.os }}-pip-py${{ matrix.python-version }}-
       - name: Install Dependencies
         run: |
           python -m pip install --upgrade pip
           pip install --upgrade wheel
-          pip install --editable ".[dev, docs]"
+          pip install --editable ".[tests]"
       - name: Check Formatting and Lint
         run: |
           python --version
           black --version
           black neuralcompression tests projects --check
           mypy --version
           mypy neuralcompression
           flake8 --version
-          flake8 neuralcompression tests projects
+          flake8 neuralcompression tests
           isort --version
           isort --check-only neuralcompression tests projects
       - name: Install NeuralCompression
         run: |
           python setup.py bdist_wheel
           pip install dist/*.whl
       - name: Run pytest
         run: |
-          echo -e "PyTorch \c" && pip show torch | grep Version 
+          echo -e "PyTorch \c" && pip show torch | grep Version
           pytest tests
```

### Comparing `neuralcompression-0.2.1/.github/workflows/publish-package.yml` & `neuralcompression-0.2.2/.github/workflows/publish-package.yml`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   deploy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: "3.8"
+          python-version: "3.10"
       - name: Install build dependencies
         run: pip install -U build setuptools wheel
       - name: Build package
         run: python -m build .
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@v1.4.2
         with:
```

### Comparing `neuralcompression-0.2.1/.gitignore` & `neuralcompression-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/LICENSE` & `neuralcompression-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/NOTICE` & `neuralcompression-0.2.2/NOTICE`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/PKG-INFO` & `neuralcompression-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: neuralcompression
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of tools for neural compression enthusiasts
 Home-page: https://github.com/facebookresearch/NeuralCompression
 Author: Facebook AI Research
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: System :: Archiving :: Compression
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: tests
 License-File: LICENSE
 
 # NeuralCompression
 
 [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/facebookresearch/NeuralCompression/tree/main/LICENSE)
 [![Build and Test](https://github.com/facebookresearch/NeuralCompression/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/facebookresearch/NeuralCompression/actions/workflows/build-and-test.yml) [![Documentation Status](https://readthedocs.org/projects/neuralcompression/badge/?version=latest)](https://neuralcompression.readthedocs.io/en/latest/?badge=latest)
 
 ## What's New
-
+- **April 2023 (video compression)** - Added [a pytorch implementation of the video compression transformer (VCT)](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/torch_vct)
+- **November 2022 (image compression)** - Added [Bits-Back coding with diffusion models](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/bits_back_diffusion)!
 - **July 2021 (image compression)** - [Released implemenation of Scale Hyperprior](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/scale_hyperprior_lightning)
 - **July 2021 (video compression)** - [Released implementation of DVC](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/deep_video_compression)
 
 ## About
 
 NeuralCompression is a Python repository dedicated to research of neural
 networks that compress data. The repository includes tools such as JAX-based
@@ -59,19 +60,19 @@
 
 ### Development Installation
 
 First, clone the repository and navigate to the NeuralCompression root
 directory and install the package in development mode by running:
 
 ```bash
-pip install --editable ".[dev, docs]"
+pip install --editable ".[tests]"
 ```
 
-If you are not interested in matching the test environment, then you only need
-to apply the second step to install.
+If you are not interested in matching the test environment, then you can just
+apply `pip install -e .`.
 
 ## Repository Structure
 
 We use a 2-tier repository structure. The `neuralcompression` package contains
 a core set of tools for doing neural compression research. Code committed to
 the core package requires stricter linting, high code quality, and rigorous
 review. The `projects` folder contains code for reproducing papers and training
@@ -142,9 +143,7 @@
 @misc{muckley2021neuralcompression,
     author={Matthew Muckley and Jordan Juravsky and Daniel Severo and Mannat Singh and Quentin Duval and Karen Ullrich},
     title={NeuralCompression},
     howpublished={\url{https://github.com/facebookresearch/NeuralCompression}},
     year={2021}
 }
 ```
-
-
```

### Comparing `neuralcompression-0.2.1/README.md` & `neuralcompression-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # NeuralCompression
 
 [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/facebookresearch/NeuralCompression/tree/main/LICENSE)
 [![Build and Test](https://github.com/facebookresearch/NeuralCompression/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/facebookresearch/NeuralCompression/actions/workflows/build-and-test.yml) [![Documentation Status](https://readthedocs.org/projects/neuralcompression/badge/?version=latest)](https://neuralcompression.readthedocs.io/en/latest/?badge=latest)
 
 ## What's New
-
+- **April 2023 (video compression)** - Added [a pytorch implementation of the video compression transformer (VCT)](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/torch_vct)
+- **November 2022 (image compression)** - Added [Bits-Back coding with diffusion models](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/bits_back_diffusion)!
 - **July 2021 (image compression)** - [Released implemenation of Scale Hyperprior](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/scale_hyperprior_lightning)
 - **July 2021 (video compression)** - [Released implementation of DVC](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/deep_video_compression)
 
 ## About
 
 NeuralCompression is a Python repository dedicated to research of neural
 networks that compress data. The repository includes tools such as JAX-based
@@ -37,19 +38,19 @@
 
 ### Development Installation
 
 First, clone the repository and navigate to the NeuralCompression root
 directory and install the package in development mode by running:
 
 ```bash
-pip install --editable ".[dev, docs]"
+pip install --editable ".[tests]"
 ```
 
-If you are not interested in matching the test environment, then you only need
-to apply the second step to install.
+If you are not interested in matching the test environment, then you can just
+apply `pip install -e .`.
 
 ## Repository Structure
 
 We use a 2-tier repository structure. The `neuralcompression` package contains
 a core set of tools for doing neural compression research. Code committed to
 the core package requires stricter linting, high code quality, and rigorous
 review. The `projects` folder contains code for reproducing papers and training
```

### Comparing `neuralcompression-0.2.1/docs/Makefile` & `neuralcompression-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/docs/examples/image.png` & `neuralcompression-0.2.2/docs/examples/image.png`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/docs/examples/plot_image_compression.py` & `neuralcompression-0.2.2/docs/examples/plot_image_compression.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/docs/make.bat` & `neuralcompression-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/docs/source/conf.py` & `neuralcompression-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/docs/source/entropy_coders.rst` & `neuralcompression-0.2.2/docs/source/entropy_coders.rst`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/docs/source/functional.rst` & `neuralcompression-0.2.2/docs/source/functional.rst`

 * *Files 16% similar despite different names*

```diff
@@ -13,10 +13,9 @@
 .. autofunction:: log_survival_function
 .. autofunction:: lower_bound
 .. autofunction:: lower_tail
 .. autofunction:: lpips
 .. autofunction:: multiscale_structural_similarity
 .. autofunction:: ndtr
 .. autofunction:: optical_flow_to_color
-.. autofunction:: pmf_to_quantized_cdf
 .. autofunction:: quantization_offset
 .. autofunction:: survival_function
```

### Comparing `neuralcompression-0.2.1/docs/source/layers.rst` & `neuralcompression-0.2.2/docs/source/layers.rst`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/docs/source/models.rst` & `neuralcompression-0.2.2/docs/source/models.rst`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/data/_clic_2020_image.py` & `neuralcompression-0.2.2/neuralcompression/data/_clic_2020_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         )
 
         self.transform = transform
 
         if download:
             self.download()
 
-        self.paths = [*self.root.joinpath(self.split).glob("*.png")]
+        self.paths = sorted([*self.root.joinpath(self.split).glob("*.png")])
 
     def __getitem__(self, index: int) -> Image:
         path = self.paths[index]
 
         image = torchvision.datasets.folder.default_loader(path)
 
         if self.transform is not None:
```

### Comparing `neuralcompression-0.2.1/neuralcompression/data/_clic_2020_video.py` & `neuralcompression-0.2.2/neuralcompression/data/_clic_2020_video.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/data/_kodak.py` & `neuralcompression-0.2.2/neuralcompression/data/_kodak.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/data/_vimeo_90k_septuplet.py` & `neuralcompression-0.2.2/neuralcompression/data/_vimeo_90k_septuplet.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/distributions/_noisy_normal.py` & `neuralcompression-0.2.2/neuralcompression/distributions/_noisy_normal.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/distributions/_uniform_noise.py` & `neuralcompression-0.2.2/neuralcompression/distributions/_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/__init__.py` & `neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/_backend.py` & `neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/_backend.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/codecs.py` & `neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/codecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,14 @@
             same message_dtype as the codecs returned by ``obs_codec_maker``.
 
     Returns:
         A Craystack codec that can be input to the coder.
     """
 
     def push(symbols, compressed_message, cdf_state):
-
         # pop latents with approximate posterior q(latents|symbols)
         latent_posterior_codec = latent_posterior_codec_maker(symbols)
         compressed_message, latents, _ = latent_posterior_codec.pop(
             0,
             compressed_message,
             jnp.zeros(latent_shape, dtype=latent_posterior_codec.message_dtype),
             latent_posterior_codec.cdf_state,
@@ -251,15 +250,14 @@
             compressed_message,
             latent_prior_codec.cdf_state,
         )
 
         return compressed_message, None
 
     def pop(msg_index, compressed_message, message, cdf_state):
-
         # pop latents with prior p(latents)
         compressed_message, latents, _ = latent_prior_codec.pop(
             0,
             compressed_message,
             jnp.zeros(latent_shape, dtype=latent_prior_codec.message_dtype),
             latent_prior_codec.cdf_state,
             latent_prior_codec.allow_empty_pops,
```

### Comparing `neuralcompression-0.2.1/neuralcompression/entropy_coders/craystack/coder.py` & `neuralcompression-0.2.2/projects/jax_entropy_coders/craystack/coder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/entropy_coders/jax_arithemetic_coder.py` & `neuralcompression-0.2.2/projects/jax_entropy_coders/jax_arithmetic_coder.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
             algorithm and max CDF value.
 
     Returns:
         A tuple containing updated versions of ``int_array``, ``byte``,
             ``idx``, ``bit_idx``, ``pending_bits``, ``high``, ``low``, and
             ``cdf_state``.
     """
+
     # jax functions - these will all be jit-compiled for our while loop
     def decrease_high(vals):
         """Based on high decreasing, we append a 0 most significant bit."""
         high, low, pending_bits, int_array, byte, idx, bit_idx = vals
         int_array, byte, idx, bit_idx = _append_bit_and_pending(
             False, pending_bits, int_array, byte, idx, bit_idx
         )
@@ -247,14 +248,15 @@
         precision: An integer specifying the operating precision of the
             algorithm and max CDF value.
 
     Returns:
         A tuple containing updated versions of ``value``, ``high``, ``low``,
             ``idx``, ``bit_idx``, ``int_array``.
     """
+
     # jax functions - these will all be jit-compiled for our while loop
     def high_cross_half(vals):
         """No need to do anything, bit is 0."""
         return vals
 
     def low_cross_half(vals):
         """Based on low increasing, adjust limits."""
```

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/__init__.py` & `neuralcompression-0.2.2/neuralcompression/functional/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 from ._log_survival_function import log_survival_function
 from ._lower_bound import lower_bound
 from ._lower_tail import lower_tail
 from ._lpips import lpips
 from ._multiscale_structural_similarity import multiscale_structural_similarity
 from ._ndtr import ndtr
 from ._optical_flow_to_color import optical_flow_to_color
-from ._pmf_to_quantized_cdf import pmf_to_quantized_cdf
 from ._quantization_offset import quantization_offset
 from ._soft_round import soft_round
 from ._soft_round_conditional_mean import soft_round_conditional_mean
 from ._soft_round_inverse import soft_round_inverse
 from ._survival_function import survival_function
 from ._upper_tail import upper_tail
```

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_count_flops.py` & `neuralcompression-0.2.2/neuralcompression/functional/_count_flops.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     for name in _SINGLE_FLOP_ESTIMATES_TO_ADD
     + [f"{n}_" for n in _SINGLE_FLOP_ESTIMATES_TO_ADD]
 }
 
 
 # Expanding on the 0-flop op list from fvcore here:
 # https://github.com/facebookresearch/fvcore/blob/166a030e093013a934642ca3744592a2e3de5ea2/fvcore/nn/jit_analysis.py#L27
-_OPS_TO_IGNORE = ["aten::empty_like"]
+_OPS_TO_IGNORE = ["aten::empty_like", "aten::numel"]
 
 
 def count_flops(
     module: nn.Module,
     inputs: Sequence[Any],
     counter_overrides: Optional[Dict[str, Handle]] = None,
     use_single_flop_estimates: bool = False,
```

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_dense_image_warp.py` & `neuralcompression-0.2.2/neuralcompression/functional/_dense_image_warp.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_estimate_tails.py` & `neuralcompression-0.2.2/neuralcompression/functional/_estimate_tails.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import torch
 
 
 def estimate_tails(
     func: typing.Callable[[torch.Tensor], torch.Tensor],
     target: float,
-    shape: int,
+    shape: torch.Size,
     device: typing.Union[torch.device, str, None] = None,
     dtype: torch.dtype = torch.float32,
 ) -> torch.Tensor:
     """Estimates approximate tail quantiles.
 
     A simple Adam iteration is ran to determine tail quantiles. The objective
     is to find an :math:`x` such that :math:`func(x) = target`. For instance,
@@ -36,33 +36,32 @@
         shape: shape representing :math:`x`.
         device: PyTorch device.
         dtype: PyTorch dtype of the computation and the return value.
 
     Returns:
         the solution, :math:`x`.
     """
+    tails: torch.Tensor
+
     if not device:
         if torch.cuda.is_available():
             device = "cuda"
         else:
             device = "cpu"
 
     eps = torch.finfo(torch.float32).eps
-
     counts = torch.zeros(shape, dtype=torch.int32)
-
     tails = torch.zeros(shape, device=device, dtype=dtype, requires_grad=True)
-
     mean = torch.zeros(shape, dtype=dtype)
-
     variance = torch.ones(shape, dtype=dtype)
 
     while torch.min(counts) < 100:
         abs(func(tails) - target).backward(torch.ones_like(tails))
 
+        assert tails.grad is not None
         gradient = tails.grad.cpu()
 
         with torch.no_grad():
             mean = 0.9 * mean + (1.0 - 0.9) * gradient
 
             variance = 0.99 * variance + (1.0 - 0.99) * torch.square(gradient)
```

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_hsv_to_rgb.py` & `neuralcompression-0.2.2/neuralcompression/functional/_hsv_to_rgb.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_information_content.py` & `neuralcompression-0.2.2/neuralcompression/functional/_information_content.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_log_cdf.py` & `neuralcompression-0.2.2/neuralcompression/functional/_log_cdf.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_log_expm1.py` & `neuralcompression-0.2.2/neuralcompression/functional/_log_expm1.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_log_ndtr.py` & `neuralcompression-0.2.2/neuralcompression/functional/_log_ndtr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import torch
 from torch import Tensor
 
 from ._ndtr import ndtr
 
 
 def _log_ndtr_asymptotic_series(x: Tensor, series_order: int = 3) -> Tensor:
-    t1 = -0.5 * (math.log(2 * math.pi) + x ** 2) - torch.log(-x)
+    t1 = -0.5 * (math.log(2 * math.pi) + x**2) - torch.log(-x)
     t2 = torch.zeros_like(x)
-    value_even_power = (x ** 2).clone()
+    value_even_power = (x**2).clone()
     double_fac = 1
     multiplier = -1
 
     for n in range(1, series_order + 1):
         t2.add_(multiplier * double_fac / value_even_power)
-        value_even_power.mul_(x ** 2)
+        value_even_power.mul_(x**2)
         double_fac *= 2 * n - 1
         multiplier *= -1
 
     return t1 + torch.log1p(t2)
 
 
 def log_ndtr(x: Tensor) -> Tensor:
```

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_log_survival_function.py` & `neuralcompression-0.2.2/neuralcompression/functional/_log_survival_function.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_lower_bound.py` & `neuralcompression-0.2.2/neuralcompression/functional/_lower_bound.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_lower_tail.py` & `neuralcompression-0.2.2/neuralcompression/functional/_lower_tail.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_lpips.py` & `neuralcompression-0.2.2/neuralcompression/functional/_lpips.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_multiscale_structural_similarity.py` & `neuralcompression-0.2.2/neuralcompression/functional/_multiscale_structural_similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     vy = uyy - uy * uy
     vxy = uxy - ux * uy
 
     # Equation (6) in MS-SSIM paper.
     a1, a2, b1, b2 = (
         2 * ux * uy + c1,
         2 * vxy + c2,
-        ux ** 2 + uy ** 2 + c1,
+        ux**2 + uy**2 + c1,
         vx + vy + c2,
     )
 
     luminance = a1 / b1
     contrast_structure = a2 / b2
 
     batch_size = luminance.size(0)
```

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_ndtr.py` & `neuralcompression-0.2.2/neuralcompression/functional/_ndtr.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_optical_flow_to_color.py` & `neuralcompression-0.2.2/neuralcompression/functional/_optical_flow_to_color.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_quantization_offset.py` & `neuralcompression-0.2.2/neuralcompression/functional/_quantization_offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,11 +34,11 @@
         a tensor broadcastable to shape ``distribution.batch_shape``,
         containing the determined quantization offsets. No gradients are
         permitted to flow through the return value.
     """
     try:
         offset = distribution.mean
     except AttributeError:
-        offset = 0
+        offset = torch.tensor(0)
 
     with torch.no_grad():
         return offset - torch.round(offset)
```

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_soft_round.py` & `neuralcompression-0.2.2/neuralcompression/functional/_soft_round.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_soft_round_conditional_mean.py` & `neuralcompression-0.2.2/neuralcompression/functional/_soft_round_conditional_mean.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_soft_round_inverse.py` & `neuralcompression-0.2.2/neuralcompression/functional/_soft_round_inverse.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_survival_function.py` & `neuralcompression-0.2.2/neuralcompression/functional/_survival_function.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/functional/_upper_tail.py` & `neuralcompression-0.2.2/neuralcompression/functional/_upper_tail.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/__init__.py` & `neuralcompression-0.2.2/neuralcompression/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_analysis_transformation_2d.py` & `neuralcompression-0.2.2/neuralcompression/layers/_analysis_transformation_2d.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_continuous_entropy.py` & `neuralcompression-0.2.2/neuralcompression/layers/_continuous_entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import abc
 from typing import Optional, Tuple, Union
 
 import torch
 import torch.nn
+from compressai.entropy_models.entropy_models import pmf_to_quantized_cdf
 from torch import IntTensor, Size, Tensor
 from torch.distributions import Distribution
 from torch.nn import Module
 
 import neuralcompression.functional as ncF
 from neuralcompression.distributions import UniformNoise
 
@@ -71,15 +72,15 @@
 
     def __init__(
         self,
         coding_rank: Optional[int] = None,
         compressible: bool = False,
         stateless: bool = False,
         prior: Optional[Union[Distribution, UniformNoise]] = None,
-        tail_mass: float = 2 ** -8,
+        tail_mass: float = 2**-8,
         prior_shape: Optional[Tuple[int, ...]] = None,
         prior_dtype: Optional[torch.dtype] = None,
         cdfs: Optional[IntTensor] = None,
         cdf_sizes: Optional[IntTensor] = None,
         cdf_offsets: Optional[IntTensor] = None,
         maximum_cdf_size: Optional[int] = None,
         range_coder_precision: int = 12,
@@ -358,15 +359,15 @@
             overflow = torch.clamp(
                 1 - torch.sum(pmf, dim=0, keepdim=True),
                 min=0.0,
             )
 
             pmf = torch.cat([pmf, overflow], dim=0)
 
-            cdf = ncF.pmf_to_quantized_cdf(
+            cdf = pmf_to_quantized_cdf(
                 pmf,
                 self._range_coder_precision,
             )
 
             cdfs[index, : cdf.size()[0]] = cdf
 
         return cdfs, cdf_sizes, cdf_offsets
```

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_generalized_divisive_normalization.py` & `neuralcompression-0.2.2/neuralcompression/layers/_generalized_divisive_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
                 self.gamma = Parameter(gamma_parameter)
 
     def forward(self, x: Tensor) -> Tensor:
         _, channels, _, _ = x.size()
 
         y = torch.nn.functional.conv2d(
-            x ** 2,
+            x**2,
             torch.reshape(
                 self._reparameterized_gamma(self.gamma),
                 (channels, channels, 1, 1),
             ),
             self._reparameterized_beta(self.beta),
         )
```

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_hyper_analysis_transformation_2d.py` & `neuralcompression-0.2.2/neuralcompression/layers/_hyper_analysis_transformation_2d.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_hyper_synthesis_transformation_2d.py` & `neuralcompression-0.2.2/neuralcompression/layers/_hyper_synthesis_transformation_2d.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_non_negative_parameterization.py` & `neuralcompression-0.2.2/neuralcompression/layers/_non_negative_parameterization.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,41 +45,41 @@
     initial_value: Optional[Tensor]
     _pedestal: Tensor
 
     def __init__(
         self,
         initial_value: Optional[Tensor] = None,
         minimum: float = 0.0,
-        offset: float = 2 ** -18,
+        offset: float = 2**-18,
         shape: Optional[Tuple[int]] = None,
         lower_bound_gradient: str = "identity_if_towards",
     ):
         super(NonNegativeParameterization, self).__init__()
 
         self._minimum = minimum
 
         self._offset = offset
 
         self._lower_bound_gradient = lower_bound_gradient
 
-        self._bound = (self._minimum + self._offset ** 2) ** 0.5
+        self._bound = (self._minimum + self._offset**2) ** 0.5
 
         if initial_value is None:
             if shape is None:
                 error_message = """
                 ``initial_value`` is ``None``, ``shape`` must be specified
                 """
 
                 raise ValueError(error_message)
 
             initial_value = torch.zeros(shape, dtype=torch.float)
 
         self.register_buffer(
             "_pedestal",
-            torch.tensor([(self._offset ** 2)], dtype=initial_value.dtype),
+            torch.tensor([(self._offset**2)], dtype=initial_value.dtype),
         )
 
         if initial_value is not None:
             self.initial_value = torch.sqrt(
                 torch.max(
                     initial_value + self._pedestal,
                     self._pedestal,
@@ -89,8 +89,8 @@
     def forward(self, x: Tensor) -> Tensor:
         lower_bound = ncF.lower_bound(
             x,
             self._bound,
             self._lower_bound_gradient,
         )
 
-        return lower_bound ** 2 - self._pedestal
+        return lower_bound**2 - self._pedestal
```

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_rate_mse_distortion_loss.py` & `neuralcompression-0.2.2/neuralcompression/layers/_rate_mse_distortion_loss.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,27 +52,25 @@
     ) -> RateDistortionLoss:
         """
         Args:
             x_hat: encoder output.
             probabilities: reconstruction likelihoods.
             x: encoder input.
         """
-        n, _, h, w = x.size()
+        if not x.ndim == 4:
+            raise ValueError("RateMSEDistortionLoss only defined for 4D inputs.")
 
-        bpps = []
+        # log-2 conversion and number of pixels
+        factor = -math.log(2) * x.shape[0] * x.shape[2] * x.shape[3]
 
-        for probability in probabilities:
-            pixels = -math.log(2) * (n * h * w)
-
-            bpps += [float(torch.log(probability).sum() / pixels)]
-
-        rate = torch.tensor(torch.sum(torch.tensor(bpps)), device=x.device)
+        rate = (
+            torch.stack(
+                [torch.log(probability).sum() for probability in probabilities]
+            ).sum()
+            / factor
+        )
 
         distortion = self.mse.forward(x_hat, x)
 
-        rate_distortion = rate + distortion
-
         return RateDistortionLoss(
-            rate,
-            distortion,
-            Tensor([self.trade_off * self.maximum ** 2 * rate_distortion]),
+            rate, distortion, self.trade_off * self.maximum**2 * distortion + rate
         )
```

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/_synthesis_transformation_2d.py` & `neuralcompression-0.2.2/neuralcompression/layers/_synthesis_transformation_2d.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/layers/gdn.py` & `neuralcompression-0.2.2/neuralcompression/layers/gdn.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/metrics/distortion.py` & `neuralcompression-0.2.2/neuralcompression/metrics/distortion.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         k1: float = 0.01,
         k2: float = 0.03,
         gaussian_std: float = 1.5,
         power_factors: Sequence[float] = MS_SSIM_FACTORS,
         compute_on_step: bool = True,
         dist_sync_on_step: bool = False,
         process_group: Optional[Any] = None,
-        dist_sync_fn: Callable = None,
+        dist_sync_fn: Optional[Callable] = None,
     ):
         """
         Computes the multi-scale structural similarity index measure.
 
         Follows the algorithm in the paper: Wang, Zhou, Eero P. Simoncelli,
         and Alan C. Bovik. "Multiscale structural similarity for image
         quality assessment." Signals, Systems and Computers, 2004.
@@ -67,15 +67,14 @@
         self.gaussian_std = gaussian_std
         self.power_factors = power_factors
 
         self.add_state("score_sum", default=torch.tensor(0.0), dist_reduce_fx="sum")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
     def update(self, preds, target):
-
         self.score_sum += multiscale_structural_similarity(
             preds,
             target,
             data_range=self.data_range,
             window_size=self.window_size,
             k1=self.k1,
             k2=self.k2,
@@ -125,17 +124,16 @@
         base_network: str = "alex",
         use_linear_calibration: bool = True,
         linear_weights_version: str = "0.1",
         normalize: bool = False,
         compute_on_step: bool = True,
         dist_sync_on_step: bool = False,
         process_group: Optional[Any] = None,
-        dist_sync_fn: Callable = None,
+        dist_sync_fn: Optional[Callable] = None,
     ):
-
         if base_network not in ("alex", "vgg", "squeeze"):
             raise ValueError(
                 f"Unknown base network {base_network}"
                 " - please pass one of 'alex', 'vgg', or 'squeeze'."
             )
 
         if linear_weights_version not in ("0.0", "0.1"):
```

### Comparing `neuralcompression-0.2.1/neuralcompression/models/__init__.py` & `neuralcompression-0.2.2/neuralcompression/models/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_factorized_prior_autoencoder.py` & `neuralcompression-0.2.2/neuralcompression/models/_factorized_prior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hific/_channel_norm_2d.py` & `neuralcompression-0.2.2/neuralcompression/models/_hific/_channel_norm_2d.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hific/_hific_discriminator.py` & `neuralcompression-0.2.2/neuralcompression/models/_hific/_hific_discriminator.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hific/_hific_encoder.py` & `neuralcompression-0.2.2/neuralcompression/models/_hific/_hific_encoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hific/_hific_generator.py` & `neuralcompression-0.2.2/neuralcompression/models/_hific/_hific_generator.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hific/_least_squares_adversarial_loss.py` & `neuralcompression-0.2.2/neuralcompression/models/_hific/_least_squares_adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hific/_non_saturating_adversarial_loss.py` & `neuralcompression-0.2.2/neuralcompression/models/_hific/_non_saturating_adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hific/_weighted_rate_loss.py` & `neuralcompression-0.2.2/neuralcompression/models/_hific/_weighted_rate_loss.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/neuralcompression/models/_hyperprior_autoencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
         hyperprior.load_state_dict(state_dict)
 
         return hyperprior
 
     def load_state_dict(
         self,
-        state_dict: OrderedDict[str, Tensor],
+        state_dict: OrderedDict[str, Tensor],  # type: ignore
         strict: bool = True,
     ):
         bottleneck_buffer_names = [
             "_quantized_cdf",
             "_offset",
             "_cdf_length",
             "scale_table",
```

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_mean_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/neuralcompression/models/_mean_scale_hyperprior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_prior_autoencoder.py` & `neuralcompression-0.2.2/neuralcompression/models/_prior_autoencoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                 continue
 
             updated |= module.update(force=force)
 
         return updated
 
     def load_state_dict(
-        self, state_dict: OrderedDict[str, Tensor], strict: bool = True
+        self, state_dict: OrderedDict[str, Tensor], strict: bool = True  # type: ignore
     ):
         for bottleneck_buffer_name in self.bottleneck_buffer_names:
             name = f"{self.bottleneck_name}.{bottleneck_buffer_name}"
 
             size = state_dict[name].size()
 
             registered_buffers = []
```

### Comparing `neuralcompression-0.2.1/neuralcompression/models/_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/neuralcompression/models/_scale_hyperprior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/deep_video_compression.py` & `neuralcompression-0.2.2/neuralcompression/models/deep_video_compression.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/neuralcompression/models/scale_hyperprior.py` & `neuralcompression-0.2.2/neuralcompression/models/scale_hyperprior.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List, Optional, Sequence, Tuple
 
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
-import torchvision.transforms.functional as tvtF
 from compressai.entropy_models import EntropyBottleneck, GaussianConditional
 from compressai.layers import GDN as GeneralizedDivisiveNormalization
 from compressai.models.google import get_scale_table
 from compressai.models.utils import update_registered_buffers
 from torch import Tensor
 from torch.nn.parameter import Parameter
 
@@ -54,72 +52,43 @@
         kernel_size=kernel_size,
         stride=stride,
         output_padding=stride - 1,
         padding=kernel_size // 2,
     )
 
 
-def _resize(x: Tensor, target_shape: Sequence[int]) -> Tensor:
-    """
-    Resizes a tensor to the target shape.
-
-    Given a tensor of shape [batch_size, num_channels, height, width] and
-    a [height, width] target_shape, this function resizes the input
-    tensor to the taget shape using center cropping if the input is larger
-    than the target shape, and using nearest neighbour interpolation if
-    the input is smaller than the target shape.
-
-    Args:
-        x: the tensor to resize, of shape [batch_size, num_channels,
-            height, width].
-        target_shape: a [height, width] pair to reshape the input to.
-
-    Returns:
-        the resized tensor.
-    """
-
-    height, width = x.shape[2:]
-    target_height, target_width = target_shape
-
-    if height >= target_height and width >= target_width:
-        return tvtF.center_crop(x, target_shape)
-    elif height <= target_height and width <= target_width:
-        return F.interpolate(x, target_shape, mode="nearest")
-    else:
-        raise ValueError(
-            f"Input tensor (with shape {x.shape}) is larger than the"
-            f" target shape of {target_shape} along one height/width axis"
-            " and is smaller than the target shape along the other axis."
-        )
-
-
 class _AbsoluteValue(nn.Module):
     def forward(self, inp: Tensor) -> Tensor:
         return torch.abs(inp)
 
 
 class ScaleHyperpriorImageAnalysis(nn.Module):
     """
     Image analysis network for the scale hyperprior model.
 
     Args:
         network_channels, compression_channels: see ScaleHyperprior
     """
 
-    def __init__(self, network_channels: int, compression_channels: int):
+    def __init__(self, network_channels: int, compression_channels: int) -> None:
         super().__init__()
         self.model = nn.Sequential(
             _conv(3, network_channels, kernel_size=5, stride=2),
             GeneralizedDivisiveNormalization(network_channels),
             _conv(network_channels, network_channels, kernel_size=5, stride=2),
             GeneralizedDivisiveNormalization(network_channels),
             _conv(network_channels, network_channels, kernel_size=5, stride=2),
             GeneralizedDivisiveNormalization(network_channels),
             _conv(network_channels, compression_channels, kernel_size=5, stride=2),
         )
+        self._num_down = 4
+
+    @property
+    def num_downsampling_layers(self) -> int:
+        return self._num_down
 
     def forward(self, x: Tensor) -> Tensor:
         return self.model(x)
 
 
 class ScaleHyperpriorImageSynthesis(nn.Module):
     """
@@ -149,24 +118,29 @@
     """
     Hyper analysis network for the scale hyperprior model.
 
     Args:
         network_channels, compression_channels: see ScaleHyperprior
     """
 
-    def __init__(self, network_channels: int, compression_channels: int):
+    def __init__(self, network_channels: int, compression_channels: int) -> None:
         super().__init__()
         self.model = nn.Sequential(
             _AbsoluteValue(),
             _conv(compression_channels, network_channels, kernel_size=3),
             nn.ReLU(inplace=True),
             _conv(network_channels, network_channels, kernel_size=5, stride=2),
             nn.ReLU(inplace=True),
             _conv(network_channels, network_channels, kernel_size=5, stride=2),
         )
+        self._num_down = 3
+
+    @property
+    def num_downsampling_layers(self) -> int:
+        return self._num_down
 
     def forward(self, x: Tensor) -> Tensor:
         return self.model(x)
 
 
 class ScaleHyperpriorHyperSynthesis(nn.Module):
     """
@@ -253,25 +227,20 @@
         image_bottleneck: Optional[nn.Module] = None,
         hyper_analysis: Optional[nn.Module] = None,
         hyper_synthesis: Optional[nn.Module] = None,
         hyper_bottleneck: Optional[nn.Module] = None,
     ):
         super().__init__()
 
-        if (
-            None
-            in [
-                image_analysis,
-                image_synthesis,
-                hyper_analysis,
-                hyper_analysis,
-                hyper_synthesis,
-            ]
-            and None in [network_channels, compression_channels]
-        ):
+        if None in [
+            image_analysis,
+            image_synthesis,
+            hyper_analysis,
+            hyper_synthesis,
+        ] and None in [network_channels, compression_channels]:
             raise ValueError(
                 "When one or more analysis or synthesis networks is unspecified, "
                 "'network_channels' and 'compressions_channels' must be"
                 " passed."
             )
 
         if hyper_bottleneck is None and network_channels is None:
@@ -316,16 +285,27 @@
             self.image_bottleneck = image_bottleneck
         else:
             self.image_bottleneck = GaussianConditional(scale_table=None)
 
         if hyper_bottleneck is not None:
             self.hyper_bottleneck = hyper_bottleneck
         else:
+            assert (
+                network_channels is not None
+            ), "<network_channels> and <hyper_bottleneck> cannot both be None"
             self.hyper_bottleneck = EntropyBottleneck(channels=network_channels)
 
+    def _pad(self, images: Tensor, sizes: Sequence[int]) -> Tensor:
+        down_image_analysis = getattr(self.image_analysis, "num_downsampling_layers")
+        down_hyper_analysis = getattr(self.hyper_analysis, "num_downsampling_layers")
+        factor = 2 ** (down_image_analysis + down_hyper_analysis)
+
+        pad_h, pad_w = [(factor - (s % factor)) % factor for s in sizes]
+        return torch.nn.functional.pad(images, (0, pad_w, 0, pad_h), "reflect")
+
     def forward(self, images: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
         """
         Calculates an image's reconstruction and compression likelihoods.
 
         This function is for use during model training. Given a batch of
         input images, this function sends the images through the model's
         encoder and decoder, using additive uniform noise as a stand-in
@@ -345,30 +325,34 @@
                 1.  The decoder's image reconstruction (this has the same
                     shape as the original input).
                 2.  The likelihoods assigned by the image bottleneck layer
                     to the quantized image latent.
                 3.  The likelihoods assigned by the hyper bottleneck layer
                     to the quantized hyper latent.
         """
+        if not self.training:
+            images_shape = images.shape[-2:]
+            images = self._pad(images, images_shape)
+        else:
+            images_shape = None
 
         latent = self.image_analysis(images)
         hyper_latent = self.hyper_analysis(latent)
         noisy_hyper_latent, hyper_latent_likelihoods = self.hyper_bottleneck(
             hyper_latent
         )
         scales = self.hyper_synthesis(noisy_hyper_latent)
 
-        if scales.shape != latent.shape:
-            scales = _resize(scales, latent.shape[2:])
-
         noisy_latent, latent_likelihoods = self.image_bottleneck(latent, scales)
         reconstruction = self.image_synthesis(noisy_latent)
 
-        if reconstruction.shape != images.shape:
-            reconstruction = _resize(reconstruction, images.shape[2:])
+        if not self.training:
+            assert images_shape is not None, "image_shape not found"
+            h, w = images_shape
+            reconstruction = reconstruction[..., :h, :w]
 
         return reconstruction, latent_likelihoods, hyper_latent_likelihoods
 
     def update(self, force=False):
         """
         Updates the entropy bottleneck(s) CDF values.
 
@@ -383,30 +367,36 @@
         """
 
         if isinstance(self.image_bottleneck, GaussianConditional):
             image_bottleneck_updated = self.image_bottleneck.update_scale_table(
                 get_scale_table(), force=force
             )
         else:
-            image_bottleneck_updated = self.image_bottleneck.update(force=force)
-
-        hyper_bottleneck_updated = self.hyper_bottleneck.update(force=force)
+            assert hasattr(
+                self.image_bottleneck, "update"
+            ), "<image_bottleneck> module has no <update> method"
+            image_bottleneck_updated = self.image_bottleneck.update(force=force)  # type: ignore
+
+        assert hasattr(
+            self.hyper_bottleneck, "update"
+        ), "<hyper_bottleneck> module has no <update> method"
+        hyper_bottleneck_updated = self.hyper_bottleneck.update(force=force)  # type: ignore
         return image_bottleneck_updated | hyper_bottleneck_updated
 
     def _on_cpu(self):
         cpu = torch.device("cpu")
         for param in self.parameters():
             if param.device != cpu:
                 return False
         return True
 
     # TODO: Switch to named tuple
     def compress(
         self, images: Tensor, force_cpu: bool = True
-    ) -> Tuple[List[str], List[str], Sequence[int], Sequence[int], Sequence[int]]:
+    ) -> Tuple[List[str], List[str], Sequence[int], Sequence[int]]:
         """
         Compress a batch of images into strings.
 
         Args:
             images: ``Tensor`` of shape [batch, channels, height, width].
             force_cpu: whether to throw an error if the model is
                 not on the CPU when compressing. Compressing/decompressing
@@ -416,64 +406,57 @@
         Returns:
             latent_strings: list containing a compressed latent string for
                 each image in the batch.
             hyper_latent_strings: list containing a compressed hyperprior
                 string for each image in the batch.
             image_shape: list storing the height and width of the
                 original images, for use during decoding.
-            latent_shape: list storing the height and width of the
-                image latent, for use during decoding.
             hyper_latent_shape: list storing the height and width of the
                 hyperprior, for use during decoding.
         """
         if not self._on_cpu() and force_cpu:
             raise ValueError("Compress not supported on GPU.")
+        image_shape = images.shape[-2:]
+        images = self._pad(images, image_shape)
 
         latent = self.image_analysis(images)
         hyper_latent = self.hyper_analysis(latent)
         hyper_latent_strings = self.hyper_bottleneck.compress(hyper_latent)  # type: ignore
         hyper_latent_decoded = self.hyper_bottleneck.decompress(  # type: ignore
             hyper_latent_strings, hyper_latent.shape[2:]
         )
         scales = self.hyper_synthesis(hyper_latent_decoded)
 
-        if scales.shape != latent.shape:
-            scales = _resize(scales, latent.shape[2:])
-
         indexes = self.image_bottleneck.build_indexes(scales)  # type: ignore
         latent_strings = self.image_bottleneck.compress(latent, indexes)  # type: ignore
         return (
             latent_strings,
             hyper_latent_strings,
-            images.shape[2:],
-            latent.shape[2:],
+            image_shape,
             hyper_latent.shape[2:],
         )
 
     def decompress(
         self,
         latent_strings: List[str],
         hyper_latent_strings: List[str],
         image_shape: Sequence[int],
-        latent_shape: Sequence[int],
         hyper_latent_shape: Sequence[int],
         force_cpu: bool = True,
     ) -> Tensor:
         """
         Decompress a batch of binary strings into images.
 
         Args:
             latent_strings: list containing a compressed latent string for
                 each image in the batch.
             hyper_latent_strings: list containing a compressed hyperprior
                 string for each image in the batch.
             image_shape: list storing the height and width of the
                 original images.
-            latent_shape: list storing the height and width of the
-                image latent.
             hyper_latent_shape: list storing the height and width of
                 the hyperprior.
             force_cpu: whether to throw an error if the model is
                 not on the CPU when decompressing. Compressing/decompressing
                 on the GPU has known numerical and reproducability
                 issues with the default entropy bottleneck implementation.
 
@@ -483,26 +466,19 @@
         if not self._on_cpu() and force_cpu:
             raise ValueError("Decompress not supported on GPU.")
 
         hyper_latent_decoded = self.hyper_bottleneck.decompress(  # type: ignore
             hyper_latent_strings, hyper_latent_shape
         )
         scales = self.hyper_synthesis(hyper_latent_decoded)
-
-        if scales.shape[2:] != tuple(latent_shape):
-            scales = _resize(scales, latent_shape)
-
         indexes = self.image_bottleneck.build_indexes(scales)  # type: ignore
         latent_decoded = self.image_bottleneck.decompress(latent_strings, indexes)  # type: ignore
         reconstruction = self.image_synthesis(latent_decoded).clamp_(0, 1)
-
-        if reconstruction.shape[2:] != tuple(image_shape):
-            reconstruction = _resize(reconstruction, image_shape)
-
-        return reconstruction
+        h, w = image_shape
+        return reconstruction[..., :h, :w]
 
     def load_state_dict(self, state_dict):
         """
         Updates the model's parameters from a saved dictionary.
 
         This model overrides the default load_state_dict implementation
         to properly load the CDF buffers of the entropy models.
```

### Comparing `neuralcompression-0.2.1/neuralcompression.egg-info/PKG-INFO` & `neuralcompression-0.2.2/neuralcompression.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: neuralcompression
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of tools for neural compression enthusiasts
 Home-page: https://github.com/facebookresearch/NeuralCompression
 Author: Facebook AI Research
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: System :: Archiving :: Compression
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: tests
 License-File: LICENSE
 
 # NeuralCompression
 
 [![LICENSE](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/facebookresearch/NeuralCompression/tree/main/LICENSE)
 [![Build and Test](https://github.com/facebookresearch/NeuralCompression/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/facebookresearch/NeuralCompression/actions/workflows/build-and-test.yml) [![Documentation Status](https://readthedocs.org/projects/neuralcompression/badge/?version=latest)](https://neuralcompression.readthedocs.io/en/latest/?badge=latest)
 
 ## What's New
-
+- **April 2023 (video compression)** - Added [a pytorch implementation of the video compression transformer (VCT)](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/torch_vct)
+- **November 2022 (image compression)** - Added [Bits-Back coding with diffusion models](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/bits_back_diffusion)!
 - **July 2021 (image compression)** - [Released implemenation of Scale Hyperprior](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/scale_hyperprior_lightning)
 - **July 2021 (video compression)** - [Released implementation of DVC](https://github.com/facebookresearch/NeuralCompression/tree/main/projects/deep_video_compression)
 
 ## About
 
 NeuralCompression is a Python repository dedicated to research of neural
 networks that compress data. The repository includes tools such as JAX-based
@@ -59,19 +60,19 @@
 
 ### Development Installation
 
 First, clone the repository and navigate to the NeuralCompression root
 directory and install the package in development mode by running:
 
 ```bash
-pip install --editable ".[dev, docs]"
+pip install --editable ".[tests]"
 ```
 
-If you are not interested in matching the test environment, then you only need
-to apply the second step to install.
+If you are not interested in matching the test environment, then you can just
+apply `pip install -e .`.
 
 ## Repository Structure
 
 We use a 2-tier repository structure. The `neuralcompression` package contains
 a core set of tools for doing neural compression research. Code committed to
 the core package requires stricter linting, high code quality, and rigorous
 review. The `projects` folder contains code for reproducing papers and training
@@ -142,9 +143,7 @@
 @misc{muckley2021neuralcompression,
     author={Matthew Muckley and Jordan Juravsky and Daniel Severo and Mannat Singh and Quentin Duval and Karen Ullrich},
     title={NeuralCompression},
     howpublished={\url{https://github.com/facebookresearch/NeuralCompression}},
     year={2021}
 }
 ```
-
-
```

### Comparing `neuralcompression-0.2.1/projects/README.md` & `neuralcompression-0.2.2/projects/README.md`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/deep_video_compression/README.md` & `neuralcompression-0.2.2/projects/deep_video_compression/README.md`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/deep_video_compression/_utils.py` & `neuralcompression-0.2.2/projects/deep_video_compression/_utils.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/deep_video_compression/config/base.yaml` & `neuralcompression-0.2.2/projects/deep_video_compression/config/base.yaml`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/deep_video_compression/data_module.py` & `neuralcompression-0.2.2/projects/deep_video_compression/data_module.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/deep_video_compression/dvc_module.py` & `neuralcompression-0.2.2/projects/deep_video_compression/dvc_module.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/deep_video_compression/train.py` & `neuralcompression-0.2.2/projects/deep_video_compression/train.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/scale_hyperprior_lightning/README.md` & `neuralcompression-0.2.2/projects/scale_hyperprior_lightning/README.md`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/scale_hyperprior_lightning/config/base.yaml` & `neuralcompression-0.2.2/projects/scale_hyperprior_lightning/config/base.yaml`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/scale_hyperprior_lightning/scale_hyperprior.py` & `neuralcompression-0.2.2/projects/scale_hyperprior_lightning/scale_hyperprior.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         bits = (
             latent_likelihoods.log().sum() + hyper_latent_likelihoods.log().sum()
         ) / -math.log(2)
         bpp_loss = bits / num_pixels
 
         distortion_loss = F.mse_loss(reconstruction, original)
-        combined_loss = self.distortion_lambda * 255 ** 2 * distortion_loss + bpp_loss
+        combined_loss = self.distortion_lambda * 255**2 * distortion_loss + bpp_loss
 
         return bpp_loss, distortion_loss, combined_loss
 
     def update(self, force=True):
         return self.model.update(force=force)
 
     def compress(
@@ -85,15 +85,14 @@
         z_shape: Sequence[int],
     ):
         return self.model.decompress(
             y_strings, z_strings, image_shape, y_shape, z_shape
         )
 
     def training_step(self, batch, batch_idx, optimizer_idx):
-
         if optimizer_idx not in [0, 1]:
             raise ValueError(
                 f"Received unexpected optimizer index {optimizer_idx}"
                 " - should be 0 or 1"
             )
 
         if optimizer_idx == 0:
```

### Comparing `neuralcompression-0.2.1/projects/scale_hyperprior_lightning/tests/test_scale_hyperprior_lightning.py` & `neuralcompression-0.2.2/projects/scale_hyperprior_lightning/tests/test_scale_hyperprior_lightning.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/scale_hyperprior_lightning/train.py` & `neuralcompression-0.2.2/projects/scale_hyperprior_lightning/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from vimeo import Vimeo90kSeptupletLightning
 
 from neuralcompression.models import ScaleHyperprior
 
 
 @hydra.main(config_path="config", config_name="base")
 def main(cfg: DictConfig):
-
     save_dir: Path = Path(hydra.utils.get_original_cwd()) / cfg.save_dir
 
     if (
         not cfg.overwrite
         and not cfg.resume_training
         and len(list(save_dir.glob("*.ckpt"))) > 0
     ):
```

### Comparing `neuralcompression-0.2.1/projects/scale_hyperprior_lightning/vimeo.py` & `neuralcompression-0.2.2/projects/scale_hyperprior_lightning/vimeo.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/variational_image_compression/lightning/_factorized_prior_autoencoder.py` & `neuralcompression-0.2.2/projects/variational_image_compression/lightning/_factorized_prior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/variational_image_compression/lightning/_mean_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/projects/variational_image_compression/lightning/_mean_scale_hyperprior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/variational_image_compression/lightning/_prior_autoencoder.py` & `neuralcompression-0.2.2/projects/variational_image_compression/lightning/_prior_autoencoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             bpps += [float(likelihood.log().sum()) / pixels]
 
         rate = Tensor(bpps).sum()
 
         distortion = F.mse_loss(x_hat, x)
 
         rate_distortion = (
-            self.hparams.distortion_trade_off * 255 ** 2 * (rate + distortion)  # type: ignore
+            self.hparams.distortion_trade_off * 255**2 * (rate + distortion)  # type: ignore
         )
 
         return rate, distortion, rate_distortion
 
     def test_dataloader(self) -> EVAL_DATALOADERS:
         return super(_PriorAutoencoder, self).test_dataloader()
```

### Comparing `neuralcompression-0.2.1/projects/variational_image_compression/lightning/_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/projects/variational_image_compression/lightning/_scale_hyperprior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/variational_image_compression/test/test_factorized_prior_autoencoder.py` & `neuralcompression-0.2.2/projects/variational_image_compression/test/test_factorized_prior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/variational_image_compression/test/test_mean_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/projects/variational_image_compression/test/test_mean_scale_hyperprior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/projects/variational_image_compression/test/test_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/projects/variational_image_compression/test/test_scale_hyperprior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/setup.cfg` & `neuralcompression-0.2.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -39,75 +39,68 @@
 
 [mypy-lpips.*]
 ignore_missing_imports = True
 
 [mypy-neuralcompression.entropy_coders.craystack.*]
 ignore_errors = True
 
-[mypy-neuralcompression.ext.*]
-ignore_errors = True
-
 [mypy-torchvision.*]
 ignore_missing_imports = True
 
 [mypy-tqdm.*]
 ignore_missing_imports = True
 
 [options]
 include_package_data = True
 install_requires = 
 	compressai>=1.1.9
 	fvcore>=0.1.5.post20211023
-	h5py>=3.1.0
-	jaxlib>=0.1.75
-	jax>=0.2.26
 	lpips>=0.1.4
-	ninja>=1.10
 	pillow>=8.4.0
-	pytorch-lightning>=1.5.5
 	pytorchvideo>=0.1.3
 	torch>=1.10.0
 	torchmetrics>=0.6.1
 	torchvision>=0.11.1
 	tqdm>=4.62.3
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.extras_require]
 dev = 
-	black==21.12b0
-	compressai==1.1.9
-	flake8==4.0.1
-	fvcore==0.1.5.post20211023
-	h5py==3.1.0
-	isort==5.10.1
-	jaxlib==0.1.75
-	jax==0.2.26
-	lpips==0.1.4
-	mypy==0.910
-	ninja==1.10.2
-	opencv-python~=4.5.4.60
-	pillow==8.4.0
-	pre-commit~=2.16.0
-	pytest==6.2.5
-	pytorch-lightning==1.5.5
-	pytorchvideo==0.1.3
-	tensorflow-addons~=0.15.0
-	tensorflow~=2.7.0
-	torch==1.10.1
-	torchmetrics==0.6.1
-	torchvision==0.11.2
+	black>=21.12b0
+	flake8>=4.0.1
+	isort>=5.10.1
+	mypy>=0.910
+	pre-commit>=2.16.0
+	pytest>=6.2.5
 docs = 
 	myst-parser>=0.15.2
 	sphinx-autodoc-typehints>=1.12.0
 	sphinx-copybutton>=0.4.0
 	sphinx-gallery>=0.10.1
 	sphinx-rtd-theme>=1.0.0
 	sphinxcontrib-katex>=0.8.6
 	sphinx>=4.3.1
+tests = 
+	black==23.3.0
+	compressai==1.2.4
+	flake8==6.0.0
+	fvcore==0.1.5.post20221221
+	isort==5.12.0
+	lpips==0.1.4
+	mypy==1.1.1
+	opencv-python~=4.7.0.72
+	pillow==9.4.0
+	pytest==7.2.2
+	pytorchvideo==0.1.5
+	tensorflow==2.12.0
+	tensorflow-addons==0.19.0
+	torch==2.0.0
+	torchmetrics==0.11.4
+	torchvision==0.15.1
 
 [options.packages.find]
 exclude = 
 	tests
 	projects
 
 [egg_info]
```

### Comparing `neuralcompression-0.2.1/tests/data/test_clic_2020_image.py` & `neuralcompression-0.2.2/tests/data/test_clic_2020_image.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/data/test_clic_2020_video.py` & `neuralcompression-0.2.2/tests/data/test_clic_2020_video.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/data/test_kodak.py` & `neuralcompression-0.2.2/tests/data/test_kodak.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/data/test_vimeo_90k_septuplet.py` & `neuralcompression-0.2.2/tests/data/test_vimeo_90k_septuplet.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/distributions/test_uniform_noise.py` & `neuralcompression-0.2.2/tests/distributions/test_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_count_flops.py` & `neuralcompression-0.2.2/tests/functional/test_count_flops.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,42 +55,42 @@
                     torch.nn.Conv2d(
                         cin, cout, kernel_size=kernel, stride=stride, padding=padding
                     )
                 )
                 cin = cout
 
         def forward(self, inp):
-            flops = torch.tensor(0)
+            flops = 0
             out = inp
             for layer, k_size in zip(self.layers, layer_kernels):
                 cin = out.shape[1]
                 out = layer(out)
                 # +3 for counting the additions to the flops variable itself
-                flops += out.numel() * k_size * k_size * cin + 3
+                flops += 3 + out.numel() * k_size * k_size * cin + 3
 
             return out, flops
 
     model = ConvModel()
     inp = torch.randn(input_shape)
     _, correct_flops = model(inp)
 
     counted_flops, _, unsupported_ops = count_flops(model, (inp,))
-    assert torch.allclose(torch.tensor(counted_flops).long(), correct_flops)
+    assert counted_flops == correct_flops
     assert len(unsupported_ops) == 0
 
 
 @pytest.mark.parametrize("input_shape", ((10, 3), (1, 1), (5, 9), (10, 9, 8)))
 def test_flop_count_elementwise(input_shape):
     # Tests that the flop counter counts flops correctly (i.e.
     # when compared to a reference value) for a model involving
     # lots of binary and elementwise operations.
 
     class ElementwiseModel(torch.nn.Module):
         def forward(self, inp):
-            flops = torch.tensor(0)
+            flops = 5  # view operations
             out = inp
 
             out = out * 2
             # +1 here and below for counting the additions to the flop
             # variable itself.
             flops += out.numel() + 1
 
@@ -108,15 +108,15 @@
     model = ElementwiseModel()
     inp = torch.randn(input_shape)
     _, correct_flops = model(inp)
 
     counted_flops, _, unsupported_ops = count_flops(
         model, (inp,), use_single_flop_estimates=True
     )
-    assert torch.allclose(torch.tensor(counted_flops).long(), correct_flops)
+    assert counted_flops == correct_flops
     assert len(unsupported_ops) == 0
 
 
 @pytest.mark.parametrize(
     "batch_size, network_channels, compression_channels, img_size", [(1, 8, 16, 128)]
 )
 def test_flop_count_hyperprior(
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_dense_image_warp.py` & `neuralcompression-0.2.2/tests/functional/test_dense_image_warp.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,20 @@
 )
 def test_dense_image_warp(shape, seed):
     rng = numpy.random.default_rng(seed)
     image = create_input(shape)
 
     # this test won't work for completely random warps - about a 10% error
     # so we create a single vector flow and rotate it randomly
-    flow = (
-        numpy.stack(
-            (
-                numpy.ones(shape[0] * shape[-2] * shape[-1]),
-                numpy.zeros(shape[0] * shape[-2] * shape[-1]),
-            )
+    flow = numpy.stack(
+        (
+            numpy.ones(shape[0] * shape[-2] * shape[-1]),
+            numpy.zeros(shape[0] * shape[-2] * shape[-1]),
         )
-        * (rng.uniform() / 10)
-    )
+    ) * (rng.uniform() / 10)
 
     angle = rng.uniform() * 2 * numpy.pi
     cos_val, sin_val = numpy.cos(angle), numpy.sin(angle)
     rot_mat = numpy.array(((cos_val, -sin_val), (sin_val, cos_val)))
     flow = numpy.reshape(
         numpy.transpose(rot_mat @ flow), (shape[0], shape[-2], shape[-1], 2)
     )
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_estimate_tails.py` & `neuralcompression-0.2.2/tests/functional/test_estimate_tails.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_hsv_to_rgb.py` & `neuralcompression-0.2.2/tests/functional/test_hsv_to_rgb.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_information_content.py` & `neuralcompression-0.2.2/tests/functional/test_information_content.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_log_cdf.py` & `neuralcompression-0.2.2/tests/functional/test_log_cdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from neuralcompression.functional import log_cdf
 
 
 def test_log_cdf():
     rng = numpy.random.default_rng(0xFEEEFEEE)
 
-    x = rng.random((32,), dtype=numpy.float)
+    x = rng.random((32,), dtype=numpy.float64)
 
     actual = log_cdf(torch.tensor(x, dtype=torch.float), Normal(0.0, 1.0))
 
     assert torch.isfinite(actual).all()
 
     torch.testing.assert_close(
         actual,
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_log_expm1.py` & `neuralcompression-0.2.2/tests/functional/test_log_expm1.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from neuralcompression.functional import log_expm1
 
 
 def test_log_expm1():
     rng = numpy.random.default_rng(0xFEEEFEEE)
 
-    x = rng.random((32,), dtype=numpy.float)
+    x = rng.random((32,), dtype=numpy.float64)
 
     actual = log_expm1(torch.tensor(x, dtype=torch.float))
 
     assert torch.isfinite(actual).all()
 
     torch.testing.assert_close(
         actual,
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_log_ndtr.py` & `neuralcompression-0.2.2/tests/functional/test_log_ndtr.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from neuralcompression.functional import log_ndtr
 
 
 def test_log_ndtr():
     rng = numpy.random.default_rng(0xDEADBEEF)
 
-    x = rng.random((32,), dtype=numpy.float)
+    x = rng.random((32,), dtype=numpy.float64)
 
     actual = log_ndtr(torch.tensor(x, dtype=torch.float))
 
     assert torch.isfinite(actual).all()
 
     torch.testing.assert_close(
         actual,
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_log_survival_function.py` & `neuralcompression-0.2.2/tests/functional/test_log_survival_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 
 def test_log_survival_function():
     rng = numpy.random.default_rng(0xFEEEFEEE)
 
     batch_size = 32
 
-    loc = rng.standard_normal(batch_size, dtype=numpy.float)
+    loc = rng.standard_normal(batch_size, dtype=numpy.float64)
 
-    scale = rng.random(batch_size, dtype=numpy.float) + 1.0
+    scale = rng.random(batch_size, dtype=numpy.float64) + 1.0
 
-    x = numpy.linspace(-8.0, 8.0, batch_size, dtype=numpy.float)
+    x = numpy.linspace(-8.0, 8.0, batch_size, dtype=numpy.float64)
 
     torch.testing.assert_allclose(
         log_survival_function(
             torch.tensor(x, dtype=torch.float),
             Normal(
                 torch.tensor(loc, dtype=torch.float),
                 torch.tensor(scale, dtype=torch.float),
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_lower_bound.py` & `neuralcompression-0.2.2/tests/functional/test_lower_bound.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_lower_tail.py` & `neuralcompression-0.2.2/tests/functional/test_lower_tail.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_lpips.py` & `neuralcompression-0.2.2/tests/functional/test_lpips.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_multiscale_structural_similarity.py` & `neuralcompression-0.2.2/tests/functional/test_multiscale_structural_similarity.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_ndtr.py` & `neuralcompression-0.2.2/tests/functional/test_ndtr.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,13 +15,13 @@
     torch.testing.assert_close(
         ndtr(torch.tensor([0.0])),
         torch.tensor([0.5]),
     )
 
     rng = numpy.random.default_rng(0xDEADBEEF)
 
-    x = rng.random((32,), dtype=numpy.float)
+    x = rng.random((32,), dtype=numpy.float64)
 
     torch.testing.assert_close(
         ndtr(torch.tensor(x, dtype=torch.float)),
         torch.tensor(scipy.special.ndtr(x), dtype=torch.float),
     )
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_optical_flow_to_rgb.py` & `neuralcompression-0.2.2/tests/functional/test_optical_flow_to_rgb.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,20 @@
 )
 def test_dense_image_warp(shape, seed):
     rng = np.random.default_rng(seed)
     image = create_input(shape)
 
     # this test won't work for completely random warps - about a 10% error
     # so we create a single vector flow and rotate it randomly
-    flow = (
-        np.stack(
-            (
-                np.ones(shape[0] * shape[-2] * shape[-1]),
-                np.zeros(shape[0] * shape[-2] * shape[-1]),
-            )
+    flow = np.stack(
+        (
+            np.ones(shape[0] * shape[-2] * shape[-1]),
+            np.zeros(shape[0] * shape[-2] * shape[-1]),
         )
-        * (rng.uniform() / 10)
-    )
+    ) * (rng.uniform() / 10)
     angle = rng.uniform() * 2 * np.pi
     cos_val, sin_val = np.cos(angle), np.sin(angle)
     rot_mat = np.array(((cos_val, -sin_val), (sin_val, cos_val)))
     flow = np.reshape(np.transpose(rot_mat @ flow), (shape[0], shape[-2], shape[-1], 2))
     flow = torch.tensor(flow).to(image)
 
     image_warp = ncF.dense_image_warp(image, flow, align_corners=True)
```

### Comparing `neuralcompression-0.2.1/tests/functional/test_soft_round.py` & `neuralcompression-0.2.2/tests/functional/test_soft_round.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_soft_round_conditional_mean.py` & `neuralcompression-0.2.2/tests/functional/test_soft_round_conditional_mean.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_soft_round_inverse.py` & `neuralcompression-0.2.2/tests/functional/test_soft_round_inverse.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_survival_function.py` & `neuralcompression-0.2.2/tests/functional/test_survival_function.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/functional/test_upper_tail.py` & `neuralcompression-0.2.2/tests/functional/test_upper_tail.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/layers/test_continuous_entropy.py` & `neuralcompression-0.2.2/tests/layers/test_continuous_entropy.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/layers/test_generalized_divisive_normalization.py` & `neuralcompression-0.2.2/tests/layers/test_generalized_divisive_normalization.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         assert normalized.shape == x.shape
 
         assert x.grad is not None
 
         assert x.grad.shape == x.shape
 
         torch.testing.assert_allclose(
-            x / torch.sqrt(1 + 0.1 * (x ** 2)),
+            x / torch.sqrt(1 + 0.1 * (x**2)),
             normalized,
         )
 
         normalization = GeneralizedDivisiveNormalization(
             32,
             inverse=True,
         )
@@ -42,10 +42,10 @@
         assert normalized.shape == x.shape
 
         assert x.grad is not None
 
         assert x.grad.shape == x.shape
 
         torch.testing.assert_allclose(
-            x * torch.sqrt(1 + 0.1 * (x ** 2)),
+            x * torch.sqrt(1 + 0.1 * (x**2)),
             normalized,
         )
```

### Comparing `neuralcompression-0.2.1/tests/layers/test_hyper_synthesis_transformation_2d.py` & `neuralcompression-0.2.2/tests/layers/test_hyper_synthesis_transformation_2d.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/layers/test_non_negative_parameterization.py` & `neuralcompression-0.2.2/tests/layers/test_non_negative_parameterization.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         parameterization = NonNegativeParameterization(x)
 
         assert parameterization.initial_value.shape == x.shape
 
         assert torch.allclose(
             parameterization.initial_value,
             torch.sqrt(torch.max(x, x - x)),
-            atol=2 ** -18,
+            atol=2**-18,
         )
 
         for _ in range(10):
             minimum = torch.rand(1)
 
             x = torch.rand((1, 8, 8, 8)) * 2 - 1
```

### Comparing `neuralcompression-0.2.1/tests/layers/test_rate_mse_distortion_loss.py` & `neuralcompression-0.2.2/tests/layers/test_rate_mse_distortion_loss.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/models/_hific/test_hific_discriminator.py` & `neuralcompression-0.2.2/tests/models/_hific/test_hific_discriminator.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/models/test_factorized_prior_autoencoder.py` & `neuralcompression-0.2.2/tests/models/test_factorized_prior_autoencoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
         assert probabilities
 
         y_probabilities = probabilities[0]
 
         assert y_probabilities.size()[0] == x.size()[0]
         assert y_probabilities.size()[1] == 192
-        assert y_probabilities.size()[2] == x.size()[2] / 2 ** 4
-        assert y_probabilities.size()[3] == x.size()[3] / 2 ** 4
+        assert y_probabilities.size()[2] == x.size()[2] / 2**4
+        assert y_probabilities.size()[3] == x.size()[3] / 2**4
 
     def test_from_state_dict(self, tmpdir):
         for n, m in [(128, 128), (128, 192), (192, 128)]:
             prior_a = FactorizedPriorAutoencoder(n, m)
 
             assert prior_a.network_channels == n
             assert prior_a.compression_channels == m
```

### Comparing `neuralcompression-0.2.1/tests/models/test_mean_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/tests/models/test_mean_scale_hyperprior_autoencoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
         assert x_hat.size() == x.size()
 
         y_scores_size = y_scores.size()
 
         assert y_scores_size[0] == x.size()[0]
         assert y_scores_size[1] == 192
-        assert y_scores_size[2] == x.size()[2] / 2 ** 4
-        assert y_scores_size[3] == x.size()[3] / 2 ** 4
+        assert y_scores_size[2] == x.size()[2] / 2**4
+        assert y_scores_size[3] == x.size()[3] / 2**4
 
         z_scores_size = z_scores.size()
 
         assert z_scores_size[0] == x.size()[0]
         assert z_scores_size[1] == 128
-        assert z_scores_size[2] == x.size()[2] / 2 ** 6
-        assert z_scores_size[3] == x.size()[3] / 2 ** 6
+        assert z_scores_size[2] == x.size()[2] / 2**6
+        assert z_scores_size[3] == x.size()[3] / 2**6
```

### Comparing `neuralcompression-0.2.1/tests/models/test_prior_autoencoder.py` & `neuralcompression-0.2.2/tests/models/test_prior_autoencoder.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/models/test_scale_hyperprior_autoencoder.py` & `neuralcompression-0.2.2/tests/models/test_scale_hyperprior_autoencoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
         assert x_hat.size() == x.size()
 
         y_scores_size = y_scores.size()
 
         assert y_scores_size[0] == x.size()[0]
         assert y_scores_size[1] == 192
-        assert y_scores_size[2] == x.size()[2] / 2 ** 4
-        assert y_scores_size[3] == x.size()[3] / 2 ** 4
+        assert y_scores_size[2] == x.size()[2] / 2**4
+        assert y_scores_size[3] == x.size()[3] / 2**4
 
         z_scores_size = z_scores.size()
 
         assert z_scores_size[0] == x.size()[0]
         assert z_scores_size[1] == 128
-        assert z_scores_size[2] == x.size()[2] / 2 ** 6
-        assert z_scores_size[3] == x.size()[3] / 2 ** 6
+        assert z_scores_size[2] == x.size()[2] / 2**6
+        assert z_scores_size[3] == x.size()[3] / 2**6
 
     def test_from_state_dict(self, tmpdir):
         for n, m in [(128, 128), (128, 192), (192, 128)]:
             model = ScaleHyperpriorAutoencoder(n, m)
 
             filepath = tmpdir.join("model.pth.rar").strpath
```

### Comparing `neuralcompression-0.2.1/tests/test_entropy_coders.py` & `neuralcompression-0.2.2/projects/jax_entropy_coders/test_entropy_coders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+import craystack
 import jax.numpy as jnp
+import jax_arithmetic_coder as jac
 import numpy as np
 import pytest
 import scipy
 
-import neuralcompression.entropy_coders
-
 
 def freqs_to_cdf(freqs, precision=16):
     # Converts a frequency count to a discretized CDF with values
     # between [0, 2**precision)
     pdf = freqs / freqs.sum(axis=-1, keepdims=True)
     cdf = jnp.append(jnp.zeros((*pdf.shape[:-1], 1)), pdf.cumsum(axis=-1), axis=-1)
-    return jnp.round(cdf * 2 ** precision).astype(jnp.uint32)
+    return jnp.round(cdf * 2**precision).astype(jnp.uint32)
 
 
 def cdf_to_pdf(cdf):
     # Converts a CDF (discretized, or not) to a PDF
     pdf = jnp.diff(cdf)  # discrete differences
     return pdf / pdf.sum()
 
@@ -73,18 +73,16 @@
     def cdf_fun(symbol, cdf_state):
         return cdf_state[0][symbol], cdf_state[0][symbol + 1], cdf_state
 
     def inverse_cdf_fun(value, cdf_state):
         symbol = jnp.argmin(value >= cdf_state[0]) - 1
         return cdf_state[0][symbol], cdf_state[0][symbol + 1], symbol, cdf_state
 
-    compressed = neuralcompression.entropy_coders.jac.encode(
-        messages, cdf_fun, cdf_state
-    )
-    decompressed = neuralcompression.entropy_coders.jac.decode(
+    compressed = jac.encode(messages, cdf_fun, cdf_state)
+    decompressed = jac.decode(
         compressed, jnp.array([message_len] * batch_size), inverse_cdf_fun, cdf_state
     )
 
     assert (decompressed == messages).all()
 
 
 @pytest.mark.parametrize(
@@ -114,18 +112,16 @@
     def cdf_fun(symbol, cdf_state):
         return cdf_state[0][symbol], cdf_state[0][symbol + 1], cdf_state
 
     def inverse_cdf_fun(value, cdf_state):
         symbol = jnp.argmin(value >= cdf_state[0]) - 1
         return cdf_state[0][symbol], cdf_state[0][symbol + 1], symbol, cdf_state
 
-    compressed = neuralcompression.entropy_coders.jac.encode(
-        messages, cdf_fun, cdf_state
-    )
-    decompressed = neuralcompression.entropy_coders.jac.decode(
+    compressed = jac.encode(messages, cdf_fun, cdf_state)
+    decompressed = jac.decode(
         compressed, jnp.array([message_len] * batch_size), inverse_cdf_fun, cdf_state
     )
 
     assert len(compressed[0]) == predicted_message_size
     assert (decompressed == messages).all()
 
 
@@ -157,18 +153,16 @@
 
     def inverse_cdf_fun(value, cdf_state):
         freqs = cdf_state[0]
         cdf = freqs_to_cdf(freqs)
         symbol = jnp.argmin(value >= cdf) - 1
         return cdf[symbol], cdf[symbol + 1], symbol, (freqs.at[symbol].add(1),)
 
-    compressed = neuralcompression.entropy_coders.jac.encode(
-        messages, cdf_fun, cdf_state
-    )
-    decompressed = neuralcompression.entropy_coders.jac.decode(
+    compressed = jac.encode(messages, cdf_fun, cdf_state)
+    decompressed = jac.decode(
         compressed, jnp.array([message_len] * batch_size), inverse_cdf_fun, cdf_state
     )
 
     assert (decompressed == messages).all()
 
 
 @pytest.mark.parametrize(
@@ -195,18 +189,16 @@
         return cdf[symbol], cdf[symbol + 1], cdf_state
 
     def inverse_cdf_fun(value, cdf_state):
         cdf = cdf_state[0]
         symbol = jnp.argmin(value >= cdf) - 1
         return cdf[symbol], cdf[symbol + 1], symbol, cdf_state
 
-    compressed = neuralcompression.entropy_coders.jac.encode(
-        messages, cdf_fun, cdf_state
-    )
-    decompressed = neuralcompression.entropy_coders.jac.decode(
+    compressed = jac.encode(messages, cdf_fun, cdf_state)
+    decompressed = jac.decode(
         compressed, jnp.array([message_len] * batch_size), inverse_cdf_fun, cdf_state
     )
 
     assert (decompressed == messages).all()
     assert len(compressed[0]) == predicted_message_size
 
 
@@ -233,27 +225,24 @@
     else:
         rng = np.random.default_rng(123)
         freqs = jnp.ones(alphabet_size) * message_len // alphabet_size
         messages = jnp.array(
             rng.integers(low=0, high=alphabet_size, size=shape, dtype=np.uint8)
         )
 
-    codec = neuralcompression.entropy_coders.craystack.fixed_array_cdf_codec(
+    codec = craystack.fixed_array_cdf_codec(
         jnp.tile(freqs_to_cdf(freqs), (batch_size, interleave_level, 1)).astype(
             jnp.uint32
         )
     )
 
-    compressed = neuralcompression.entropy_coders.craystack.encode(messages, codec)[0]
-    decompressed = neuralcompression.entropy_coders.craystack.decode(
-        compressed,
-        message_len,
-        messages.shape[2:],
-        codec,
-    )[0]
+    compressed = craystack.encode(messages, codec)[0]
+    decompressed = craystack.decode(compressed, message_len, messages.shape[2:], codec)[
+        0
+    ]
 
     assert (decompressed == messages).all()
 
 
 @pytest.mark.parametrize(
     "shape1, shape2, alphabet_size",
     [
@@ -272,43 +261,38 @@
     messages1 = jnp.array(
         rng.integers(low=0, high=alphabet_size, size=shape1, dtype=np.uint8)
     )
     messages2 = jnp.array(
         rng.integers(low=0, high=alphabet_size, size=shape2, dtype=np.uint8)
     )
 
-    codec1 = neuralcompression.entropy_coders.craystack.fixed_array_cdf_codec(
+    codec1 = craystack.fixed_array_cdf_codec(
         jnp.tile(freqs_to_cdf(freqs), (batch_size, interleave_level1, 1)).astype(
             jnp.uint32
         )
     )
 
-    codec2 = neuralcompression.entropy_coders.craystack.fixed_array_cdf_codec(
+    codec2 = craystack.fixed_array_cdf_codec(
         jnp.tile(freqs_to_cdf(freqs), (batch_size, interleave_level2, 1)).astype(
             jnp.uint32
         )
     )
 
-    compressed = neuralcompression.entropy_coders.craystack.encode(
-        messages1, codec1, tail_capacity=tail_capacity
+    compressed = craystack.encode(messages1, codec1, tail_capacity=tail_capacity)[0]
+    compressed = craystack.encode(
+        messages2, codec2, start_buffers=compressed, tail_capacity=tail_capacity
     )[0]
-    compressed = neuralcompression.entropy_coders.craystack.encode(
-        messages2,
-        codec2,
-        start_buffers=compressed,
-        tail_capacity=tail_capacity,
-    )[0]
-    decompressed2, compressed, _ = neuralcompression.entropy_coders.craystack.decode(
+    decompressed2, compressed, _ = craystack.decode(
         compressed,
         message_len2,
         messages2.shape[2:],
         codec2,
         tail_capacity=tail_capacity,
     )
-    decompressed1, _, _ = neuralcompression.entropy_coders.craystack.decode(
+    decompressed1, _, _ = craystack.decode(
         compressed,
         message_len1,
         messages1.shape[2:],
         codec1,
         tail_capacity=tail_capacity,
     )
 
@@ -351,30 +335,21 @@
         symbols = jnp.argmin(jnp.expand_dims(cdf_value, -1) >= cdf, axis=-1) - 1
 
         for symbol in jnp.flip(symbols):
             freqs.at[symbol].add(-1)
 
         return cdf[symbols], cdf[symbols + 1], symbols, (freqs,)
 
-    codec = neuralcompression.entropy_coders.craystack.default_rans_codec(
-        cdf_fun, inverse_cdf_fun, cdf_state
-    )
+    codec = craystack.default_rans_codec(cdf_fun, inverse_cdf_fun, cdf_state)
 
-    compressed, cdf_state = neuralcompression.entropy_coders.craystack.encode(
-        messages, codec
-    )
-    codec = neuralcompression.entropy_coders.craystack.default_rans_codec(
-        cdf_fun, inverse_cdf_fun, cdf_state
-    )
-    decompressed = neuralcompression.entropy_coders.craystack.decode(
-        compressed,
-        message_len,
-        messages.shape[2:],
-        codec,
-    )[0]
+    compressed, cdf_state = craystack.encode(messages, codec)
+    codec = craystack.default_rans_codec(cdf_fun, inverse_cdf_fun, cdf_state)
+    decompressed = craystack.decode(compressed, message_len, messages.shape[2:], codec)[
+        0
+    ]
 
     assert (decompressed == messages).all()
 
 
 @pytest.mark.parametrize(
     "batch_size, message_len, interleave_levels, alphabet_size",
     [(1, 1, 1, 2), (100, 5, 784, 2), (100, 10, 50, 10)],
@@ -388,30 +363,25 @@
     freqs = jnp.array(
         rng.integers(
             low=1,
             high=10,
             size=(batch_size, interleave_levels, alphabet_size),
         )
     )
-    codec = neuralcompression.entropy_coders.craystack.fixed_array_cdf_codec(
-        freqs_to_cdf(freqs)
-    )
+    codec = craystack.fixed_array_cdf_codec(freqs_to_cdf(freqs))
     messages = jnp.array(
         rng.integers(
             low=0,
             high=alphabet_size,
             size=(batch_size, message_len, interleave_levels),
             dtype=np.int64,
         )
     )
-    decompressed = neuralcompression.entropy_coders.craystack.decode(
-        neuralcompression.entropy_coders.craystack.encode(messages, codec)[0],
-        message_len,
-        messages.shape[2:],
-        codec,
+    decompressed = craystack.decode(
+        craystack.encode(messages, codec)[0], message_len, messages.shape[2:], codec
     )[0]
     assert (decompressed == messages).all()
 
 
 @pytest.mark.parametrize(
     (
         "batch_size, message_len, interleave_levels, obs_alphabet_size,"
@@ -431,75 +401,58 @@
     # Uses an identical CDF for all interleave levels,
     # but is a function of symbols and latents
     obs_shape = latent_shape = (interleave_levels,)
 
     rng = np.random.default_rng(123)
     cdf_latent_prior = freqs_to_cdf(  # p(z)
         jnp.array(
-            rng.integers(
-                low=1,
-                high=10,
-                size=(*latent_shape, latent_alphabet_size),
-            )
+            rng.integers(low=1, high=10, size=(*latent_shape, latent_alphabet_size))
         )
     )
     cdf_latent_posterior = freqs_to_cdf(  # q(z|x)
         jnp.array(
-            rng.integers(
-                low=1,
-                high=10,
-                size=(obs_alphabet_size, latent_alphabet_size),
-            )
+            rng.integers(low=1, high=10, size=(obs_alphabet_size, latent_alphabet_size))
         )
     )
     cdf_obs = freqs_to_cdf(  # p(x|z)
         jnp.array(
-            rng.integers(
-                low=1,
-                high=10,
-                size=(latent_alphabet_size, obs_alphabet_size),
-            )
+            rng.integers(low=1, high=10, size=(latent_alphabet_size, obs_alphabet_size))
         )
     )
 
     messages = jnp.array(
         rng.integers(
             low=0,
             high=obs_alphabet_size,
             size=(batch_size, message_len, *obs_shape),
             dtype=message_dtype,
         )
     )
 
-    latent_prior_codec = (
-        neuralcompression.entropy_coders.craystack.fixed_array_cdf_codec(
-            cdf_latent_prior, message_dtype=message_dtype
-        )
+    latent_prior_codec = craystack.fixed_array_cdf_codec(
+        cdf_latent_prior, message_dtype=message_dtype
     )
 
     def latent_posterior_codec_maker(symbols):
-        return neuralcompression.entropy_coders.craystack.fixed_array_cdf_codec(
+        return craystack.fixed_array_cdf_codec(
             cdf_latent_posterior[symbols],
             allow_empty_pops=True,
             message_dtype=message_dtype,
         )
 
     def obs_codec_maker(latents):
-        return neuralcompression.entropy_coders.craystack.fixed_array_cdf_codec(
+        return craystack.fixed_array_cdf_codec(
             cdf_obs[latents], message_dtype=message_dtype
         )
 
-    codec = neuralcompression.entropy_coders.craystack.bitsback_ans_codec(
+    codec = craystack.bitsback_ans_codec(
         latent_prior_codec,
         latent_posterior_codec_maker,
         obs_codec_maker,
         latent_shape,
         message_dtype,
     )
 
-    decompressed = neuralcompression.entropy_coders.craystack.decode(
-        neuralcompression.entropy_coders.craystack.encode(messages, codec)[0],
-        message_len,
-        messages.shape[2:],
-        codec,
+    decompressed = craystack.decode(
+        craystack.encode(messages, codec)[0], message_len, messages.shape[2:], codec
     )[0]
     assert (decompressed == messages).all()
```

### Comparing `neuralcompression-0.2.1/tests/test_layers_gdn.py` & `neuralcompression-0.2.2/tests/test_layers_gdn.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/test_models.py` & `neuralcompression-0.2.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tests/test_scale_hyperprior.py` & `neuralcompression-0.2.2/tests/test_scale_hyperprior.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     # This test also verifies that the model's image reconstruction has
     # the same shape as the original image.
 
     inp = torch.randn(1, 3, img_size, img_size)
     model = ScaleHyperprior(
         network_channels=network_channels, compression_channels=compression_channels
     )
+    model.eval()
     outputs = model(inp)
     assert outputs[0].shape == inp.shape
 
 
 @pytest.mark.parametrize(
     "network_channels,compression_channels,img_size", [(128, 256, 256), (256, 128, 100)]
 )
```

### Comparing `neuralcompression-0.2.1/tests/utils.py` & `neuralcompression-0.2.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tutorials/Flop_Count_Example.ipynb` & `neuralcompression-0.2.2/tutorials/Flop_Count_Example.ipynb`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tutorials/Metrics_Example.ipynb` & `neuralcompression-0.2.2/tutorials/Metrics_Example.ipynb`

 * *Files identical despite different names*

### Comparing `neuralcompression-0.2.1/tutorials/image_compression.ipynb` & `neuralcompression-0.2.2/tutorials/image_compression.ipynb`

 * *Files identical despite different names*

