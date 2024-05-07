# Comparing `tmp/keras-mdn-layer-0.3.0.tar.gz` & `tmp/keras_mdn_layer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/keras-mdn-layer-0.3.0.tar", last modified: Mon Nov  4 02:19:24 2019, max compression
+gzip compressed data, was "keras_mdn_layer-0.4.0.tar", max compression
```

## Comparing `keras-mdn-layer-0.3.0.tar` & `keras_mdn_layer-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,8 @@
-drwxr-xr-x   0 charles    (502) staff       (20)        0 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/
--rw-r--r--   0 charles    (502) staff       (20)     7441 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/PKG-INFO
-drwxr-xr-x   0 charles    (502) staff       (20)        0 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/mdn/
--rw-r--r--   0 charles    (502) staff       (20)       22 2019-11-04 02:16:10.000000 keras-mdn-layer-0.3.0/mdn/version.py
--rw-r--r--   0 charles    (502) staff       (20)    11003 2019-11-04 02:16:10.000000 keras-mdn-layer-0.3.0/mdn/__init__.py
--rw-r--r--   0 charles    (502) staff       (20)     6114 2019-11-01 00:19:30.000000 keras-mdn-layer-0.3.0/README.md
--rw-r--r--   0 charles    (502) staff       (20)     1160 2019-11-01 00:19:30.000000 keras-mdn-layer-0.3.0/setup.py
--rw-r--r--   0 charles    (502) staff       (20)       59 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/setup.cfg
-drwxr-xr-x   0 charles    (502) staff       (20)        0 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/keras_mdn_layer.egg-info/
--rw-r--r--   0 charles    (502) staff       (20)     7441 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/keras_mdn_layer.egg-info/PKG-INFO
--rw-r--r--   0 charles    (502) staff       (20)      205 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/keras_mdn_layer.egg-info/SOURCES.txt
--rw-r--r--   0 charles    (502) staff       (20)        4 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/keras_mdn_layer.egg-info/top_level.txt
--rw-r--r--   0 charles    (502) staff       (20)        1 2019-11-04 02:19:24.000000 keras-mdn-layer-0.3.0/keras_mdn_layer.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0     1055 2024-04-02 01:45:40.378650 keras_mdn_layer-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     6271 2024-05-07 05:20:40.827978 keras_mdn_layer-0.4.0/README.md
+-rw-r--r--   0        0        0    11003 2024-04-02 01:45:40.379305 keras_mdn_layer-0.4.0/keras_mdn_layer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 01:45:40.379390 keras_mdn_layer-0.4.0/keras_mdn_layer/tests/__init__.py
+-rw-r--r--   0        0        0     1755 2024-05-07 05:20:14.085692 keras_mdn_layer-0.4.0/keras_mdn_layer/tests/test_mdn.py
+-rw-r--r--   0        0        0       22 2024-05-07 05:36:23.633125 keras_mdn_layer-0.4.0/keras_mdn_layer/version.py
+-rw-r--r--   0        0        0      663 2024-05-07 05:37:22.504410 keras_mdn_layer-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6916 1970-01-01 00:00:00.000000 keras_mdn_layer-0.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `keras-mdn-layer-0.3.0/PKG-INFO` & `keras_mdn_layer-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,97 @@
-Metadata-Version: 1.1
-Name: keras-mdn-layer
-Version: 0.3.0
-Summary: An MDN Layer for Keras using TensorFlow Probability.
-Home-page: https://github.com/cpmpercussion/keras-mdn-layer
-Author: Charles Martin
-Author-email: charlepm@ifi.uio.no
-License: MIT
-Description: # Keras Mixture Density Network Layer
-        
-        [![Build Status](https://travis-ci.com/cpmpercussion/keras-mdn-layer.svg?branch=master)](https://travis-ci.com/cpmpercussion/keras-mdn-layer)
-        ![MIT License](https://img.shields.io/github/license/cpmpercussion/keras-mdn-layer.svg?style=flat)
-        [![DOI](https://zenodo.org/badge/137585470.svg)](https://zenodo.org/badge/latestdoi/137585470)
-        [![PyPI version](https://badge.fury.io/py/keras-mdn-layer.svg)](https://badge.fury.io/py/keras-mdn-layer)
-        
-        A mixture density network (MDN) Layer for Keras using TensorFlow's distributions module. This makes it a bit more simple to experiment with neural networks that predict multiple real-valued variables that can take on multiple equally likely values.
-        
-        This layer can help build MDN-RNNs similar to those used in [RoboJam](https://github.com/cpmpercussion/robojam), [Sketch-RNN](https://experiments.withgoogle.com/sketch-rnn-demo), [handwriting generation](https://distill.pub/2016/handwriting/), and maybe even [world models](https://worldmodels.github.io). You can do a lot of cool stuff with MDNs!
-        
-        One benefit of this implementation is that you can predict any number of real-values. TensorFlow's `Mixture`, `Categorical`, and `MultivariateNormalDiag` distribution functions are used to generate the loss function (the probability density function of a mixture of multivariate normal distributions with a diagonal covariance matrix). In previous work, the loss function has often been specified by hand which is fine for 1D or 2D prediction, but becomes a bit more annoying after that.
-        
-        Two important functions are provided for training and prediction:
-        
-        - `get_mixture_loss_func(output_dim, num_mixtures)`: This function generates a loss function with the correct output dimensiona and number of mixtures.
-        - `sample_from_output(params, output_dim, num_mixtures, temp=1.0)`: This functions samples from the mixture distribution output by the model.
-        
-        ## Installation 
-        
-        This project requires Python 3.6+. You can easily install this package from [PyPI](https://pypi.org/project/keras-mdn-layer/) via `pip` like so:
-        
-            python3 -m pip install keras-mdn-layer
-        
-        And finally, import the `mdn` module in Python: `import mdn`
-        
-        Alternatively, you can clone or download this repository and then install via `python setup.py install`, or copy the `mdn` folder into your own project.
-        
-        ## Examples
-        
-        Some examples are provided in the notebooks directory.
-        
-        There's scripts for fitting multivalued functions, a standard MDN toy problem:
-        
-        <img src="https://preview.ibb.co/mZzkpd/Keras_MDN_Demo.jpg" alt="Keras MDN Demo" border="0">
-        
-        There's also a script for generating fake kanji characters:
-        
-        <img src="https://i.ibb.co/yFvtgkL/kanji-mdn-examples.png" alt="kanji test 1" border="0" width="600"/>
-        
-        And finally, for learning how to generate musical touch-screen performances with a temporal component:
-        
-        <img src="https://i.ibb.co/WpzSCV8/robojam-examples.png" alt="Robojam Model Examples" border="0">
-        
-        ## How to use
-        
-        The MDN layer should be the last in your network and you should use `get_mixture_loss_func` to generate a loss function. Here's an example of a simple network with one Dense layer followed by the MDN.
-        
-            import keras
-            import mdn
-        
-            N_HIDDEN = 15  # number of hidden units in the Dense layer
-            N_MIXES = 10  # number of mixture components
-            OUTPUT_DIMS = 2  # number of real-values predicted by each mixture component
-        
-            model = keras.Sequential()
-            model.add(keras.layers.Dense(N_HIDDEN, batch_input_shape=(None, 1), activation='relu'))
-            model.add(mdn.MDN(OUTPUT_DIMS, N_MIXES))
-            model.compile(loss=mdn.get_mixture_loss_func(OUTPUT_DIMS,N_MIXES), optimizer=keras.optimizers.Adam())
-            model.summary()
-        
-        Fit as normal:
-        
-            history = model.fit(x=x_train, y=y_train)
-        
-        The predictions from the network are parameters of the mixture models, so you have to apply the `sample_from_output` function to generate samples.
-        
-            y_test = model.predict(x_test)
-            y_samples = np.apply_along_axis(sample_from_output, 1, y_test, OUTPUT_DIMS, N_MIXES, temp=1.0)
-        
-        See the notebooks directory for examples in jupyter notebooks!
-        
-        ### Load/Save Model
-        
-        Saving models is straight forward:
-        
-            model.save('test_save.h5')
-        
-        But loading requires `cutom_objects` to be filled with the MDN layer, and a loss function with the appropriate parameters:
-        
-            m_2 = keras.models.load_model('test_save.h5', custom_objects={'MDN': mdn.MDN, 'mdn_loss_func': mdn.get_mixture_loss_func(1, N_MIXES)})
-        
-        
-        ## Acknowledgements
-        
-        - Hat tip to [Omimo's Keras MDN layer](https://github.com/omimo/Keras-MDN) for a starting point for this code.
-        - Super hat tip to [hardmaru's MDN explanation, projects, and good ideas for sampling functions](http://blog.otoro.net/2015/11/24/mixture-density-networks-with-tensorflow/) etc.
-        - Many good ideas from [Axel Brando's Master's Thesis](https://github.com/axelbrando/Mixture-Density-Networks-for-distribution-and-uncertainty-estimation)
-        - Mixture Density Networks in Edward [tutorial](http://edwardlib.org/tutorials/mixture-density-network).
-        
-        ## References
-        
-        1. Christopher M. Bishop. 1994. Mixture Density Networks. [Technical Report NCRG/94/004](http://publications.aston.ac.uk/373/). Neural Computing Research Group, Aston University. http://publications.aston.ac.uk/373/
-        2. Axel Brando. 2017. Mixture Density Networks (MDN) for distribution and uncertainty estimation. Master’s thesis. Universitat Politècnica de Catalunya.
-        3. A. Graves. 2013. Generating Sequences With Recurrent Neural Networks. ArXiv e-prints (Aug. 2013). https://arxiv.org/abs/1308.0850
-        4. David Ha and Douglas Eck. 2017. A Neural Representation of Sketch Drawings. ArXiv e-prints (April 2017). https://arxiv.org/abs/1704.03477
-        5. Charles P. Martin and Jim Torresen. 2018. RoboJam: A Musical Mixture Density Network for Collaborative Touchscreen Interaction. In Evolutionary and Biologically Inspired Music, Sound, Art and Design: EvoMUSART ’18, A. Liapis et al. (Ed.). Lecture Notes in Computer Science, Vol. 10783. Springer International Publishing. DOI:[10.1007/9778-3-319-77583-8_11](http://dx.doi.org/10.1007/9778-3-319-77583-8_11)
-        
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+# Keras Mixture Density Network Layer
+
+[![Build and test keras-mdn-layer](https://github.com/cpmpercussion/keras-mdn-layer/actions/workflows/python-app.yml/badge.svg)](https://github.com/cpmpercussion/keras-mdn-layer/actions/workflows/python-app.yml)
+![MIT License](https://img.shields.io/github/license/cpmpercussion/keras-mdn-layer.svg?style=flat)
+[![DOI](https://zenodo.org/badge/137585470.svg)](https://zenodo.org/badge/latestdoi/137585470)
+[![PyPI version](https://badge.fury.io/py/keras-mdn-layer.svg)](https://badge.fury.io/py/keras-mdn-layer)
+
+A mixture density network (MDN) Layer for Keras using TensorFlow's distributions module. This makes it a bit more simple to experiment with neural networks that predict multiple real-valued variables that can take on multiple equally likely values.
+
+This layer can help build MDN-RNNs similar to those used in [RoboJam](https://github.com/cpmpercussion/robojam), [Sketch-RNN](https://experiments.withgoogle.com/sketch-rnn-demo), [handwriting generation](https://distill.pub/2016/handwriting/), and maybe even [world models](https://worldmodels.github.io). You can do a lot of cool stuff with MDNs!
+
+One benefit of this implementation is that you can predict any number of real-values. TensorFlow's `Mixture`, `Categorical`, and `MultivariateNormalDiag` distribution functions are used to generate the loss function (the probability density function of a mixture of multivariate normal distributions with a diagonal covariance matrix). In previous work, the loss function has often been specified by hand which is fine for 1D or 2D prediction, but becomes a bit more annoying after that.
+
+Two important functions are provided for training and prediction:
+
+- `get_mixture_loss_func(output_dim, num_mixtures)`: This function generates a loss function with the correct output dimensiona and number of mixtures.
+- `sample_from_output(params, output_dim, num_mixtures, temp=1.0)`: This functions samples from the mixture distribution output by the model.
+
+## Installation 
+
+This project requires Python 3.6+, TensorFlow and TensorFlow Probability. You can easily install this package from [PyPI](https://pypi.org/project/keras-mdn-layer/) via `pip` like so:
+
+    python3 -m pip install keras-mdn-layer
+
+And finally, import the module in Python: `import keras_mdn_layer as mdn`
+
+Alternatively, you can clone or download this repository and then install via `python setup.py install`, or copy the `mdn` folder into your own project.
+
+## Examples
+
+Some examples are provided in the notebooks directory.
+
+There's scripts for fitting multivalued functions, a standard MDN toy problem:
+
+<img src="https://preview.ibb.co/mZzkpd/Keras_MDN_Demo.jpg" alt="Keras MDN Demo" border="0">
+
+There's also a script for generating fake kanji characters:
+
+<img src="https://i.ibb.co/yFvtgkL/kanji-mdn-examples.png" alt="kanji test 1" border="0" width="600"/>
+
+And finally, for learning how to generate musical touch-screen performances with a temporal component:
+
+<img src="https://i.ibb.co/WpzSCV8/robojam-examples.png" alt="Robojam Model Examples" border="0">
+
+## How to use
+
+The MDN layer should be the last in your network and you should use `get_mixture_loss_func` to generate a loss function. Here's an example of a simple network with one Dense layer followed by the MDN.
+
+    from tensorflow import keras
+    import keras_mdn_layer as mdn
+
+    N_HIDDEN = 15  # number of hidden units in the Dense layer
+    N_MIXES = 10  # number of mixture components
+    OUTPUT_DIMS = 2  # number of real-values predicted by each mixture component
+
+    model = keras.Sequential()
+    model.add(keras.layers.Dense(N_HIDDEN, batch_input_shape=(None, 1), activation='relu'))
+    model.add(mdn.MDN(OUTPUT_DIMS, N_MIXES))
+    model.compile(loss=mdn.get_mixture_loss_func(OUTPUT_DIMS,N_MIXES), optimizer=keras.optimizers.Adam())
+    model.summary()
+
+Fit as normal:
+
+    history = model.fit(x=x_train, y=y_train)
+
+The predictions from the network are parameters of the mixture models, so you have to apply the `sample_from_output` function to generate samples.
+
+    y_test = model.predict(x_test)
+    y_samples = np.apply_along_axis(sample_from_output, 1, y_test, OUTPUT_DIMS, N_MIXES, temp=1.0)
+
+See the notebooks directory for examples in jupyter notebooks!
+
+### Load/Save Model
+
+Saving models is straight forward:
+
+    model.save('test_save.h5')
+
+But loading requires `cutom_objects` to be filled with the MDN layer, and a loss function with the appropriate parameters:
+
+    m_2 = keras.models.load_model('test_save.h5', custom_objects={'MDN': mdn.MDN, 'mdn_loss_func': mdn.get_mixture_loss_func(1, N_MIXES)})
+
+
+## Acknowledgements
+
+- Hat tip to [Omimo's Keras MDN layer](https://github.com/omimo/Keras-MDN) for a starting point for this code.
+- Super hat tip to [hardmaru's MDN explanation, projects, and good ideas for sampling functions](http://blog.otoro.net/2015/11/24/mixture-density-networks-with-tensorflow/) etc.
+- Many good ideas from [Axel Brando's Master's Thesis](https://github.com/axelbrando/Mixture-Density-Networks-for-distribution-and-uncertainty-estimation)
+- Mixture Density Networks in Edward [tutorial](http://edwardlib.org/tutorials/mixture-density-network).
+
+## References
+
+1. Christopher M. Bishop. 1994. Mixture Density Networks. [Technical Report NCRG/94/004](http://publications.aston.ac.uk/373/). Neural Computing Research Group, Aston University. http://publications.aston.ac.uk/373/
+2. Axel Brando. 2017. Mixture Density Networks (MDN) for distribution and uncertainty estimation. Master’s thesis. Universitat Politècnica de Catalunya.
+3. A. Graves. 2013. Generating Sequences With Recurrent Neural Networks. ArXiv e-prints (Aug. 2013). https://arxiv.org/abs/1308.0850
+4. David Ha and Douglas Eck. 2017. A Neural Representation of Sketch Drawings. ArXiv e-prints (April 2017). https://arxiv.org/abs/1704.03477
+5. Charles P. Martin and Jim Torresen. 2018. RoboJam: A Musical Mixture Density Network for Collaborative Touchscreen Interaction. In Evolutionary and Biologically Inspired Music, Sound, Art and Design: EvoMUSART ’18, A. Liapis et al. (Ed.). Lecture Notes in Computer Science, Vol. 10783. Springer International Publishing. DOI:[10.1007/9778-3-319-77583-8_11](http://dx.doi.org/10.1007/9778-3-319-77583-8_11)
```

### Comparing `keras-mdn-layer-0.3.0/mdn/__init__.py` & `keras_mdn_layer-0.4.0/keras_mdn_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-mdn-layer-0.3.0/README.md` & `keras_mdn_layer-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,27 @@
+Metadata-Version: 2.1
+Name: keras-mdn-layer
+Version: 0.4.0
+Summary: An MDN Layer for Keras using TensorFlow's distributions module
+License: MIT
+Author: Charles Martin
+Author-email: cpm@charlesmartin.au
+Requires-Python: >=3.11,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: tensorflow (==2.15.0) ; sys_platform == "linux"
+Requires-Dist: tensorflow-macos (==2.15.0) ; sys_platform == "darwin"
+Requires-Dist: tensorflow-probability (==0.23.0)
+Description-Content-Type: text/markdown
+
 # Keras Mixture Density Network Layer
 
-[![Build Status](https://travis-ci.com/cpmpercussion/keras-mdn-layer.svg?branch=master)](https://travis-ci.com/cpmpercussion/keras-mdn-layer)
+[![Build and test keras-mdn-layer](https://github.com/cpmpercussion/keras-mdn-layer/actions/workflows/python-app.yml/badge.svg)](https://github.com/cpmpercussion/keras-mdn-layer/actions/workflows/python-app.yml)
 ![MIT License](https://img.shields.io/github/license/cpmpercussion/keras-mdn-layer.svg?style=flat)
 [![DOI](https://zenodo.org/badge/137585470.svg)](https://zenodo.org/badge/latestdoi/137585470)
 [![PyPI version](https://badge.fury.io/py/keras-mdn-layer.svg)](https://badge.fury.io/py/keras-mdn-layer)
 
 A mixture density network (MDN) Layer for Keras using TensorFlow's distributions module. This makes it a bit more simple to experiment with neural networks that predict multiple real-valued variables that can take on multiple equally likely values.
 
 This layer can help build MDN-RNNs similar to those used in [RoboJam](https://github.com/cpmpercussion/robojam), [Sketch-RNN](https://experiments.withgoogle.com/sketch-rnn-demo), [handwriting generation](https://distill.pub/2016/handwriting/), and maybe even [world models](https://worldmodels.github.io). You can do a lot of cool stuff with MDNs!
@@ -14,19 +31,19 @@
 Two important functions are provided for training and prediction:
 
 - `get_mixture_loss_func(output_dim, num_mixtures)`: This function generates a loss function with the correct output dimensiona and number of mixtures.
 - `sample_from_output(params, output_dim, num_mixtures, temp=1.0)`: This functions samples from the mixture distribution output by the model.
 
 ## Installation 
 
-This project requires Python 3.6+. You can easily install this package from [PyPI](https://pypi.org/project/keras-mdn-layer/) via `pip` like so:
+This project requires Python 3.6+, TensorFlow and TensorFlow Probability. You can easily install this package from [PyPI](https://pypi.org/project/keras-mdn-layer/) via `pip` like so:
 
     python3 -m pip install keras-mdn-layer
 
-And finally, import the `mdn` module in Python: `import mdn`
+And finally, import the module in Python: `import keras_mdn_layer as mdn`
 
 Alternatively, you can clone or download this repository and then install via `python setup.py install`, or copy the `mdn` folder into your own project.
 
 ## Examples
 
 Some examples are provided in the notebooks directory.
 
@@ -42,16 +59,16 @@
 
 <img src="https://i.ibb.co/WpzSCV8/robojam-examples.png" alt="Robojam Model Examples" border="0">
 
 ## How to use
 
 The MDN layer should be the last in your network and you should use `get_mixture_loss_func` to generate a loss function. Here's an example of a simple network with one Dense layer followed by the MDN.
 
-    import keras
-    import mdn
+    from tensorflow import keras
+    import keras_mdn_layer as mdn
 
     N_HIDDEN = 15  # number of hidden units in the Dense layer
     N_MIXES = 10  # number of mixture components
     OUTPUT_DIMS = 2  # number of real-values predicted by each mixture component
 
     model = keras.Sequential()
     model.add(keras.layers.Dense(N_HIDDEN, batch_input_shape=(None, 1), activation='relu'))
@@ -91,7 +108,8 @@
 ## References
 
 1. Christopher M. Bishop. 1994. Mixture Density Networks. [Technical Report NCRG/94/004](http://publications.aston.ac.uk/373/). Neural Computing Research Group, Aston University. http://publications.aston.ac.uk/373/
 2. Axel Brando. 2017. Mixture Density Networks (MDN) for distribution and uncertainty estimation. Master’s thesis. Universitat Politècnica de Catalunya.
 3. A. Graves. 2013. Generating Sequences With Recurrent Neural Networks. ArXiv e-prints (Aug. 2013). https://arxiv.org/abs/1308.0850
 4. David Ha and Douglas Eck. 2017. A Neural Representation of Sketch Drawings. ArXiv e-prints (April 2017). https://arxiv.org/abs/1704.03477
 5. Charles P. Martin and Jim Torresen. 2018. RoboJam: A Musical Mixture Density Network for Collaborative Touchscreen Interaction. In Evolutionary and Biologically Inspired Music, Sound, Art and Design: EvoMUSART ’18, A. Liapis et al. (Ed.). Lecture Notes in Computer Science, Vol. 10783. Springer International Publishing. DOI:[10.1007/9778-3-319-77583-8_11](http://dx.doi.org/10.1007/9778-3-319-77583-8_11)
+
```

