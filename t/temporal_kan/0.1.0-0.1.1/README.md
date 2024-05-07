# Comparing `tmp/temporal_kan-0.1.0.tar.gz` & `tmp/temporal_kan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temporal_kan-0.1.0.tar", max compression
+gzip compressed data, was "temporal_kan-0.1.1.tar", max compression
```

## Comparing `temporal_kan-0.1.0.tar` & `temporal_kan-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      489 2024-05-07 12:34:24.615303 temporal_kan-0.1.0/README.md
--rw-r--r--   0        0        0      410 2024-05-07 13:07:15.540482 temporal_kan-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      613 2024-05-07 13:15:31.231940 temporal_kan-0.1.0/temporal_kan/__init__.py
--rw-r--r--   0        0        0     6069 2024-05-07 13:36:07.241550 temporal_kan-0.1.0/temporal_kan/glstm.py
--rw-r--r--   0        0        0     3805 2024-05-07 13:36:08.725557 temporal_kan-0.1.0/temporal_kan/gr.py
--rw-r--r--   0        0        0     4213 2024-05-07 13:36:10.609567 temporal_kan-0.1.0/temporal_kan/sltsm.py
--rw-r--r--   0        0        0      132 2024-05-07 13:02:40.269087 temporal_kan-0.1.0/temporal_kan/spline.py
--rw-r--r--   0        0        0     3472 2024-05-07 13:36:05.109539 temporal_kan-0.1.0/temporal_kan/sr.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 temporal_kan-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      489 2024-05-07 12:34:24.615303 temporal_kan-0.1.1/README.md
+-rw-r--r--   0        0        0      411 2024-05-07 14:02:23.161227 temporal_kan-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      613 2024-05-07 13:15:31.231940 temporal_kan-0.1.1/temporal_kan/__init__.py
+-rw-r--r--   0        0        0     6021 2024-05-07 13:56:07.437067 temporal_kan-0.1.1/temporal_kan/glstm.py
+-rw-r--r--   0        0        0     3757 2024-05-07 13:56:12.573077 temporal_kan-0.1.1/temporal_kan/gr.py
+-rw-r--r--   0        0        0     4165 2024-05-07 13:56:18.197088 temporal_kan-0.1.1/temporal_kan/sltsm.py
+-rw-r--r--   0        0        0      132 2024-05-07 13:02:40.269087 temporal_kan-0.1.1/temporal_kan/spline.py
+-rw-r--r--   0        0        0     3424 2024-05-07 13:56:26.321103 temporal_kan-0.1.1/temporal_kan/sr.py
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 temporal_kan-0.1.1/PKG-INFO
```

### Comparing `temporal_kan-0.1.0/temporal_kan/__init__.py` & `temporal_kan-0.1.1/temporal_kan/__init__.py`

 * *Files identical despite different names*

### Comparing `temporal_kan-0.1.0/temporal_kan/glstm.py` & `temporal_kan-0.1.1/temporal_kan/glstm.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.aggregation_transform = tf.keras.layers.Dense(num_outputs, activation=power_spline(act))
 
 
         # Sub-layer LSTM components
         self.sub_layers = []
         self.sub_lstm_gates = {'input': [], 'forget': [], 'output': [], 'cell': []}
         for act in activation_funcs:
-            self.sub_layers.append(tf.keras.layers.Dense(1, activation=power_spline(act) if isinstance(act, (int, float, np.float32, np.float64, tf.float32, tf.float64)) else act))
+            self.sub_layers.append(tf.keras.layers.Dense(1, activation=power_spline(act) if isinstance(act, (int, float)) else act))
             for gate in ['input', 'forget', 'output', 'cell']:
                 self.sub_lstm_gates[gate].append(
                     self.add_weight(shape=(1, 1), initializer='glorot_uniform', trainable=True))
 
         # Global LSTM gate weights
         self.global_lstm_gates = {
             'Wi': self.add_weight(shape=(self.num_outputs, self.num_outputs), initializer='glorot_uniform', trainable=True),
```

### Comparing `temporal_kan-0.1.0/temporal_kan/gr.py` & `temporal_kan-0.1.1/temporal_kan/gr.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.num_outputs = num_outputs
         self.recurrent_activation = tf.keras.activations.get(recurrent_activation)
         self.return_sequences = return_sequences
         self.recurrent_dropout = recurrent_dropout
         self.kernel_regularizer = regularizers.get(kernel_regularizer)
         self.recurrent_regularizer = regularizers.get(recurrent_regularizer)
         self.bias_regularizer = regularizers.get(bias_regularizer)
-        self.sub_layers = [Dense(1, activation=power_spline(act) if isinstance(act, (int, float, np.float32, np.float64, tf.float32, tf.float64)) else act,
+        self.sub_layers = [Dense(1, activation=power_spline(act) if isinstance(act, (int, float)) else act,
                                  kernel_regularizer=self.kernel_regularizer,
                                  bias_regularizer=self.bias_regularizer)
                            for act in activation_funcs]
 
         # Recurrent kernels for each sub-layer
         self.sub_recurrent_kernels = [self.add_weight(shape=(1, 1), initializer='uniform', trainable=True, regularizer=self.kernel_regularizer) for _ in activation_funcs]
         # Global recurrent kernel
```

### Comparing `temporal_kan-0.1.0/temporal_kan/sltsm.py` & `temporal_kan-0.1.1/temporal_kan/sltsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class SLSTM_KAN(Layer):
     def __init__(self, activation_funcs: List[str | int], num_outputs: int, return_sequences: bool = False, recurrent_dropout : float = 0.0, **kwargs):
         super(SLSTM_KAN, self).__init__(**kwargs)
         self.activation_funcs = activation_funcs
         self.num_outputs = num_outputs
         self.return_sequences = return_sequences
         self.recurrent_dropout = recurrent_dropout
-        self.sub_layers = [tf.keras.layers.Dense(1, activation=power_spline(act) if isinstance(act, (int, float, np.float32, np.float64, tf.float32, tf.float64)) else act) for act in activation_funcs]
+        self.sub_layers = [tf.keras.layers.Dense(1, activation=power_spline(act) if isinstance(act, (int, float)) else act) for act in activation_funcs]
 
         # LSTM gate weights
         self.Wi = self.add_weight(shape=(self.num_outputs, self.num_outputs), initializer='glorot_uniform', trainable=True)
         self.Wf = self.add_weight(shape=(self.num_outputs, self.num_outputs), initializer='glorot_uniform', trainable=True)
         self.Wo = self.add_weight(shape=(self.num_outputs, self.num_outputs), initializer='glorot_uniform', trainable=True)
         self.Wc = self.add_weight(shape=(self.num_outputs, self.num_outputs), initializer='glorot_uniform', trainable=True)
```

### Comparing `temporal_kan-0.1.0/temporal_kan/sr.py` & `temporal_kan-0.1.1/temporal_kan/sr.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.recurrent_dropout = recurrent_dropout
         self.recurrent_activation = tf.keras.activations.get(recurrent_activation)
         self.kernel_regularizer = regularizers.get(kernel_regularizer)
         self.recurrent_regularizer = regularizers.get(recurrent_regularizer)
         self.bias_regularizer = regularizers.get(bias_regularizer)
 
         # Initialize sub_layers with regularizers
-        self.sub_layers = [Dense(1, activation=power_spline(act) if isinstance(act, (int, float, np.float32, np.float64, tf.float32, tf.float64)) else act,
+        self.sub_layers = [Dense(1, activation=power_spline(act) if isinstance(act, (int, float)) else act,
                                  kernel_regularizer=self.kernel_regularizer,
                                  bias_regularizer=self.bias_regularizer)
                            for act in activation_funcs]
 
     def build(self, input_shape):
         # Aggregation weights that combine outputs from each sub-layer
         self.aggregation_weights = self.add_weight(
```

### Comparing `temporal_kan-0.1.0/PKG-INFO` & `temporal_kan-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: temporal_kan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Temporal KAN model
 Author: Rémi Genet
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.2,<2)
 Requires-Dist: pyarrow (>=15.0.0)
 Requires-Dist: tensorflow (>=2.14,<2.16)
 Description-Content-Type: text/markdown
 
 # REPONAME
```

