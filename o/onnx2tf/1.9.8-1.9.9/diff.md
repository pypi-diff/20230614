# Comparing `tmp/onnx2tf-1.9.8.tar.gz` & `tmp/onnx2tf-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2tf-1.9.8.tar", last modified: Wed Apr 19 00:10:59 2023, max compression
+gzip compressed data, was "onnx2tf-1.9.9.tar", last modified: Fri Apr 21 15:12:54 2023, max compression
```

## Comparing `onnx2tf-1.9.8.tar` & `onnx2tf-1.9.9.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:10:59.593104 onnx2tf-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/LICENSE_onnx-tensorflow
--rw-r--r--   0 runner    (1001) docker     (123)   104992 2023-04-19 00:10:59.593104 onnx2tf-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   104450 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:10:59.569103 onnx2tf-1.9.8/onnx2tf/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96544 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/onnx2tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:10:59.593104 onnx2tf-1.9.8/onnx2tf/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Abs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Acos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Acosh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/And.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ArgMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ArgMin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Asin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Asinh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Atan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Atanh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/AveragePool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/BatchNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Bernoulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/BitShift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Celu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ConcatFromSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ConstantOfShape.py
--rw-r--r--   0 runner    (1001) docker     (123)    37236 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ConvTranspose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Cos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Cosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/CumSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/DepthToSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/DequantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Det.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Div.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/DynamicQuantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Einsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Elu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Equal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Erf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/EyeLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/FusedConv.py
--rw-r--r--   0 runner    (1001) docker     (123)    30230 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GRU.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GatherElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GatherND.py
--rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Gemm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GlobalAveragePool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GlobalLpPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GlobalMaxPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Greater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GreaterOrEqual.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/GridSample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/HardSigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/HardSwish.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Hardmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/If.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/InstanceNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/IsInf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/IsNaN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/LRN.py
--rw-r--r--   0 runner    (1001) docker     (123)    43038 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/LayerNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/LeakyRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Less.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/LessOrEqual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/LogSoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/LpNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/MatMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/MatMulInteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Max.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/MaxPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/MaxUnpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/MeanVarianceNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Min.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Mul.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Multinomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Neg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/NonMaxSuppression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/NonZero.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Not.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/OneHot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Or.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/PRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Pow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearAdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearConcat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearLeakyRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearMatMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearMul.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearSigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QLinearSoftmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/QuantizeLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    27641 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/RNN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/RandomNormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/RandomNormalLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/RandomUniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/RandomUniformLike.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceL1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceL2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceLogSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceLogSumExp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceMax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceMean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceMin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceProd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceSum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReduceSumSquare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Relu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    25352 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ReverseSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/RoiAlign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Round.py
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ScaleAndTranslate.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ScatterElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ScatterND.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Selu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SequenceAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SequenceConstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SequenceEmpty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SequenceErase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SequenceInsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SequenceLength.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Shrink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Sin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Sinh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Size.py
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Softplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Softsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SpaceToDepth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/SplitToSequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Sqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Squeeze.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Tan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/ThresholdedRelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/TopK.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Trilu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Unique.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Where.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/Xor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/_Loop.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:10:59.593104 onnx2tf-1.9.8/onnx2tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)   199977 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/utils/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/onnx2tf/utils/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:10:59.569103 onnx2tf-1.9.8/onnx2tf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   104992 2023-04-19 00:10:59.000000 onnx2tf-1.9.8/onnx2tf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-19 00:10:59.000000 onnx2tf-1.9.8/onnx2tf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:10:59.000000 onnx2tf-1.9.8/onnx2tf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 00:10:59.000000 onnx2tf-1.9.8/onnx2tf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 00:10:59.000000 onnx2tf-1.9.8/onnx2tf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:10:59.593104 onnx2tf-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:10:59.593104 onnx2tf-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-19 00:10:44.000000 onnx2tf-1.9.8/tests/test_model_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:12:54.058656 onnx2tf-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/LICENSE_onnx-tensorflow
+-rw-r--r--   0 runner    (1001) docker     (123)   105538 2023-04-21 15:12:54.054656 onnx2tf-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   104996 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:12:54.034656 onnx2tf-1.9.9/onnx2tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96544 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/onnx2tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:12:54.054656 onnx2tf-1.9.9/onnx2tf/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Abs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Acos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Acosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/And.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ArgMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ArgMin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Asin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Asinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Atan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Atanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/AveragePool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/BatchNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Bernoulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/BitShift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Celu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ConcatFromSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ConstantOfShape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37236 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ConvTranspose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Cos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Cosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/CumSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/DepthToSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/DequantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Det.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Div.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/DynamicQuantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Elu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Erf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/EyeLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/FusedConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30230 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GRU.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GatherElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GatherND.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Gemm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GlobalAveragePool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GlobalLpPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GlobalMaxPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Greater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GreaterOrEqual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/GridSample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/HardSigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/HardSwish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Hardmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/If.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/InstanceNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/IsInf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/IsNaN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/LRN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43038 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/LayerNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/LeakyRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Less.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/LessOrEqual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/LogSoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/LpNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/MatMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/MatMulInteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Max.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/MaxPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/MaxUnpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/MeanVarianceNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Mul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Multinomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/NonMaxSuppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/NonZero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Not.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/OneHot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Or.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/PRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Pow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearAdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearConcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearLeakyRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearMatMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearMul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearSigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QLinearSoftmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/QuantizeLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27641 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/RNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/RandomNormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/RandomNormalLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/RandomUniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/RandomUniformLike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceL1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceL2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceLogSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceLogSumExp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceMax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceMean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceMin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceProd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceSum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReduceSumSquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25352 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ReverseSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/RoiAlign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Round.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ScaleAndTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ScatterElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ScatterND.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Selu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SequenceAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SequenceConstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SequenceEmpty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SequenceErase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SequenceInsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SequenceLength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Shrink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Sin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Sinh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Softplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Softsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SpaceToDepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/SplitToSequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Tan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/ThresholdedRelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/TopK.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Trilu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/Xor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/_Loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:12:54.054656 onnx2tf-1.9.9/onnx2tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199977 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/utils/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/onnx2tf/utils/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:12:54.034656 onnx2tf-1.9.9/onnx2tf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   105538 2023-04-21 15:12:54.000000 onnx2tf-1.9.9/onnx2tf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-21 15:12:54.000000 onnx2tf-1.9.9/onnx2tf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:12:54.000000 onnx2tf-1.9.9/onnx2tf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 15:12:54.000000 onnx2tf-1.9.9/onnx2tf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 15:12:54.000000 onnx2tf-1.9.9/onnx2tf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:12:54.058656 onnx2tf-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:12:54.054656 onnx2tf-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-04-21 15:12:42.000000 onnx2tf-1.9.9/tests/test_model_convert.py
```

### Comparing `onnx2tf-1.9.8/LICENSE` & `onnx2tf-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/LICENSE_onnx-tensorflow` & `onnx2tf-1.9.9/LICENSE_onnx-tensorflow`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/PKG-INFO` & `onnx2tf-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2tf
-Version: 1.9.8
+Version: 1.9.9
 Summary: Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in onnx-tensorflow (onnx-tf).
 Home-page: https://github.com/PINTO0309/onnx2tf
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -225,15 +225,15 @@
 
 ## Demo
 Video speed is adjusted approximately 50 times slower than actual speed.
 ![render1665941718294](https://user-images.githubusercontent.com/33194443/196049928-57520fc2-842d-459c-9f28-7ee5f040c226.gif)
 
 ## Environment
 - onnx
-- onnxruntime
+- onnxruntime==1.13.1 See: [When using onnxruntime v1.14.1, all output values of Sigmoid are Nan. #14885](https://github.com/microsoft/onnxruntime/issues/14885)
 - onnx-simplifier==0.4.17 See: https://github.com/PINTO0309/onnx2tf/issues/312
 - onnx_graphsurgeon
 - simple_onnx_processing_tools
 - tensorflow==2.12.0
 - flatbuffers-compiler (Optional, Only when using the `-coion` option. Executable file named `flatc`.)
   ```bash
   # Custom flatc binary for Ubuntu 20.04+
@@ -252,15 +252,15 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.8
+  ghcr.io/pinto0309/onnx2tf:1.9.9
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
@@ -531,14 +531,15 @@
     ```
 
 - Other recommended replacement OP
 
     |Before|After|
     |:-:|:-:|
     |`HardSwish`<br>![image](https://user-images.githubusercontent.com/33194443/226223099-c7344bcf-d24d-4b35-a1d6-2a03dbfce8c7.png)|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
+    |`ReLU6`<br>![image](https://user-images.githubusercontent.com/33194443/233639086-721e5e80-08c3-4785-9c1a-002bbfc0fa3d.png)<br>Paper: [A Quantization-Friendly Separable Convolution for MobileNets](https://arxiv.org/pdf/1803.08607.pdf) https://arxiv.org/pdf/1803.08607.pdf|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
 
 
 ### 7. Calibration data creation for INT8 quantization
 Calibration data (.npy) for INT8 quantization (`-cind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
```

### Comparing `onnx2tf-1.9.8/README.md` & `onnx2tf-1.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
 ## Demo
 Video speed is adjusted approximately 50 times slower than actual speed.
 ![render1665941718294](https://user-images.githubusercontent.com/33194443/196049928-57520fc2-842d-459c-9f28-7ee5f040c226.gif)
 
 ## Environment
 - onnx
-- onnxruntime
+- onnxruntime==1.13.1 See: [When using onnxruntime v1.14.1, all output values of Sigmoid are Nan. #14885](https://github.com/microsoft/onnxruntime/issues/14885)
 - onnx-simplifier==0.4.17 See: https://github.com/PINTO0309/onnx2tf/issues/312
 - onnx_graphsurgeon
 - simple_onnx_processing_tools
 - tensorflow==2.12.0
 - flatbuffers-compiler (Optional, Only when using the `-coion` option. Executable file named `flatc`.)
   ```bash
   # Custom flatc binary for Ubuntu 20.04+
@@ -237,15 +237,15 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.8
+  ghcr.io/pinto0309/onnx2tf:1.9.9
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
@@ -516,14 +516,15 @@
     ```
 
 - Other recommended replacement OP
 
     |Before|After|
     |:-:|:-:|
     |`HardSwish`<br>![image](https://user-images.githubusercontent.com/33194443/226223099-c7344bcf-d24d-4b35-a1d6-2a03dbfce8c7.png)|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
+    |`ReLU6`<br>![image](https://user-images.githubusercontent.com/33194443/233639086-721e5e80-08c3-4785-9c1a-002bbfc0fa3d.png)<br>Paper: [A Quantization-Friendly Separable Convolution for MobileNets](https://arxiv.org/pdf/1803.08607.pdf) https://arxiv.org/pdf/1803.08607.pdf|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
 
 
 ### 7. Calibration data creation for INT8 quantization
 Calibration data (.npy) for INT8 quantization (`-cind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
```

### Comparing `onnx2tf-1.9.8/onnx2tf/onnx2tf.py` & `onnx2tf-1.9.9/onnx2tf/onnx2tf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Abs.py` & `onnx2tf-1.9.9/onnx2tf/ops/Abs.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Acos.py` & `onnx2tf-1.9.9/onnx2tf/ops/Acos.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Acosh.py` & `onnx2tf-1.9.9/onnx2tf/ops/Acosh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Add.py` & `onnx2tf-1.9.9/onnx2tf/ops/Add.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/And.py` & `onnx2tf-1.9.9/onnx2tf/ops/And.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ArgMax.py` & `onnx2tf-1.9.9/onnx2tf/ops/ArgMax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ArgMin.py` & `onnx2tf-1.9.9/onnx2tf/ops/ArgMin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Asin.py` & `onnx2tf-1.9.9/onnx2tf/ops/Asin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Asinh.py` & `onnx2tf-1.9.9/onnx2tf/ops/Asinh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Atan.py` & `onnx2tf-1.9.9/onnx2tf/ops/Atan.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Atanh.py` & `onnx2tf-1.9.9/onnx2tf/ops/Atanh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/AveragePool.py` & `onnx2tf-1.9.9/onnx2tf/ops/AveragePool.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,20 @@
     print_node_info,
     inverted_operation_enable_disable,
     make_tf_node_info,
     get_replacement_parameter,
     pre_process_transpose,
     post_process_transpose,
     calc_tf_pooling_pads,
-    calc_extra_padding_with_ceil
+    calc_extra_padding_with_ceil,
+    transpose_with_flexing_deterrence,
 )
 
+INF_INDEX_VALUE: int = 4294967296
+
 
 def summarize_multiplier(arr):
     """
     summarize consecutive numbers in average multiplier
     Parameters
     ----------
     arr: List
@@ -83,23 +86,66 @@
     )
     graph_node_output: gs.Variable = graph_node.outputs[0]
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
         if isinstance(graph_node_input, gs.Variable) else graph_node_input
+    input_tensor_shape = input_tensor.shape
 
     # Pre-process transpose
     input_tensor = pre_process_transpose(
         value_before_transpose=input_tensor,
         param_target='inputs',
         param_name=graph_node.inputs[0].name,
         **kwargs,
     )
 
+    # Workaround to avoid as many conversion failures as possible
+    # for models with useless Transpose immediately before them.
+    # If the input geometry of the ONNX and the input geometry of the TF model match,
+    # the input geometry on the TF model side is forcibly transposed to the NWC or NHWC or NDHWC format.
+    # However, if all dimensions of CW or CHW or CDHW have the same value,
+    # the forced transposition process is skipped because it may destroy the structure of the model.
+    onnx_input_shape = [
+        dim if isinstance(dim, int) else None for dim in graph_node.inputs[0].shape
+    ] if graph_node.inputs[0].shape is not None else None
+    tf_input_shape = [
+        dim if isinstance(dim, int) else None for dim in input_tensor_shape
+    ]
+    if onnx_input_shape is not None \
+        and len(onnx_input_shape) > 1 and len(tf_input_shape) > 1 \
+        and onnx_input_shape == tf_input_shape:
+
+        shape_for_judging_skip = [
+            dim if dim is not None else INF_INDEX_VALUE for dim in onnx_input_shape[1:]
+        ]
+        if shape_for_judging_skip.count(shape_for_judging_skip[0]) != len(shape_for_judging_skip):
+            if len(onnx_input_shape) == 3:
+                # 1D - Overall model
+                input_tensor = transpose_with_flexing_deterrence(
+                    input_tensor=input_tensor,
+                    perm=[0,2,1],
+                    **kwargs,
+                )
+            elif len(onnx_input_shape) == 4:
+                # 2D - Overall model
+                input_tensor = transpose_with_flexing_deterrence(
+                    input_tensor=input_tensor,
+                    perm=[0,2,3,1],
+                    **kwargs,
+                )
+            elif len(onnx_input_shape) == 5:
+                # 3D - Overall model
+                input_tensor = transpose_with_flexing_deterrence(
+                    input_tensor=input_tensor,
+                    perm=[0,2,3,4,1],
+                    **kwargs,
+                )
+
     auto_pad = graph_node.attrs.get('auto_pad', 'NOTSET')
     ceil_mode = bool(graph_node.attrs.get('ceil_mode', 0))
     count_include_pad = bool(graph_node.attrs.get('count_include_pad', 0))
     kernel_shape = graph_node.attrs['kernel_shape']
     spatial_size = len(kernel_shape)
     dilations = graph_node.attrs.get('dilations', [1] * spatial_size)
     pads = graph_node.attrs.get('pads', [0] * spatial_size * 2)
@@ -110,23 +156,24 @@
     extra_pads = [0] * spatial_size
     average_multiplier = None
 
     # default tensorflow action is 'SAME_UPPER' mode (extra padding in the end for odd numbers)
     # explicit pad layer is added for tensorflow incompatible cases
     tf_pad_mode = 'VALID'
     is_explicit_padding = False
-    tf_pads = calc_tf_pooling_pads(input_shape=input_tensor_shape,
-                                   kernel=kernel_shape,
-                                   strides=strides)
+    tf_pads = calc_tf_pooling_pads(
+        input_shape=input_tensor_shape,
+        kernel=kernel_shape,
+        strides=strides
+    )
 
     func = math.ceil if ceil_mode else math.floor
     output_spatial_shape = [
         func((i + pb + pe - d * (k - 1) - 1) / s + 1)
-        for i, pb, pe, k, d, s in zip(input_tensor_shape[1:-1], pads[:len(pads) // 2], pads[len(pads) // 2:],
-                                      kernel_shape, dilations, strides)
+        for i, pb, pe, k, d, s in zip(input_tensor_shape[1:-1], pads[:len(pads) // 2], pads[len(pads) // 2:], kernel_shape, dilations, strides)
     ]
 
     # onnx padding value is ignored if auto_pad is not 'NOTSET'
     if auto_pad == 'NOTSET':
 
         # check if onnx padding is same with tensorflow padding mode 'SAME'
         # this is to avoid flex operations since tflite builtin pooling operator does not support manual padding
@@ -138,19 +185,21 @@
             auto_pad = 'VALID'
             is_explicit_padding = True
 
             # extra padding to end side (right, bottom) may be needed when ceil_mode is True
             # this extra padding should not be counted as padding when count_include_pad is True
             if ceil_mode:
                 extra_pads = \
-                    calc_extra_padding_with_ceil(input_shape=input_tensor_shape[1:-1],
-                                                 kernel=kernel_shape,
-                                                 pads=pads,
-                                                 dilations=dilations,
-                                                 strides=strides)
+                    calc_extra_padding_with_ceil(
+                        input_shape=input_tensor_shape[1:-1],
+                        kernel=kernel_shape,
+                        pads=pads,
+                        dilations=dilations,
+                        strides=strides,
+                    )
                 pads = pads[:len(pads) // 2] + [p + e for p, e in zip(pads[len(pads) // 2:], extra_pads)]
 
             tf_pads = pads
 
     elif auto_pad == 'SAME_UPPER':
         tf_pad_mode = 'SAME'
 
@@ -193,33 +242,35 @@
 
     # default tensorflow option for count_include_pad is True and cannot control
     # average value should be compensated in cases below
     # 1. when extra padding layer is added and count_include_pad is False
     # 2. when extra padding layer is not added and count_include_pad is True
     # 3. when last stride has extra padding due to ceil_mode and count_include_pad is True
     if is_explicit_padding and tf_pads != [0] * spatial_size * 2:
-        warning_msg = f'{Color.YELLOW}WARNING:{Color.RESET} ' \
-                      f'Tensorflow incompatible padding detected. ' \
-                      f'Extra pad layer is inserted automatically. '
+        warning_msg = \
+            f'{Color.YELLOW}WARNING:{Color.RESET} ' \
+            f'Tensorflow incompatible padding detected. ' \
+            f'Extra pad layer is inserted automatically. '
         print(warning_msg)
 
         if auto_pad == 'SAME_LOWER':
             # switch the order of pads
             tf_pads = [i for tup in zip(tf_pads[len(tf_pads) // 2:], tf_pads[:len(tf_pads) // 2]) for i in tup]
 
         if not count_include_pad and need_multiplier:
             average_multiplier = []
             for k, non_zero_count in zip(kernel_shape, non_zero_counts):
                 multiplier = [k / n if n != 0 else 1 for n in non_zero_count]
                 average_multiplier.append(multiplier)
 
         # convert to tensorflow padding format
-        tf_pads = [[0, 0]] + \
-                  [list(i) for i in zip(tf_pads[:len(tf_pads) // 2], tf_pads[len(tf_pads) // 2:])] + \
-                  [[0, 0]]
+        tf_pads = \
+            [[0, 0]] + \
+            [list(i) for i in zip(tf_pads[:len(tf_pads) // 2], tf_pads[len(tf_pads) // 2:])] + \
+            [[0, 0]]
 
         padded_tensor = tf.pad(
             tensor=input_tensor,
             paddings=tf_pads,
             mode='CONSTANT',
         )
 
@@ -245,14 +296,15 @@
                 average_multiplier[i][-1] = k / (k - extra_pad)
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
+        'nhwc': True,
     }
 
     # Generation of TF OP
     tf_op_type = None
     if len(kernel_shape) == 1:
         pooled_tensor = AveragePooling1D(
             pool_size=kernel_shape,
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/BatchNormalization.py` & `onnx2tf-1.9.9/onnx2tf/ops/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Bernoulli.py` & `onnx2tf-1.9.9/onnx2tf/ops/Bernoulli.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/BitShift.py` & `onnx2tf-1.9.9/onnx2tf/ops/BitShift.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Cast.py` & `onnx2tf-1.9.9/onnx2tf/ops/Cast.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Ceil.py` & `onnx2tf-1.9.9/onnx2tf/ops/Ceil.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Celu.py` & `onnx2tf-1.9.9/onnx2tf/ops/Celu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Clip.py` & `onnx2tf-1.9.9/onnx2tf/ops/Clip.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Compress.py` & `onnx2tf-1.9.9/onnx2tf/ops/Compress.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Concat.py` & `onnx2tf-1.9.9/onnx2tf/ops/Concat.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ConcatFromSequence.py` & `onnx2tf-1.9.9/onnx2tf/ops/ConcatFromSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Constant.py` & `onnx2tf-1.9.9/onnx2tf/ops/Constant.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ConstantOfShape.py` & `onnx2tf-1.9.9/onnx2tf/ops/ConstantOfShape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Conv.py` & `onnx2tf-1.9.9/onnx2tf/ops/Conv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ConvTranspose.py` & `onnx2tf-1.9.9/onnx2tf/ops/ConvTranspose.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Cos.py` & `onnx2tf-1.9.9/onnx2tf/ops/Cos.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Cosh.py` & `onnx2tf-1.9.9/onnx2tf/ops/Cosh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/CumSum.py` & `onnx2tf-1.9.9/onnx2tf/ops/CumSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/DepthToSpace.py` & `onnx2tf-1.9.9/onnx2tf/ops/DepthToSpace.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/DequantizeLinear.py` & `onnx2tf-1.9.9/onnx2tf/ops/DequantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Det.py` & `onnx2tf-1.9.9/onnx2tf/ops/Det.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Div.py` & `onnx2tf-1.9.9/onnx2tf/ops/Div.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Dropout.py` & `onnx2tf-1.9.9/onnx2tf/ops/Dropout.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/DynamicQuantizeLinear.py` & `onnx2tf-1.9.9/onnx2tf/ops/DynamicQuantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Einsum.py` & `onnx2tf-1.9.9/onnx2tf/ops/Einsum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Elu.py` & `onnx2tf-1.9.9/onnx2tf/ops/Elu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Equal.py` & `onnx2tf-1.9.9/onnx2tf/ops/Equal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Erf.py` & `onnx2tf-1.9.9/onnx2tf/ops/Erf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Exp.py` & `onnx2tf-1.9.9/onnx2tf/ops/Exp.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Expand.py` & `onnx2tf-1.9.9/onnx2tf/ops/Expand.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/EyeLike.py` & `onnx2tf-1.9.9/onnx2tf/ops/EyeLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Flatten.py` & `onnx2tf-1.9.9/onnx2tf/ops/Flatten.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Floor.py` & `onnx2tf-1.9.9/onnx2tf/ops/Floor.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/FusedConv.py` & `onnx2tf-1.9.9/onnx2tf/ops/FusedConv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GRU.py` & `onnx2tf-1.9.9/onnx2tf/ops/GRU.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Gather.py` & `onnx2tf-1.9.9/onnx2tf/ops/Gather.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GatherElements.py` & `onnx2tf-1.9.9/onnx2tf/ops/GatherElements.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GatherND.py` & `onnx2tf-1.9.9/onnx2tf/ops/GatherND.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Gemm.py` & `onnx2tf-1.9.9/onnx2tf/ops/Gemm.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GlobalAveragePool.py` & `onnx2tf-1.9.9/onnx2tf/ops/Range.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,104 @@
 import random
 random.seed(0)
 import numpy as np
 np.random.seed(0)
 import tensorflow as tf
 import onnx_graphsurgeon as gs
-from tensorflow.python.keras.layers import (
-    GlobalAveragePooling1D,
-    GlobalAveragePooling2D,
-    GlobalAveragePooling3D,
-)
 from onnx2tf.utils.common_functions import (
     get_constant_or_variable,
     print_node_info,
     inverted_operation_enable_disable,
     make_tf_node_info,
-    get_replacement_parameter,
-    pre_process_transpose,
-    post_process_transpose,
 )
+from onnx2tf.utils.enums import NUMPY_DTYPES_TO_TF_DTYPES
 
 
 @print_node_info
 @inverted_operation_enable_disable
-@get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """GlobalAveragePool
+    """Range
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
         optype, shape, dtype, tensorflow graph
     """
     before_op_output_shape_trans_1 = \
         tf_layers_dict.get(graph_node.inputs[0].name, {}).get('before_op_output_shape_trans', True)
+    before_op_output_shape_trans_2 = \
+        tf_layers_dict.get(graph_node.inputs[1].name, {}).get('before_op_output_shape_trans', True)
+    before_op_output_shape_trans_3 = \
+        tf_layers_dict.get(graph_node.inputs[2].name, {}).get('before_op_output_shape_trans', True)
     before_op_output_shape_trans = \
-        before_op_output_shape_trans_1
+        before_op_output_shape_trans_1 \
+        and before_op_output_shape_trans_2 \
+        and before_op_output_shape_trans_3
 
-    graph_node_input = get_constant_or_variable(
+    graph_node_input_1 = get_constant_or_variable(
         graph_node.inputs[0],
         before_op_output_shape_trans,
     )
-    graph_node_output: gs.Variable = graph_node.outputs[0]
-
-    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
-        if isinstance(graph_node_input, gs.Variable) else graph_node_input
-    input_tensor_rank = len(input_tensor.shape)
+    graph_node_input_2 = get_constant_or_variable(
+        graph_node.inputs[1],
+        before_op_output_shape_trans,
+    )
+    graph_node_input_3 = get_constant_or_variable(
+        graph_node.inputs[2],
+        before_op_output_shape_trans,
+    )
 
+    graph_node_output: gs.Variable = graph_node.outputs[0]
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
-    # Pre-process transpose
-    input_tensor = pre_process_transpose(
-        value_before_transpose=input_tensor,
-        param_target='inputs',
-        param_name=graph_node.inputs[0].name,
-        **kwargs,
-    )
-
     # Generation of TF OP
-    axis = [dim for dim in range(1, input_tensor_rank - 1)]
-    if len(axis) == 1:
-        tf_layers_dict[graph_node_output.name]['tf_node'] = \
-            GlobalAveragePooling1D(
-                keepdims=True,
-            )(input_tensor)
-    elif len(axis) == 2:
-        tf_layers_dict[graph_node_output.name]['tf_node'] = \
-            GlobalAveragePooling2D(
-                keepdims=True,
-            )(input_tensor)
-    elif len(axis) == 3:
-        tf_layers_dict[graph_node_output.name]['tf_node'] = \
-            GlobalAveragePooling3D(
-                keepdims=True,
-            )(input_tensor)
-    else:
-        tf_layers_dict[graph_node_output.name]['tf_node'] = \
-            tf.reduce_mean(
-                input_tensor=input_tensor,
-                axis=axis,
-                keepdims=True,
-                name=graph_node.name,
-            )
-
-    # Post-process transpose
-    tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
-        value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
-        param_target='outputs',
-        param_name=graph_node.outputs[0].name,
-        **kwargs,
-    )
+    input_tensor_1 = tf_layers_dict[graph_node_input_1.name]['tf_node'] \
+        if isinstance(graph_node_input_1, gs.Variable) else graph_node_input_1
+    input_tensor_2 = tf_layers_dict[graph_node_input_2.name]['tf_node'] \
+        if isinstance(graph_node_input_2, gs.Variable) else graph_node_input_2
+    input_tensor_3 = tf_layers_dict[graph_node_input_3.name]['tf_node'] \
+        if isinstance(graph_node_input_3, gs.Variable) else graph_node_input_3
+
+    output_dtype = NUMPY_DTYPES_TO_TF_DTYPES[dtype] \
+        if isinstance(dtype, np.dtype) else dtype
+
+    tf_layers_dict[graph_node_output.name]['tf_node'] = \
+        tf.range(
+            start=input_tensor_1,
+            limit=input_tensor_2,
+            delta=input_tensor_3,
+            dtype=output_dtype,
+            name=graph_node.name,
+        )
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': tf.reduce_mean,
+                'tf_op_type': tf.range,
                 'tf_inputs': {
-                    'input_tensor': input_tensor,
-                    'axis': axis,
-                    'keepdims': True,
+                    'start': input_tensor_1,
+                    'limit': input_tensor_2,
+                    'delta': input_tensor_3,
+                    'dtype': dtype,
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GlobalLpPool.py` & `onnx2tf-1.9.9/onnx2tf/ops/NonZero.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """GlobalLpPool
+    """NonZero
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
@@ -41,23 +41,20 @@
 
     graph_node_input = get_constant_or_variable(
         graph_node.inputs[0],
         before_op_output_shape_trans,
     )
     graph_node_output: gs.Variable = graph_node.outputs[0]
 
-    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
-        if isinstance(graph_node_input, gs.Variable) else graph_node_input
-    input_tensor_rank = len(input_tensor.shape)
-
-    p = graph_node.attrs.get('p', 2)
-
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
+    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
+        if isinstance(graph_node_input, gs.Variable) else graph_node_input
+
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
@@ -66,43 +63,39 @@
         value_before_transpose=input_tensor,
         param_target='inputs',
         param_name=graph_node.inputs[0].name,
         **kwargs,
     )
 
     # Generation of TF OP
-    dims = list(range(input_tensor_rank))
-    dim_window = dims[1:-1]
-    if len(dim_window) > 1 and p == 2:
-        p = "euclidean"
+    condition = tf.not_equal(
+        input_tensor,
+        tf.zeros_like(input_tensor),
+    )
+    nonzero_indices = tf.where(condition)
     tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.norm(
-            input_tensor,
-            ord=p,
-            axis=dim_window,
-            keepdims=True,
+        tf.transpose(
+            a=nonzero_indices,
+            name=graph_node.name,
         )
 
     # Post-process transpose
     tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
         value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
         param_target='outputs',
         param_name=graph_node.outputs[0].name,
         **kwargs,
     )
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': tf.norm,
+                'tf_op_type': 'NonZero',
                 'tf_inputs': {
-                    'tensor': input_tensor,
-                    'ord': p,
-                    'axis': dim_window,
-                    'keepdims': True,
+                    'input_tensor': input_tensor,
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GlobalMaxPool.py` & `onnx2tf-1.9.9/onnx2tf/ops/Size.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """GlobalMaxPool
+    """Size
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
@@ -40,44 +40,40 @@
         before_op_output_shape_trans_1
 
     graph_node_input = get_constant_or_variable(
         graph_node.inputs[0],
         before_op_output_shape_trans,
     )
     graph_node_output: gs.Variable = graph_node.outputs[0]
-
-    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
-        if isinstance(graph_node_input, gs.Variable) else graph_node_input
-    input_tensor_rank = len(input_tensor.shape)
-
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
+    # Generation of TF OP
+    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
+        if isinstance(graph_node_input, gs.Variable) else graph_node_input
+
     # Pre-process transpose
     input_tensor = pre_process_transpose(
         value_before_transpose=input_tensor,
         param_target='inputs',
         param_name=graph_node.inputs[0].name,
         **kwargs,
     )
 
-    # Generation of TF OP
-    axis = [dim for dim in range(1, input_tensor_rank - 1)]
     tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.reduce_max(
-            input_tensor=input_tensor,
-            axis=axis,
-            keepdims=True,
+        tf.size(
+            input=input_tensor,
+            out_type=tf.int64,
             name=graph_node.name,
         )
 
     # Post-process transpose
     tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
         value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
         param_target='outputs',
@@ -85,18 +81,16 @@
         **kwargs,
     )
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': tf.reduce_max,
+                'tf_op_type': tf.size,
                 'tf_inputs': {
-                    'input_tensor': input_tensor,
-                    'axis': axis,
-                    'keepdims': True,
+                    'input': input_tensor,
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Greater.py` & `onnx2tf-1.9.9/onnx2tf/ops/Greater.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GreaterOrEqual.py` & `onnx2tf-1.9.9/onnx2tf/ops/GreaterOrEqual.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/GridSample.py` & `onnx2tf-1.9.9/onnx2tf/ops/GridSample.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/HardSigmoid.py` & `onnx2tf-1.9.9/onnx2tf/ops/HardSigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/HardSwish.py` & `onnx2tf-1.9.9/onnx2tf/ops/HardSwish.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Hardmax.py` & `onnx2tf-1.9.9/onnx2tf/ops/Hardmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Identity.py` & `onnx2tf-1.9.9/onnx2tf/ops/Identity.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/If.py` & `onnx2tf-1.9.9/onnx2tf/ops/If.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Input.py` & `onnx2tf-1.9.9/onnx2tf/ops/Input.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/InstanceNormalization.py` & `onnx2tf-1.9.9/onnx2tf/ops/InstanceNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Inverse.py` & `onnx2tf-1.9.9/onnx2tf/ops/Inverse.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/IsInf.py` & `onnx2tf-1.9.9/onnx2tf/ops/IsInf.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/IsNaN.py` & `onnx2tf-1.9.9/onnx2tf/ops/IsNaN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/LRN.py` & `onnx2tf-1.9.9/onnx2tf/ops/LRN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/LSTM.py` & `onnx2tf-1.9.9/onnx2tf/ops/LSTM.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/LayerNormalization.py` & `onnx2tf-1.9.9/onnx2tf/ops/LayerNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/LeakyRelu.py` & `onnx2tf-1.9.9/onnx2tf/ops/LeakyRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Less.py` & `onnx2tf-1.9.9/onnx2tf/ops/Less.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/LessOrEqual.py` & `onnx2tf-1.9.9/onnx2tf/ops/LessOrEqual.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Log.py` & `onnx2tf-1.9.9/onnx2tf/ops/Log.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/LogSoftmax.py` & `onnx2tf-1.9.9/onnx2tf/ops/LogSoftmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/LpNormalization.py` & `onnx2tf-1.9.9/onnx2tf/ops/LpNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/MatMul.py` & `onnx2tf-1.9.9/onnx2tf/ops/MatMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/MatMulInteger.py` & `onnx2tf-1.9.9/onnx2tf/ops/MatMulInteger.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Max.py` & `onnx2tf-1.9.9/onnx2tf/ops/Max.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/MaxPool.py` & `onnx2tf-1.9.9/onnx2tf/ops/MaxPool.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,20 @@
     inverted_operation_enable_disable,
     make_tf_node_info,
     get_replacement_parameter,
     pre_process_transpose,
     post_process_transpose,
     calc_tf_pooling_pads,
     calc_extra_padding_with_ceil,
+    transpose_with_flexing_deterrence,
 )
 from onnx2tf.utils.colors import Color
 
+INF_INDEX_VALUE: int = 4294967296
+
 
 @print_node_info
 @inverted_operation_enable_disable
 @get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
@@ -51,23 +54,66 @@
     )
     graph_node_output: gs.Variable = graph_node.outputs[0]
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
         if isinstance(graph_node_input, gs.Variable) else graph_node_input
+    input_tensor_shape = input_tensor.shape
 
     # Pre-process transpose
     input_tensor = pre_process_transpose(
         value_before_transpose=input_tensor,
         param_target='inputs',
         param_name=graph_node.inputs[0].name,
         **kwargs,
     )
 
+    # Workaround to avoid as many conversion failures as possible
+    # for models with useless Transpose immediately before them.
+    # If the input geometry of the ONNX and the input geometry of the TF model match,
+    # the input geometry on the TF model side is forcibly transposed to the NWC or NHWC or NDHWC format.
+    # However, if all dimensions of CW or CHW or CDHW have the same value,
+    # the forced transposition process is skipped because it may destroy the structure of the model.
+    onnx_input_shape = [
+        dim if isinstance(dim, int) else None for dim in graph_node.inputs[0].shape
+    ] if graph_node.inputs[0].shape is not None else None
+    tf_input_shape = [
+        dim if isinstance(dim, int) else None for dim in input_tensor_shape
+    ]
+    if onnx_input_shape is not None \
+        and len(onnx_input_shape) > 1 and len(tf_input_shape) > 1 \
+        and onnx_input_shape == tf_input_shape:
+
+        shape_for_judging_skip = [
+            dim if dim is not None else INF_INDEX_VALUE for dim in onnx_input_shape[1:]
+        ]
+        if shape_for_judging_skip.count(shape_for_judging_skip[0]) != len(shape_for_judging_skip):
+            if len(onnx_input_shape) == 3:
+                # 1D - Overall model
+                input_tensor = transpose_with_flexing_deterrence(
+                    input_tensor=input_tensor,
+                    perm=[0,2,1],
+                    **kwargs,
+                )
+            elif len(onnx_input_shape) == 4:
+                # 2D - Overall model
+                input_tensor = transpose_with_flexing_deterrence(
+                    input_tensor=input_tensor,
+                    perm=[0,2,3,1],
+                    **kwargs,
+                )
+            elif len(onnx_input_shape) == 5:
+                # 3D - Overall model
+                input_tensor = transpose_with_flexing_deterrence(
+                    input_tensor=input_tensor,
+                    perm=[0,2,3,4,1],
+                    **kwargs,
+                )
+
     if len(graph_node.outputs) > 1:
         error_msg = \
             f'{Color.RED}ERROR:{Color.RESET} ' \
             f'MaxPoolWithArgmax is not yet implemented. ' \
             f'Pull requests are welcome. \n' \
             f'https://github.com/onnx/onnx-tensorflow/blob/f9ebc35dba8a9555112a8d0b84f5a3d51278cca9/onnx_tf/handlers/backend/dilated_pooling.py#L544 \n' \
             f'graph_node.name: {graph_node.name}'
@@ -122,19 +168,21 @@
             auto_pad = 'VALID'
             is_explicit_padding = True
 
             # extra padding may be needed for ceiling
             # this padding is added to end side (right, bottom) only
             if ceil_mode:
                 extra_pads = \
-                    calc_extra_padding_with_ceil(input_shape=input_tensor_shape[1:-1],
-                                                 kernel=kernel_shape,
-                                                 pads=pads,
-                                                 dilations=dilations,
-                                                 strides=strides)
+                    calc_extra_padding_with_ceil(
+                        input_shape=input_tensor_shape[1:-1],
+                        kernel=kernel_shape,
+                        pads=pads,
+                        dilations=dilations,
+                        strides=strides,
+                    )
                 pads = pads[:len(pads) // 2] + [p + e for p, e in zip(pads[len(pads) // 2:], extra_pads)]
 
             tf_pads = pads
 
     elif auto_pad == 'SAME_UPPER':
         tf_pad_mode = 'SAME'
 
@@ -179,14 +227,15 @@
         padded_tensor = input_tensor
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
+        'nhwc': True,
     }
 
     # Generation of TF OP
     tf_op_type = None
 
     # tf.nn.dilation2d
     if spatial_size == 2 and dilations != [1] * spatial_size:
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/MaxUnpool.py` & `onnx2tf-1.9.9/onnx2tf/ops/MaxUnpool.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Mean.py` & `onnx2tf-1.9.9/onnx2tf/ops/Mean.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/MeanVarianceNormalization.py` & `onnx2tf-1.9.9/onnx2tf/ops/MeanVarianceNormalization.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Min.py` & `onnx2tf-1.9.9/onnx2tf/ops/Min.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Mish.py` & `onnx2tf-1.9.9/onnx2tf/ops/Mish.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Mod.py` & `onnx2tf-1.9.9/onnx2tf/ops/Mod.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Mul.py` & `onnx2tf-1.9.9/onnx2tf/ops/Mul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Multinomial.py` & `onnx2tf-1.9.9/onnx2tf/ops/Multinomial.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Neg.py` & `onnx2tf-1.9.9/onnx2tf/ops/Neg.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/NonMaxSuppression.py` & `onnx2tf-1.9.9/onnx2tf/ops/NonMaxSuppression.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/NonZero.py` & `onnx2tf-1.9.9/onnx2tf/ops/SpaceToDepth.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,40 +20,41 @@
 @get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """NonZero
+    """SpaceToDepth
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
         optype, shape, dtype, tensorflow graph
     """
     before_op_output_shape_trans_1 = \
         tf_layers_dict.get(graph_node.inputs[0].name, {}).get('before_op_output_shape_trans', True)
     before_op_output_shape_trans = \
         before_op_output_shape_trans_1
 
-    graph_node_input = get_constant_or_variable(
+    graph_node_input_1 = get_constant_or_variable(
         graph_node.inputs[0],
         before_op_output_shape_trans,
     )
     graph_node_output: gs.Variable = graph_node.outputs[0]
-
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
-    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
-        if isinstance(graph_node_input, gs.Variable) else graph_node_input
+    input_tensor = tf_layers_dict[graph_node_input_1.name]['tf_node'] \
+        if isinstance(graph_node_input_1, gs.Variable) else graph_node_input_1
+
+    blocksize = graph_node.attrs.get('blocksize', 1)
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
@@ -63,22 +64,18 @@
         value_before_transpose=input_tensor,
         param_target='inputs',
         param_name=graph_node.inputs[0].name,
         **kwargs,
     )
 
     # Generation of TF OP
-    condition = tf.not_equal(
-        input_tensor,
-        tf.zeros_like(input_tensor),
-    )
-    nonzero_indices = tf.where(condition)
     tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.transpose(
-            a=nonzero_indices,
+        tf.nn.space_to_depth(
+            input=input_tensor,
+            block_size=blocksize,
             name=graph_node.name,
         )
 
     # Post-process transpose
     tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
         value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
         param_target='outputs',
@@ -86,16 +83,17 @@
         **kwargs,
     )
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': 'NonZero',
+                'tf_op_type': tf.nn.space_to_depth,
                 'tf_inputs': {
-                    'input_tensor': input_tensor,
+                    'input': input_tensor,
+                    'block_size': blocksize,
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Not.py` & `onnx2tf-1.9.9/onnx2tf/ops/Not.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/OneHot.py` & `onnx2tf-1.9.9/onnx2tf/ops/OneHot.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Or.py` & `onnx2tf-1.9.9/onnx2tf/ops/Or.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/PRelu.py` & `onnx2tf-1.9.9/onnx2tf/ops/PRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Pad.py` & `onnx2tf-1.9.9/onnx2tf/ops/Pad.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Pow.py` & `onnx2tf-1.9.9/onnx2tf/ops/Pow.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearAdd.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearAdd.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearConcat.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearConcat.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearConv.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearConv.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearLeakyRelu.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearLeakyRelu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearMatMul.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearMatMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearMul.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearMul.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearSigmoid.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearSigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QLinearSoftmax.py` & `onnx2tf-1.9.9/onnx2tf/ops/QLinearSoftmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/QuantizeLinear.py` & `onnx2tf-1.9.9/onnx2tf/ops/QuantizeLinear.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/RNN.py` & `onnx2tf-1.9.9/onnx2tf/ops/RNN.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/RandomNormal.py` & `onnx2tf-1.9.9/onnx2tf/ops/RandomNormal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/RandomNormalLike.py` & `onnx2tf-1.9.9/onnx2tf/ops/RandomNormalLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/RandomUniform.py` & `onnx2tf-1.9.9/onnx2tf/ops/RandomUniform.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/RandomUniformLike.py` & `onnx2tf-1.9.9/onnx2tf/ops/RandomUniformLike.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Range.py` & `onnx2tf-1.9.9/onnx2tf/ops/SequenceConstruct.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,88 +17,70 @@
 @inverted_operation_enable_disable
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """Range
+    """SequenceConstruct
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
         optype, shape, dtype, tensorflow graph
     """
     before_op_output_shape_trans_1 = \
         tf_layers_dict.get(graph_node.inputs[0].name, {}).get('before_op_output_shape_trans', True)
-    before_op_output_shape_trans_2 = \
-        tf_layers_dict.get(graph_node.inputs[1].name, {}).get('before_op_output_shape_trans', True)
-    before_op_output_shape_trans_3 = \
-        tf_layers_dict.get(graph_node.inputs[2].name, {}).get('before_op_output_shape_trans', True)
     before_op_output_shape_trans = \
-        before_op_output_shape_trans_1 \
-        and before_op_output_shape_trans_2 \
-        and before_op_output_shape_trans_3
-
-    graph_node_input_1 = get_constant_or_variable(
-        graph_node.inputs[0],
-        before_op_output_shape_trans,
-    )
-    graph_node_input_2 = get_constant_or_variable(
-        graph_node.inputs[1],
-        before_op_output_shape_trans,
-    )
-    graph_node_input_3 = get_constant_or_variable(
-        graph_node.inputs[2],
-        before_op_output_shape_trans,
+        before_op_output_shape_trans_1
+
+    input_sequence = tf.ragged.constant(
+        [],
+        dtype=NUMPY_DTYPES_TO_TF_DTYPES[graph_node.inputs[0].dtype] \
+            if isinstance(graph_node.inputs[0].dtype, np.dtype) else graph_node.inputs[0].dtype
     )
 
     graph_node_output: gs.Variable = graph_node.outputs[0]
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
     # Generation of TF OP
-    input_tensor_1 = tf_layers_dict[graph_node_input_1.name]['tf_node'] \
-        if isinstance(graph_node_input_1, gs.Variable) else graph_node_input_1
-    input_tensor_2 = tf_layers_dict[graph_node_input_2.name]['tf_node'] \
-        if isinstance(graph_node_input_2, gs.Variable) else graph_node_input_2
-    input_tensor_3 = tf_layers_dict[graph_node_input_3.name]['tf_node'] \
-        if isinstance(graph_node_input_3, gs.Variable) else graph_node_input_3
-
-    output_dtype = NUMPY_DTYPES_TO_TF_DTYPES[dtype] \
-        if isinstance(dtype, np.dtype) else dtype
-
-    tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.range(
-            start=input_tensor_1,
-            limit=input_tensor_2,
-            delta=input_tensor_3,
-            dtype=output_dtype,
-            name=graph_node.name,
+    output_seq = None
+    for input in graph_node.inputs:
+        graph_node_input = get_constant_or_variable(
+            input,
+            before_op_output_shape_trans,
         )
+        input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
+            if isinstance(graph_node_input, gs.Variable) else graph_node_input
+        expanded_input_tensor = tf.expand_dims(input_tensor, 0)
+        if input_sequence.shape[0] == 0:
+            output_seq = tf.RaggedTensor.from_tensor(expanded_input_tensor)
+        else:
+            output_seq = tf.concat([input_sequence, expanded_input_tensor], axis=0)
+        input_sequence = output_seq
+
+    tf_layers_dict[graph_node_output.name]['tf_node'] = output_seq
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': tf.range,
+                'tf_op_type': 'SequenceConstruct',
                 'tf_inputs': {
-                    'start': input_tensor_1,
-                    'limit': input_tensor_2,
-                    'delta': input_tensor_3,
-                    'dtype': dtype,
+                    'graph_node.inputs[0]': graph_node.inputs[0],
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Reciprocal.py` & `onnx2tf-1.9.9/onnx2tf/ops/Reciprocal.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceL1.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceL1.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceL2.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceL2.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceLogSum.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceLogSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceLogSumExp.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceLogSumExp.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceMax.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceMax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceMean.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceMean.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceMin.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceMin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceProd.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceProd.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceSum.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceSum.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReduceSumSquare.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReduceSumSquare.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Relu.py` & `onnx2tf-1.9.9/onnx2tf/ops/Relu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Reshape.py` & `onnx2tf-1.9.9/onnx2tf/ops/Reshape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Resize.py` & `onnx2tf-1.9.9/onnx2tf/ops/Resize.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ReverseSequence.py` & `onnx2tf-1.9.9/onnx2tf/ops/ReverseSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/RoiAlign.py` & `onnx2tf-1.9.9/onnx2tf/ops/RoiAlign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Round.py` & `onnx2tf-1.9.9/onnx2tf/ops/Round.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ScaleAndTranslate.py` & `onnx2tf-1.9.9/onnx2tf/ops/ScaleAndTranslate.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Scatter.py` & `onnx2tf-1.9.9/onnx2tf/ops/Scatter.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ScatterElements.py` & `onnx2tf-1.9.9/onnx2tf/ops/ScatterElements.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/ScatterND.py` & `onnx2tf-1.9.9/onnx2tf/ops/ScatterND.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Selu.py` & `onnx2tf-1.9.9/onnx2tf/ops/Selu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SequenceAt.py` & `onnx2tf-1.9.9/onnx2tf/ops/SequenceAt.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SequenceConstruct.py` & `onnx2tf-1.9.9/onnx2tf/ops/SequenceEmpty.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,65 @@
 import random
 random.seed(0)
 import numpy as np
 np.random.seed(0)
 import tensorflow as tf
 import onnx_graphsurgeon as gs
 from onnx2tf.utils.common_functions import (
-    get_constant_or_variable,
     print_node_info,
     inverted_operation_enable_disable,
     make_tf_node_info,
 )
-from onnx2tf.utils.enums import NUMPY_DTYPES_TO_TF_DTYPES
+from onnx2tf.utils.enums import ONNX_DTYPES_TO_TF_DTYPES
 
 
 @print_node_info
 @inverted_operation_enable_disable
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """SequenceConstruct
+    """SequenceEmpty
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
         optype, shape, dtype, tensorflow graph
     """
-    before_op_output_shape_trans_1 = \
-        tf_layers_dict.get(graph_node.inputs[0].name, {}).get('before_op_output_shape_trans', True)
-    before_op_output_shape_trans = \
-        before_op_output_shape_trans_1
-
-    input_sequence = tf.ragged.constant(
-        [],
-        dtype=NUMPY_DTYPES_TO_TF_DTYPES[graph_node.inputs[0].dtype] \
-            if isinstance(graph_node.inputs[0].dtype, np.dtype) else graph_node.inputs[0].dtype
-    )
+    sequence_dtype = ONNX_DTYPES_TO_TF_DTYPES(graph_node.attrs.get('dtype', 1)) # Float32
 
     graph_node_output: gs.Variable = graph_node.outputs[0]
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
     # Generation of TF OP
-    output_seq = None
-    for input in graph_node.inputs:
-        graph_node_input = get_constant_or_variable(
-            input,
-            before_op_output_shape_trans,
-        )
-        input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
-            if isinstance(graph_node_input, gs.Variable) else graph_node_input
-        expanded_input_tensor = tf.expand_dims(input_tensor, 0)
-        if input_sequence.shape[0] == 0:
-            output_seq = tf.RaggedTensor.from_tensor(expanded_input_tensor)
-        else:
-            output_seq = tf.concat([input_sequence, expanded_input_tensor], axis=0)
-        input_sequence = output_seq
+    ragged = tf.RaggedTensor.from_row_lengths(values=[], row_lengths=[])
+    sparse = tf.cast(ragged.to_sparse(), sequence_dtype)
 
-    tf_layers_dict[graph_node_output.name]['tf_node'] = output_seq
+    tf_layers_dict[graph_node_output.name]['tf_node'] = \
+        tf.RaggedTensor.from_sparse(sparse)
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': 'SequenceConstruct',
+                'tf_op_type': 'SequenceEmpty',
                 'tf_inputs': {
-                    'graph_node.inputs[0]': graph_node.inputs[0],
+                    'dtype': sequence_dtype,
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SequenceEmpty.py` & `onnx2tf-1.9.9/onnx2tf/ops/Sum.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,104 @@
 import random
 random.seed(0)
 import numpy as np
 np.random.seed(0)
 import tensorflow as tf
 import onnx_graphsurgeon as gs
 from onnx2tf.utils.common_functions import (
+    get_constant_or_variable,
     print_node_info,
     inverted_operation_enable_disable,
     make_tf_node_info,
+    get_replacement_parameter,
+    pre_process_transpose,
+    post_process_transpose,
 )
-from onnx2tf.utils.enums import ONNX_DTYPES_TO_TF_DTYPES
 
 
 @print_node_info
 @inverted_operation_enable_disable
+@get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """SequenceEmpty
+    """Sum
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
         optype, shape, dtype, tensorflow graph
     """
-    sequence_dtype = ONNX_DTYPES_TO_TF_DTYPES(graph_node.attrs.get('dtype', 1)) # Float32
+    before_op_output_shape_trans = True
+    for graph_node_input in graph_node.inputs:
+        before_op_output_shape_trans_n = \
+            tf_layers_dict.get(graph_node_input.name, {}).get('before_op_output_shape_trans', True)
+        before_op_output_shape_trans = \
+            before_op_output_shape_trans and before_op_output_shape_trans_n
+
+    values = []
+    for graph_node_input in graph_node.inputs:
+        const_or_var = get_constant_or_variable(
+            graph_node_input,
+            before_op_output_shape_trans,
+        )
+        # Pre-process transpose
+        const_or_var = pre_process_transpose(
+            value_before_transpose=const_or_var,
+            param_target='inputs',
+            param_name=graph_node_input.name,
+            **kwargs,
+        )
+        if isinstance(const_or_var, gs.Variable):
+            values.append(tf_layers_dict[const_or_var.name]['tf_node'])
+        else:
+            values.append(
+                const_or_var \
+                    if not isinstance(const_or_var, np.ndarray) \
+                        else tf.convert_to_tensor(const_or_var)
+            )
 
     graph_node_output: gs.Variable = graph_node.outputs[0]
+
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
     # Generation of TF OP
-    ragged = tf.RaggedTensor.from_row_lengths(values=[], row_lengths=[])
-    sparse = tf.cast(ragged.to_sparse(), sequence_dtype)
-
     tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.RaggedTensor.from_sparse(sparse)
+        tf.add_n(
+            inputs=values,
+            name=graph_node.name,
+        )
+
+    # Post-process transpose
+    tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
+        value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
+        param_target='outputs',
+        param_name=graph_node.outputs[0].name,
+        **kwargs,
+    )
 
     # Generation of Debug Info
+    tf_inputs = {f"input{idx}": value for idx, value in enumerate(values)}
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': 'SequenceEmpty',
-                'tf_inputs': {
-                    'dtype': sequence_dtype,
-                },
+                'tf_op_type': tf.concat,
+                'tf_inputs': tf_inputs,
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SequenceErase.py` & `onnx2tf-1.9.9/onnx2tf/ops/SequenceErase.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SequenceInsert.py` & `onnx2tf-1.9.9/onnx2tf/ops/SequenceInsert.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SequenceLength.py` & `onnx2tf-1.9.9/onnx2tf/ops/SequenceLength.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Shape.py` & `onnx2tf-1.9.9/onnx2tf/ops/Shape.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Shrink.py` & `onnx2tf-1.9.9/onnx2tf/ops/Shrink.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Sigmoid.py` & `onnx2tf-1.9.9/onnx2tf/ops/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Sign.py` & `onnx2tf-1.9.9/onnx2tf/ops/Sign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Sin.py` & `onnx2tf-1.9.9/onnx2tf/ops/Sin.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Sinh.py` & `onnx2tf-1.9.9/onnx2tf/ops/Sinh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Size.py` & `onnx2tf-1.9.9/onnx2tf/ops/ThresholdedRelu.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """Size
+    """ThresholdedRelu
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
@@ -39,58 +39,76 @@
     before_op_output_shape_trans = \
         before_op_output_shape_trans_1
 
     graph_node_input = get_constant_or_variable(
         graph_node.inputs[0],
         before_op_output_shape_trans,
     )
+    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
+        if isinstance(graph_node_input, gs.Variable) else graph_node_input
+
     graph_node_output: gs.Variable = graph_node.outputs[0]
+
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
+    alpha = graph_node.attrs.get('alpha', 1.0)
+    epsilon = 1e-5
+
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
+        'nhwc': tf_layers_dict[graph_node_input.name]['nhwc'] \
+            if isinstance(graph_node_input, gs.Variable) \
+                and 'nhwc' in tf_layers_dict[graph_node_input.name].keys() else False
     }
 
-    # Generation of TF OP
-    input_tensor = tf_layers_dict[graph_node_input.name]['tf_node'] \
-        if isinstance(graph_node_input, gs.Variable) else graph_node_input
-
     # Pre-process transpose
+    before_trans_shape = input_tensor.shape
     input_tensor = pre_process_transpose(
         value_before_transpose=input_tensor,
         param_target='inputs',
         param_name=graph_node.inputs[0].name,
         **kwargs,
     )
+    after_trans_shape = input_tensor.shape
+    if 'nhwc' in tf_layers_dict[graph_node_output.name].keys() \
+        and tf_layers_dict[graph_node_output.name]['nhwc'] == True \
+        and before_trans_shape != after_trans_shape:
+        tf_layers_dict[graph_node_output.name].pop('nhwc')
 
+    # Generation of TF OP
     tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.size(
-            input=input_tensor,
-            out_type=tf.int64,
-            name=graph_node.name,
-        )
+        tf.nn.relu(input_tensor) - \
+            tf.nn.relu(tf.sign((alpha + epsilon) - input_tensor) * input_tensor)
 
     # Post-process transpose
+    before_trans_shape = tf_layers_dict[graph_node_output.name]['tf_node'].shape
     tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
         value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
         param_target='outputs',
         param_name=graph_node.outputs[0].name,
         **kwargs,
     )
+    after_trans_shape = tf_layers_dict[graph_node_output.name]['tf_node'].shape
+    if 'nhwc' in tf_layers_dict[graph_node_output.name].keys() \
+        and tf_layers_dict[graph_node_output.name]['nhwc'] == True \
+        and before_trans_shape != after_trans_shape:
+        tf_layers_dict[graph_node_output.name].pop('nhwc')
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': tf.size,
+                'tf_op_type': 'ThresholdedRelu',
                 'tf_inputs': {
-                    'input': input_tensor,
+                    'x': input_tensor,
+                    'alpha': alpha,
+                    'epsilon': epsilon,
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Slice.py` & `onnx2tf-1.9.9/onnx2tf/ops/Slice.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Softmax.py` & `onnx2tf-1.9.9/onnx2tf/ops/Softmax.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Softplus.py` & `onnx2tf-1.9.9/onnx2tf/ops/Softplus.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Softsign.py` & `onnx2tf-1.9.9/onnx2tf/ops/Softsign.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SpaceToDepth.py` & `onnx2tf-1.9.9/onnx2tf/ops/Where.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,62 +20,91 @@
 @get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """SpaceToDepth
+    """Where
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
         optype, shape, dtype, tensorflow graph
     """
     before_op_output_shape_trans_1 = \
         tf_layers_dict.get(graph_node.inputs[0].name, {}).get('before_op_output_shape_trans', True)
+    before_op_output_shape_trans_2 = \
+        tf_layers_dict.get(graph_node.inputs[1].name, {}).get('before_op_output_shape_trans', True)
+    before_op_output_shape_trans_3 = \
+        tf_layers_dict.get(graph_node.inputs[2].name, {}).get('before_op_output_shape_trans', True)
     before_op_output_shape_trans = \
-        before_op_output_shape_trans_1
+        before_op_output_shape_trans_1 \
+        and before_op_output_shape_trans_2 \
+        and before_op_output_shape_trans_3
 
     graph_node_input_1 = get_constant_or_variable(
         graph_node.inputs[0],
         before_op_output_shape_trans,
     )
+    graph_node_input_2 = get_constant_or_variable(
+        graph_node.inputs[1],
+        before_op_output_shape_trans,
+    )
+    graph_node_input_3 = get_constant_or_variable(
+        graph_node.inputs[2],
+        before_op_output_shape_trans,
+    )
+    condition = tf_layers_dict[graph_node_input_1.name]['tf_node'] \
+        if isinstance(graph_node_input_1, gs.Variable) else graph_node_input_1
+    X = tf_layers_dict[graph_node_input_2.name]['tf_node'] \
+        if isinstance(graph_node_input_2, gs.Variable) else graph_node_input_2
+    Y = tf_layers_dict[graph_node_input_3.name]['tf_node'] \
+        if isinstance(graph_node_input_3, gs.Variable) else graph_node_input_3
+
     graph_node_output: gs.Variable = graph_node.outputs[0]
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
-    input_tensor = tf_layers_dict[graph_node_input_1.name]['tf_node'] \
-        if isinstance(graph_node_input_1, gs.Variable) else graph_node_input_1
-
-    blocksize = graph_node.attrs.get('blocksize', 1)
-
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
     # Pre-process transpose
-    input_tensor = pre_process_transpose(
-        value_before_transpose=input_tensor,
+    condition = pre_process_transpose(
+        value_before_transpose=condition,
         param_target='inputs',
         param_name=graph_node.inputs[0].name,
         **kwargs,
     )
+    X = pre_process_transpose(
+        value_before_transpose=X,
+        param_target='inputs',
+        param_name=graph_node.inputs[1].name,
+        **kwargs,
+    )
+    Y = pre_process_transpose(
+        value_before_transpose=Y,
+        param_target='inputs',
+        param_name=graph_node.inputs[2].name,
+        **kwargs,
+    )
 
     # Generation of TF OP
     tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.nn.space_to_depth(
-            input=input_tensor,
-            block_size=blocksize,
+        tf.where(
+            condition=condition,
+            x=X,
+            y=Y,
             name=graph_node.name,
         )
 
     # Post-process transpose
     tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
         value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
         param_target='outputs',
@@ -83,17 +112,18 @@
         **kwargs,
     )
 
     # Generation of Debug Info
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': tf.nn.space_to_depth,
+                'tf_op_type': tf.where,
                 'tf_inputs': {
-                    'input': input_tensor,
-                    'block_size': blocksize,
+                    'condition': condition,
+                    'x': X,
+                    'y': Y,
                 },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Split.py` & `onnx2tf-1.9.9/onnx2tf/ops/Split.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/SplitToSequence.py` & `onnx2tf-1.9.9/onnx2tf/ops/SplitToSequence.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Sqrt.py` & `onnx2tf-1.9.9/onnx2tf/ops/Sqrt.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Squeeze.py` & `onnx2tf-1.9.9/onnx2tf/ops/Squeeze.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Sub.py` & `onnx2tf-1.9.9/onnx2tf/ops/Sub.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Sum.py` & `onnx2tf-1.9.9/onnx2tf/ops/Xor.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import tensorflow as tf
 import onnx_graphsurgeon as gs
 from onnx2tf.utils.common_functions import (
     get_constant_or_variable,
     print_node_info,
     inverted_operation_enable_disable,
     make_tf_node_info,
+    shape_unmatched_special_avoidance_workaround,
     get_replacement_parameter,
     pre_process_transpose,
     post_process_transpose,
 )
 
 
 @print_node_info
@@ -20,85 +21,107 @@
 @get_replacement_parameter
 def make_node(
     *,
     graph_node: gs.Node,
     tf_layers_dict: dict,
     **kwargs: dict,
 ):
-    """Sum
+    """Xor
 
     Parameters
     ----------
     graph_node: gs.Node
         graph_surgeon Node
 
     tf_layers_dict: dict
         optype, shape, dtype, tensorflow graph
     """
-    before_op_output_shape_trans = True
-    for graph_node_input in graph_node.inputs:
-        before_op_output_shape_trans_n = \
-            tf_layers_dict.get(graph_node_input.name, {}).get('before_op_output_shape_trans', True)
-        before_op_output_shape_trans = \
-            before_op_output_shape_trans and before_op_output_shape_trans_n
-
-    values = []
-    for graph_node_input in graph_node.inputs:
-        const_or_var = get_constant_or_variable(
-            graph_node_input,
-            before_op_output_shape_trans,
-        )
-        # Pre-process transpose
-        const_or_var = pre_process_transpose(
-            value_before_transpose=const_or_var,
-            param_target='inputs',
-            param_name=graph_node_input.name,
-            **kwargs,
-        )
-        if isinstance(const_or_var, gs.Variable):
-            values.append(tf_layers_dict[const_or_var.name]['tf_node'])
-        else:
-            values.append(
-                const_or_var \
-                    if not isinstance(const_or_var, np.ndarray) \
-                        else tf.convert_to_tensor(const_or_var)
-            )
-
+    before_op_output_shape_trans_1 = \
+        tf_layers_dict.get(graph_node.inputs[0].name, {}).get('before_op_output_shape_trans', True)
+    before_op_output_shape_trans_2 = \
+        tf_layers_dict.get(graph_node.inputs[1].name, {}).get('before_op_output_shape_trans', True)
+    before_op_output_shape_trans = \
+        before_op_output_shape_trans_1 \
+        and before_op_output_shape_trans_2
+
+    graph_node_input_1 = get_constant_or_variable(
+        graph_node.inputs[0],
+        before_op_output_shape_trans,
+    )
+    graph_node_input_2 = get_constant_or_variable(
+        graph_node.inputs[1],
+        before_op_output_shape_trans,
+    )
     graph_node_output: gs.Variable = graph_node.outputs[0]
 
     shape = graph_node_output.shape
     dtype = graph_node_output.dtype
 
     # Preserving Graph Structure (Dict)
     tf_layers_dict[graph_node_output.name] = {
         'optype': graph_node.op,
         'shape': shape,
         'dtype': dtype,
     }
 
     # Generation of TF OP
+    input_tensor_1 = tf_layers_dict[graph_node_input_1.name]['tf_node'] \
+        if isinstance(graph_node_input_1, gs.Variable) else graph_node_input_1
+    input_tensor_2 = tf_layers_dict[graph_node_input_2.name]['tf_node'] \
+        if isinstance(graph_node_input_2, gs.Variable) else graph_node_input_2
+
+    # Shape Unmatched Special Avoidance Workaround
+    # At least one True value for same_input_shape_as_onnx
+    # At least one True value in nhwc_flags
+    # same_input_shape_as_onnx == True and nhwc_flags == False and 3D or 4D or 5D tensor is NHWC transposed
+    input_tensor_1, input_tensor_2 = shape_unmatched_special_avoidance_workaround(
+        graph_node_input_1=graph_node_input_1,
+        graph_node_input_2=graph_node_input_2,
+        input_tensor_1=input_tensor_1,
+        input_tensor_2=input_tensor_2,
+        tf_layers_dict=tf_layers_dict,
+        **kwargs,
+    )
+
+    # Pre-process transpose
+    input_tensor_1 = pre_process_transpose(
+        value_before_transpose=input_tensor_1,
+        param_target='inputs',
+        param_name=graph_node.inputs[0].name,
+        **kwargs,
+    )
+    input_tensor_2 = pre_process_transpose(
+        value_before_transpose=input_tensor_2,
+        param_target='inputs',
+        param_name=graph_node.inputs[1].name,
+        **kwargs,
+    )
+
     tf_layers_dict[graph_node_output.name]['tf_node'] = \
-        tf.add_n(
-            inputs=values,
+        tf.math.logical_xor(
+            x=input_tensor_1,
+            y=input_tensor_2,
             name=graph_node.name,
         )
 
     # Post-process transpose
     tf_layers_dict[graph_node_output.name]['tf_node'] = post_process_transpose(
         value_before_transpose=tf_layers_dict[graph_node_output.name]['tf_node'],
         param_target='outputs',
         param_name=graph_node.outputs[0].name,
         **kwargs,
     )
 
     # Generation of Debug Info
-    tf_inputs = {f"input{idx}": value for idx, value in enumerate(values)}
     tf_layers_dict[graph_node_output.name]['tf_node_info'] = \
         make_tf_node_info(
             node_info={
-                'tf_op_type': tf.concat,
-                'tf_inputs': tf_inputs,
+                'tf_op_type': tf.math.logical_xor,
+                'tf_inputs': {
+                    'x': input_tensor_1,
+                    'y': input_tensor_2,
+                },
                 'tf_outputs': {
                     'output': tf_layers_dict[graph_node_output.name]['tf_node'],
                 },
             }
         )
```

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Tan.py` & `onnx2tf-1.9.9/onnx2tf/ops/Tan.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Tanh.py` & `onnx2tf-1.9.9/onnx2tf/ops/Tanh.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Tile.py` & `onnx2tf-1.9.9/onnx2tf/ops/Tile.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/TopK.py` & `onnx2tf-1.9.9/onnx2tf/ops/TopK.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Transpose.py` & `onnx2tf-1.9.9/onnx2tf/ops/Transpose.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Trilu.py` & `onnx2tf-1.9.9/onnx2tf/ops/Trilu.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Unique.py` & `onnx2tf-1.9.9/onnx2tf/ops/Unique.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Unsqueeze.py` & `onnx2tf-1.9.9/onnx2tf/ops/Unsqueeze.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/Upsample.py` & `onnx2tf-1.9.9/onnx2tf/ops/Upsample.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/ops/_Loop.py` & `onnx2tf-1.9.9/onnx2tf/ops/_Loop.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/utils/colors.py` & `onnx2tf-1.9.9/onnx2tf/utils/colors.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/utils/common_functions.py` & `onnx2tf-1.9.9/onnx2tf/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf/utils/enums.py` & `onnx2tf-1.9.9/onnx2tf/utils/enums.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/onnx2tf.egg-info/PKG-INFO` & `onnx2tf-1.9.9/onnx2tf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2tf
-Version: 1.9.8
+Version: 1.9.9
 Summary: Self-Created Tools to convert ONNX files (NCHW) to TensorFlow/TFLite/Keras format (NHWC). The purpose of this tool is to solve the massive Transpose extrapolation problem in onnx-tensorflow (onnx-tf).
 Home-page: https://github.com/PINTO0309/onnx2tf
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -225,15 +225,15 @@
 
 ## Demo
 Video speed is adjusted approximately 50 times slower than actual speed.
 ![render1665941718294](https://user-images.githubusercontent.com/33194443/196049928-57520fc2-842d-459c-9f28-7ee5f040c226.gif)
 
 ## Environment
 - onnx
-- onnxruntime
+- onnxruntime==1.13.1 See: [When using onnxruntime v1.14.1, all output values of Sigmoid are Nan. #14885](https://github.com/microsoft/onnxruntime/issues/14885)
 - onnx-simplifier==0.4.17 See: https://github.com/PINTO0309/onnx2tf/issues/312
 - onnx_graphsurgeon
 - simple_onnx_processing_tools
 - tensorflow==2.12.0
 - flatbuffers-compiler (Optional, Only when using the `-coion` option. Executable file named `flatc`.)
   ```bash
   # Custom flatc binary for Ubuntu 20.04+
@@ -252,15 +252,15 @@
 ## Sample Usage
 ### 1. Install
 - HostPC
   ```
   $ docker run --rm -it \
   -v `pwd`:/workdir \
   -w /workdir \
-  ghcr.io/pinto0309/onnx2tf:1.9.8
+  ghcr.io/pinto0309/onnx2tf:1.9.9
 
   or
 
   $ pip install -U onnx \
   && pip install -U nvidia-pyindex \
   && pip install -U onnx-graphsurgeon \
   && pip install -U onnxruntime==1.13.1 \
@@ -531,14 +531,15 @@
     ```
 
 - Other recommended replacement OP
 
     |Before|After|
     |:-:|:-:|
     |`HardSwish`<br>![image](https://user-images.githubusercontent.com/33194443/226223099-c7344bcf-d24d-4b35-a1d6-2a03dbfce8c7.png)|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
+    |`ReLU6`<br>![image](https://user-images.githubusercontent.com/33194443/233639086-721e5e80-08c3-4785-9c1a-002bbfc0fa3d.png)<br>Paper: [A Quantization-Friendly Separable Convolution for MobileNets](https://arxiv.org/pdf/1803.08607.pdf) https://arxiv.org/pdf/1803.08607.pdf|`ReLU`<br>![image](https://user-images.githubusercontent.com/33194443/226223213-bd714994-f353-416e-9f54-6d0954a70bb8.png)|
 
 
 ### 7. Calibration data creation for INT8 quantization
 Calibration data (.npy) for INT8 quantization (`-cind`) is generated as follows. This is a sample when the data used for training is image data. See: https://github.com/PINTO0309/onnx2tf/issues/222
 
 https://www.tensorflow.org/lite/performance/post_training_quantization
```

### Comparing `onnx2tf-1.9.8/onnx2tf.egg-info/SOURCES.txt` & `onnx2tf-1.9.9/onnx2tf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/setup.py` & `onnx2tf-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `onnx2tf-1.9.8/tests/test_model_convert.py` & `onnx2tf-1.9.9/tests/test_model_convert.py`

 * *Files identical despite different names*

