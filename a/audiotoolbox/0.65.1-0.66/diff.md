# Comparing `tmp/audiotoolbox-0.65.1.tar.gz` & `tmp/audiotoolbox-0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiotoolbox-0.65.1.tar", last modified: Tue May 30 01:01:03 2023, max compression
+gzip compressed data, was "audiotoolbox-0.66.tar", last modified: Thu Jun 22 05:01:55 2023, max compression
```

## Comparing `audiotoolbox-0.65.1.tar` & `audiotoolbox-0.66.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/
--rw-r--r--   0 joerg     (1000) joerg     (1000)    35148 2021-07-02 20:55:17.000000 audiotoolbox-0.65.1/LICENSE
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     2154 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/PKG-INFO
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1630 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/README.md
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotoolbox.egg-info/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     2154 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      989 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 joerg     (1000) joerg     (1000)        1 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       39 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/requires.txt
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       11 2023-05-30 01:01:03.000000 audiotoolbox-0.65.1/audiotoolbox.egg-info/top_level.txt
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      400 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/__init__.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    51410 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/audiotools.py
--rw-r--r--   0 joerg     (1000) joerg     (1000)     1139 2021-07-02 20:55:19.000000 audiotoolbox-0.65.1/audiotools/auditory_filter.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1921 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/din_iso_226.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/filter/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      278 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/__init__.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/filter/bank/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      127 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/bank/__init__.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1378 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/bank/default_banks.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     7049 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/audiotools/filter/bank/filterbank.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3215 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/filter/bank/octave_bank.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1121 2021-08-20 11:41:33.000000 audiotoolbox-0.65.1/audiotools/filter/brickwall_filt.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     4694 2023-05-02 01:30:47.000000 audiotoolbox-0.65.1/audiotools/filter/butterworth_filt.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3658 2022-08-15 12:42:15.000000 audiotoolbox-0.65.1/audiotools/filter/filter.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     5415 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/audiotools/filter/gammatone_filt.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/audiotools/oaudio/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       55 2021-08-20 11:41:33.000000 audiotoolbox-0.65.1/audiotools/oaudio/__init__.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     6154 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/oaudio/base_signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     5914 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/oaudio/freqdomain_signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    26505 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/audiotools/oaudio/signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1132 2022-10-20 08:07:26.000000 audiotoolbox-0.65.1/audiotools/oaudio/stats.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3684 2022-09-26 08:51:11.000000 audiotoolbox-0.65.1/audiotools/wav.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      126 2022-08-15 12:42:15.000000 audiotoolbox-0.65.1/pyproject.toml
--rw-rw-r--   0 joerg     (1000) joerg     (1000)       38 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/setup.cfg
--rw-rw-r--   0 joerg     (1000) joerg     (1000)      883 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/setup.py
-drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-05-30 01:01:03.752671 audiotoolbox-0.65.1/tests/
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    26895 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_audiotools.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1301 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_audiotools_stats.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     7468 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_filter.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     8403 2023-05-30 00:59:17.000000 audiotoolbox-0.65.1/tests/test_filterbank.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     3553 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_freqdomainsignal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)    14681 2023-05-29 06:07:14.000000 audiotoolbox-0.65.1/tests/test_signal.py
--rw-rw-r--   0 joerg     (1000) joerg     (1000)     1427 2023-05-29 06:52:39.000000 audiotoolbox-0.65.1/tests/test_wav.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-06-22 05:01:55.401365 audiotoolbox-0.66/
+-rw-r--r--   0 joerg     (1000) joerg     (1000)    35148 2021-07-02 20:55:17.000000 audiotoolbox-0.66/LICENSE
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     2152 2023-06-22 05:01:55.401365 audiotoolbox-0.66/PKG-INFO
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1630 2023-05-30 00:59:17.000000 audiotoolbox-0.66/README.md
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-06-22 05:01:55.401365 audiotoolbox-0.66/audiotoolbox.egg-info/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     2152 2023-06-22 05:01:55.000000 audiotoolbox-0.66/audiotoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      989 2023-06-22 05:01:55.000000 audiotoolbox-0.66/audiotoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)        1 2023-06-22 05:01:55.000000 audiotoolbox-0.66/audiotoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       39 2023-06-22 05:01:55.000000 audiotoolbox-0.66/audiotoolbox.egg-info/requires.txt
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       11 2023-06-22 05:01:55.000000 audiotoolbox-0.66/audiotoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-06-22 05:01:55.401365 audiotoolbox-0.66/audiotools/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      400 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/__init__.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    52004 2023-06-22 04:58:38.000000 audiotoolbox-0.66/audiotools/audiotools.py
+-rw-r--r--   0 joerg     (1000) joerg     (1000)     1139 2021-07-02 20:55:19.000000 audiotoolbox-0.66/audiotools/auditory_filter.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1921 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/din_iso_226.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-06-22 05:01:55.401365 audiotoolbox-0.66/audiotools/filter/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      278 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/filter/__init__.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-06-22 05:01:55.401365 audiotoolbox-0.66/audiotools/filter/bank/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      127 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/filter/bank/__init__.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1378 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/filter/bank/default_banks.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     7049 2023-05-30 00:59:17.000000 audiotoolbox-0.66/audiotools/filter/bank/filterbank.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3215 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/filter/bank/octave_bank.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1121 2021-08-20 11:41:33.000000 audiotoolbox-0.66/audiotools/filter/brickwall_filt.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     4694 2023-05-02 01:30:47.000000 audiotoolbox-0.66/audiotools/filter/butterworth_filt.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3658 2022-08-15 12:42:15.000000 audiotoolbox-0.66/audiotools/filter/filter.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     5415 2023-05-30 00:59:17.000000 audiotoolbox-0.66/audiotools/filter/gammatone_filt.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-06-22 05:01:55.401365 audiotoolbox-0.66/audiotools/oaudio/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       55 2021-08-20 11:41:33.000000 audiotoolbox-0.66/audiotools/oaudio/__init__.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     6154 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/oaudio/base_signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     5914 2023-05-29 06:07:14.000000 audiotoolbox-0.66/audiotools/oaudio/freqdomain_signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    26661 2023-06-22 04:58:38.000000 audiotoolbox-0.66/audiotools/oaudio/signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1132 2022-10-20 08:07:26.000000 audiotoolbox-0.66/audiotools/oaudio/stats.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3684 2022-09-26 08:51:11.000000 audiotoolbox-0.66/audiotools/wav.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      126 2022-08-15 12:42:15.000000 audiotoolbox-0.66/pyproject.toml
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)       38 2023-06-22 05:01:55.401365 audiotoolbox-0.66/setup.cfg
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)      881 2023-06-22 04:59:14.000000 audiotoolbox-0.66/setup.py
+drwxrwxr-x   0 joerg     (1000) joerg     (1000)        0 2023-06-22 05:01:55.401365 audiotoolbox-0.66/tests/
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    26711 2023-06-22 04:58:38.000000 audiotoolbox-0.66/tests/test_audiotools.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1301 2023-05-29 06:07:14.000000 audiotoolbox-0.66/tests/test_audiotools_stats.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     7468 2023-05-29 06:07:14.000000 audiotoolbox-0.66/tests/test_filter.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     8744 2023-06-22 04:58:38.000000 audiotoolbox-0.66/tests/test_filterbank.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     3553 2023-05-29 06:07:14.000000 audiotoolbox-0.66/tests/test_freqdomainsignal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)    14681 2023-06-22 04:09:49.000000 audiotoolbox-0.66/tests/test_signal.py
+-rw-rw-r--   0 joerg     (1000) joerg     (1000)     1427 2023-05-29 06:52:39.000000 audiotoolbox-0.66/tests/test_wav.py
```

### Comparing `audiotoolbox-0.65.1/LICENSE` & `audiotoolbox-0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/PKG-INFO` & `audiotoolbox-0.66/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiotoolbox
-Version: 0.65.1
+Version: 0.66
 Summary: Toolbox for generating and working with audio signals
 Home-page: https://jencke.github.io/audiotools/
 Author: Jörg Encke
 Author-email: joerg.encke@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `audiotoolbox-0.65.1/README.md` & `audiotoolbox-0.66/README.md`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotoolbox.egg-info/PKG-INFO` & `audiotoolbox-0.66/audiotoolbox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiotoolbox
-Version: 0.65.1
+Version: 0.66
 Summary: Toolbox for generating and working with audio signals
 Home-page: https://jencke.github.io/audiotools/
 Author: Jörg Encke
 Author-email: joerg.encke@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `audiotoolbox-0.65.1/audiotoolbox.egg-info/SOURCES.txt` & `audiotoolbox-0.66/audiotoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/audiotools.py` & `audiotoolbox-0.66/audiotools/audiotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,14 @@
         # diveide through envelope and restrict
         noise /= env
         noise = filter.brickwall(noise, fc - bw / 2, fc + bw / 2, fs)
         noise /= noise.std(axis=0) * std
 
     return noise
 
-
 def generate_noise(duration, fs=None, ntype="white", n_channels=1, seed=None):
     r"""Generate Noise
 
     Generate gaussian noise with a variance of 1 and different
     spectral shapes. The noise is generated in the frequency domain
     using the gaussian pseudorandom generator ``numpy.random.randn``.
     The real and imaginary part of each frequency component is set
@@ -387,14 +386,16 @@
     f_weights = np.zeros(nfft)
     if ntype == "pink":
         # Power proportinal to 1 / f
         f_weights[lowbin:highbin] = 1.0 / np.sqrt(freqs[lowbin:])
     elif ntype == "brown":
         # Power proportional to 1 / f**2
         f_weights[lowbin:highbin] = 1.0 / freqs[lowbin:]
+    else:
+        raise(ValueError('ntype not implemented'))
 
     # generate noise
     a = np.zeros([nfft])
     b = np.zeros([nfft])
     a[lowbin:highbin] = np.random.randn(highbin - lowbin)
     b[lowbin:highbin] = np.random.randn(highbin - lowbin)
     fspec = a + 1j * b
@@ -418,14 +419,15 @@
 
 
 def generate_uncorr_noise(
     duration,
     fs,
     n_channels=2,
     corr=0,
+    ntype='white',
     seed=None,
     bandpass=None,
     lowpass=None,
     highpass=None,
 ):
     r"""Generate partly uncorrelated noise
 
@@ -457,14 +459,16 @@
         Noise duration in seconds
     fs : int
         Sampling frequency
     n_channels : int
         number of indipendant noise channels
     corr : int, optional
         Desired correlation of the noise tokens, (default=0).
+    ntype : {'white', 'pink', 'brown'}
+        spectral shape of the noise
     seed : int or 1-d array_like, optional
         Seed for `RandomState`.
         Must be convertible to 32 bit unsigned integers.
     bandpass : dict, optional
         Parameters for an bandpass filter, these are passed as arguments to the
         audiotools.filter.bandpass function
     lowpass : dict, optional
@@ -485,15 +489,15 @@
 
     .. [1] Hartmann, W. M., & Cho, Y. J. (2011). Generating partially
       correlated noise—a comparison of methods. The Journal of the
       Acoustical Society of America, 130(1),
       292–301. http://dx.doi.org/10.1121/1.3596475
 
     """
-    np.random.seed(seed)
+    # np.random.seed(seed)
 
     if corr < 0:
         Warning(
             ValueError(
                 "Resulting correlations will be positive"
                 + " to gain negative correlations, multiply"
                 + " channel with -1"
@@ -507,15 +511,28 @@
     else:
         shape = n_channels
 
     # correlated noise in multiple channels is generated by using the
     # N+1 generator method
 
     len_signal = nsamples(duration, fs)
-    noise = np.random.randn(len_signal, n_channels + 1)
+
+    noise = generate_noise(duration,
+                           fs=fs,
+                           ntype=ntype,
+                           n_channels=1,
+                           seed=seed)
+    for i in range(n_channels):
+        n_noise = generate_noise(duration,
+                                 fs=fs,
+                                 ntype=ntype,
+                                 n_channels=1,
+                                 seed=seed)
+        noise = np.column_stack([noise, n_noise])
+
     noise -= noise.mean(axis=0)
 
     if bandpass is not None:
         noise = filter.bandpass(signal=noise, fs=fs, **bandpass)
     if lowpass is not None:
         noise = filter.lowpass(signal=noise, fs=fs, **lowpass)
     if highpass is not None:
```

### Comparing `audiotoolbox-0.65.1/audiotools/auditory_filter.py` & `audiotoolbox-0.66/audiotools/auditory_filter.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/din_iso_226.py` & `audiotoolbox-0.66/audiotools/din_iso_226.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/filter/bank/default_banks.py` & `audiotoolbox-0.66/audiotools/filter/bank/default_banks.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/filter/bank/filterbank.py` & `audiotoolbox-0.66/audiotools/filter/bank/filterbank.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/filter/bank/octave_bank.py` & `audiotoolbox-0.66/audiotools/filter/bank/octave_bank.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/filter/brickwall_filt.py` & `audiotoolbox-0.66/audiotools/filter/brickwall_filt.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/filter/butterworth_filt.py` & `audiotoolbox-0.66/audiotools/filter/butterworth_filt.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/filter/filter.py` & `audiotoolbox-0.66/audiotools/filter/filter.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/filter/gammatone_filt.py` & `audiotoolbox-0.66/audiotools/filter/gammatone_filt.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/oaudio/base_signal.py` & `audiotoolbox-0.66/audiotools/oaudio/base_signal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/oaudio/freqdomain_signal.py` & `audiotoolbox-0.66/audiotools/oaudio/freqdomain_signal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/oaudio/signal.py` & `audiotoolbox-0.66/audiotools/oaudio/signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     def add_noise(self, ntype='white', variance=1, seed=None):
         r"""Add uncorrelated noise to the signal.
 
         add gaussian noise with a defined variance and different
         spectral shapes. The noise is generated in the frequency domain
         using the gaussian pseudorandom generator ``numpy.random.randn``.
-        The real and imaginary part of each frequency component is set
+        The real and imaginarny part of each frequency component is set
         using the psudorandom generator. Each frequency bin is then
         weighted dependent on the spectral shape. The resulting spektrum
         is then transformed into the time domain using ``numpy.fft.ifft``
 
         Weighting functions:
 
          - white: :math:`w(f) = 1`
@@ -156,15 +156,15 @@
         noise = audio.generate_noise(self.duration, self.fs,
                                      ntype=ntype, n_channels=1,
                                      seed=seed)
 
         self[:] = (self.T + noise.T * np.sqrt(variance)).T
         return self
 
-    def add_uncorr_noise(self, corr=0, variance=1, seed=None,
+    def add_uncorr_noise(self, corr=0, variance=1, ntype='white', seed=None,
                          bandpass=None, highpass=None, lowpass=None):
         r"""Add partly uncorrelated noise.
 
         This function adds partly uncorrelated noise using the N+1
         generator method.
 
         To generate N partly uncorrelated noises with a desired
@@ -185,14 +185,16 @@
 
         Parameters
         ----------
         corr : int, optional
             Desired correlation of the noise tokens, (default=0)
         variance : scalar, optional
             The desired variance of the noise, (default=1)
+        ntype : {'white', 'pink', 'brown'}
+            spectral shape of the noise
         seed : int or 1-d array_like, optional
             Seed for `RandomState`.
             Must be convertible to 32 bit unsigned integers.
         bandpass : dict, optional
             Parameters for an bandpass filter, these are passed as arguments to
             the audiotools.filter.bandpass function
         lowpass : dict, optional
@@ -219,14 +221,15 @@
           Acoustical Society of America, 130(1),
           292–301. http://dx.doi.org/10.1121/1.3596475
 
         """
         noise = audio.generate_uncorr_noise(duration=self.duration,
                                             fs=self.fs,
                                             n_channels=self.n_channels,
+                                            ntype=ntype,
                                             corr=corr,
                                             seed=seed,
                                             bandpass=bandpass,
                                             highpass=highpass,
                                             lowpass=lowpass)
 
         self += noise * np.sqrt(variance)
```

### Comparing `audiotoolbox-0.65.1/audiotools/oaudio/stats.py` & `audiotoolbox-0.66/audiotools/oaudio/stats.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/audiotools/wav.py` & `audiotoolbox-0.66/audiotools/wav.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/setup.py` & `audiotoolbox-0.66/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="audiotoolbox",
-    version="0.65.1",
+    version="0.66",
     author="Jörg Encke",
     author_email="joerg.encke@posteo.de",
     description="Toolbox for generating and working with audio signals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://jencke.github.io/audiotools/",
     python_requires='>=3',
```

### Comparing `audiotoolbox-0.65.1/tests/test_audiotools.py` & `audiotoolbox-0.66/tests/test_audiotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,16 +557,14 @@
     noise = audio.generate_noise(1, 10, n_channels=(2, 3), ntype="pink")
     assert noise.shape == (10, 2, 3)
     testing.assert_array_equal(noise[:, 0, :], noise[:, 1, :])
     testing.assert_array_equal(noise[:, :, 0], noise[:, :, 1])
 
 
 def test_generate_uncorr_noise():
-    from scipy.stats import pearsonr
-
     duration = 1
     fs = 100e3
     noise = audio.generate_uncorr_noise(duration, fs, n_channels=2)
     noise1 = noise[:, 0]
     noise2 = noise[:, 1]
     # Test equal Power assumption
     testing.assert_almost_equal(noise1.var(), noise2.var())
@@ -581,14 +579,22 @@
     # Test multichannel
     res_noise = audio.generate_uncorr_noise(1, fs=48000, n_channels=3, corr=0.5)
     cv = np.corrcoef(res_noise.T)
     lower_tri = np.tril(cv, -1)
     lower_tri[lower_tri == 0] = np.nan
     testing.assert_almost_equal(lower_tri[~np.isnan(lower_tri)], 0.5)
 
+    # Test multichannel
+    res_noise = audio.generate_uncorr_noise(1, fs=48000, n_channels=3,
+                                            corr=0.5, ntype='pink')
+    cv = np.corrcoef(res_noise.T)
+    lower_tri = np.tril(cv, -1)
+    lower_tri[lower_tri == 0] = np.nan
+    testing.assert_almost_equal(lower_tri[~np.isnan(lower_tri)], 0.5)
+
     # Test vor variance = 1
     noise = audio.generate_uncorr_noise(duration, fs, 2, corr=0.5)
     testing.assert_almost_equal(noise.var(axis=0), 1)
 
     # Test multiple dimensions:
     noise = audio.generate_uncorr_noise(duration, fs, (2, 3, 4), corr=0.5)
     assert noise.shape[1:] == (2, 3, 4)
@@ -824,21 +830,7 @@
 
     a = np.random.random(1000)
     b = audio.audiotools._copy_to_dim(a, (2, 3))
     assert b.shape == (1000, 2, 3)
 
     b = audio.audiotools._copy_to_dim(a, 3)
     assert b.shape == (1000, 3)
-
-    # def test_from_wav():
-    #     fs = 41200
-    #     signal = audio.Signal(2, 2, fs)
-    #     signal[:] = np.linspace(-1, 1, signal.n_samples)[:, None]
-
-    #     bitdepth = 16
-    #     audio.wav.writewav('test.wav', signal, signal.fs, 32)
-
-    #     signal_out = audio.from_wav('test.wav')
-    #     testing.assert_allclose(signal_out,
-    #                             signal,
-    #                             atol=2 / 2**bitdepth,
-    #                             rtol=1)
```

### Comparing `audiotoolbox-0.65.1/tests/test_audiotools_stats.py` & `audiotoolbox-0.66/tests/test_audiotools_stats.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/tests/test_filter.py` & `audiotoolbox-0.66/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/tests/test_filterbank.py` & `audiotoolbox-0.66/tests/test_filterbank.py`

 * *Files 5% similar despite different names*

```diff
@@ -230,7 +230,17 @@
     # white noise
     fs = 48000
     filt_bank = octave_bank(fs)
     noise = audio.Signal(1, 10, 48000).add_noise("pink")
     bank_out = filt_bank.filt(noise)
     power = np.var(bank_out, axis=0)
     assert power.std() < 0.01
+
+    fs = 48000
+    filt_bank = octave_bank(fs)
+    noise = audio.Signal(2, 20, 48000).add_uncorr_noise(0, ntype="pink")
+    bank_out = filt_bank.filt(noise.ch[0])
+    power = np.var(bank_out, axis=0)
+    assert power.std() < 0.01
+    bank_out = filt_bank.filt(noise.ch[1])
+    power = np.var(bank_out, axis=0)
+    assert power.std() < 0.01
```

### Comparing `audiotoolbox-0.65.1/tests/test_freqdomainsignal.py` & `audiotoolbox-0.66/tests/test_freqdomainsignal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/tests/test_signal.py` & `audiotoolbox-0.66/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `audiotoolbox-0.65.1/tests/test_wav.py` & `audiotoolbox-0.66/tests/test_wav.py`

 * *Files identical despite different names*

