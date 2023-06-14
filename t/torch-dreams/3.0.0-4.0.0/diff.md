# Comparing `tmp/torch-dreams-3.0.0.tar.gz` & `tmp/torch-dreams-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torch-dreams-3.0.0.tar", last modified: Sat Nov  5 19:48:40 2022, max compression
+gzip compressed data, was "torch-dreams-4.0.0.tar", last modified: Wed Jun 14 08:22:41 2023, max compression
```

## Comparing `torch-dreams-3.0.0.tar` & `torch-dreams-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 mayukh    (1000) mayukh    (1000)        0 2022-11-05 19:48:40.508269 torch-dreams-3.0.0/
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     1064 2021-11-12 09:53:31.000000 torch-dreams-3.0.0/LICENSE
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)    18737 2022-11-05 19:48:40.508066 torch-dreams-3.0.0/PKG-INFO
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)    14176 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/README.md
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)       38 2022-11-05 19:48:40.508348 torch-dreams-3.0.0/setup.cfg
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     1420 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/setup.py
-drwxrwxrwx   0 mayukh    (1000) mayukh    (1000)        0 2022-11-05 19:48:40.504169 torch-dreams-3.0.0/torch_dreams/
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)      394 2022-11-05 19:24:16.000000 torch-dreams-3.0.0/torch_dreams/__init__.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     4324 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/auto_image_param.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     2476 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/batched_image_param.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     1147 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/batched_objective.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)      692 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/constants.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     3556 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/custom_image_param.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)    15650 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/dreamer.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)      738 2022-11-03 18:53:29.000000 torch-dreams-3.0.0/torch_dreams/dreamer_utils.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)      510 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/error_handlers.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     1672 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/image_transforms.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     1708 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/losses.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     3390 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/masked_image_param.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)      572 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/model_bunch.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     1629 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/noisegrad.py
-drwxrwxrwx   0 mayukh    (1000) mayukh    (1000)        0 2022-11-05 19:48:40.507558 torch-dreams-3.0.0/torch_dreams/tests/
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)       23 2021-11-12 09:53:31.000000 torch-dreams-3.0.0/torch_dreams/tests/__init__.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)    10327 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/tests/test.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     2886 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/tests/test_batched.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     2522 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/transforms.py
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)     4700 2022-11-05 19:23:58.000000 torch-dreams-3.0.0/torch_dreams/utils.py
-drwxrwxrwx   0 mayukh    (1000) mayukh    (1000)        0 2022-11-05 19:48:40.506242 torch-dreams-3.0.0/torch_dreams.egg-info/
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)    18737 2022-11-05 19:48:40.000000 torch-dreams-3.0.0/torch_dreams.egg-info/PKG-INFO
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)      766 2022-11-05 19:48:40.000000 torch-dreams-3.0.0/torch_dreams.egg-info/SOURCES.txt
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)        1 2022-11-05 19:48:40.000000 torch-dreams-3.0.0/torch_dreams.egg-info/dependency_links.txt
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)       61 2022-11-05 19:48:40.000000 torch-dreams-3.0.0/torch_dreams.egg-info/requires.txt
--rwxrwxrwx   0 mayukh    (1000) mayukh    (1000)       13 2022-11-05 19:48:40.000000 torch-dreams-3.0.0/torch_dreams.egg-info/top_level.txt
+drwxrwxr-x   0 ratan     (1000) ratan     (1000)        0 2023-06-14 08:22:41.114270 torch-dreams-4.0.0/
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     1064 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/LICENSE
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)    15120 2023-06-14 08:22:41.114270 torch-dreams-4.0.0/PKG-INFO
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)    14185 2023-06-14 07:58:35.000000 torch-dreams-4.0.0/README.md
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)       38 2023-06-14 08:22:41.114270 torch-dreams-4.0.0/setup.cfg
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     1924 2023-06-14 08:19:16.000000 torch-dreams-4.0.0/setup.py
+drwxrwxr-x   0 ratan     (1000) ratan     (1000)        0 2023-06-14 08:22:41.114270 torch-dreams-4.0.0/torch_dreams/
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)      394 2023-06-14 08:13:44.000000 torch-dreams-4.0.0/torch_dreams/__init__.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     4672 2023-05-25 06:58:07.000000 torch-dreams-4.0.0/torch_dreams/auto_image_param.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     2476 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/batched_image_param.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     1361 2023-05-31 12:31:12.000000 torch-dreams-4.0.0/torch_dreams/batched_objective.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)      692 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/constants.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     3409 2023-05-25 06:58:07.000000 torch-dreams-4.0.0/torch_dreams/custom_image_param.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)    15466 2023-06-14 07:17:57.000000 torch-dreams-4.0.0/torch_dreams/dreamer.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)      738 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/dreamer_utils.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)      510 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/error_handlers.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     1536 2023-06-14 07:34:40.000000 torch-dreams-4.0.0/torch_dreams/image_transforms.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     1708 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/losses.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     3390 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/masked_image_param.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)      572 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/model_bunch.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     1629 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/noisegrad.py
+drwxrwxr-x   0 ratan     (1000) ratan     (1000)        0 2023-06-14 08:22:41.114270 torch-dreams-4.0.0/torch_dreams/tests/
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)       23 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/tests/__init__.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)    10353 2023-06-14 07:33:26.000000 torch-dreams-4.0.0/torch_dreams/tests/test.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     2893 2023-06-14 07:20:27.000000 torch-dreams-4.0.0/torch_dreams/tests/test_batched.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     2522 2023-05-25 05:40:37.000000 torch-dreams-4.0.0/torch_dreams/transforms.py
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)     4828 2023-06-14 07:17:32.000000 torch-dreams-4.0.0/torch_dreams/utils.py
+drwxrwxr-x   0 ratan     (1000) ratan     (1000)        0 2023-06-14 08:22:41.114270 torch-dreams-4.0.0/torch_dreams.egg-info/
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)    15120 2023-06-14 08:22:41.000000 torch-dreams-4.0.0/torch_dreams.egg-info/PKG-INFO
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)      766 2023-06-14 08:22:41.000000 torch-dreams-4.0.0/torch_dreams.egg-info/SOURCES.txt
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)        1 2023-06-14 08:22:41.000000 torch-dreams-4.0.0/torch_dreams.egg-info/dependency_links.txt
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)       61 2023-06-14 08:22:41.000000 torch-dreams-4.0.0/torch_dreams.egg-info/requires.txt
+-rw-rw-r--   0 ratan     (1000) ratan     (1000)       13 2023-06-14 08:22:41.000000 torch-dreams-4.0.0/torch_dreams.egg-info/top_level.txt
```

### Comparing `torch-dreams-3.0.0/LICENSE` & `torch-dreams-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/PKG-INFO` & `torch-dreams-4.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,472 +1,471 @@
 Metadata-Version: 2.1
 Name: torch-dreams
-Version: 3.0.0
+Version: 4.0.0
 Summary: Making neural networks more interpretable, for research and art
 Home-page: https://github.com/Mayukhdeb/torch-dreams
 Author: Mayukh Deb
 Author-email: mayukhmainak2000@gmail.com
-License: UNKNOWN
-Description: # Torch-Dreams
-        Making neural networks more interpretable, for research and art. 
-        
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb)
-        [![build](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml/badge.svg)](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml)
-        [![codecov](https://codecov.io/gh/Mayukhdeb/torch-dreams/branch/master/graph/badge.svg?token=krU6dNleoJ)](https://codecov.io/gh/Mayukhdeb/torch-dreams)
-        <!-- [![](https://img.shields.io/twitter/url?label=Docs&style=flat-square&url=https%3A%2F%2Fapp.gitbook.com%2F%40mayukh09%2Fs%2Ftorch-dreams%2F)](https://app.gitbook.com/@mayukh09/s/torch-dreams/) -->
-        
-        
-        <img src = "https://github.com/Mayukhdeb/torch-dreams/blob/master/images/banner_segmentation_model.png?raw=true">
-        
-        ```
-        pip install torch-dreams 
-        ```
-        
-        ## Contents:
-        
-        * [Minimal example](https://github.com/Mayukhdeb/torch-dreams#minimal-example)
-        * [Not so minimal example](https://github.com/Mayukhdeb/torch-dreams#not-so-minimal-example)
-        * [Visualizing individual channels with `custom_func`](https://github.com/Mayukhdeb/torch-dreams#visualizing-individual-channels-with-custom_func)
-        * [Caricatures](https://github.com/Mayukhdeb/torch-dreams#caricatures)
-        * [Visualize features from multiple models simultaneously](https://github.com/Mayukhdeb/torch-dreams#visualize-features-from-multiple-models-simultaneously)
-        * [Use custom transforms](https://github.com/Mayukhdeb/torch-dreams#using-custom-transforms)
-        * [Feedback loops](https://github.com/Mayukhdeb/torch-dreams#you-can-also-use-outputs-of-one-render-as-the-input-of-another-to-create-feedback-loops)
-        * [Custom images](https://github.com/Mayukhdeb/torch-dreams#using-custom-images)
-        * [Working on models with different image normalizations](https://github.com/Mayukhdeb/torch-dreams#working-on-models-with-different-image-normalizations)
-        * [Masked image parametrs](https://github.com/Mayukhdeb/torch-dreams#masked-image-parameters)
-        * [Other conveniences](https://github.com/Mayukhdeb/torch-dreams#other-conveniences)
-        * [Development](https://github.com/Mayukhdeb/torch-dreams#development)
-        
-        ## Minimal example
-        > Make sure you also check out the [quick start colab notebook](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb) 
-        
-        
-        ```python
-        import matplotlib.pyplot as plt
-        import torchvision.models as models
-        from torch_dreams import Dreamer
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device = 'cuda')
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_5b],
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Not so minimal example
-        ```python
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device = 'cuda', quiet = False)
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_5b],
-            width = 256,
-            height = 256,
-            iters = 150,
-            lr = 9e-3,
-            rotate_degrees = 15,
-            scale_max = 1.2,
-            scale_min =  0.5,
-            translate_x = 0.2,
-            translate_y = 0.2,
-            custom_func = None,
-            weight_decay = 1e-2,
-            grad_clip = 1.,
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Visualizing individual channels with `custom_func`
-        
-        ```python
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device = 'cuda')
-        
-        layers_to_use = [model.Mixed_6b.branch1x1.conv]
-        
-        def make_custom_func(layer_number = 0, channel_number= 0): 
-            def custom_func(layer_outputs):
-                loss = layer_outputs[layer_number][channel_number].mean()
-                return -loss
-            return custom_func
-        
-        my_custom_func = make_custom_func(layer_number= 0, channel_number = 119)
-        
-        image_param = dreamy_boi.render(
-            layers = layers_to_use,
-            custom_func = my_custom_func,
-        )
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Batched generation for large scale experiments
-        
-        The `BatchedAutoImageParam` paired with the `BatchedObjective` can be used to generate multiple feature visualizations in parallel. This takes up more memory based on the batch size, but is also faster than generating one visualization at a time.
-        
-        ```python
-        from torch_dreams import Dreamer
-        import torchvision.models as models
-        from torch_dreams.batched_objective import BatchedObjective
-        from torch_dreams.batched_image_param import BatchedAutoImageParam
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device="cuda")
-        
-        ## specify list of neuron indices to visualize
-        batch_neuron_indices = [i for i in range(10,20)]
-        
-        ## set up a batch of trainable image parameters
-        bap = BatchedAutoImageParam(
-            batch_size=len(batch_neuron_indices), 
-            width=256, 
-            height=256, 
-            standard_deviation=0.01
-        )
-        
-        ## objective generator for each neuron
-        def make_custom_func(layer_number=0, channel_number=0):
-            def custom_func(layer_outputs):
-                loss = layer_outputs[layer_number][channel_number].norm()
-                return -loss
-        
-            return custom_func
-        
-        ## prepare objective functions for each neuron index
-        batched_objective = BatchedObjective(
-            objectives=[make_custom_func(channel_number=i) for i in batch_neuron_indices]
-        )
-        
-        ## render activation maximization signals
-        result_batch = dreamy_boi.render(
-            layers=[model.Mixed_5b],
-            image_parameter=bap,
-            iters=120,
-            custom_func=batched_objective,
-        )
-        
-        ## save results in a folder
-        for i in batch_neuron_indices:
-            result_batch[batch_neuron_indices.index(i)].save(f"results/{i}.jpg")
-        ```
-        
-        ## Caricatures
-        
-        Caricatures create a new image that has a similar but more extreme activation pattern to the input image at a given layer (or multiple layers at a time). It's inspired from [this issue](https://github.com/tensorflow/lucid/issues/121)
-        
-        <img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/caricature.png" width = "70%">
-        
-        In this case, let's use googlenet 
-        
-        ```python
-        model = models.googlenet(pretrained = True)
-        dreamy_boi = Dreamer(model = model, quiet= False, device= 'cuda')
-        
-        image_param = dreamy_boi.caricature(
-            input_tensor = image_tensor, 
-            layers = [model.inception4c],   ## feel free to append more layers for more interesting caricatures 
-            power= 1.2,                     ## higher -> more "exaggerated" features
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        ## Visualize features from multiple models simultaneously
-        
-        First, let's pick 2 models and specify which layers we'd want to work with
-        
-        ```python
-        from torch_dreams.model_bunch import ModelBunch
-        
-        bunch = ModelBunch(
-            model_dict = {
-                'inception': models.inception_v3(pretrained=True).eval(),
-                'resnet':    models.resnet18(pretrained= True).eval()
-            }
-        )
-        
-        layers_to_use = [
-                    bunch.model_dict['inception'].Mixed_6a,
-                    bunch.model_dict['resnet'].layer2[0].conv1
-                ]
-        
-        dreamy_boi = Dreamer(model = bunch, quiet= False, device= 'cuda')
-        ```
-        
-        Then define a `custom_func` which determines which exact activations of the models we have to optimize
-        
-        ```python
-        def custom_func(layer_outputs):
-            loss =   layer_outputs[0].mean()*2.0 + layer_outputs[1][89].mean() 
-            return -loss
-        ```
-        
-        Run the optimization
-        
-        ```python
-        image_param = dreamy_boi.render(
-            layers = layers_to_use,
-            custom_func= custom_func,
-            iters= 100
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        
-        ## Using custom transforms:
-        
-        ```python
-        import torchvision.transforms as transforms
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
-        
-        my_transforms = transforms.Compose([
-            transforms.RandomAffine(degrees = 10, translate = (0.5,0.5)),
-            transforms.RandomHorizontalFlip(p = 0.3)
-        ])
-        
-        dreamy_boi.set_custom_transforms(transforms = my_transforms)
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_5b],
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## You can also use outputs of one `render()` as the input of another to create feedback loops.
-        
-        ```python
-        import matplotlib.pyplot as plt
-        import torchvision.models as models
-        from torch_dreams import Dreamer
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_6c],
-        )
-        
-        image_param = dreamy_boi.render(
-            image_parameter= image_param,
-            layers = [model.Mixed_5b],
-            iters = 20
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Using custom images
-        
-        Note that you might have to use smaller values for certain hyperparameters like `lr` and `grad_clip`.
-        
-        ```python
-        from torch_dreams.custom_image_param import CustomImageParam
-        param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cuda')  ## image could either be a filename or a torch.tensor of shape NCHW
-        
-        image_param = dreamy_boi.render(
-            image_parameter= param,
-            layers = [model.Mixed_6c],
-            lr = 2e-4,
-            grad_clip = 0.1,
-            weight_decay= 1e-1,
-            iters = 120
-        )
-        ```
-        
-        ## Working on models with different image normalizations
-        
-        `torch-dreams` generally works with models trained on images normalized with imagenet `mean` and `std`, but that can be easily overriden to support any other normalization. For example, if you have a model with `mean = [0.5, 0.5, 0.5]` and `std = [0.5, 0.5, 0.5]`: 
-        
-        ```python 
-        t = torchvision.transforms.Normalize(
-                        mean = [0.5, 0.5, 0.5],
-                        std =  [0.5, 0.5, 0.5]
-                    )
-        
-        dreamy_boi.set_custom_normalization(normalization_transform = t) ## normalization_transform could be any instance of torch.nn.Module
-        ```
-        
-        ## Masked Image parameters
-        
-        Can be used to optimize only certain parts of the image using a mask whose values are clipped between `[0,1]`.
-        
-        <img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/masked_param.png" width = "80%">
-        
-        Here's an example with a vertical gradient 
-        
-        ```python 
-        from torch_dreams.masked_image_param import MaskedImageParam
-        
-        mask = torch.ones(1,1,512,512)
-        
-        for i in range(0, 512, 1):  ## vertical gradient
-            mask[:,:,i,:] = (i/512)
-        
-        param = MaskedImageParam(
-            image= 'images/sample_small.jpg',  ## optional
-            mask_tensor = mask,
-            device = 'cuda'
-        )
-        
-        param = dreamy_boi.render(
-            layers = [model.inception4c],
-            image_parameter= param,
-            lr = 1e-4,
-            grad_clip= 0.1,
-            weight_decay= 1e-1,
-            iters= 200,
-        )
-        
-        param.save('masked_param_output.jpg')
-        ```
-        
-        It's also possible to update the mask on the fly with `param.update_mask(some_mask)`
-        
-        ```python
-        
-        param.update_mask(mask = torch.flip(mask, dims = (2,)))
-        
-        param = dreamy_boi.render(
-            layers = [model.inception4a],
-            image_parameter= param,
-            lr = 1e-4,
-            grad_clip= 0.1,
-            weight_decay= 1e-1,
-            iters= 200,
-        )
-        
-        param.save('masked_param_output_2.jpg')
-        ```
-        
-        
-        ## Other conveniences 
-        
-        The following methods are handy for an [`auto_image_param`](https://github.com/Mayukhdeb/torch-dreams/blob/master/torch_dreams/auto_image_param.py) instance:
-        
-        1. Saving outputs as images:
-        
-        ```python
-        image_param.save('output.jpg')
-        ```
-        
-        2. Torch Tensor of dimensions `(height, width, color_channels)`
-        
-        ```python
-        torch_image = image_param.to_hwc_tensor(device = 'cpu')
-        ```
-        
-        3. Torch Tensor of dimensions `(color_channels, height, width)`
-        
-        ```python
-        torch_image_chw = image_param.to_chw_tensor(device = 'cpu')
-        ```
-        
-        4. Displaying outputs on matplotlib. 
-        
-        ```python
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        5. For instances of `custom_image_param`, you can set any NCHW tensor as the image parameter: 
-        
-        ```python
-        image_tensor = image_param.to_nchw_tensor()
-        
-        ## do some stuff with image_tensor
-        t = transforms.Compose([
-            transforms.RandomRotation(5)
-        ])
-        transformed_image_tensor = t(image_tensor) 
-        
-        image_param.set_param(tensor = transformed_image_tensor)
-        ```
-        
-        ## Args for `render()`
-        
-        * `layers` (`iterable`): List of the layers of model(s)'s layers to work on. `[model.layer1, model.layer2...]`
-        * `image_parameter` (`auto_image_param`, optional): Instance of `torch_dreams.auto_image_param.auto_image_param`
-        
-        * `width` (`int`, optional): Width of image to be optimized 
-        * `height` (`int`, optional): Height of image to be optimized 
-        * `iters` (`int`, optional): Number of iterations, higher -> stronger visualization
-        * `lr` (`float`, optional): Learning rate
-        * `rotate_degrees` (`int`, optional): Max rotation in default transforms
-        * `scale_max` (`float`, optional): Max image size factor. Defaults to 1.1.
-        * `scale_min` (`float`, optional): Minimum image size factor. Defaults to 0.5.
-        * `translate_x` (`float`, optional): Maximum translation factor in x direction
-        * `translate_y` (`float`, optional): Maximum translation factor in y direction
-        * `custom_func` (`function`, optional): Can be used to define custom optimiziation conditions to `render()`. Defaults to None.
-        * `weight_decay` (`float`, optional): Weight decay for default optimizer. Helps prevent high frequency noise. Defaults to 0.
-        * `grad_clip` (`float`, optional): Maximum value of the norm of gradient. Defaults to 1.
-        
-        ## Args for `Dreamer.__init__()`
-         * `model` (`nn.Module` or  `torch_dreams.model_bunch.Modelbunch`): Almost any PyTorch model which was trained on imagenet `mean` and `std`, and supports variable sized images as inputs. You can pass multiple models into this argument as a `torch_dreams.model_bunch.Modelbunch` instance.
-         * `quiet` (`bool`): Set to `True` if you want to disable any progress bars
-         * `device` (`str`): `cuda` or `cpu` depending on your runtime 
-        
-         ## Development
-        
-        1. Clone the repo and navigate into the folder
-        ```
-        git clone git@github.com:Mayukhdeb/torch-dreams.git
-        cd torch-dreams/
-        ```
-        
-        2. Install dependencies
-        ```
-        pip install -r requirements.txt
-        ```
-        
-        3. Install `torch-dreams` as an editable module
-        ```
-        python3 setup.py develop
-        ```
-        
-        ## Citation
-        ```
-        @misc{mayukhdebtorchdreams,
-          title={Feature Visualization library for PyTorch},
-          author={Mayukh Deb},
-          year={2021},
-          publisher={GitHub},
-          howpublished={\url{https://github.com/Mayukhdeb/torch-dreams}},
-        }
-        ```
-        
-        ## Acknowledgements
-        
-        * [amFOSS](https://amfoss.in/)
-        * [Gene Kogan](https://github.com/genekogan) 
-        
-        ## Recommended Reading 
-        
-        * [Feature Visualization](https://distill.pub/2017/feature-visualization/)
-        * [Google AI blog on Deepdreams](https://ai.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)
-        
 Keywords: PyTorch,machine learning,neural networks,convolutional neural networks,feature visualization,optimization
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Torch-Dreams
+Making neural networks more interpretable, for research and art. 
+
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb)
+[![build](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml/badge.svg)](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/Mayukhdeb/torch-dreams/branch/master/graph/badge.svg?token=krU6dNleoJ)](https://codecov.io/gh/Mayukhdeb/torch-dreams)
+<!-- [![](https://img.shields.io/twitter/url?label=Docs&style=flat-square&url=https%3A%2F%2Fapp.gitbook.com%2F%40mayukh09%2Fs%2Ftorch-dreams%2F)](https://app.gitbook.com/@mayukh09/s/torch-dreams/) -->
+
+
+<img src = "https://github.com/Mayukhdeb/torch-dreams/blob/master/images/banner_segmentation_model.png?raw=true">
+
+```
+pip install torch-dreams 
+```
+
+## Contents:
+
+* [Minimal example](https://github.com/Mayukhdeb/torch-dreams#minimal-example)
+* [Not so minimal example](https://github.com/Mayukhdeb/torch-dreams#not-so-minimal-example)
+* [Visualizing individual channels with `custom_func`](https://github.com/Mayukhdeb/torch-dreams#visualizing-individual-channels-with-custom_func)
+* [Caricatures](https://github.com/Mayukhdeb/torch-dreams#caricatures)
+* [Visualize features from multiple models simultaneously](https://github.com/Mayukhdeb/torch-dreams#visualize-features-from-multiple-models-simultaneously)
+* [Use custom transforms](https://github.com/Mayukhdeb/torch-dreams#using-custom-transforms)
+* [Feedback loops](https://github.com/Mayukhdeb/torch-dreams#you-can-also-use-outputs-of-one-render-as-the-input-of-another-to-create-feedback-loops)
+* [Custom images](https://github.com/Mayukhdeb/torch-dreams#using-custom-images)
+* [Working on models with different image normalizations](https://github.com/Mayukhdeb/torch-dreams#working-on-models-with-different-image-normalizations)
+* [Masked image parametrs](https://github.com/Mayukhdeb/torch-dreams#masked-image-parameters)
+* [Other conveniences](https://github.com/Mayukhdeb/torch-dreams#other-conveniences)
+* [Development](https://github.com/Mayukhdeb/torch-dreams#development)
+
+## Minimal example
+> Make sure you also check out the [quick start colab notebook](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb) 
+
+
+```python
+import matplotlib.pyplot as plt
+import torchvision.models as models
+from torch_dreams import Dreamer
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device = 'cuda')
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_5b],
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## Not so minimal example
+```python
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device = 'cuda', quiet = False)
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_5b],
+    width = 256,
+    height = 256,
+    iters = 150,
+    lr = 9e-3,
+    rotate_degrees = 15,
+    scale_max = 1.2,
+    scale_min =  0.5,
+    translate_x = 0.2,
+    translate_y = 0.2,
+    custom_func = None,
+    weight_decay = 1e-2,
+    grad_clip = 1.,
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## Visualizing individual channels with `custom_func`
+
+```python
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device = 'cuda')
+
+layers_to_use = [model.Mixed_6b.branch1x1.conv]
+
+def make_custom_func(layer_number = 0, channel_number= 0): 
+    def custom_func(layer_outputs):
+        loss = layer_outputs[layer_number][:, channel_number].mean()
+        return -loss
+    return custom_func
+
+my_custom_func = make_custom_func(layer_number= 0, channel_number = 119)
+
+image_param = dreamy_boi.render(
+    layers = layers_to_use,
+    custom_func = my_custom_func,
+)
+plt.imshow(image_param)
+plt.show()
+```
+
+## Batched generation for large scale experiments
+
+The `BatchedAutoImageParam` paired with the `BatchedObjective` can be used to generate multiple feature visualizations in parallel. This takes up more memory based on the batch size, but is also faster than generating one visualization at a time.
+
+```python
+from torch_dreams import Dreamer
+import torchvision.models as models
+from torch_dreams.batched_objective import BatchedObjective
+from torch_dreams.batched_image_param import BatchedAutoImageParam
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device="cuda")
+
+## specify list of neuron indices to visualize
+batch_neuron_indices = [i for i in range(10,20)]
+
+## set up a batch of trainable image parameters
+bap = BatchedAutoImageParam(
+    batch_size=len(batch_neuron_indices), 
+    width=256, 
+    height=256, 
+    standard_deviation=0.01
+)
+
+## objective generator for each neuron
+def make_custom_func(layer_number=0, channel_number=0):
+    def custom_func(layer_outputs):
+        loss = layer_outputs[layer_number][:, channel_number].norm()
+        return -loss
+
+    return custom_func
+
+## prepare objective functions for each neuron index
+batched_objective = BatchedObjective(
+    objectives=[make_custom_func(channel_number=i) for i in batch_neuron_indices]
+)
+
+## render activation maximization signals
+result_batch = dreamy_boi.render(
+    layers=[model.Mixed_5b],
+    image_parameter=bap,
+    iters=120,
+    custom_func=batched_objective,
+)
+
+## save results in a folder
+for i in batch_neuron_indices:
+    result_batch[batch_neuron_indices.index(i)].save(f"results/{i}.jpg")
+```
+
+## Caricatures
+
+Caricatures create a new image that has a similar but more extreme activation pattern to the input image at a given layer (or multiple layers at a time). It's inspired from [this issue](https://github.com/tensorflow/lucid/issues/121)
+
+<img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/caricature.png" width = "70%">
+
+In this case, let's use googlenet 
+
+```python
+model = models.googlenet(pretrained = True)
+dreamy_boi = Dreamer(model = model, quiet= False, device= 'cuda')
+
+image_param = dreamy_boi.caricature(
+    input_tensor = image_tensor, 
+    layers = [model.inception4c],   ## feel free to append more layers for more interesting caricatures 
+    power= 1.2,                     ## higher -> more "exaggerated" features
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+## Visualize features from multiple models simultaneously
+
+First, let's pick 2 models and specify which layers we'd want to work with
+
+```python
+from torch_dreams.model_bunch import ModelBunch
+
+bunch = ModelBunch(
+    model_dict = {
+        'inception': models.inception_v3(pretrained=True).eval(),
+        'resnet':    models.resnet18(pretrained= True).eval()
+    }
+)
+
+layers_to_use = [
+            bunch.model_dict['inception'].Mixed_6a,
+            bunch.model_dict['resnet'].layer2[0].conv1
+        ]
+
+dreamy_boi = Dreamer(model = bunch, quiet= False, device= 'cuda')
+```
+
+Then define a `custom_func` which determines which exact activations of the models we have to optimize
+
+```python
+def custom_func(layer_outputs):
+    loss =   layer_outputs[0].mean()*2.0 + layer_outputs[1][:, 89].mean() 
+    return -loss
+```
+
+Run the optimization
+
+```python
+image_param = dreamy_boi.render(
+    layers = layers_to_use,
+    custom_func= custom_func,
+    iters= 100
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+
+## Using custom transforms:
+
+```python
+import torchvision.transforms as transforms
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
+
+my_transforms = transforms.Compose([
+    transforms.RandomAffine(degrees = 10, translate = (0.5,0.5)),
+    transforms.RandomHorizontalFlip(p = 0.3)
+])
+
+dreamy_boi.set_custom_transforms(transforms = my_transforms)
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_5b],
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## You can also use outputs of one `render()` as the input of another to create feedback loops.
+
+```python
+import matplotlib.pyplot as plt
+import torchvision.models as models
+from torch_dreams import Dreamer
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_6c],
+)
+
+image_param = dreamy_boi.render(
+    image_parameter= image_param,
+    layers = [model.Mixed_5b],
+    iters = 20
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## Using custom images
+
+Note that you might have to use smaller values for certain hyperparameters like `lr` and `grad_clip`.
+
+```python
+from torch_dreams.custom_image_param import CustomImageParam
+param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cuda')  ## image could either be a filename or a torch.tensor of shape NCHW
+
+image_param = dreamy_boi.render(
+    image_parameter= param,
+    layers = [model.Mixed_6c],
+    lr = 2e-4,
+    grad_clip = 0.1,
+    weight_decay= 1e-1,
+    iters = 120
+)
+```
+
+## Working on models with different image normalizations
+
+`torch-dreams` generally works with models trained on images normalized with imagenet `mean` and `std`, but that can be easily overriden to support any other normalization. For example, if you have a model with `mean = [0.5, 0.5, 0.5]` and `std = [0.5, 0.5, 0.5]`: 
+
+```python 
+t = torchvision.transforms.Normalize(
+                mean = [0.5, 0.5, 0.5],
+                std =  [0.5, 0.5, 0.5]
+            )
+
+dreamy_boi.set_custom_normalization(normalization_transform = t) ## normalization_transform could be any instance of torch.nn.Module
+```
+
+## Masked Image parameters
+
+Can be used to optimize only certain parts of the image using a mask whose values are clipped between `[0,1]`.
+
+<img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/masked_param.png" width = "80%">
+
+Here's an example with a vertical gradient 
+
+```python 
+from torch_dreams.masked_image_param import MaskedImageParam
+
+mask = torch.ones(1,1,512,512)
+
+for i in range(0, 512, 1):  ## vertical gradient
+    mask[:,:,i,:] = (i/512)
+
+param = MaskedImageParam(
+    image= 'images/sample_small.jpg',  ## optional
+    mask_tensor = mask,
+    device = 'cuda'
+)
+
+param = dreamy_boi.render(
+    layers = [model.inception4c],
+    image_parameter= param,
+    lr = 1e-4,
+    grad_clip= 0.1,
+    weight_decay= 1e-1,
+    iters= 200,
+)
+
+param.save('masked_param_output.jpg')
+```
+
+It's also possible to update the mask on the fly with `param.update_mask(some_mask)`
+
+```python
+
+param.update_mask(mask = torch.flip(mask, dims = (2,)))
+
+param = dreamy_boi.render(
+    layers = [model.inception4a],
+    image_parameter= param,
+    lr = 1e-4,
+    grad_clip= 0.1,
+    weight_decay= 1e-1,
+    iters= 200,
+)
+
+param.save('masked_param_output_2.jpg')
+```
+
+
+## Other conveniences 
+
+The following methods are handy for an [`auto_image_param`](https://github.com/Mayukhdeb/torch-dreams/blob/master/torch_dreams/auto_image_param.py) instance:
+
+1. Saving outputs as images:
+
+```python
+image_param.save('output.jpg')
+```
+
+2. Torch Tensor of dimensions `(height, width, color_channels)`
+
+```python
+torch_image = image_param.to_hwc_tensor(device = 'cpu')
+```
+
+3. Torch Tensor of dimensions `(color_channels, height, width)`
+
+```python
+torch_image_chw = image_param.to_chw_tensor(device = 'cpu')
+```
+
+4. Displaying outputs on matplotlib. 
+
+```python
+plt.imshow(image_param)
+plt.show()
+```
+
+5. For instances of `custom_image_param`, you can set any NCHW tensor as the image parameter: 
+
+```python
+image_tensor = image_param.to_nchw_tensor()
+
+## do some stuff with image_tensor
+t = transforms.Compose([
+    transforms.RandomRotation(5)
+])
+transformed_image_tensor = t(image_tensor) 
+
+image_param.set_param(tensor = transformed_image_tensor)
+```
+
+## Args for `render()`
+
+* `layers` (`iterable`): List of the layers of model(s)'s layers to work on. `[model.layer1, model.layer2...]`
+* `image_parameter` (`auto_image_param`, optional): Instance of `torch_dreams.auto_image_param.auto_image_param`
+
+* `width` (`int`, optional): Width of image to be optimized 
+* `height` (`int`, optional): Height of image to be optimized 
+* `iters` (`int`, optional): Number of iterations, higher -> stronger visualization
+* `lr` (`float`, optional): Learning rate
+* `rotate_degrees` (`int`, optional): Max rotation in default transforms
+* `scale_max` (`float`, optional): Max image size factor. Defaults to 1.1.
+* `scale_min` (`float`, optional): Minimum image size factor. Defaults to 0.5.
+* `translate_x` (`float`, optional): Maximum translation factor in x direction
+* `translate_y` (`float`, optional): Maximum translation factor in y direction
+* `custom_func` (`function`, optional): Can be used to define custom optimiziation conditions to `render()`. Defaults to None.
+* `weight_decay` (`float`, optional): Weight decay for default optimizer. Helps prevent high frequency noise. Defaults to 0.
+* `grad_clip` (`float`, optional): Maximum value of the norm of gradient. Defaults to 1.
+
+## Args for `Dreamer.__init__()`
+ * `model` (`nn.Module` or  `torch_dreams.model_bunch.Modelbunch`): Almost any PyTorch model which was trained on imagenet `mean` and `std`, and supports variable sized images as inputs. You can pass multiple models into this argument as a `torch_dreams.model_bunch.Modelbunch` instance.
+ * `quiet` (`bool`): Set to `True` if you want to disable any progress bars
+ * `device` (`str`): `cuda` or `cpu` depending on your runtime 
+
+ ## Development
+
+1. Clone the repo and navigate into the folder
+```
+git clone git@github.com:Mayukhdeb/torch-dreams.git
+cd torch-dreams/
+```
+
+2. Install dependencies
+```
+pip install -r requirements.txt
+```
+
+3. Install `torch-dreams` as an editable module
+```
+python3 setup.py develop
+```
+
+## Citation
+```
+@misc{mayukhdebtorchdreams,
+  title={Feature Visualization library for PyTorch},
+  author={Mayukh Deb},
+  year={2021},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/Mayukhdeb/torch-dreams}},
+}
+```
+
+## Acknowledgements
+
+* [amFOSS](https://amfoss.in/)
+* [Gene Kogan](https://github.com/genekogan) 
+
+## Recommended Reading 
+
+* [Feature Visualization](https://distill.pub/2017/feature-visualization/)
+* [Google AI blog on Deepdreams](https://ai.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)
```

### Comparing `torch-dreams-3.0.0/README.md` & `torch-dreams-4.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 model = models.inception_v3(pretrained=True)
 dreamy_boi = Dreamer(model, device = 'cuda')
 
 layers_to_use = [model.Mixed_6b.branch1x1.conv]
 
 def make_custom_func(layer_number = 0, channel_number= 0): 
     def custom_func(layer_outputs):
-        loss = layer_outputs[layer_number][channel_number].mean()
+        loss = layer_outputs[layer_number][:, channel_number].mean()
         return -loss
     return custom_func
 
 my_custom_func = make_custom_func(layer_number= 0, channel_number = 119)
 
 image_param = dreamy_boi.render(
     layers = layers_to_use,
@@ -121,15 +121,15 @@
     height=256, 
     standard_deviation=0.01
 )
 
 ## objective generator for each neuron
 def make_custom_func(layer_number=0, channel_number=0):
     def custom_func(layer_outputs):
-        loss = layer_outputs[layer_number][channel_number].norm()
+        loss = layer_outputs[layer_number][:, channel_number].norm()
         return -loss
 
     return custom_func
 
 ## prepare objective functions for each neuron index
 batched_objective = BatchedObjective(
     objectives=[make_custom_func(channel_number=i) for i in batch_neuron_indices]
@@ -191,15 +191,15 @@
 dreamy_boi = Dreamer(model = bunch, quiet= False, device= 'cuda')
 ```
 
 Then define a `custom_func` which determines which exact activations of the models we have to optimize
 
 ```python
 def custom_func(layer_outputs):
-    loss =   layer_outputs[0].mean()*2.0 + layer_outputs[1][89].mean() 
+    loss =   layer_outputs[0].mean()*2.0 + layer_outputs[1][:, 89].mean() 
     return -loss
 ```
 
 Run the optimization
 
 ```python
 image_param = dreamy_boi.render(
```

### Comparing `torch-dreams-3.0.0/torch_dreams/auto_image_param.py` & `torch-dreams-4.0.0/torch_dreams/auto_image_param.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     Args:
         height (int): Height of image
         width (int): Width of image
         device (str): 'cpu' or 'cuda'
         standard_deviation (float): Standard deviation of the image initiated in the frequency domain. ). 0.01 works well
     """
 
-    def __init__(self, height, width, device, standard_deviation):
+    def __init__(self, height, width, device, standard_deviation, batch_size: int = 1):
 
         super().__init__()
         self.height = height
         self.width = width
 
         """
         odd width is resized to even with one extra column
@@ -122,14 +122,15 @@
                 width=self.width,
                 sd=standard_deviation,
                 device=device,
             )
 
         self.param.requires_grad_()
         self.optimizer = None
+        self.batch_size = batch_size
 
     def postprocess(self, device):
         img = fft_to_rgb(
             height=self.height,
             width=self.width,
             image_parameter=self.param,
             device=device,
@@ -138,8 +139,17 @@
         img = torch.sigmoid(img)
         return img
 
     def normalize(self, x, device):
         return normalize(x=x, device=device)
 
     def forward(self, device):
-        return self.normalize(self.postprocess(device=device), device=device)
+        if self.batch_size == 1:
+            return self.normalize(self.postprocess(device=device), device=device)
+        else:
+            return torch.cat(
+                [
+                    self.normalize(self.postprocess(device=device), device=device)
+                    for i in range(self.batch_size)
+                ],
+                dim=0,
+            )
```

### Comparing `torch-dreams-3.0.0/torch_dreams/batched_image_param.py` & `torch-dreams-4.0.0/torch_dreams/batched_image_param.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/batched_objective.py` & `torch-dreams-4.0.0/torch_dreams/batched_objective.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,18 @@
         Args:
             objectives (List[Callable]): list of all custom_func i.e objective functions. It's length should be same as that of the batch size.
         """
         self.objectives = objectives
 
     def __call__(self, x: list):
 
+        '''
+        x (List[torch.tensor]): x is a list of torch tensors. Each of which has the same batch size.
+        The index in the list corresponds to the layers in layers_to_use
+        '''
         for y in x:
             assert torch.is_tensor(
                 y
             ), f"Expected every item in x to be a torch.tensor, but got: {type(y)}"
 
         batch_size = x[0].shape[0]
 
@@ -25,11 +29,11 @@
             self.objectives
         ), f"Batch size of x and len(self.objectives) do not match: {x[0].shape[0]} and {len(self.objectives)}"
 
         loss_sum = torch.tensor(0.0).to(x[0].device)
 
         for batch_idx in range(batch_size):
             loss_sum += self.objectives[batch_idx](
-                x[0][batch_idx].unsqueeze(0)
+                [item[batch_idx].unsqueeze(0) for item in x]
             )  ## is unsqueeze this really necessary? idk
 
         return loss_sum  ## then call loss_sum.backward()
```

### Comparing `torch-dreams-3.0.0/torch_dreams/constants.py` & `torch-dreams-4.0.0/torch_dreams/constants.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/custom_image_param.py` & `torch-dreams-4.0.0/torch_dreams/custom_image_param.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from .auto_image_param import BaseImageParam
 
 import cv2 
 import torch
-import numpy as np
-
-from .constants import Constants
-from .error_handlers import PytorchVersionError
 
 from .utils import (
     lucid_colorspace_to_rgb, 
     normalize,
     get_fft_scale_custom_img,
-    denormalize,
-    rgb_to_lucid_colorspace,
     chw_rgb_to_fft_param,
     fft_to_rgb_custom_img
 )
 
 class CustomImageParam(BaseImageParam):
     """FFT parameterization for custom images
```

### Comparing `torch-dreams-3.0.0/torch_dreams/dreamer.py` & `torch-dreams-4.0.0/torch_dreams/dreamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .constants import Constants
 from .losses import CaricatureLoss
 from .image_transforms import InverseTransform
 from .auto_image_param import AutoImageParam
 from .dreamer_utils import Hook, default_func_mean
 from .masked_image_param import MaskedImageParam
 from .batched_image_param import BatchedImageParam
+from .utils import check_pytorch_version
 
 
 class Dreamer:
     """wrapper over a pytorch model for feature visualization
 
     Args:
         model (torch.nn.Module): pytorch model
@@ -41,14 +42,15 @@
         self.model.eval()
         self.device = device
         self.model.to(self.device)
         self.default_func = default_func_mean
         self.transforms = None
         self.quiet = quiet
         self.__custom_normalization_transform__ = None
+        check_pytorch_version()
 
     def get_default_transforms(
         self, rotate, scale_max, scale_min, translate_x, translate_y
     ):
         self.transforms = transforms.Compose(
             [
                 transforms.RandomAffine(
@@ -230,21 +232,16 @@
                 img = self.transforms(img)
 
             model_out = self.model(img)
 
             layer_outputs = []
 
             for hook in hooks:
-                ## if it's a BatchedImageParam, then include all batch items from hook output
-                if isinstance(image_parameter, BatchedImageParam):
-                    out = hook.output
-                else:
-                    ## else select only the first and only batch item
-                    out = hook.output[0]
-
+                ## shape: (batch_size, *)
+                out = hook.output
                 layer_outputs.append(out)
 
             if custom_func is not None:
                 loss = custom_func(layer_outputs)
             else:
                 loss = self.default_func(layer_outputs)
             loss.backward()
```

### Comparing `torch-dreams-3.0.0/torch_dreams/dreamer_utils.py` & `torch-dreams-4.0.0/torch_dreams/dreamer_utils.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/image_transforms.py` & `torch-dreams-4.0.0/torch_dreams/image_transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import torchvision.transforms as transforms
-import torch
 import torch.nn.functional as F
 import torch.nn as nn
 
 
 import warnings
 
 warnings.filterwarnings("ignore")
@@ -16,34 +15,32 @@
         transforms.RandomRotation(
             degrees=5, expand=False, center=None, fill=None
         ),
         transforms.ToTensor(),
     ]
 )
 
+def unnormalize_image_tensor(img, mean, std):
+    img = img * std.view(1,3,1,1) + mean.view(1,3,1,1)
+    return img.clamp(0,1)
+
 
 class InverseTransform(nn.Module):
     def __init__(self, old_mean, old_std, new_transforms):
         super().__init__()
-        self.inverse_transform = transforms.Compose(
-            [
-                transforms.Normalize(
-                    mean=[0.0, 0.0, 0.0],
-                    std=[1 / old_std[0], 1 / old_std[1], 1 / old_std[2]],
-                ),
-                transforms.Normalize(
-                    mean=[-old_mean[0], -old_mean[1], -old_mean[2]], std=[1.0, 1.0, 1.0]
-                ),
-            ]
-        )
-
+        self.old_mean = old_mean
+        self.old_std = old_std
         self.new_transform = new_transforms
 
     def forward(self, x):
-        x = self.inverse_transform(x)
+        x = unnormalize_image_tensor(
+            img = x,
+            mean = self.old_mean,
+            std = self.old_std
+        )
         x = self.new_transform(x)
         return x
 
     def __repr__(self):
         return (
             "InverseTransform(\n        "
             + str(self.inverse_transform)
```

### Comparing `torch-dreams-3.0.0/torch_dreams/losses.py` & `torch-dreams-4.0.0/torch_dreams/losses.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/masked_image_param.py` & `torch-dreams-4.0.0/torch_dreams/masked_image_param.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/model_bunch.py` & `torch-dreams-4.0.0/torch_dreams/model_bunch.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/noisegrad.py` & `torch-dreams-4.0.0/torch_dreams/noisegrad.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/tests/test.py` & `torch-dreams-4.0.0/torch_dreams/tests/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 import numpy as np
 import torch
 import os 
 
     
 def make_custom_func(layer_number = 0, channel_number= 0): 
     def custom_func(layer_outputs):
-        loss = layer_outputs[layer_number][channel_number].mean()
+        loss = layer_outputs[layer_number][:, channel_number].mean()
         return -loss
     return custom_func
 
 class test(unittest.TestCase):
 
     def test_single_model(self):
 
-        model = models.inception_v3(pretrained=True)
+        model = models.inception_v3(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model = model, device= 'cpu', quiet= False)
 
         image_param = dreamy_boi.render(
             layers = [model.Mixed_6a],
             iters = 5
         )
@@ -43,15 +43,15 @@
         self.assertTrue(isinstance(image_param.__array__(), np.ndarray))
         self.assertTrue(isinstance(image_param.to_hwc_tensor(), torch.Tensor), 'should be a torch.Tensor')
         self.assertTrue(isinstance(image_param.to_chw_tensor(), torch.Tensor), 'should be a torch.Tensor')
         os.remove('test_single_model.jpg')
 
     def test_custom_size(self):
 
-        model = models.inception_v3(pretrained=True)
+        model = models.inception_v3(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model = model, device= 'cpu', quiet= False)
 
         image_param = dreamy_boi.render(
             layers = [model.Mixed_6a],
             iters = 5,
             width = 255,
@@ -64,15 +64,15 @@
         self.assertTrue(isinstance(image_param, AutoImageParam), 'should be an instance of auto_image_param')
         self.assertTrue(isinstance(image_param.__array__(), np.ndarray))
         self.assertTrue(isinstance(image_param.to_hwc_tensor(), torch.Tensor), 'should be a torch.Tensor')
         self.assertTrue(isinstance(image_param.to_chw_tensor(), torch.Tensor), 'should be a torch.Tensor')
         os.remove('test_custom_size.jpg')
 
     def  test_single_model_custom_func(self):
-        model = models.inception_v3(pretrained=True)
+        model = models.inception_v3(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model = model, device= 'cpu', quiet= False)
 
         image_param = dreamy_boi.render(
             layers = [model.Mixed_6a],
             iters = 5,
             custom_func= make_custom_func(layer_number= 0, channel_number= 10)
@@ -85,15 +85,15 @@
         self.assertTrue(isinstance(image_param.__array__(), np.ndarray))
         self.assertTrue(isinstance(image_param.to_hwc_tensor(), torch.Tensor), 'should be a torch.Tensor')
         self.assertTrue(isinstance(image_param.to_chw_tensor(), torch.Tensor), 'should be a torch.Tensor')
         os.remove('test_single_model_custom_func.jpg')
 
     def test_multiple_models_custom_func(self):
 
-        model1  = models.inception_v3(pretrained=True).eval()
+        model1  = models.inception_v3(weights='DEFAULT').eval()
         model2  = models.resnet18(pretrained= True).eval() 
 
         bunch = ModelBunch(
             model_dict = {
                 'inception': model1,
                 'resnet':  model2
             }
@@ -103,15 +103,15 @@
             bunch.model_dict['inception'].Mixed_6a,
             bunch.model_dict['resnet'].layer2[0].conv1
         ]
 
         dreamy_boi = Dreamer(model = bunch, quiet= False, device= 'cpu')
 
         def custom_func(layer_outputs):
-            loss =  layer_outputs[1][89].mean() + layer_outputs[0].mean()**2
+            loss =  layer_outputs[1][:, 89].mean() + layer_outputs[0].mean()**2
             return -loss
 
         image_param = dreamy_boi.render(
             layers = layers_to_use,
             custom_func= custom_func,
             iters= 5
         )
@@ -124,15 +124,15 @@
         self.assertTrue(isinstance(image_param.to_hwc_tensor(), torch.Tensor), 'should be a torch.Tensor')
         self.assertTrue(isinstance(image_param.to_chw_tensor(), torch.Tensor), 'should be a torch.Tensor')
 
         os.remove('test_multiple_models_custom_func.jpg')
 
     def test_custom_image_param(self):
 
-        model = models.inception_v3(pretrained=True)
+        model = models.inception_v3(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model = model, device= 'cpu', quiet= False)
         param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cpu')
 
         image_param = dreamy_boi.render(
             image_parameter= param,
             layers = [model.Mixed_6a],
@@ -152,15 +152,15 @@
         os.remove('test_custom_image_param.jpg')
 
     def test_custom_image_param_set_param(self):
         """
         checks if custom_image_param.set_param correctly 
         loads the image without discrepancies with an absolute tolerance of 1e-5 element-wise
         """
-        model = models.inception_v3(pretrained=True)
+        model = models.inception_v3(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model = model, device= 'cpu', quiet= False)
         param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cpu')
 
         image_param = dreamy_boi.render(
             image_parameter= param,
             layers = [model.Mixed_6a],
@@ -175,15 +175,15 @@
         image_param.set_param(tensor = image_tensor)
         # print(torch.abs((image_tensor - image_param.to_nchw_tensor())).mean())
 
         self.assertTrue(torch.allclose(image_tensor ,image_param.to_nchw_tensor(), atol = 1e-5))
 
     def test_MaskedImageParam(self):
 
-        model = models.inception_v3(pretrained=True)
+        model = models.inception_v3(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model = model, device= 'cpu', quiet= False)
 
         mask_tensor = torch.ones(1,3,512,512)
         mask_tensor[:,:,:256,:] = 0.
 
         param = MaskedImageParam(
@@ -208,15 +208,15 @@
         self.assertTrue(isinstance(image_param.__array__(), np.ndarray))
         self.assertTrue(isinstance(image_param.to_hwc_tensor(), torch.Tensor), 'should be a torch.Tensor')
         self.assertTrue(isinstance(image_param.to_chw_tensor(), torch.Tensor), 'should be a torch.Tensor')
         os.remove('test_MaskedImageParam.jpg')     
 
     def test_caricature(self):
 
-        model = models.resnet18(pretrained=True)
+        model = models.resnet18(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model, device = 'cpu')
         param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cpu')
 
         image_tensor = param.to_nchw_tensor()
 
         param = dreamy_boi.caricature(
@@ -226,15 +226,15 @@
             iters = 5
         )
 
         self.assertTrue(isinstance(param, AutoImageParam), 'should be an auto_image_param')
 
     def test_static_caricature(self):
 
-        model = models.resnet18(pretrained=True)
+        model = models.resnet18(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model, device = 'cpu')
         param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cpu')
 
         image_tensor = param.to_nchw_tensor()
 
         param = dreamy_boi.caricature(
@@ -245,15 +245,15 @@
             static= True
         )
 
         self.assertTrue(isinstance(param, AutoImageParam), 'should be an auto_image_param')
 
     def test_custom_normalization(self):
 
-        model = models.resnet18(pretrained=True)
+        model = models.resnet18(weights='DEFAULT')
 
         dreamy_boi = Dreamer(model, device = 'cpu')
 
         t = transforms.Normalize(
                 mean=[0.485, 0.456, 0.406],
                 std=[0.229, 0.224, 0.225]
             )
```

### Comparing `torch-dreams-3.0.0/torch_dreams/tests/test_batched.py` & `torch-dreams-4.0.0/torch_dreams/tests/test_batched.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 import os
 
 import pytest
 
 
 def make_custom_func(layer_number=0, channel_number=0):
     def custom_func(layer_outputs):
-        loss = layer_outputs[layer_number][channel_number].mean()
+        loss = layer_outputs[layer_number][:, channel_number].mean()
         return -loss
 
     return custom_func
 
 
 @pytest.mark.parametrize("iters", [1, 2, 10, 20])
 @pytest.mark.parametrize("batch_size", [1, 2, 5])
 def test_batched_auto_image_param(iters, batch_size):
 
-    model = models.inception_v3(pretrained=True)
+    model = models.inception_v3(weights='DEFAULT')
     dreamy_boi = Dreamer(model=model, device="cpu", quiet=False)
 
     image_param = BatchedAutoImageParam(batch_size=batch_size, device="cpu")
 
     result = dreamy_boi.render(
         layers=[model.Mixed_6a], iters=iters, image_parameter=image_param
     )
@@ -51,15 +51,15 @@
         os.remove(filename)
 
 
 @pytest.mark.parametrize("iters", [1, 2, 10, 20])
 @pytest.mark.parametrize("batch_size", [1, 2, 5])
 def test_batched_auto_image_param_with_custom_func(iters, batch_size):
 
-    model = models.inception_v3(pretrained=True)
+    model = models.inception_v3(weights='DEFAULT')
     dreamy_boi = Dreamer(model=model, device="cpu", quiet=False)
 
     image_param = BatchedAutoImageParam(batch_size=batch_size, device="cpu")
 
     objective_functions = []
     for i in range(batch_size):
         objective_functions.append(make_custom_func(layer_number=0, channel_number=i))
```

### Comparing `torch-dreams-3.0.0/torch_dreams/transforms.py` & `torch-dreams-4.0.0/torch_dreams/transforms.py`

 * *Files identical despite different names*

### Comparing `torch-dreams-3.0.0/torch_dreams/utils.py` & `torch-dreams-4.0.0/torch_dreams/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,33 @@
 from torch import tensor
 from torchvision import transforms
 
 from .image_transforms import resize_4d_tensor_by_size
 from .error_handlers import PytorchVersionError
 from .constants import Constants
 
+def check_pytorch_version():
+    '''
+    does not raise error if torch >=1.8.x
+    else raises PytorchVersionError
+    '''
+
+    version = torch.__version__.split(".")
+    main_version = int(version[0])
+
+    if main_version < 1:
+        PytorchVersionError(version=torch.__version__)
+    elif main_version == 1:
+        sub_version = int(version[1])
+        if sub_version < 8:
+            PytorchVersionError(version=torch.__version__)
+        else:
+            pass
+    else:
+        pass
 
 def init_image_param(height, width, sd=0.01, device="cuda"):
     """Initializes an image parameter in the frequency domain
 
     Args:
         height (int): height of image
         width (int): width of image
@@ -72,20 +91,15 @@
     image_parameter = torch.complex(image_parameter[..., 0], image_parameter[..., 1])
     t = scale * image_parameter
 
     version = torch.__version__.split(".")[:2]
     main_version = int(version[0])
     sub_version = int(version[1])
 
-    if (
-        main_version >= 1 and sub_version >= 8
-    ):  ## if torch.__version__ is greater than 1.8
-        t = torch.fft.irfft2(t, s=(height, width), norm="ortho")
-    else:
-        raise PytorchVersionError(version=torch.__version__)
+    t = torch.fft.irfft2(t, s=(height, width), norm="ortho")
 
     return t
 
 
 def lucid_colorspace_to_rgb(t, device="cuda"):
 
     t_flat = t.permute(0, 2, 3, 1)
@@ -145,15 +159,10 @@
     )
     t = scale * image_parameter
 
     version = torch.__version__.split(".")[:2]
     main_version = int(version[0])
     sub_version = int(version[1])
 
-    if (
-        main_version >= 1 and sub_version >= 8
-    ):  ## if torch.__version__ is greater than 1.8
-        t = torch.fft.irfft2(t, s=(height, width), norm="ortho")
-    else:
-        raise PytorchVersionError(version=torch.__version__)
-
+    t = torch.fft.irfft2(t, s=(height, width), norm="ortho")
+    
     return t
```

### Comparing `torch-dreams-3.0.0/torch_dreams.egg-info/PKG-INFO` & `torch-dreams-4.0.0/torch_dreams.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,472 +1,471 @@
 Metadata-Version: 2.1
 Name: torch-dreams
-Version: 3.0.0
+Version: 4.0.0
 Summary: Making neural networks more interpretable, for research and art
 Home-page: https://github.com/Mayukhdeb/torch-dreams
 Author: Mayukh Deb
 Author-email: mayukhmainak2000@gmail.com
-License: UNKNOWN
-Description: # Torch-Dreams
-        Making neural networks more interpretable, for research and art. 
-        
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb)
-        [![build](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml/badge.svg)](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml)
-        [![codecov](https://codecov.io/gh/Mayukhdeb/torch-dreams/branch/master/graph/badge.svg?token=krU6dNleoJ)](https://codecov.io/gh/Mayukhdeb/torch-dreams)
-        <!-- [![](https://img.shields.io/twitter/url?label=Docs&style=flat-square&url=https%3A%2F%2Fapp.gitbook.com%2F%40mayukh09%2Fs%2Ftorch-dreams%2F)](https://app.gitbook.com/@mayukh09/s/torch-dreams/) -->
-        
-        
-        <img src = "https://github.com/Mayukhdeb/torch-dreams/blob/master/images/banner_segmentation_model.png?raw=true">
-        
-        ```
-        pip install torch-dreams 
-        ```
-        
-        ## Contents:
-        
-        * [Minimal example](https://github.com/Mayukhdeb/torch-dreams#minimal-example)
-        * [Not so minimal example](https://github.com/Mayukhdeb/torch-dreams#not-so-minimal-example)
-        * [Visualizing individual channels with `custom_func`](https://github.com/Mayukhdeb/torch-dreams#visualizing-individual-channels-with-custom_func)
-        * [Caricatures](https://github.com/Mayukhdeb/torch-dreams#caricatures)
-        * [Visualize features from multiple models simultaneously](https://github.com/Mayukhdeb/torch-dreams#visualize-features-from-multiple-models-simultaneously)
-        * [Use custom transforms](https://github.com/Mayukhdeb/torch-dreams#using-custom-transforms)
-        * [Feedback loops](https://github.com/Mayukhdeb/torch-dreams#you-can-also-use-outputs-of-one-render-as-the-input-of-another-to-create-feedback-loops)
-        * [Custom images](https://github.com/Mayukhdeb/torch-dreams#using-custom-images)
-        * [Working on models with different image normalizations](https://github.com/Mayukhdeb/torch-dreams#working-on-models-with-different-image-normalizations)
-        * [Masked image parametrs](https://github.com/Mayukhdeb/torch-dreams#masked-image-parameters)
-        * [Other conveniences](https://github.com/Mayukhdeb/torch-dreams#other-conveniences)
-        * [Development](https://github.com/Mayukhdeb/torch-dreams#development)
-        
-        ## Minimal example
-        > Make sure you also check out the [quick start colab notebook](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb) 
-        
-        
-        ```python
-        import matplotlib.pyplot as plt
-        import torchvision.models as models
-        from torch_dreams import Dreamer
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device = 'cuda')
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_5b],
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Not so minimal example
-        ```python
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device = 'cuda', quiet = False)
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_5b],
-            width = 256,
-            height = 256,
-            iters = 150,
-            lr = 9e-3,
-            rotate_degrees = 15,
-            scale_max = 1.2,
-            scale_min =  0.5,
-            translate_x = 0.2,
-            translate_y = 0.2,
-            custom_func = None,
-            weight_decay = 1e-2,
-            grad_clip = 1.,
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Visualizing individual channels with `custom_func`
-        
-        ```python
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device = 'cuda')
-        
-        layers_to_use = [model.Mixed_6b.branch1x1.conv]
-        
-        def make_custom_func(layer_number = 0, channel_number= 0): 
-            def custom_func(layer_outputs):
-                loss = layer_outputs[layer_number][channel_number].mean()
-                return -loss
-            return custom_func
-        
-        my_custom_func = make_custom_func(layer_number= 0, channel_number = 119)
-        
-        image_param = dreamy_boi.render(
-            layers = layers_to_use,
-            custom_func = my_custom_func,
-        )
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Batched generation for large scale experiments
-        
-        The `BatchedAutoImageParam` paired with the `BatchedObjective` can be used to generate multiple feature visualizations in parallel. This takes up more memory based on the batch size, but is also faster than generating one visualization at a time.
-        
-        ```python
-        from torch_dreams import Dreamer
-        import torchvision.models as models
-        from torch_dreams.batched_objective import BatchedObjective
-        from torch_dreams.batched_image_param import BatchedAutoImageParam
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model, device="cuda")
-        
-        ## specify list of neuron indices to visualize
-        batch_neuron_indices = [i for i in range(10,20)]
-        
-        ## set up a batch of trainable image parameters
-        bap = BatchedAutoImageParam(
-            batch_size=len(batch_neuron_indices), 
-            width=256, 
-            height=256, 
-            standard_deviation=0.01
-        )
-        
-        ## objective generator for each neuron
-        def make_custom_func(layer_number=0, channel_number=0):
-            def custom_func(layer_outputs):
-                loss = layer_outputs[layer_number][channel_number].norm()
-                return -loss
-        
-            return custom_func
-        
-        ## prepare objective functions for each neuron index
-        batched_objective = BatchedObjective(
-            objectives=[make_custom_func(channel_number=i) for i in batch_neuron_indices]
-        )
-        
-        ## render activation maximization signals
-        result_batch = dreamy_boi.render(
-            layers=[model.Mixed_5b],
-            image_parameter=bap,
-            iters=120,
-            custom_func=batched_objective,
-        )
-        
-        ## save results in a folder
-        for i in batch_neuron_indices:
-            result_batch[batch_neuron_indices.index(i)].save(f"results/{i}.jpg")
-        ```
-        
-        ## Caricatures
-        
-        Caricatures create a new image that has a similar but more extreme activation pattern to the input image at a given layer (or multiple layers at a time). It's inspired from [this issue](https://github.com/tensorflow/lucid/issues/121)
-        
-        <img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/caricature.png" width = "70%">
-        
-        In this case, let's use googlenet 
-        
-        ```python
-        model = models.googlenet(pretrained = True)
-        dreamy_boi = Dreamer(model = model, quiet= False, device= 'cuda')
-        
-        image_param = dreamy_boi.caricature(
-            input_tensor = image_tensor, 
-            layers = [model.inception4c],   ## feel free to append more layers for more interesting caricatures 
-            power= 1.2,                     ## higher -> more "exaggerated" features
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        ## Visualize features from multiple models simultaneously
-        
-        First, let's pick 2 models and specify which layers we'd want to work with
-        
-        ```python
-        from torch_dreams.model_bunch import ModelBunch
-        
-        bunch = ModelBunch(
-            model_dict = {
-                'inception': models.inception_v3(pretrained=True).eval(),
-                'resnet':    models.resnet18(pretrained= True).eval()
-            }
-        )
-        
-        layers_to_use = [
-                    bunch.model_dict['inception'].Mixed_6a,
-                    bunch.model_dict['resnet'].layer2[0].conv1
-                ]
-        
-        dreamy_boi = Dreamer(model = bunch, quiet= False, device= 'cuda')
-        ```
-        
-        Then define a `custom_func` which determines which exact activations of the models we have to optimize
-        
-        ```python
-        def custom_func(layer_outputs):
-            loss =   layer_outputs[0].mean()*2.0 + layer_outputs[1][89].mean() 
-            return -loss
-        ```
-        
-        Run the optimization
-        
-        ```python
-        image_param = dreamy_boi.render(
-            layers = layers_to_use,
-            custom_func= custom_func,
-            iters= 100
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        
-        ## Using custom transforms:
-        
-        ```python
-        import torchvision.transforms as transforms
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
-        
-        my_transforms = transforms.Compose([
-            transforms.RandomAffine(degrees = 10, translate = (0.5,0.5)),
-            transforms.RandomHorizontalFlip(p = 0.3)
-        ])
-        
-        dreamy_boi.set_custom_transforms(transforms = my_transforms)
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_5b],
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## You can also use outputs of one `render()` as the input of another to create feedback loops.
-        
-        ```python
-        import matplotlib.pyplot as plt
-        import torchvision.models as models
-        from torch_dreams import Dreamer
-        
-        model = models.inception_v3(pretrained=True)
-        dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
-        
-        image_param = dreamy_boi.render(
-            layers = [model.Mixed_6c],
-        )
-        
-        image_param = dreamy_boi.render(
-            image_parameter= image_param,
-            layers = [model.Mixed_5b],
-            iters = 20
-        )
-        
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        ## Using custom images
-        
-        Note that you might have to use smaller values for certain hyperparameters like `lr` and `grad_clip`.
-        
-        ```python
-        from torch_dreams.custom_image_param import CustomImageParam
-        param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cuda')  ## image could either be a filename or a torch.tensor of shape NCHW
-        
-        image_param = dreamy_boi.render(
-            image_parameter= param,
-            layers = [model.Mixed_6c],
-            lr = 2e-4,
-            grad_clip = 0.1,
-            weight_decay= 1e-1,
-            iters = 120
-        )
-        ```
-        
-        ## Working on models with different image normalizations
-        
-        `torch-dreams` generally works with models trained on images normalized with imagenet `mean` and `std`, but that can be easily overriden to support any other normalization. For example, if you have a model with `mean = [0.5, 0.5, 0.5]` and `std = [0.5, 0.5, 0.5]`: 
-        
-        ```python 
-        t = torchvision.transforms.Normalize(
-                        mean = [0.5, 0.5, 0.5],
-                        std =  [0.5, 0.5, 0.5]
-                    )
-        
-        dreamy_boi.set_custom_normalization(normalization_transform = t) ## normalization_transform could be any instance of torch.nn.Module
-        ```
-        
-        ## Masked Image parameters
-        
-        Can be used to optimize only certain parts of the image using a mask whose values are clipped between `[0,1]`.
-        
-        <img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/masked_param.png" width = "80%">
-        
-        Here's an example with a vertical gradient 
-        
-        ```python 
-        from torch_dreams.masked_image_param import MaskedImageParam
-        
-        mask = torch.ones(1,1,512,512)
-        
-        for i in range(0, 512, 1):  ## vertical gradient
-            mask[:,:,i,:] = (i/512)
-        
-        param = MaskedImageParam(
-            image= 'images/sample_small.jpg',  ## optional
-            mask_tensor = mask,
-            device = 'cuda'
-        )
-        
-        param = dreamy_boi.render(
-            layers = [model.inception4c],
-            image_parameter= param,
-            lr = 1e-4,
-            grad_clip= 0.1,
-            weight_decay= 1e-1,
-            iters= 200,
-        )
-        
-        param.save('masked_param_output.jpg')
-        ```
-        
-        It's also possible to update the mask on the fly with `param.update_mask(some_mask)`
-        
-        ```python
-        
-        param.update_mask(mask = torch.flip(mask, dims = (2,)))
-        
-        param = dreamy_boi.render(
-            layers = [model.inception4a],
-            image_parameter= param,
-            lr = 1e-4,
-            grad_clip= 0.1,
-            weight_decay= 1e-1,
-            iters= 200,
-        )
-        
-        param.save('masked_param_output_2.jpg')
-        ```
-        
-        
-        ## Other conveniences 
-        
-        The following methods are handy for an [`auto_image_param`](https://github.com/Mayukhdeb/torch-dreams/blob/master/torch_dreams/auto_image_param.py) instance:
-        
-        1. Saving outputs as images:
-        
-        ```python
-        image_param.save('output.jpg')
-        ```
-        
-        2. Torch Tensor of dimensions `(height, width, color_channels)`
-        
-        ```python
-        torch_image = image_param.to_hwc_tensor(device = 'cpu')
-        ```
-        
-        3. Torch Tensor of dimensions `(color_channels, height, width)`
-        
-        ```python
-        torch_image_chw = image_param.to_chw_tensor(device = 'cpu')
-        ```
-        
-        4. Displaying outputs on matplotlib. 
-        
-        ```python
-        plt.imshow(image_param)
-        plt.show()
-        ```
-        
-        5. For instances of `custom_image_param`, you can set any NCHW tensor as the image parameter: 
-        
-        ```python
-        image_tensor = image_param.to_nchw_tensor()
-        
-        ## do some stuff with image_tensor
-        t = transforms.Compose([
-            transforms.RandomRotation(5)
-        ])
-        transformed_image_tensor = t(image_tensor) 
-        
-        image_param.set_param(tensor = transformed_image_tensor)
-        ```
-        
-        ## Args for `render()`
-        
-        * `layers` (`iterable`): List of the layers of model(s)'s layers to work on. `[model.layer1, model.layer2...]`
-        * `image_parameter` (`auto_image_param`, optional): Instance of `torch_dreams.auto_image_param.auto_image_param`
-        
-        * `width` (`int`, optional): Width of image to be optimized 
-        * `height` (`int`, optional): Height of image to be optimized 
-        * `iters` (`int`, optional): Number of iterations, higher -> stronger visualization
-        * `lr` (`float`, optional): Learning rate
-        * `rotate_degrees` (`int`, optional): Max rotation in default transforms
-        * `scale_max` (`float`, optional): Max image size factor. Defaults to 1.1.
-        * `scale_min` (`float`, optional): Minimum image size factor. Defaults to 0.5.
-        * `translate_x` (`float`, optional): Maximum translation factor in x direction
-        * `translate_y` (`float`, optional): Maximum translation factor in y direction
-        * `custom_func` (`function`, optional): Can be used to define custom optimiziation conditions to `render()`. Defaults to None.
-        * `weight_decay` (`float`, optional): Weight decay for default optimizer. Helps prevent high frequency noise. Defaults to 0.
-        * `grad_clip` (`float`, optional): Maximum value of the norm of gradient. Defaults to 1.
-        
-        ## Args for `Dreamer.__init__()`
-         * `model` (`nn.Module` or  `torch_dreams.model_bunch.Modelbunch`): Almost any PyTorch model which was trained on imagenet `mean` and `std`, and supports variable sized images as inputs. You can pass multiple models into this argument as a `torch_dreams.model_bunch.Modelbunch` instance.
-         * `quiet` (`bool`): Set to `True` if you want to disable any progress bars
-         * `device` (`str`): `cuda` or `cpu` depending on your runtime 
-        
-         ## Development
-        
-        1. Clone the repo and navigate into the folder
-        ```
-        git clone git@github.com:Mayukhdeb/torch-dreams.git
-        cd torch-dreams/
-        ```
-        
-        2. Install dependencies
-        ```
-        pip install -r requirements.txt
-        ```
-        
-        3. Install `torch-dreams` as an editable module
-        ```
-        python3 setup.py develop
-        ```
-        
-        ## Citation
-        ```
-        @misc{mayukhdebtorchdreams,
-          title={Feature Visualization library for PyTorch},
-          author={Mayukh Deb},
-          year={2021},
-          publisher={GitHub},
-          howpublished={\url{https://github.com/Mayukhdeb/torch-dreams}},
-        }
-        ```
-        
-        ## Acknowledgements
-        
-        * [amFOSS](https://amfoss.in/)
-        * [Gene Kogan](https://github.com/genekogan) 
-        
-        ## Recommended Reading 
-        
-        * [Feature Visualization](https://distill.pub/2017/feature-visualization/)
-        * [Google AI blog on Deepdreams](https://ai.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)
-        
 Keywords: PyTorch,machine learning,neural networks,convolutional neural networks,feature visualization,optimization
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Torch-Dreams
+Making neural networks more interpretable, for research and art. 
+
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb)
+[![build](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml/badge.svg)](https://github.com/Mayukhdeb/torch-dreams/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/Mayukhdeb/torch-dreams/branch/master/graph/badge.svg?token=krU6dNleoJ)](https://codecov.io/gh/Mayukhdeb/torch-dreams)
+<!-- [![](https://img.shields.io/twitter/url?label=Docs&style=flat-square&url=https%3A%2F%2Fapp.gitbook.com%2F%40mayukh09%2Fs%2Ftorch-dreams%2F)](https://app.gitbook.com/@mayukh09/s/torch-dreams/) -->
+
+
+<img src = "https://github.com/Mayukhdeb/torch-dreams/blob/master/images/banner_segmentation_model.png?raw=true">
+
+```
+pip install torch-dreams 
+```
+
+## Contents:
+
+* [Minimal example](https://github.com/Mayukhdeb/torch-dreams#minimal-example)
+* [Not so minimal example](https://github.com/Mayukhdeb/torch-dreams#not-so-minimal-example)
+* [Visualizing individual channels with `custom_func`](https://github.com/Mayukhdeb/torch-dreams#visualizing-individual-channels-with-custom_func)
+* [Caricatures](https://github.com/Mayukhdeb/torch-dreams#caricatures)
+* [Visualize features from multiple models simultaneously](https://github.com/Mayukhdeb/torch-dreams#visualize-features-from-multiple-models-simultaneously)
+* [Use custom transforms](https://github.com/Mayukhdeb/torch-dreams#using-custom-transforms)
+* [Feedback loops](https://github.com/Mayukhdeb/torch-dreams#you-can-also-use-outputs-of-one-render-as-the-input-of-another-to-create-feedback-loops)
+* [Custom images](https://github.com/Mayukhdeb/torch-dreams#using-custom-images)
+* [Working on models with different image normalizations](https://github.com/Mayukhdeb/torch-dreams#working-on-models-with-different-image-normalizations)
+* [Masked image parametrs](https://github.com/Mayukhdeb/torch-dreams#masked-image-parameters)
+* [Other conveniences](https://github.com/Mayukhdeb/torch-dreams#other-conveniences)
+* [Development](https://github.com/Mayukhdeb/torch-dreams#development)
+
+## Minimal example
+> Make sure you also check out the [quick start colab notebook](https://colab.research.google.com/github/Mayukhdeb/torch-dreams-notebooks/blob/main/docs_notebooks/hello_torch_dreams.ipynb) 
+
+
+```python
+import matplotlib.pyplot as plt
+import torchvision.models as models
+from torch_dreams import Dreamer
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device = 'cuda')
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_5b],
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## Not so minimal example
+```python
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device = 'cuda', quiet = False)
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_5b],
+    width = 256,
+    height = 256,
+    iters = 150,
+    lr = 9e-3,
+    rotate_degrees = 15,
+    scale_max = 1.2,
+    scale_min =  0.5,
+    translate_x = 0.2,
+    translate_y = 0.2,
+    custom_func = None,
+    weight_decay = 1e-2,
+    grad_clip = 1.,
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## Visualizing individual channels with `custom_func`
+
+```python
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device = 'cuda')
+
+layers_to_use = [model.Mixed_6b.branch1x1.conv]
+
+def make_custom_func(layer_number = 0, channel_number= 0): 
+    def custom_func(layer_outputs):
+        loss = layer_outputs[layer_number][:, channel_number].mean()
+        return -loss
+    return custom_func
+
+my_custom_func = make_custom_func(layer_number= 0, channel_number = 119)
+
+image_param = dreamy_boi.render(
+    layers = layers_to_use,
+    custom_func = my_custom_func,
+)
+plt.imshow(image_param)
+plt.show()
+```
+
+## Batched generation for large scale experiments
+
+The `BatchedAutoImageParam` paired with the `BatchedObjective` can be used to generate multiple feature visualizations in parallel. This takes up more memory based on the batch size, but is also faster than generating one visualization at a time.
+
+```python
+from torch_dreams import Dreamer
+import torchvision.models as models
+from torch_dreams.batched_objective import BatchedObjective
+from torch_dreams.batched_image_param import BatchedAutoImageParam
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model, device="cuda")
+
+## specify list of neuron indices to visualize
+batch_neuron_indices = [i for i in range(10,20)]
+
+## set up a batch of trainable image parameters
+bap = BatchedAutoImageParam(
+    batch_size=len(batch_neuron_indices), 
+    width=256, 
+    height=256, 
+    standard_deviation=0.01
+)
+
+## objective generator for each neuron
+def make_custom_func(layer_number=0, channel_number=0):
+    def custom_func(layer_outputs):
+        loss = layer_outputs[layer_number][:, channel_number].norm()
+        return -loss
+
+    return custom_func
+
+## prepare objective functions for each neuron index
+batched_objective = BatchedObjective(
+    objectives=[make_custom_func(channel_number=i) for i in batch_neuron_indices]
+)
+
+## render activation maximization signals
+result_batch = dreamy_boi.render(
+    layers=[model.Mixed_5b],
+    image_parameter=bap,
+    iters=120,
+    custom_func=batched_objective,
+)
+
+## save results in a folder
+for i in batch_neuron_indices:
+    result_batch[batch_neuron_indices.index(i)].save(f"results/{i}.jpg")
+```
+
+## Caricatures
+
+Caricatures create a new image that has a similar but more extreme activation pattern to the input image at a given layer (or multiple layers at a time). It's inspired from [this issue](https://github.com/tensorflow/lucid/issues/121)
+
+<img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/caricature.png" width = "70%">
+
+In this case, let's use googlenet 
+
+```python
+model = models.googlenet(pretrained = True)
+dreamy_boi = Dreamer(model = model, quiet= False, device= 'cuda')
+
+image_param = dreamy_boi.caricature(
+    input_tensor = image_tensor, 
+    layers = [model.inception4c],   ## feel free to append more layers for more interesting caricatures 
+    power= 1.2,                     ## higher -> more "exaggerated" features
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+## Visualize features from multiple models simultaneously
+
+First, let's pick 2 models and specify which layers we'd want to work with
+
+```python
+from torch_dreams.model_bunch import ModelBunch
+
+bunch = ModelBunch(
+    model_dict = {
+        'inception': models.inception_v3(pretrained=True).eval(),
+        'resnet':    models.resnet18(pretrained= True).eval()
+    }
+)
+
+layers_to_use = [
+            bunch.model_dict['inception'].Mixed_6a,
+            bunch.model_dict['resnet'].layer2[0].conv1
+        ]
+
+dreamy_boi = Dreamer(model = bunch, quiet= False, device= 'cuda')
+```
+
+Then define a `custom_func` which determines which exact activations of the models we have to optimize
+
+```python
+def custom_func(layer_outputs):
+    loss =   layer_outputs[0].mean()*2.0 + layer_outputs[1][:, 89].mean() 
+    return -loss
+```
+
+Run the optimization
+
+```python
+image_param = dreamy_boi.render(
+    layers = layers_to_use,
+    custom_func= custom_func,
+    iters= 100
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+
+## Using custom transforms:
+
+```python
+import torchvision.transforms as transforms
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
+
+my_transforms = transforms.Compose([
+    transforms.RandomAffine(degrees = 10, translate = (0.5,0.5)),
+    transforms.RandomHorizontalFlip(p = 0.3)
+])
+
+dreamy_boi.set_custom_transforms(transforms = my_transforms)
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_5b],
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## You can also use outputs of one `render()` as the input of another to create feedback loops.
+
+```python
+import matplotlib.pyplot as plt
+import torchvision.models as models
+from torch_dreams import Dreamer
+
+model = models.inception_v3(pretrained=True)
+dreamy_boi = Dreamer(model,  device = 'cuda', quiet =  False)
+
+image_param = dreamy_boi.render(
+    layers = [model.Mixed_6c],
+)
+
+image_param = dreamy_boi.render(
+    image_parameter= image_param,
+    layers = [model.Mixed_5b],
+    iters = 20
+)
+
+plt.imshow(image_param)
+plt.show()
+```
+
+## Using custom images
+
+Note that you might have to use smaller values for certain hyperparameters like `lr` and `grad_clip`.
+
+```python
+from torch_dreams.custom_image_param import CustomImageParam
+param = CustomImageParam(image = 'images/sample_small.jpg', device= 'cuda')  ## image could either be a filename or a torch.tensor of shape NCHW
+
+image_param = dreamy_boi.render(
+    image_parameter= param,
+    layers = [model.Mixed_6c],
+    lr = 2e-4,
+    grad_clip = 0.1,
+    weight_decay= 1e-1,
+    iters = 120
+)
+```
+
+## Working on models with different image normalizations
+
+`torch-dreams` generally works with models trained on images normalized with imagenet `mean` and `std`, but that can be easily overriden to support any other normalization. For example, if you have a model with `mean = [0.5, 0.5, 0.5]` and `std = [0.5, 0.5, 0.5]`: 
+
+```python 
+t = torchvision.transforms.Normalize(
+                mean = [0.5, 0.5, 0.5],
+                std =  [0.5, 0.5, 0.5]
+            )
+
+dreamy_boi.set_custom_normalization(normalization_transform = t) ## normalization_transform could be any instance of torch.nn.Module
+```
+
+## Masked Image parameters
+
+Can be used to optimize only certain parts of the image using a mask whose values are clipped between `[0,1]`.
+
+<img src = "https://raw.githubusercontent.com/Mayukhdeb/torch-dreams/master/images/masked_param.png" width = "80%">
+
+Here's an example with a vertical gradient 
+
+```python 
+from torch_dreams.masked_image_param import MaskedImageParam
+
+mask = torch.ones(1,1,512,512)
+
+for i in range(0, 512, 1):  ## vertical gradient
+    mask[:,:,i,:] = (i/512)
+
+param = MaskedImageParam(
+    image= 'images/sample_small.jpg',  ## optional
+    mask_tensor = mask,
+    device = 'cuda'
+)
+
+param = dreamy_boi.render(
+    layers = [model.inception4c],
+    image_parameter= param,
+    lr = 1e-4,
+    grad_clip= 0.1,
+    weight_decay= 1e-1,
+    iters= 200,
+)
+
+param.save('masked_param_output.jpg')
+```
+
+It's also possible to update the mask on the fly with `param.update_mask(some_mask)`
+
+```python
+
+param.update_mask(mask = torch.flip(mask, dims = (2,)))
+
+param = dreamy_boi.render(
+    layers = [model.inception4a],
+    image_parameter= param,
+    lr = 1e-4,
+    grad_clip= 0.1,
+    weight_decay= 1e-1,
+    iters= 200,
+)
+
+param.save('masked_param_output_2.jpg')
+```
+
+
+## Other conveniences 
+
+The following methods are handy for an [`auto_image_param`](https://github.com/Mayukhdeb/torch-dreams/blob/master/torch_dreams/auto_image_param.py) instance:
+
+1. Saving outputs as images:
+
+```python
+image_param.save('output.jpg')
+```
+
+2. Torch Tensor of dimensions `(height, width, color_channels)`
+
+```python
+torch_image = image_param.to_hwc_tensor(device = 'cpu')
+```
+
+3. Torch Tensor of dimensions `(color_channels, height, width)`
+
+```python
+torch_image_chw = image_param.to_chw_tensor(device = 'cpu')
+```
+
+4. Displaying outputs on matplotlib. 
+
+```python
+plt.imshow(image_param)
+plt.show()
+```
+
+5. For instances of `custom_image_param`, you can set any NCHW tensor as the image parameter: 
+
+```python
+image_tensor = image_param.to_nchw_tensor()
+
+## do some stuff with image_tensor
+t = transforms.Compose([
+    transforms.RandomRotation(5)
+])
+transformed_image_tensor = t(image_tensor) 
+
+image_param.set_param(tensor = transformed_image_tensor)
+```
+
+## Args for `render()`
+
+* `layers` (`iterable`): List of the layers of model(s)'s layers to work on. `[model.layer1, model.layer2...]`
+* `image_parameter` (`auto_image_param`, optional): Instance of `torch_dreams.auto_image_param.auto_image_param`
+
+* `width` (`int`, optional): Width of image to be optimized 
+* `height` (`int`, optional): Height of image to be optimized 
+* `iters` (`int`, optional): Number of iterations, higher -> stronger visualization
+* `lr` (`float`, optional): Learning rate
+* `rotate_degrees` (`int`, optional): Max rotation in default transforms
+* `scale_max` (`float`, optional): Max image size factor. Defaults to 1.1.
+* `scale_min` (`float`, optional): Minimum image size factor. Defaults to 0.5.
+* `translate_x` (`float`, optional): Maximum translation factor in x direction
+* `translate_y` (`float`, optional): Maximum translation factor in y direction
+* `custom_func` (`function`, optional): Can be used to define custom optimiziation conditions to `render()`. Defaults to None.
+* `weight_decay` (`float`, optional): Weight decay for default optimizer. Helps prevent high frequency noise. Defaults to 0.
+* `grad_clip` (`float`, optional): Maximum value of the norm of gradient. Defaults to 1.
+
+## Args for `Dreamer.__init__()`
+ * `model` (`nn.Module` or  `torch_dreams.model_bunch.Modelbunch`): Almost any PyTorch model which was trained on imagenet `mean` and `std`, and supports variable sized images as inputs. You can pass multiple models into this argument as a `torch_dreams.model_bunch.Modelbunch` instance.
+ * `quiet` (`bool`): Set to `True` if you want to disable any progress bars
+ * `device` (`str`): `cuda` or `cpu` depending on your runtime 
+
+ ## Development
+
+1. Clone the repo and navigate into the folder
+```
+git clone git@github.com:Mayukhdeb/torch-dreams.git
+cd torch-dreams/
+```
+
+2. Install dependencies
+```
+pip install -r requirements.txt
+```
+
+3. Install `torch-dreams` as an editable module
+```
+python3 setup.py develop
+```
+
+## Citation
+```
+@misc{mayukhdebtorchdreams,
+  title={Feature Visualization library for PyTorch},
+  author={Mayukh Deb},
+  year={2021},
+  publisher={GitHub},
+  howpublished={\url{https://github.com/Mayukhdeb/torch-dreams}},
+}
+```
+
+## Acknowledgements
+
+* [amFOSS](https://amfoss.in/)
+* [Gene Kogan](https://github.com/genekogan) 
+
+## Recommended Reading 
+
+* [Feature Visualization](https://distill.pub/2017/feature-visualization/)
+* [Google AI blog on Deepdreams](https://ai.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)
```

### Comparing `torch-dreams-3.0.0/torch_dreams.egg-info/SOURCES.txt` & `torch-dreams-4.0.0/torch_dreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

