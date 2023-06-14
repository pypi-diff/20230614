# Comparing `tmp/vocex-0.1.6.tar.gz` & `tmp/vocex-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocex-0.1.6.tar", last modified: Fri Jun  9 11:25:58 2023, max compression
+gzip compressed data, was "vocex-0.1.7.tar", last modified: Wed Jun 14 00:41:03 2023, max compression
```

## Comparing `vocex-0.1.6.tar` & `vocex-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)        0 2023-06-09 11:25:58.824476 vocex-0.1.6/
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)      227 2023-06-09 11:25:58.824476 vocex-0.1.6/PKG-INFO
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)        8 2023-06-08 08:33:20.000000 vocex-0.1.6/README.md
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)       38 2023-06-09 11:25:58.824476 vocex-0.1.6/setup.cfg
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)      470 2023-06-09 11:22:42.000000 vocex-0.1.6/setup.py
-drwxrwxr-x   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)        0 2023-06-09 11:25:58.820475 vocex-0.1.6/test/
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)       30 2023-06-08 17:35:48.000000 vocex-0.1.6/test/__init__.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)     9582 2023-06-09 11:23:26.000000 vocex-0.1.6/test/test.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)     3033 2023-06-08 17:34:50.000000 vocex-0.1.6/test/wada_snr.py
-drwxrwxr-x   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)        0 2023-06-09 11:25:58.820475 vocex-0.1.6/vocex/
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)    12086 2023-06-09 11:21:41.000000 vocex-0.1.6/vocex/__init__.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)     3250 2023-06-08 11:03:36.000000 vocex-0.1.6/vocex/conformer_layer.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)    10299 2023-06-08 16:45:34.000000 vocex-0.1.6/vocex/conformer_model.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)     4208 2023-06-08 08:33:21.000000 vocex-0.1.6/vocex/scaler.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)     3830 2023-06-08 08:33:21.000000 vocex-0.1.6/vocex/softdtw.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)     3377 2023-06-08 11:05:02.000000 vocex-0.1.6/vocex/transformer.py
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)     1756 2023-06-08 08:33:21.000000 vocex-0.1.6/vocex/utils.py
-drwxrwxr-x   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)        0 2023-06-09 11:25:58.824476 vocex-0.1.6/vocex.egg-info/
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)      227 2023-06-09 11:25:58.000000 vocex-0.1.6/vocex.egg-info/PKG-INFO
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)      346 2023-06-09 11:25:58.000000 vocex-0.1.6/vocex.egg-info/SOURCES.txt
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)        1 2023-06-09 11:25:58.000000 vocex-0.1.6/vocex.egg-info/dependency_links.txt
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)       60 2023-06-09 11:25:58.000000 vocex-0.1.6/vocex.egg-info/requires.txt
--rw-rw-r--   0 christoph.minixhofer  (2007) christoph.minixhofer  (2007)       11 2023-06-09 11:25:58.000000 vocex-0.1.6/vocex.egg-info/top_level.txt
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      227 2023-06-14 00:41:03.886232 vocex-0.1.7/PKG-INFO
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)        9 2023-06-11 08:34:35.000000 vocex-0.1.7/README.md
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       38 2023-06-14 00:41:03.886232 vocex-0.1.7/setup.cfg
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      470 2023-06-13 23:51:22.000000 vocex-0.1.7/setup.py
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/test/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       30 2023-06-11 08:34:35.000000 vocex-0.1.7/test/__init__.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    10149 2023-06-11 08:34:35.000000 vocex-0.1.7/test/test.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3033 2023-06-11 08:34:35.000000 vocex-0.1.7/test/wada_snr.py
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/vocex/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    18362 2023-06-13 23:52:59.000000 vocex-0.1.7/vocex/__init__.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3250 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/conformer_layer.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)    10614 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/conformer_model.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     1067 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/image_helpers.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3559 2023-06-13 13:06:09.000000 vocex-0.1.7/vocex/onnx_stft.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     4203 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/scaler.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3830 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/softdtw.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     3377 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/transformer.py
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)     1756 2023-06-13 13:05:43.000000 vocex-0.1.7/vocex/utils.py
+drwxrwxr-x   0 cdminix   (1000) cdminix   (1000)        0 2023-06-14 00:41:03.886232 vocex-0.1.7/vocex.egg-info/
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      227 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/PKG-INFO
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)      388 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/SOURCES.txt
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)        1 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/dependency_links.txt
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       60 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/requires.txt
+-rw-rw-r--   0 cdminix   (1000) cdminix   (1000)       11 2023-06-14 00:41:03.000000 vocex-0.1.7/vocex.egg-info/top_level.txt
```

### Comparing `vocex-0.1.6/test/test.py` & `vocex-0.1.7/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -229,7 +229,21 @@
 def test_numpy_array_input(setup_data_and_model):
     dataset, _, vocex = setup_data_and_model
     first_example = next(iter(dataset))
     assert vocex(np.random.randn(16000), 16000)["overall_snr"].shape == (1,)
     # no nan values in voice_activity_binary
     assert not np.isnan(vocex(np.random.randn(16000), 16000)["voice_activity_binary"]).any()
 
+def test_speaker_avatar(setup_data_and_model):
+    _, _, vocex = setup_data_and_model
+    #iter_dataset = iter(dataset)
+    #first_example = next(iter_dataset)
+    #second_example = next(iter_dataset)
+    import torchaudio
+    first_example, sr = torchaudio.load("celina_phone_example.wav")
+    result = vocex(first_example, sr, speaker_avatar=True)
+    plt.figure(figsize=(5,5))
+    plt.imshow(result["avatars"][0], aspect="auto", origin="lower")
+    plt.tight_layout()
+    plt.savefig("plots/speaker_avatar.png")
+
+    assert result["avatars"].shape == (1, 8, 8, 3)
```

### Comparing `vocex-0.1.6/test/wada_snr.py` & `vocex-0.1.7/test/wada_snr.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.6/vocex/__init__.py` & `vocex-0.1.7/vocex/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import gzip
 
 import torch
 import torchaudio.transforms as T
 from librosa.filters import mel as librosa_mel
 import numpy as np
+from torch import nn
 
 from .conformer_model import VocexModel
+from .image_helpers import QuantizeToGivenPalette, transformYIQ2RGB
+from .onnx_stft import TacotronSTFT
 
 class Vocex():
     """ 
     This is a wrapper class for the vocex model. 
     It is used to load the model and perform inference on given audio file(s).
     """
 
     @staticmethod
     def _drc(x, C=1, clip_val=1e-7):
         return torch.log(torch.clamp(x, min=clip_val) * C)
 
     @staticmethod
-    def from_pretrained(model_file, compressed=True, **postprocess_kwargs):
+    def from_pretrained(model_file, compressed=True, for_onnx=False, **postprocess_kwargs):
         """ 
         Load a pretrained model from a given .pt file.
         Also accepts huggingface model names.
         """
         if compressed:
             # decompress
             with gzip.open(model_file, "rb") as f:
                 checkpoint = torch.load(f)
         else:
             checkpoint = torch.load(model_file)
         model_args = checkpoint["model_args"]
         model = VocexModel(**model_args)
         model.load_state_dict(checkpoint["state_dict"])
-        return Vocex(model, **postprocess_kwargs)
+        return Vocex(model, for_onnx, **postprocess_kwargs)
 
     def __init__(self, model, seed=42, **postprocess_kwargs):
+        super().__init__()
         self.model = model
         self.mel_spectrogram = T.Spectrogram(
             n_fft=1024,
             win_length=1024,
             hop_length=256,
             pad=0,
             window_fn=torch.hann_window,
@@ -83,15 +87,14 @@
                 elif measure == "energy":
                     self.postprocess_kwargs[measure]["vad_threshold_min"] = 0.0
                     self.postprocess_kwargs[measure]["vad_threshold_max"] = 1.0
                 
         # set to eval mode
         self.model.eval()
         self.seed = seed
-                    
 
     def save_checkpoint(self, path, compressed=True):
         """ Save the model to a given path. """
         # get state dict
         state_dict = self.model.state_dict()
         # get model args
         model_args = self.model.hparams
@@ -140,14 +143,15 @@
                 audio = audio / 32768
             elif audio.dtype == torch.float64:
                 audio = audio.to(torch.float32)
             audio = T.Resample(sr, 22050)(audio)
         if audio.ndim == 1:
             # normalize unbatched
             audio = audio / audio.abs().max()
+            audio = audio.unsqueeze(0)
         elif audio.ndim == 2:
             # normalize batched
             audio = audio / audio.abs().max(dim=-1, keepdim=True)[0]
         elif audio.ndim == 3:
             # normalize batched and make mono
             audio = audio.mean(dim=-1)
             audio = audio / audio.abs().max(dim=-1, keepdim=True)[0]
@@ -219,26 +223,27 @@
                 measure = torch.nn.functional.pad(measure, (convolution_window_size // 2, convolution_window_size // 2), mode="reflect")
             if measure.ndim == 1:
                 # add batch dimension if necessary
                 measure = measure.unsqueeze(0)
             if measure.shape[0] == 1:
                 measure = torch.nn.functional.conv1d(measure, window, padding="same")
             else:
-                # for batch size > 0, we want to apply the convolution to each batch element separately
                 measure = torch.stack([torch.nn.functional.conv1d(m.unsqueeze(0), window, padding="same") for m in measure]).squeeze(1)
             # remove padding
             measure = measure[:, convolution_window_size // 2:-convolution_window_size // 2]
         if normalize:
             # normalize
             measure = measure / measure.abs().max(dim=-1, keepdim=True)[0]
         measure = _interpolate(measure, vad)
         return measure
 
-    def __call__(self, audio, sr=22050, return_activations=False, return_attention=False):
+    def __call__(self, audio, sr=22050, return_activations=False, return_attention=False, speaker_avatar=False):
         """ Perform inference on given audio. """
+        is_onnx = hasattr(self.model, "onnx_export") and self.model.onnx_export
+
         # preprocess
         mel = self._preprocess(audio, sr)
         # forward pass
         with torch.no_grad():
             if self.seed is not None:
                 torch.manual_seed(self.seed)
                 np.random.seed(self.seed)
@@ -246,38 +251,180 @@
 
         if return_activations:
             out["activations"] = torch.stack(out["activations"]).transpose(0, 1).cpu().numpy()
         
         if return_attention:
             out["attention"] = torch.stack(out["attention"]).transpose(0, 1).cpu().numpy()
 
-        del out["loss"]
-        del out["compound_losses"]
+        if not is_onnx:
+            del out["loss"]
+            del out["compound_losses"]
 
         # convert to numpy
-        for measure in out["measures"].keys():
-            out[measure] = out["measures"][measure].cpu().numpy()
+        if not is_onnx:
+            for measure in out["measures"].keys():
+                out["measures"][measure] = out["measures"][measure].cpu().numpy()
         # do voice activity postprocessing first
         voice_activity = None
-        if "voice_activity_binary" in out:
-            voice_activity_vals = out["voice_activity_binary"]
-            out["voice_activity_binary"] = self.postprocess(voice_activity_vals, None, **self.postprocess_kwargs["voice_activity_binary"])
-            voice_activity = out["voice_activity_binary"]
+        if "voice_activity_binary" in out["measures"] or (is_onnx and "voice_activity_binary" in self.model.measures):
+            if not is_onnx:
+                voice_activity_vals = out["measures"]["voice_activity_binary"]
+            else:
+                # use index of voice activity in self.model.measures
+                voice_activity_vals = out[self.model.measures.index("voice_activity_binary")]
+            voice_activity = self.postprocess(voice_activity_vals, None, **self.postprocess_kwargs["voice_activity_binary"])
+            if not is_onnx:
+                out["measures"]["voice_activity_binary"] = voice_activity
         # do other postprocessing
-        for measure in out["measures"].keys():
+        for measure in self.model.measures:
             if measure != "voice_activity_binary":
-                measure_vals = out["measures"][measure]
-                out[measure] = self.postprocess(measure_vals, voice_activity, **self.postprocess_kwargs[measure])
-        del out["measures"]
-        if "dvector" in out:
+                if not is_onnx:
+                    measure_vals = out["measures"][measure]
+                else:
+                    # use index of measure in self.model.measures
+                    measure_vals = out[self.model.measures.index(measure)]
+                measure_vals = self.postprocess(measure_vals, voice_activity, **self.postprocess_kwargs[measure])
+                if not is_onnx:
+                    out["measures"][measure] = measure_vals
+                else:
+                    # use index of measure in self.model.measures
+                    out[self.model.measures.index(measure)] = measure_vals
+        
+        if not is_onnx:
             out["dvector"] = out["dvector"].cpu().numpy()
-        for measure in out.keys():
-            if isinstance(out[measure], torch.Tensor):
-                out[measure] = out[measure].cpu().numpy()
-        if "snr" in out and "voice_activity_binary" in out:
-            out["overall_snr"] = (out["snr"] * out["voice_activity_binary"]).sum(axis=-1) / out["voice_activity_binary"].sum(axis=-1)
-        if "srmr" in out and "voice_activity_binary" in out:
-            va_mask = out["voice_activity_binary"] > 0.5
-            out["overall_srmr"] = (out["srmr"] * va_mask).sum(axis=-1) / va_mask.sum(axis=-1)
-            if np.isnan(out["overall_srmr"]).any():
-                out["overall_srmr"][np.isnan(out["overall_srmr"])] = out["srmr"][np.isnan(out["overall_srmr"])].mean(axis=-1)
+        if speaker_avatar:
+            from scipy import ndimage
+            import seaborn as sns
+            avatars = []
+            for dvec in out["dvector"]:
+                # convert to 8 x 8 x 2
+                dvec = dvec.reshape(8, 8, 2, 2).mean(axis=-1)
+                # normalize
+                dvec = dvec / 0.1
+                # create 8 x 8 image using the 2 channels as i and q values at y=0.5
+                # for this, we add one channel with .5 values
+                dvec = np.concatenate([np.ones_like(dvec) * 0.5, dvec], axis=-1)
+                dvec = dvec[:, :, [0, 2, 3]]
+                # move to correct range for i (-0.5957, 0.5957)
+                dvec[:, :, 1] = dvec[:, :, 1] * 0.5957
+                # move to correct range for q (-0.5226, 0.5226)
+                dvec[:, :, 2] = dvec[:, :, 2] * 0.5226
+                # convert to rgb
+                dvec = transformYIQ2RGB(dvec)
+                # scale up to 256 x 256
+                dvec = ndimage.zoom(dvec, (32, 32, 1), order=1)
+                # make symmetric
+                dvec = np.concatenate([dvec, dvec[:, ::-1]], axis=1)
+                dvec = np.concatenate([dvec, dvec[::-1]], axis=0)
+                inPalette = np.array(sns.color_palette("hls", 5))
+                dvec = QuantizeToGivenPalette(dvec, inPalette)
+                # add to list
+                avatars.append(dvec)
+            out["avatars"] = np.stack(avatars)
+
+        if not is_onnx:
+            for measure in out.keys():
+                if isinstance(out[measure], torch.Tensor):
+                    out[measure] = out[measure].cpu().numpy()
+            if "snr" in out["measures"] and "voice_activity_binary" in out["measures"]:
+                out["overall_snr"] = (out["measures"]["snr"] * out["measures"]["voice_activity_binary"]).sum(axis=-1) / out["measures"]["voice_activity_binary"].sum(axis=-1)
+            if "srmr" in out["measures"] and "voice_activity_binary" in out["measures"]:
+                va_mask = out["measures"]["voice_activity_binary"] > 0.5
+                out["overall_srmr"] = (out["measures"]["srmr"] * va_mask).sum(axis=-1) / va_mask.sum(axis=-1)
+                if np.isnan(out["overall_srmr"]).any():
+                    out["overall_srmr"][np.isnan(out["overall_srmr"])] = out["measures"]["srmr"][np.isnan(out["overall_srmr"])].mean(axis=-1)
+            if "pitch" in out["measures"] and "voice_activity_binary" in out["measures"]:
+                out["overall_pitch"] = (out["measures"]["pitch"] * out["measures"]["voice_activity_binary"]).sum(axis=-1) / out["measures"]["voice_activity_binary"].sum(axis=-1)
+            if "energy" in out["measures"] and "voice_activity_binary" in out["measures"]:
+                out["overall_energy"] = (out["measures"]["energy"] * out["measures"]["voice_activity_binary"]).sum(axis=-1) / out["measures"]["voice_activity_binary"].sum(axis=-1)
+        return out
+    
+
+class OnnxVocexWrapper(nn.Module):
+    """
+    Same as above, but with one-size-fits-all postprocessing (simple smoothing)
+    """
+    
+    def from_pretrained(model_file, compressed=True):
+        """ 
+        Load a pretrained model from a given .pt file.
+        Also accepts huggingface model names.
+        """
+        if compressed:
+            # decompress
+            with gzip.open(model_file, "rb") as f:
+                checkpoint = torch.load(f)
+        else:
+            checkpoint = torch.load(model_file)
+        model_args = checkpoint["model_args"]
+        model = VocexModel(**model_args)
+        model.load_state_dict(checkpoint["state_dict"])
+        return OnnxVocexWrapper(model)
+    
+    def __init__(self, model):
+        super().__init__()
+        self.model = model
+        self.mel_spectrogram = TacotronSTFT(
+            filter_length=1024,
+            hop_length=256,
+            win_length=1024,
+            n_mel_channels=80,
+            sampling_rate=22050,
+            mel_fmin=0,
+            mel_fmax=8000,
+        )
+        mel_basis = librosa_mel(
+            sr=22050,
+            n_fft=1024,
+            n_mels=80,
+            fmin=0,
+            fmax=8000,
+        )
+        self.mel_basis = torch.from_numpy(mel_basis).float()
+        # set to eval mode
+        self.model.eval()
+        self.model.onnx_export = True
+
+    def _preprocess(self, audio, sr=22050):
+        """ Preprocess audio, we only need to take batch size 1 into account. """
+        # convert to tensor
+        if isinstance(audio, np.ndarray):
+            audio = torch.from_numpy(audio).float()
+        # dtypes
+        if audio.dtype == torch.int16:
+            audio = audio / 32768
+        elif audio.dtype == torch.float64:
+            audio = audio.to(torch.float32)
+        # resample if necessary
+        if sr != 22050:
+            audio = T.Resample(sr, 22050)(audio)
+        audio = audio / audio.abs().max()
+        # make mono if necessary
+        if audio.ndim == 2:
+            audio = audio.mean(dim=-1)
+        # convert to spectrogram
+        mel = self.mel_spectrogram(audio.unsqueeze(0))
+        # convert to mel spectrogram
+        mel = torch.matmul(self.mel_basis, mel)
+        # dynamic range compression
+        mel = Vocex._drc(mel)
+        # transpose
+        if mel.ndim == 2:
+            # add batch dimension if necessary
+            mel = mel.unsqueeze(0)
+        mel = mel.transpose(1, 2)
+        return mel
+    
+    def forward(self, audio, sr=22050):
+        """ Perform inference on given audio. Return list instead of dict. """
+        # preprocess
+        mel = self._preprocess(audio, sr)
+        # forward pass
+        with torch.no_grad():
+            out = self.model(mel, inference=True)
+        # do simple smoothing
+        # for i, measure in enumerate(out):
+        #     if measure.ndim == 1:
+        #         # add batch dimension if necessary
+        #         measure = measure.unsqueeze(0)
+        #     out[i] = torch.nn.functional.avg_pool1d(measure.unsqueeze(1), kernel_size=10, stride=1).squeeze(1)
         return out
```

### Comparing `vocex-0.1.6/vocex/conformer_layer.py` & `vocex-0.1.7/vocex/conformer_layer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.6/vocex/conformer_model.py` & `vocex-0.1.7/vocex/conformer_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,36 +154,38 @@
 
         if return_activations:
             self.layers.return_additional_layers = list(range(self.hparams["measure_nlayers"]))
 
         if not self.scalers["mel"].is_fit:
             self.scalers["mel"].partial_fit(mel)
         x = self.scalers["mel"].transform(mel)
-        x = x + (torch.randn_like(x) * x.std() + x.mean()) * self.noise_factor
+        is_onnx = (hasattr(self, "onnx_export") and self.onnx_export)
+        if is_onnx:
+            random_noise = (torch.randn_like(x, dtype=float) * x.std() + x.mean()) * self.noise_factor
+        else:
+            random_noise = (torch.randn_like(x) * x.std() + x.mean()) * self.noise_factor
+        if is_onnx:
+            x_dtype = x.dtype
+            x = x + random_noise
+            x = x.to(x_dtype)
+        else:
+            x = x + random_noise
         out = self.in_layer(x)
-        if self.verbose:
-            print(out.mean(), "1")
         out = self.positional_encoding(out)
-        if self.verbose:
-            print(out.mean(), "2")
         res = self.layers(out, src_key_padding_mask=mel_padding_mask, need_weights=return_attention)
         if return_activations:
             activations = res["activations"]
             out_conv = res["output"]
             self.layers.return_additional_layers = None
         if return_attention:
             attention = res["attention"]
             out_conv = res["output"]
         if not return_activations and not return_attention:
             out_conv = res
-        if self.verbose:
-            print(out_conv.mean(), "3")
         out = self.linear(out_conv)
-        if self.verbose:
-            print(out.mean(), "4")
         out = out.transpose(1, 2)
 
         measure_results = {}
         measure_true = {}
         loss_dict = {}
         for i, measure in enumerate(self.measures):
             measure_out = out[:, i]
@@ -236,15 +238,15 @@
             dvector_loss = nn.L1Loss()(dvector_pred, true_dvector)
             loss_dict["dvector"] = dvector_loss
             if loss is not None:
                 loss += dvector_loss
                 loss /= 2
             else:
                 loss = dvector_loss
-        if not inference:
+        if (not inference) and not (hasattr(self, "onnx_export") and self.onnx_export):
             results = {
                 "loss": loss,
                 "compound_losses": loss_dict,
             }
             if return_activations:
                 results["activations"] = [a.detach() for a in activations]
             if return_attention:
@@ -256,14 +258,16 @@
                 if not measure.endswith("_binary"):
                     measure_results[measure] = self.scalers[measure].inverse_transform(
                         measure_results[measure]
                     )
                 else:
                     measure_results[measure] = torch.sigmoid(measure_results[measure]).detach()
             dvector_pred = self.scalers["dvector"].inverse_transform(dvector_pred)
+            if is_onnx:
+                return [measure_results[measure] for measure in self.measures] + [dvector_pred]
             results = {
                 "loss": loss,
                 "compound_losses": loss_dict,
                 "measures": measure_results,
                 "dvector": dvector_pred,
             }
             if return_activations:
```

### Comparing `vocex-0.1.6/vocex/scaler.py` & `vocex-0.1.7/vocex/scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             self.is_fit = True
 
     def transform(self, X):
         X = X - self.min + self.floor
         if self.for_tensors:
             X = X.clamp_(min=self.floor)
             if self.sqrt:
-                X = torch.sqrt(X)
+                X = X ** 0.5
             # print if any nan values
             # if torch.isnan(X).any():
             #     print("NAN values in GaussianMinMaxScaler!")
         else:
             X = np.clip(X, a_min=self.floor, a_max=None)
             if self.sqrt:
                 X = np.sqrt(X)
```

### Comparing `vocex-0.1.6/vocex/softdtw.py` & `vocex-0.1.7/vocex/softdtw.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.6/vocex/transformer.py` & `vocex-0.1.7/vocex/transformer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.6/vocex/utils.py` & `vocex-0.1.7/vocex/utils.py`

 * *Files identical despite different names*

