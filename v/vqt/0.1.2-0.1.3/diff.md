# Comparing `tmp/vqt-0.1.2.tar.gz` & `tmp/vqt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vqt-0.1.2.tar", last modified: Sun Feb 11 01:42:30 2024, max compression
+gzip compressed data, was "vqt-0.1.3.tar", last modified: Mon Apr  1 19:32:09 2024, max compression
```

## Comparing `vqt-0.1.2.tar` & `vqt-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 01:42:30.912768 vqt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34655 2024-02-11 01:42:18.000000 vqt-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-11 01:42:18.000000 vqt-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-02-11 01:42:30.912768 vqt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-02-11 01:42:18.000000 vqt-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-11 01:42:18.000000 vqt-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-11 01:42:30.912768 vqt-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-11 01:42:18.000000 vqt-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 01:42:30.912768 vqt-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-02-11 01:42:18.000000 vqt-0.1.2/tests/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 01:42:30.912768 vqt-0.1.2/vqt/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-11 01:42:18.000000 vqt-0.1.2/vqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-02-11 01:42:18.000000 vqt-0.1.2/vqt/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19921 2024-02-11 01:42:18.000000 vqt-0.1.2/vqt/vqt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 01:42:30.912768 vqt-0.1.2/vqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-02-11 01:42:30.000000 vqt-0.1.2/vqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-11 01:42:30.000000 vqt-0.1.2/vqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 01:42:30.000000 vqt-0.1.2/vqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-11 01:42:30.000000 vqt-0.1.2/vqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-11 01:42:30.000000 vqt-0.1.2/vqt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:32:09.615019 vqt-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34655 2024-04-01 19:32:06.000000 vqt-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 19:32:06.000000 vqt-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-04-01 19:32:09.615019 vqt-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-01 19:32:06.000000 vqt-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 19:32:06.000000 vqt-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 19:32:09.615019 vqt-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-01 19:32:06.000000 vqt-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:32:09.615019 vqt-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-01 19:32:06.000000 vqt-0.1.3/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:32:09.615019 vqt-0.1.3/vqt/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-01 19:32:06.000000 vqt-0.1.3/vqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-04-01 19:32:06.000000 vqt-0.1.3/vqt/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20571 2024-04-01 19:32:06.000000 vqt-0.1.3/vqt/vqt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:32:09.615019 vqt-0.1.3/vqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-04-01 19:32:09.000000 vqt-0.1.3/vqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 19:32:09.000000 vqt-0.1.3/vqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:32:09.000000 vqt-0.1.3/vqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 19:32:09.000000 vqt-0.1.3/vqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 19:32:09.000000 vqt-0.1.3/vqt.egg-info/top_level.txt
```

### Comparing `vqt-0.1.2/LICENSE.md` & `vqt-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vqt-0.1.2/PKG-INFO` & `vqt-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 Metadata-Version: 2.1
 Name: vqt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Variable Q-Transform with PyTorch backend
 Home-page: https://github.com/RichieHakim/vqt
 Author: Richard Hakim
 License: LICENSE
 Keywords: neuroscience,neuroimaging,machine learning,deep learning
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: matplotlib
 Requires-Dist: numpy
-Requires-Dist: pytest
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: torch
 Requires-Dist: pytest
 Requires-Dist: hypothesis
 
-## VQT: Variable Q-Transform
+# VQT: Variable Q-Transform
 [![PyPI
 version](https://badge.fury.io/py/vqt.svg)](https://badge.fury.io/py/vqt)
 
 Contributions are welcome! Feel free to open an issue or a pull request.
 
 ### Variable Q-Transform
 
 This is a novel python implementation of the variable Q-transform that was
-developed due to the need for a more accurate and flexible VQT for the use in
+developed due to the need for a more accurate and flexible VQT for use in
 research. It is battle-tested and has been used in a number of research
 projects. <br>
 - **Accuracy**: The approach is different in that it is a **direct
 implementation** of a spectrogram  via a Hilbert transformation at each desired
 frequency. This results in an exact computation of the spectrogram and is
 appropriate for research applications where accuracy is critical. The
 implementation seen in `librosa` and `nnAudio` uses recursive downsampling,
 which can introduce artifacts in the spectrogram under certain conditions.
 - **Flexibility**: The parameters and codebase are less complex than in other
 libraries, and the filter bank is fully customizable and exposed to the user.
 Built in plotting of the filter bank makes tuning the parameters easy and
-intuitive.
+intuitive. The main class is a PyTorch Module and the gradient function is
+maintained, so backpropagation is possible.
 - **Speed**: The backend is written using PyTorch, and allows for GPU
-acceleration. It is faster than the `librosa` implementation under most cases,
-and roughly as fast as the `nnAudio` implementation. See below section 'What to
-improve on?' for more details on how to speed it up further.
+acceleration. It is faster than the `librosa` implementation under most cases.
+Though it is typically a bit slower (1X-8X) than the `nnAudio` implementation,
+however under some conditions (low hop_length), it is as fast or faster. See
+below section 'What to improve on?' for more details on how to speed it up
+further.
 
 
-### Installation
-From PyPI: `pip install vqt`
+## Installation
+Using `pip`: 
+```
+pip install vqt
+```
 
 From source:
 ```
 git clone https://github.com/RichieHakim/vqt.git
 cd vqt
 pip install -e .
 ```
@@ -61,93 +66,113 @@
 ### Usage
 <img src="docs/media/filter_bank.png" alt="filter_bank" width="300"
 align="right"  style="margin-left: 10px"/>
 
 ```
 import vqt
 
-signal = X  ## numpy or torch array of shape (n_channels, n_samples)
+signal = torch.as_tensor(X)  ## torch Tensor of shape (n_channels, n_samples)
 
-transformer = vqt.VQT(
+my_vqt = vqt.VQT(
     Fs_sample=1000,  ## In Hz
     Q_lowF=3,  ## In periods per octave
     Q_highF=20,  ## In periods per octave
     F_min=10,  ## In Hz
     F_max=400,  ## In Hz
     n_freq_bins=55,  ## Number of frequency bins
-    DEVICE_compute='cpu',
-    return_complex=False,
-    filters=None,  ## Use custom filters
+    window_type='hann',
+    downsample_factor=8,  ## Reduce the output sample rate
+    fft_conv=True,  ## Use FFT convolution for speed
     plot_pref=False,  ## Can show the filter bank
 )
 
-spectrograms, x_axis, frequencies = transformer(signal)
+spectrograms = my_vqt(signal)
+x_axis = my_vqt.get_xAxis(n_samples=signal.shape[1])
+frequencies = my_vqt.get_freqs()
 ```
 <img src="docs/media/freqs.png" alt="freqs" width="300"  align="right"
 style="margin-left: 10px"/>
 
 #### What is the Variable Q-Transform?
 
-The Variable Q-Transform (VQT) is a time-frequency analysis tool that generates
-spectrograms, similar to the Short-time Fourier Transform (STFT). It can also be
-defined as a special case of a wavelet transform, as well as the generalization
-of the Constant Q-Transform (CQT). In fact, the VQT subsumes the CQT and STFT as
-both can be recreated using specific parameters of the VQT.
+The [Variable Q-Transform
+(VQT)](https://en.wikipedia.org/wiki/Constant-Q_transform#Variable-Q_bandwidth_calculation)
+is a time-frequency analysis tool that generates spectrograms, similar to the
+Short-time Fourier Transform (STFT). It can also be defined as a special case of
+a wavelet transform (complex Morlet), as well as the generalization of the
+[Constant Q-Transform
+(CQT)](https://en.wikipedia.org/wiki/Constant-Q_transform). In fact, the VQT
+subsumes the CQT and the STFT since both can be recreated using specific
+parameters of the VQT. <br>
+<br>
+In brief, the VQT generates a spectrogram where the frequencies are spaced
+logarithmically, and the bandwidth of the filters are tuned using two
+parameters: `Q_low` and `Q_high`, where `Q` describes the number of periods of
+the oscillatory wavelet at a particular frequency (aka the 'bandwidth'); 'low'
+refers to the lowest frequency bin, and 'high' refers to the highest frequency
+bin.
 
 #### Why use the VQT?
 
 It provides enough knobs to tune the time-frequency resolution trade-off to suit
-your needs.
+your needs. It is especially useful when time resolution is needed at lower
+frequencies.
 
 #### How exactly does this implementation differ from others?
 <img src="docs/media/freq_response.png" alt="freq_response" width="300"
 align="right"  style="margin-left: 10px"/>
 
 This function works differently than the VQT from `librosa` or `nnAudio` in that
 it does not use the recursive downsampling algorithm from [this
 paper](http://academics.wellesley.edu/Physics/brown/pubs/effalgV92P2698-P2701.pdf).
 Instead, it computes the power at each frequency using either direct- or
 FFT-convolution with a filter bank of complex oscillations, followed by a
-Hilbert transform. This results in a more accurate computation of the same
-spectrogram. The direct computation approach also results in code that is more
-flexible, easier to understand, and it has fewer constraints on the input
-parameters compared to `librosa` and `nnAudio`.
+Hilbert transform. This results in a **more accurate** computation of the same
+spectrogram without any artifacts. The direct computation approach also results
+in code that is more flexible, easier to understand, and it has fewer
+constraints on the input parameters compared to `librosa` and `nnAudio`.
 
 #### What to improve on?
 Contributions are welcome! Feel free to open an issue or a pull request.
-
-- Flexibility:
-  - `librosa` parameter mode: It would be nice to have a mode that allows for
-    the same parameters as `librosa` to be used.
-  - Make `VQT` class a full `torch.nn.Module` so that it can be used in a
-    `torch.nn.Sequential` model. Ensure backpropagation works.
-  - Make `VQT` class compatible with `torch.jit.script` and `torch.jit.trace`.
   
-- Speed:
+- Speed / Memory usage:
   - **Lossless approaches**:
-    - For the `fft_conv` approach: I believe a massive (5-100x) speedup is
-      possible using a sparse or non-uniform FFT. A direct approach where only
-      the non-zero frequencies are computed in the `fft`, product, and `ifft`
-      should get us closer to a theoretically optimal lossless approach. There
-      is an implmentation of the NUFFT in PyTorch
-      [here](https://github.com/mmuckley/torchkbnufft).
     - For the `conv1d` approach: I think it would be much faster if we cropped
       the filters to remove the blank space from the higher frequency filters.
       This would be pretty easy to implement and could give a >10x speedup.
   - **Lossy approaches**:
+    - For the `fft_conv` approach: I believe a large (5-50x) speedup is
+      possible. The lower frequency filters use only a small portion of the
+      spectrum, therefore most of the compute is spent multiplying zeros.
+      - Idea 1: Separate out filters in the filter bank whose spectra are all
+        zeros above `n_samples_downsampled`, crop the spectra above that level,
+        then use `ifft` with `n=n_samples_downsampled` to downsample the filter.
+        This would allow for a much faster convolution. For filters that can't
+        be cropped, downsampling would have to be done after the iFFT.
+      - Idea 2: using an efficient sparse or non-uniform FFT. An approach where
+        only the non-zero frequencies are computed in the `fft`, product, and
+        `ifft`. There is an implmentation of the NUFFT in PyTorch
+        [here](https://github.com/mmuckley/torchkbnufft).
+      - Idea 3: Similar to above, a log-frequency iFFT could be used to allow
+        for only the non-zero segment of the filter's spectrum to be used in the
+        convolution.
+      - Idea 4: Try using the overlap-add method.
     - Recursive downsampling: Under many circumstances (like when `Q_high` is
       not much greater than `Q_low`), recursive downsampling is fine.
       Implementing it would be nice just for completeness ([from this
       paper](http://academics.wellesley.edu/Physics/brown/pubs/effalgV92P2698-P2701.pdf))
     - For conv1d approach: Use a strided convolution.
     - For fftconv approach: Downsample using `n=n_samples_downsampled` in `ifft`
       function.
   - Non-trivial ideas that theoretically could speed things up:
     - An FFT implementation that allows for a reduced set of frequencies to be
       computed.
+- Flexibility:
+  - `librosa` parameter mode: It would be nice to have a mode that allows for
+    the same parameters as `librosa` to be used.
 
 #### Demo:
 <img src="docs/media/example_ECG.png" alt="ECG" width="500"  align="right"
 style="margin-left: 10px"/>
 
 ```
 import vqt
@@ -171,15 +196,17 @@
     downsample_factor=8,
     padding='same',
     fft_conv=True,
     take_abs=True,
     plot_pref=False,
 )
 
-specs, xaxis, freqs = my_vqt(data_ecg)
+specs = my_vqt(data_ecg)
+xaxis = my_vqt.get_xAxis(n_samples=data_ecg.shape[0])
+freqs = my_vqt.get_freqs()
 
 fig, axs = plt.subplots(nrows=2, ncols=1, sharex=True, )
 axs[0].plot(np.arange(data_ecg.shape[0]) / sample_rate, data_ecg)
 axs[0].title.set_text('Electrocardiogram')
 axs[1].pcolor(
     xaxis / sample_rate, 
     np.arange(specs[0].shape[0]), specs[0] * (freqs)[:, None],
```

### Comparing `vqt-0.1.2/README.md` & `vqt-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-## VQT: Variable Q-Transform
+# VQT: Variable Q-Transform
 [![PyPI
 version](https://badge.fury.io/py/vqt.svg)](https://badge.fury.io/py/vqt)
 
 Contributions are welcome! Feel free to open an issue or a pull request.
 
 ### Variable Q-Transform
 
 This is a novel python implementation of the variable Q-transform that was
-developed due to the need for a more accurate and flexible VQT for the use in
+developed due to the need for a more accurate and flexible VQT for use in
 research. It is battle-tested and has been used in a number of research
 projects. <br>
 - **Accuracy**: The approach is different in that it is a **direct
 implementation** of a spectrogram  via a Hilbert transformation at each desired
 frequency. This results in an exact computation of the spectrogram and is
 appropriate for research applications where accuracy is critical. The
 implementation seen in `librosa` and `nnAudio` uses recursive downsampling,
 which can introduce artifacts in the spectrogram under certain conditions.
 - **Flexibility**: The parameters and codebase are less complex than in other
 libraries, and the filter bank is fully customizable and exposed to the user.
 Built in plotting of the filter bank makes tuning the parameters easy and
-intuitive.
+intuitive. The main class is a PyTorch Module and the gradient function is
+maintained, so backpropagation is possible.
 - **Speed**: The backend is written using PyTorch, and allows for GPU
-acceleration. It is faster than the `librosa` implementation under most cases,
-and roughly as fast as the `nnAudio` implementation. See below section 'What to
-improve on?' for more details on how to speed it up further.
+acceleration. It is faster than the `librosa` implementation under most cases.
+Though it is typically a bit slower (1X-8X) than the `nnAudio` implementation,
+however under some conditions (low hop_length), it is as fast or faster. See
+below section 'What to improve on?' for more details on how to speed it up
+further.
 
 
-### Installation
-From PyPI: `pip install vqt`
+## Installation
+Using `pip`: 
+```
+pip install vqt
+```
 
 From source:
 ```
 git clone https://github.com/RichieHakim/vqt.git
 cd vqt
 pip install -e .
 ```
@@ -42,93 +48,113 @@
 ### Usage
 <img src="docs/media/filter_bank.png" alt="filter_bank" width="300"
 align="right"  style="margin-left: 10px"/>
 
 ```
 import vqt
 
-signal = X  ## numpy or torch array of shape (n_channels, n_samples)
+signal = torch.as_tensor(X)  ## torch Tensor of shape (n_channels, n_samples)
 
-transformer = vqt.VQT(
+my_vqt = vqt.VQT(
     Fs_sample=1000,  ## In Hz
     Q_lowF=3,  ## In periods per octave
     Q_highF=20,  ## In periods per octave
     F_min=10,  ## In Hz
     F_max=400,  ## In Hz
     n_freq_bins=55,  ## Number of frequency bins
-    DEVICE_compute='cpu',
-    return_complex=False,
-    filters=None,  ## Use custom filters
+    window_type='hann',
+    downsample_factor=8,  ## Reduce the output sample rate
+    fft_conv=True,  ## Use FFT convolution for speed
     plot_pref=False,  ## Can show the filter bank
 )
 
-spectrograms, x_axis, frequencies = transformer(signal)
+spectrograms = my_vqt(signal)
+x_axis = my_vqt.get_xAxis(n_samples=signal.shape[1])
+frequencies = my_vqt.get_freqs()
 ```
 <img src="docs/media/freqs.png" alt="freqs" width="300"  align="right"
 style="margin-left: 10px"/>
 
 #### What is the Variable Q-Transform?
 
-The Variable Q-Transform (VQT) is a time-frequency analysis tool that generates
-spectrograms, similar to the Short-time Fourier Transform (STFT). It can also be
-defined as a special case of a wavelet transform, as well as the generalization
-of the Constant Q-Transform (CQT). In fact, the VQT subsumes the CQT and STFT as
-both can be recreated using specific parameters of the VQT.
+The [Variable Q-Transform
+(VQT)](https://en.wikipedia.org/wiki/Constant-Q_transform#Variable-Q_bandwidth_calculation)
+is a time-frequency analysis tool that generates spectrograms, similar to the
+Short-time Fourier Transform (STFT). It can also be defined as a special case of
+a wavelet transform (complex Morlet), as well as the generalization of the
+[Constant Q-Transform
+(CQT)](https://en.wikipedia.org/wiki/Constant-Q_transform). In fact, the VQT
+subsumes the CQT and the STFT since both can be recreated using specific
+parameters of the VQT. <br>
+<br>
+In brief, the VQT generates a spectrogram where the frequencies are spaced
+logarithmically, and the bandwidth of the filters are tuned using two
+parameters: `Q_low` and `Q_high`, where `Q` describes the number of periods of
+the oscillatory wavelet at a particular frequency (aka the 'bandwidth'); 'low'
+refers to the lowest frequency bin, and 'high' refers to the highest frequency
+bin.
 
 #### Why use the VQT?
 
 It provides enough knobs to tune the time-frequency resolution trade-off to suit
-your needs.
+your needs. It is especially useful when time resolution is needed at lower
+frequencies.
 
 #### How exactly does this implementation differ from others?
 <img src="docs/media/freq_response.png" alt="freq_response" width="300"
 align="right"  style="margin-left: 10px"/>
 
 This function works differently than the VQT from `librosa` or `nnAudio` in that
 it does not use the recursive downsampling algorithm from [this
 paper](http://academics.wellesley.edu/Physics/brown/pubs/effalgV92P2698-P2701.pdf).
 Instead, it computes the power at each frequency using either direct- or
 FFT-convolution with a filter bank of complex oscillations, followed by a
-Hilbert transform. This results in a more accurate computation of the same
-spectrogram. The direct computation approach also results in code that is more
-flexible, easier to understand, and it has fewer constraints on the input
-parameters compared to `librosa` and `nnAudio`.
+Hilbert transform. This results in a **more accurate** computation of the same
+spectrogram without any artifacts. The direct computation approach also results
+in code that is more flexible, easier to understand, and it has fewer
+constraints on the input parameters compared to `librosa` and `nnAudio`.
 
 #### What to improve on?
 Contributions are welcome! Feel free to open an issue or a pull request.
-
-- Flexibility:
-  - `librosa` parameter mode: It would be nice to have a mode that allows for
-    the same parameters as `librosa` to be used.
-  - Make `VQT` class a full `torch.nn.Module` so that it can be used in a
-    `torch.nn.Sequential` model. Ensure backpropagation works.
-  - Make `VQT` class compatible with `torch.jit.script` and `torch.jit.trace`.
   
-- Speed:
+- Speed / Memory usage:
   - **Lossless approaches**:
-    - For the `fft_conv` approach: I believe a massive (5-100x) speedup is
-      possible using a sparse or non-uniform FFT. A direct approach where only
-      the non-zero frequencies are computed in the `fft`, product, and `ifft`
-      should get us closer to a theoretically optimal lossless approach. There
-      is an implmentation of the NUFFT in PyTorch
-      [here](https://github.com/mmuckley/torchkbnufft).
     - For the `conv1d` approach: I think it would be much faster if we cropped
       the filters to remove the blank space from the higher frequency filters.
       This would be pretty easy to implement and could give a >10x speedup.
   - **Lossy approaches**:
+    - For the `fft_conv` approach: I believe a large (5-50x) speedup is
+      possible. The lower frequency filters use only a small portion of the
+      spectrum, therefore most of the compute is spent multiplying zeros.
+      - Idea 1: Separate out filters in the filter bank whose spectra are all
+        zeros above `n_samples_downsampled`, crop the spectra above that level,
+        then use `ifft` with `n=n_samples_downsampled` to downsample the filter.
+        This would allow for a much faster convolution. For filters that can't
+        be cropped, downsampling would have to be done after the iFFT.
+      - Idea 2: using an efficient sparse or non-uniform FFT. An approach where
+        only the non-zero frequencies are computed in the `fft`, product, and
+        `ifft`. There is an implmentation of the NUFFT in PyTorch
+        [here](https://github.com/mmuckley/torchkbnufft).
+      - Idea 3: Similar to above, a log-frequency iFFT could be used to allow
+        for only the non-zero segment of the filter's spectrum to be used in the
+        convolution.
+      - Idea 4: Try using the overlap-add method.
     - Recursive downsampling: Under many circumstances (like when `Q_high` is
       not much greater than `Q_low`), recursive downsampling is fine.
       Implementing it would be nice just for completeness ([from this
       paper](http://academics.wellesley.edu/Physics/brown/pubs/effalgV92P2698-P2701.pdf))
     - For conv1d approach: Use a strided convolution.
     - For fftconv approach: Downsample using `n=n_samples_downsampled` in `ifft`
       function.
   - Non-trivial ideas that theoretically could speed things up:
     - An FFT implementation that allows for a reduced set of frequencies to be
       computed.
+- Flexibility:
+  - `librosa` parameter mode: It would be nice to have a mode that allows for
+    the same parameters as `librosa` to be used.
 
 #### Demo:
 <img src="docs/media/example_ECG.png" alt="ECG" width="500"  align="right"
 style="margin-left: 10px"/>
 
 ```
 import vqt
@@ -152,15 +178,17 @@
     downsample_factor=8,
     padding='same',
     fft_conv=True,
     take_abs=True,
     plot_pref=False,
 )
 
-specs, xaxis, freqs = my_vqt(data_ecg)
+specs = my_vqt(data_ecg)
+xaxis = my_vqt.get_xAxis(n_samples=data_ecg.shape[0])
+freqs = my_vqt.get_freqs()
 
 fig, axs = plt.subplots(nrows=2, ncols=1, sharex=True, )
 axs[0].plot(np.arange(data_ecg.shape[0]) / sample_rate, data_ecg)
 axs[0].title.set_text('Electrocardiogram')
 axs[1].pcolor(
     xaxis / sample_rate, 
     np.arange(specs[0].shape[0]), specs[0] * (freqs)[:, None],
```

### Comparing `vqt-0.1.2/setup.py` & `vqt-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `vqt-0.1.2/tests/test_all.py` & `vqt-0.1.3/tests/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,46 +33,48 @@
 
 
 # 1. Test Zero Signal Transformation
 def test_zero_signal_transformation():
     params = copy.deepcopy(params_vqt) 
     v = vqt.VQT(**params)  # Create a new instance for each test case
     input_signal = torch.zeros(1024, dtype=torch.float32)  # A zero signal of length 1024
-    output, _, _ = v(input_signal)
+    output = v(input_signal)
     assert torch.all(output == 0), "VQT output for a zero signal should be zero across all frequency bins"
 
 # 2. Test Impulse Signal Transformation
 def test_impulse_signal_transformation():
     params = copy.deepcopy(params_vqt) 
     v = vqt.VQT(**params)  # Create a new instance for each test case
     input_signal = torch.zeros(1024, dtype=torch.float32)
     input_signal[512] = 1  # Set the middle point to 1, creating an impulse
-    output, _, _ = v(input_signal)
+    output = v(input_signal)
     assert not torch.all(output == 0), "VQT output for an impulse signal should not be zero"
     assert output.shape[1] == v.filters.shape[0], "VQT output should have the same number of frequency bins as filters"
 
 # 3. Test Sinusoidal Signal Transformation
 @given(frequency=st.floats(
     # min_value=copy.deepcopy(params_vqt['F_min']), 
     # min_value=params_vqt['F_min'], 
     min_value=10,
     max_value=400,
     # max_value=copy.deepcopy(params_vqt['F_max']),
 ))
+@settings(deadline=500)
 def test_peak_in_spectrogram_at_sine_wave_frequency(
     frequency,
 ):
     """Test to verify a peak in the spectrogram at a specific sine wave frequency."""
     params = copy.deepcopy(params_vqt) 
     v = vqt.VQT(**params)  # Create a new instance for each test case
     # Generate the sine wave signal
     t = torch.arange(0, 1.0, 1/params['Fs_sample'], dtype=torch.float32)
     input_signal = torch.sin(2 * np.pi * frequency * t)
     # Apply the VQT to this sine wave
-    spectrogram, _, freqs = v(input_signal)
+    spectrogram = v(input_signal)
+    freqs = v.get_freqs()
     # Convert freqs to a tensor for easier handling
     freqs_tensor = torch.as_tensor(freqs, dtype=torch.float32)
     # Locate the peak in the spectrogram
     peak_index = torch.argmax(spectrogram[0], dim=0)  # Assuming the output shape is (n_channels, n_freq_bins, time_bins) 
     assert torch.all(peak_index == peak_index[0]), "Expected a single peak in the spectrogram"
     peak_index = peak_index[0]
     # Find the frequency corresponding to the peak
@@ -88,15 +90,15 @@
         f"Expected a peak at index: {idx_nearest.item()} and frequency: {frequency_nearest.item()} Hz, found one at index: {peak_index.item()} and frequency: {peak_frequency.item()} Hz within a tolerance of 2 indices."
         
 # 4. Test Constant Signal Transformation
 def test_constant_signal_transformation():
     params = copy.deepcopy(params_vqt) 
     v = vqt.VQT(**params)  # Create a new instance for each test case
     input_signal = torch.ones(1024, dtype=torch.float32)  # A constant signal
-    output, _, _ = v(input_signal)
+    output = v(input_signal)
     # In a constant signal, the energy should be concentrated at the lowest frequency bin
     assert torch.all(output[0] > output[1:]), "VQT output for a constant signal should peak at the lowest frequency bin"
 
 # 5. Test various params
 @settings(max_examples=1000, deadline=None, suppress_health_check=(HealthCheck.too_slow,))
 @given(
     Fs_sample=st.floats(min_value=1, max_value=10000),
@@ -161,15 +163,15 @@
 
     # Make signal
     len_signal = params['win_size'] if params['win_size'] is not None else int(params['Q_lowF'] * params['Fs_sample'])
     input_signal = torch.rand(n_channels, len_signal + np.random.randint(1, 1000), dtype=torch.float32)
     if n_dim == 1:
         input_signal = input_signal[0]
     # Apply the VQT to this signal
-    output, _, _ = v(input_signal)
+    output = v(input_signal)
     
     # Perform validations on the output
     assert output is not None, "Output should not be None"
     # Check output shape
     assert output.shape[1] == params['n_freq_bins'], "VQT output shape does not match the number of frequency bins"
     # Check all output is real if take_abs is True
     if params['take_abs']:
@@ -223,15 +225,14 @@
 ## Other functions ##
 #####################
 
 
 # Test Hilbert Transform Equivalence
 def test_hilbert_transform_equivalence():
     params = copy.deepcopy(params_vqt) 
-    v = vqt.VQT(**params)  # Create a new instance for each test case
     # Generate a random signal
     input_signal = np.random.rand(1024).astype(np.float64)  ## Implementations for fft are different between numpy and torch for float32
     # Use the VQT class's Hilbert transform
     hilbert_vqt = vqt.helpers.torch_hilbert(torch.as_tensor(input_signal)).numpy()
     # Compare with scipy's Hilbert transform
     hilbert_scipy = scipy.signal.hilbert(input_signal)
     # Check if they are approximately equal
```

### Comparing `vqt-0.1.2/vqt/helpers.py` & `vqt-0.1.3/vqt/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,18 +364,18 @@
         else:
             raise ValueError("symmetry must be 'center', 'left', or 'right'")
         wins *= heaviside
         ### Taper the center of the window by multiplying center sample of window by 0.5
         if taper_asymmetric:
             wins[:, win_size//2] = wins[:, win_size//2] * 0.5
 
-    filts = torch.stack([torch.cos(torch.linspace(-np.pi, np.pi, win_size) * freq * (win_size/Fs_sample)) * win for freq, win in zip(freqs, wins)], dim=0)    
+    filts = torch.stack([torch.cos(torch.linspace(-np.pi, np.pi, win_size) * freq * (win_size/Fs_sample)) * win for freq, win in zip(freqs, wins)], dim=0)
     filts_complex = torch_hilbert(filts.T, dim=0).T
     ## Normalize filters to have unit magnitude
-    filts_complex = filts_complex / torch.linalg.norm(filts_complex, ord=2, dim=1, keepdim=True)
+    filts_complex = filts_complex / torch.linalg.norm(filts_complex, ord=1, dim=1, keepdim=True)  ## Note: ord=1 is L1 norm. This makes the filters have unit magnitude.
     
     freqs = torch.as_tensor(freqs, dtype=torch.float32)
 
     ## Plot
     if plot_pref:
         plt.figure()
         plt.plot(freqs)
```

### Comparing `vqt-0.1.2/vqt/vqt.py` & `vqt-0.1.3/vqt/vqt.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,98 @@
 # import scipy.signal
 from tqdm import tqdm
 # import scipy.fftpack
 
 from . import helpers
 
 class VQT(torch.nn.Module):
+    """
+    Variable Q Transform. Class for applying the variable Q transform to
+    signals. \n
+
+    This function works differently than the VQT from librosa or nnAudio.
+    This one does not use iterative lowpass filtering. \n 
+    If fft_conv is False, then it uses a fixed set of filters, a Hilbert
+    transform to compute the analytic signal, and then takes the magnitude. \n 
+    If fft_conv is True, then it uses FFT convolution to compute the transform.
+    \n
+    
+    Uses Pytorch for GPU acceleration, and allows gradients to pass through. \n
+
+    Q: quality factor; roughly corresponds to the number of cycles in a
+    filter. Here, Q is similar to the number of cycles within 4 sigma (95%)
+    of a gaussian window. \n
+
+    For running batches on GPU, transferring back to CPU tends to be the slowest
+    part. \n
+
+    RH 2022-2024
+
+    Args:
+        Fs_sample (float):
+            Sampling frequency of the signal.
+        Q_lowF (float):
+            Q factor to use for the lowest frequency.
+        Q_highF (float):
+            Q factor to use for the highest frequency.
+        F_min (float):
+            Lowest frequency to use.
+        F_max (float):
+            Highest frequency to use.
+        n_freq_bins (int):
+            Number of frequency bins to use.
+        win_size (int, None):
+            Size of the window to use, in samples. \n
+            If None, will be set to the next odd number after Q_lowF * (Fs_sample / F_min).
+        window_type (str, np.ndarray, list, tuple):
+            Window to use for the mother wavelet. \n
+                * If string: Will be passed to scipy.signal.windows.get_window.
+                See that documentation for options. Except for 'gaussian',
+                which you should just pass the string 'gaussian' without any
+                other arguments.
+                * If array-like: Will be used as the window directly.
+        symmetry (str):
+            Whether to use a symmetric window or a single-sided window. \n
+                * 'center': Use a symmetric / centered / 'two-sided' window.
+                    \n
+                * 'left': Use a one-sided, left-half window. Only left half
+                of the filter will be nonzero. \n * 'right': Use a
+                one-sided, right-half window. Only right half of the filter
+                will be nonzero. \n
+        taper_asymmetric (bool):
+            Only used if symmetry is not 'center'. Whether to taper the
+            center of the window by multiplying center sample of window by
+            0.5.
+        downsample_factor (int):
+            Factor to downsample the signal by. If the length of the input
+            signal is not divisible by downsample_factor, the signal will be
+            zero-padded at the end so that it is.
+        padding (str):
+            Padding mode to use: \n
+                * If fft_conv==False: ['valid', 'same'] \n
+                * If fft_conv==True: ['full', 'valid', 'same'] \n
+        fft_conv (bool):
+            Whether to use FFT convolution. This is faster, but may be less
+            accurate. If False, uses torch's conv1d.
+        fast_length (bool):
+            Whether to use scipy.fftpack.next_fast_len to 
+                find the next fast length for the FFT.
+            This may be faster, but uses more memory.
+        take_abs (bool):
+            Whether to return the complex version of the transform. If
+            True, then returns the absolute value (envelope) of the
+            transform. If False, returns the complex transform.
+        filters (Torch tensor):
+            Filters to use. If None, will make new filters. Should be
+            complex sinusoids. shape: (n_freq_bins, win_size)
+        verbose (int):
+            Verbosity. True to print warnings.
+        plot_pref (bool):
+            Whether to plot the filters.
+    """
     def __init__(
         self,
         Fs_sample: Union[int, float]=1000,
         Q_lowF: Union[int, float]=1,
         Q_highF: Union[int, float]=20,
         F_min: Union[int, float]=1,
         F_max: Union[int, float]=400,
@@ -26,96 +110,14 @@
         fft_conv: bool=True,
         fast_length: bool=True,
         take_abs: bool=True,
         filters: Optional[torch.Tensor]=None,
         verbose: Union[int, bool]=True,
         plot_pref: bool=False,
     ):
-        """
-        Variable Q Transform. Class for applying the variable Q transform to
-        signals.
-
-        This function works differently than the VQT from librosa or nnAudio.
-        This one does not use iterative lowpass filtering. \n If fft_conv is
-        False, then it uses a fixed set of filters, a Hilbert transform to
-        compute the analytic signal, and then takes the magnitude. \n If
-        fft_conv is True, then it uses FFT convolution to compute the transform.
-        \n
-        
-        Uses Pytorch for GPU acceleration, and allows gradients to pass through.
-        \n
-
-        Q: quality factor; roughly corresponds to the number of cycles in a
-        filter. Here, Q is similar to the number of cycles within 4 sigma (95%)
-        of a gaussian window. \n
-
-        RH 2022-2024
-
-        Args:
-            Fs_sample (float):
-                Sampling frequency of the signal.
-            Q_lowF (float):
-                Q factor to use for the lowest frequency.
-            Q_highF (float):
-                Q factor to use for the highest frequency.
-            F_min (float):
-                Lowest frequency to use.
-            F_max (float):
-                Highest frequency to use.
-            n_freq_bins (int):
-                Number of frequency bins to use.
-            win_size (int, None):
-                Size of the window to use, in samples. \n
-                If None, will be set to the next odd number after Q_lowF * (Fs_sample / F_min).
-            window_type (str, np.ndarray, list, tuple):
-                Window to use for the mother wavelet. \n
-                    * If string: Will be passed to scipy.signal.windows.get_window.
-                    See that documentation for options. Except for 'gaussian',
-                    which you should just pass the string 'gaussian' without any
-                    other arguments.
-                    * If array-like: Will be used as the window directly.
-            symmetry (str):
-                Whether to use a symmetric window or a single-sided window. \n
-                    * 'center': Use a symmetric / centered / 'two-sided' window.
-                      \n
-                    * 'left': Use a one-sided, left-half window. Only left half
-                    of the filter will be nonzero. \n * 'right': Use a
-                    one-sided, right-half window. Only right half of the filter
-                    will be nonzero. \n
-            taper_asymmetric (bool):
-                Only used if symmetry is not 'center'. Whether to taper the
-                center of the window by multiplying center sample of window by
-                0.5.
-            downsample_factor (int):
-                Factor to downsample the signal by. If the length of the input
-                signal is not divisible by downsample_factor, the signal will be
-                zero-padded at the end so that it is.
-            padding (str):
-                Padding mode to use: \n
-                    * If fft_conv==False: ['valid', 'same'] \n
-                    * If fft_conv==True: ['full', 'valid', 'same'] \n
-            fft_conv (bool):
-                Whether to use FFT convolution. This is faster, but may be less
-                accurate. If False, uses torch's conv1d.
-            fast_length (bool):
-                Whether to use scipy.fftpack.next_fast_len to 
-                 find the next fast length for the FFT.
-                This may be faster, but uses more memory.
-            take_abs (bool):
-                Whether to return the complex version of the transform. If
-                True, then returns the absolute value (envelope) of the
-                transform. If False, returns the complex transform.
-            filters (Torch tensor):
-                Filters to use. If None, will make new filters. Should be
-                complex sinusoids. shape: (n_freq_bins, win_size)
-            verbose (int):
-                Verbosity. True to print warnings.
-            plot_pref (bool):
-                Whether to plot the filters.
-        """
         super().__init__()
         ## Prepare filters
         self.using_custom_filters = True if filters is not None else False
         self.filters = filters ## This line here is just for torch.jit.script to work. Delete it if you want to forget about jit.
         if filters is not None:
             ## Use provided filters
             self.filters = filters
@@ -180,32 +182,27 @@
             ## Warn if win_size is > 1024 to use fft_conv
             if win_size > 1024 and fft_conv == False:
                 print(f"Warning: win_size is {win_size}, which is large for conv1d. Consider using fft_conv=True for faster computation.")
             
     def forward(
         self,
         X: torch.Tensor,
-    ):
+    ) -> torch.Tensor:
         """
         Forward pass of VQT.
 
         Args:
             X (Torch tensor):
                 Input signal.
                 shape: (n_channels, n_samples)
 
         Returns:
             Spectrogram (Torch tensor):
                 Spectrogram of the input signal.
                 shape: (n_channels, n_samples_ds, n_freq_bins)
-            x_axis (Torch tensor):
-                New x-axis for the spectrogram in units of samples.
-                Get units of time by dividing by Fs_sample.
-            self.freqs (Torch tensor):
-                Frequencies of the spectrogram.
         """
         assert isinstance(X, torch.Tensor), "X should be a torch tensor"
         X = X.type(torch.float32)
 
         ## Check that X and filters are on the same device
         assert X.device == self.filters.device, "X and filters should be on the same device"
 
@@ -224,40 +221,70 @@
                 fft_conv=self.fft_conv,
                 padding=self.padding,
                 fast_length=self.fast_length,
             ), 
             ds_factor=self.downsample_factor,
         )
 
+        return specs
+        
+    def get_freqs(self) -> torch.Tensor:
+        """
+        Get the frequencies of the spectrogram.
+        
+        Args:
+            None
+
+        Returns:
+            torch.Tensor:
+                Frequencies of the spectrogram. \n
+                shape: (n_freq_bins,)
+        """
+        assert hasattr(self, 'freqs'), "freqs not found. This should not happen."
+        return self.freqs
+    
+    def get_xAxis(self, n_samples: int) -> torch.Tensor:
+        """
+        Get the x-axis for the spectrogram. \n
+        RH 2024
+
+        Args:
+            n_samples (int):
+                Number of samples in the signal.
+
+        Returns:
+            torch.Tensor:
+                x-axis for the spectrogram in units of samples. \n
+                shape: (n_samples_ds,)
+        """
         ## Make x_axis
         x_axis = make_conv_xAxis(
-            n_s=X.shape[-1],
+            n_s=n_samples,
             n_k=self.filters.shape[-1],
             padding=self.padding,
             downsample_factor=self.downsample_factor,
-            device=X.device,
+            device='cpu',
         )
-
-        return specs, x_axis, self.freqs
+        return x_axis
 
     def __repr__(self):
         if self.using_custom_filters:
             return f"VQT with custom filters"
         else:
             attributes_to_print = []
             for k, v in self.__dict__.items():
                 if (k not in ['filters', 'freqs', 'wins']) and (not k.startswith('_')) and (not callable(v)):
                     attributes_to_print.append(k)
-            return f"VQT object with parameters: {''.join([f'{k}={getattr(self, k)}, ' for k in attributes_to_print])[:-2]}"            
+            return f"VQT object with parameters: {''.join([f'{k}={getattr(self, k)}, ' for k in attributes_to_print])[:-2]}"
         
 
 def downsample(
     X: torch.Tensor, 
     ds_factor: int=4, 
-):
+) -> torch.Tensor:
     """
     Downsample a signal using average pooling. \n
     If X is complex, it will be split into magnitude and phase, downsampled,
     and then recombined. \n
 
     RH 2024
 
@@ -284,26 +311,26 @@
     
     ## Check is X is complex
     if X.is_complex() == False:
         return _helper_ds(X, ds_factor=ds_factor)
     elif X.is_complex() == True:
         ## Unfortunately, torch.nn.functional.avg_pool1d does not support complex numbers. So we have to split it up into
         ##  phases and magnitudes (convert imaginary to polar, split, downsample, recombine with polar to complex conversion)
-        out = _helper_imag_to_polarReal(X).reshape(2, -1)
-        out = torch.stack([_helper_ds(out[ii], ds_factor=ds_factor) for ii in range(2)], dim=0)
-        out = _helper_polarReal_to_imag(out)
-        return out
+        X = _helper_imag_to_polarReal(X)
+        X = torch.stack([_helper_ds(X[ii], ds_factor=ds_factor) for ii in range(2)], dim=0)
+        X = _helper_polarReal_to_imag(X)
+        return X
 
     else:
         raise ValueError("X should be a torch tensor of type float or complex")
-def _helper_polarReal_to_imag(arr: torch.Tensor):
+def _helper_polarReal_to_imag(arr: torch.Tensor) -> torch.Tensor:
     return arr[0] * torch.exp(1j * arr[1])
-def _helper_imag_to_polarReal(arr: torch.Tensor):
+def _helper_imag_to_polarReal(arr: torch.Tensor) -> torch.Tensor:
     return torch.stack([torch.abs(arr), torch.angle(arr)], dim=0)
-def _helper_ds(arr: torch.Tensor, ds_factor: int):
+def _helper_ds(arr: torch.Tensor, ds_factor: int) -> torch.Tensor:
     return torch.nn.functional.avg_pool1d(
         arr,
         kernel_size=[int(ds_factor)],
         stride=ds_factor,
         ceil_mode=True,
         # padding=0,
         count_include_pad=False,  ## Prevents edge effects
@@ -312,15 +339,15 @@
 def convolve(
     arr: torch.Tensor, 
     kernels: torch.Tensor, 
     take_abs: bool=False,
     padding: str='same', 
     fft_conv: bool=False, 
     fast_length: bool=False,
-):
+) -> torch.Tensor:
     """
     Convolve a signal with a set of kernels. \n
 
     RH 2024
 
     Args:
         arr (torch.Tensor):
@@ -339,15 +366,16 @@
             Whether to use FFT convolution.
         fast_length (bool):
             Whether to use scipy.fftpack.next_fast_len to find the next fast
             length for the FFT.
 
     Returns:
         torch.Tensor:
-            Result of the convolution.
+            Result of the convolution. \n
+            ``shape``: (n_channels, n_samples, n_kernels)
     """
     assert all(isinstance(arg, torch.Tensor) for arg in [arr, kernels]), "arr and kernels should be torch tensors"
 
     arr = arr[None,:] if arr.ndim==1 else arr
     kernels = kernels[None,:] if kernels.ndim==1 else kernels
 
     arr = arr[:,None,:]  ## Shape: (n_channels, 1, n_samples)
@@ -377,25 +405,24 @@
         
         if flag_kernels_complex:
             out = torch.complex(out_conv[0], out_conv[1])
         else:
             out = out_conv[0]
         
     if take_abs:
-        return torch.abs(out)
-    else:
-        return out
+        out = torch.abs(out)
+    return out
 
 
 def fftconvolve(
     x: torch.Tensor, 
     y: torch.Tensor, 
     mode: str='valid',
     fast_length: bool=False,
-):
+) -> torch.Tensor:
     """
     Convolution using the FFT method. \n
     This is adapted from of torchaudio.functional.fftconvolve that handles
     complex numbers. Code is added for handling complex inputs. \n
     NOTE: For mode='same' and y length even, torch's conv1d convention is used,
     which pads 1 more at the end and 1 fewer at the beginning (which is
     different from numpy/scipy's convolve). See apply_padding_mode for more
@@ -415,15 +442,17 @@
         fast_length (bool):
             Whether to use scipy.fftpack.next_fast_len to 
              find the next fast length for the FFT.
             Set to False if you want to use backpropagation.
 
     Returns:
         torch.Tensor:
-            Result of the convolution.
+            Result of the convolution. \n
+            Padding applied to last dimension. \n
+            ``shape``: (..., n_samples)
     """
     ## Compute the convolution
     n_original = x.shape[-1] + y.shape[-1] - 1
     # n = scipy.fftpack.next_fast_len(n_original) if fast_length else n_original
     n = next_fast_len(n_original) if fast_length else n_original
     # n = n_original
     f = torch.fft.fft(x, n=n, dim=-1) * torch.fft.fft(y, n=n, dim=-1)
@@ -433,15 +462,15 @@
         x_length=x.shape[-1],
         y_length=y.shape[-1],
         mode=mode,
     )
 
 ## For some reason jit is slower here
 # @torch.jit.script
-def next_fast_len(size: int):
+def next_fast_len(size: int) -> int:
     """
     Taken from PyTorch Forecasting:
     Returns the next largest number ``n >= size`` whose prime factors are all
     2, 3, or 5. These sizes are efficient for fast fourier transforms.
     Equivalent to :func:`scipy.fftpack.next_fast_len`.
 
     Implementation from pyro
@@ -489,15 +518,16 @@
         y_length (int):
             Length of the second input.
         mode (str):
             Padding mode to use.
 
     Returns:
         torch.Tensor:
-            Result of the convolution with the specified padding mode.
+            Result of the convolution with the specified padding mode. \n
+            ``shape``: (..., n_samples)
     """
     n = x_length + y_length - 1
     valid_convolve_modes = ["full", "valid", "same"]
     if mode == "full":
         return conv_result
     elif mode == "valid":
         len_target = max(x_length, y_length) - min(x_length, y_length) + 1
@@ -513,15 +543,15 @@
 
 def make_conv_xAxis(
     n_s: int,
     n_k: int,
     padding: str='same',
     downsample_factor: int=4,
     device: torch.device='cpu',
-):
+) -> torch.Tensor:
     """
     Make the x-axis for the result of a convolution.
     This is adapted from torchaudio.functional._make_conv_xAxis.
 
     RH 2024
 
     Args:
@@ -534,15 +564,16 @@
         downsample_factor (int):
             Factor to downsample the signal by.
         device (str):
             Device to use.
 
     Returns:
         torch.Tensor:
-            x-axis for the result of a convolution.
+            x-axis for the result of a convolution. \n
+            ``shape``: (n_samples_ds,)
     """
 
     ## If n_k is odd, then no offset, if even, then offset by 0.5
     ### PyTorch's conv1d and for 'same' pads more to the right, so on the first index of the output the kernel is centered at an offset of 0.5
     offset = 0.5 if n_k % 2 == 0 else 0.0
 
     x_axis_full = torch.arange(
```

### Comparing `vqt-0.1.2/vqt.egg-info/PKG-INFO` & `vqt-0.1.3/vqt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 Metadata-Version: 2.1
 Name: vqt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Variable Q-Transform with PyTorch backend
 Home-page: https://github.com/RichieHakim/vqt
 Author: Richard Hakim
 License: LICENSE
 Keywords: neuroscience,neuroimaging,machine learning,deep learning
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: matplotlib
 Requires-Dist: numpy
-Requires-Dist: pytest
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: torch
 Requires-Dist: pytest
 Requires-Dist: hypothesis
 
-## VQT: Variable Q-Transform
+# VQT: Variable Q-Transform
 [![PyPI
 version](https://badge.fury.io/py/vqt.svg)](https://badge.fury.io/py/vqt)
 
 Contributions are welcome! Feel free to open an issue or a pull request.
 
 ### Variable Q-Transform
 
 This is a novel python implementation of the variable Q-transform that was
-developed due to the need for a more accurate and flexible VQT for the use in
+developed due to the need for a more accurate and flexible VQT for use in
 research. It is battle-tested and has been used in a number of research
 projects. <br>
 - **Accuracy**: The approach is different in that it is a **direct
 implementation** of a spectrogram  via a Hilbert transformation at each desired
 frequency. This results in an exact computation of the spectrogram and is
 appropriate for research applications where accuracy is critical. The
 implementation seen in `librosa` and `nnAudio` uses recursive downsampling,
 which can introduce artifacts in the spectrogram under certain conditions.
 - **Flexibility**: The parameters and codebase are less complex than in other
 libraries, and the filter bank is fully customizable and exposed to the user.
 Built in plotting of the filter bank makes tuning the parameters easy and
-intuitive.
+intuitive. The main class is a PyTorch Module and the gradient function is
+maintained, so backpropagation is possible.
 - **Speed**: The backend is written using PyTorch, and allows for GPU
-acceleration. It is faster than the `librosa` implementation under most cases,
-and roughly as fast as the `nnAudio` implementation. See below section 'What to
-improve on?' for more details on how to speed it up further.
+acceleration. It is faster than the `librosa` implementation under most cases.
+Though it is typically a bit slower (1X-8X) than the `nnAudio` implementation,
+however under some conditions (low hop_length), it is as fast or faster. See
+below section 'What to improve on?' for more details on how to speed it up
+further.
 
 
-### Installation
-From PyPI: `pip install vqt`
+## Installation
+Using `pip`: 
+```
+pip install vqt
+```
 
 From source:
 ```
 git clone https://github.com/RichieHakim/vqt.git
 cd vqt
 pip install -e .
 ```
@@ -61,93 +66,113 @@
 ### Usage
 <img src="docs/media/filter_bank.png" alt="filter_bank" width="300"
 align="right"  style="margin-left: 10px"/>
 
 ```
 import vqt
 
-signal = X  ## numpy or torch array of shape (n_channels, n_samples)
+signal = torch.as_tensor(X)  ## torch Tensor of shape (n_channels, n_samples)
 
-transformer = vqt.VQT(
+my_vqt = vqt.VQT(
     Fs_sample=1000,  ## In Hz
     Q_lowF=3,  ## In periods per octave
     Q_highF=20,  ## In periods per octave
     F_min=10,  ## In Hz
     F_max=400,  ## In Hz
     n_freq_bins=55,  ## Number of frequency bins
-    DEVICE_compute='cpu',
-    return_complex=False,
-    filters=None,  ## Use custom filters
+    window_type='hann',
+    downsample_factor=8,  ## Reduce the output sample rate
+    fft_conv=True,  ## Use FFT convolution for speed
     plot_pref=False,  ## Can show the filter bank
 )
 
-spectrograms, x_axis, frequencies = transformer(signal)
+spectrograms = my_vqt(signal)
+x_axis = my_vqt.get_xAxis(n_samples=signal.shape[1])
+frequencies = my_vqt.get_freqs()
 ```
 <img src="docs/media/freqs.png" alt="freqs" width="300"  align="right"
 style="margin-left: 10px"/>
 
 #### What is the Variable Q-Transform?
 
-The Variable Q-Transform (VQT) is a time-frequency analysis tool that generates
-spectrograms, similar to the Short-time Fourier Transform (STFT). It can also be
-defined as a special case of a wavelet transform, as well as the generalization
-of the Constant Q-Transform (CQT). In fact, the VQT subsumes the CQT and STFT as
-both can be recreated using specific parameters of the VQT.
+The [Variable Q-Transform
+(VQT)](https://en.wikipedia.org/wiki/Constant-Q_transform#Variable-Q_bandwidth_calculation)
+is a time-frequency analysis tool that generates spectrograms, similar to the
+Short-time Fourier Transform (STFT). It can also be defined as a special case of
+a wavelet transform (complex Morlet), as well as the generalization of the
+[Constant Q-Transform
+(CQT)](https://en.wikipedia.org/wiki/Constant-Q_transform). In fact, the VQT
+subsumes the CQT and the STFT since both can be recreated using specific
+parameters of the VQT. <br>
+<br>
+In brief, the VQT generates a spectrogram where the frequencies are spaced
+logarithmically, and the bandwidth of the filters are tuned using two
+parameters: `Q_low` and `Q_high`, where `Q` describes the number of periods of
+the oscillatory wavelet at a particular frequency (aka the 'bandwidth'); 'low'
+refers to the lowest frequency bin, and 'high' refers to the highest frequency
+bin.
 
 #### Why use the VQT?
 
 It provides enough knobs to tune the time-frequency resolution trade-off to suit
-your needs.
+your needs. It is especially useful when time resolution is needed at lower
+frequencies.
 
 #### How exactly does this implementation differ from others?
 <img src="docs/media/freq_response.png" alt="freq_response" width="300"
 align="right"  style="margin-left: 10px"/>
 
 This function works differently than the VQT from `librosa` or `nnAudio` in that
 it does not use the recursive downsampling algorithm from [this
 paper](http://academics.wellesley.edu/Physics/brown/pubs/effalgV92P2698-P2701.pdf).
 Instead, it computes the power at each frequency using either direct- or
 FFT-convolution with a filter bank of complex oscillations, followed by a
-Hilbert transform. This results in a more accurate computation of the same
-spectrogram. The direct computation approach also results in code that is more
-flexible, easier to understand, and it has fewer constraints on the input
-parameters compared to `librosa` and `nnAudio`.
+Hilbert transform. This results in a **more accurate** computation of the same
+spectrogram without any artifacts. The direct computation approach also results
+in code that is more flexible, easier to understand, and it has fewer
+constraints on the input parameters compared to `librosa` and `nnAudio`.
 
 #### What to improve on?
 Contributions are welcome! Feel free to open an issue or a pull request.
-
-- Flexibility:
-  - `librosa` parameter mode: It would be nice to have a mode that allows for
-    the same parameters as `librosa` to be used.
-  - Make `VQT` class a full `torch.nn.Module` so that it can be used in a
-    `torch.nn.Sequential` model. Ensure backpropagation works.
-  - Make `VQT` class compatible with `torch.jit.script` and `torch.jit.trace`.
   
-- Speed:
+- Speed / Memory usage:
   - **Lossless approaches**:
-    - For the `fft_conv` approach: I believe a massive (5-100x) speedup is
-      possible using a sparse or non-uniform FFT. A direct approach where only
-      the non-zero frequencies are computed in the `fft`, product, and `ifft`
-      should get us closer to a theoretically optimal lossless approach. There
-      is an implmentation of the NUFFT in PyTorch
-      [here](https://github.com/mmuckley/torchkbnufft).
     - For the `conv1d` approach: I think it would be much faster if we cropped
       the filters to remove the blank space from the higher frequency filters.
       This would be pretty easy to implement and could give a >10x speedup.
   - **Lossy approaches**:
+    - For the `fft_conv` approach: I believe a large (5-50x) speedup is
+      possible. The lower frequency filters use only a small portion of the
+      spectrum, therefore most of the compute is spent multiplying zeros.
+      - Idea 1: Separate out filters in the filter bank whose spectra are all
+        zeros above `n_samples_downsampled`, crop the spectra above that level,
+        then use `ifft` with `n=n_samples_downsampled` to downsample the filter.
+        This would allow for a much faster convolution. For filters that can't
+        be cropped, downsampling would have to be done after the iFFT.
+      - Idea 2: using an efficient sparse or non-uniform FFT. An approach where
+        only the non-zero frequencies are computed in the `fft`, product, and
+        `ifft`. There is an implmentation of the NUFFT in PyTorch
+        [here](https://github.com/mmuckley/torchkbnufft).
+      - Idea 3: Similar to above, a log-frequency iFFT could be used to allow
+        for only the non-zero segment of the filter's spectrum to be used in the
+        convolution.
+      - Idea 4: Try using the overlap-add method.
     - Recursive downsampling: Under many circumstances (like when `Q_high` is
       not much greater than `Q_low`), recursive downsampling is fine.
       Implementing it would be nice just for completeness ([from this
       paper](http://academics.wellesley.edu/Physics/brown/pubs/effalgV92P2698-P2701.pdf))
     - For conv1d approach: Use a strided convolution.
     - For fftconv approach: Downsample using `n=n_samples_downsampled` in `ifft`
       function.
   - Non-trivial ideas that theoretically could speed things up:
     - An FFT implementation that allows for a reduced set of frequencies to be
       computed.
+- Flexibility:
+  - `librosa` parameter mode: It would be nice to have a mode that allows for
+    the same parameters as `librosa` to be used.
 
 #### Demo:
 <img src="docs/media/example_ECG.png" alt="ECG" width="500"  align="right"
 style="margin-left: 10px"/>
 
 ```
 import vqt
@@ -171,15 +196,17 @@
     downsample_factor=8,
     padding='same',
     fft_conv=True,
     take_abs=True,
     plot_pref=False,
 )
 
-specs, xaxis, freqs = my_vqt(data_ecg)
+specs = my_vqt(data_ecg)
+xaxis = my_vqt.get_xAxis(n_samples=data_ecg.shape[0])
+freqs = my_vqt.get_freqs()
 
 fig, axs = plt.subplots(nrows=2, ncols=1, sharex=True, )
 axs[0].plot(np.arange(data_ecg.shape[0]) / sample_rate, data_ecg)
 axs[0].title.set_text('Electrocardiogram')
 axs[1].pcolor(
     xaxis / sample_rate, 
     np.arange(specs[0].shape[0]), specs[0] * (freqs)[:, None],
```

