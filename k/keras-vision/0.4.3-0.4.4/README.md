# Comparing `tmp/keras-vision-0.4.3.tar.gz` & `tmp/keras_vision-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-vision-0.4.3.tar", last modified: Sun May  5 19:00:49 2024, max compression
+gzip compressed data, was "keras_vision-0.4.4.tar", last modified: Tue May  7 20:45:48 2024, max compression
```

## Comparing `keras-vision-0.4.3.tar` & `keras_vision-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:00:49.632152 keras-vision-0.4.3/
--rw-rw-rw-   0        0        0     1396 2024-05-05 19:00:49.630149 keras-vision-0.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-05 19:00:49.613615 keras-vision-0.4.3/keras_vision/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:00:49.629142 keras-vision-0.4.3/keras_vision/MobileViT_v1/
--rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras-vision-0.4.3/keras_vision/MobileViT_v1/__init__.py
--rw-rw-rw-   0        0        0     4516 2024-05-03 18:38:00.000000 keras-vision-0.4.3/keras_vision/MobileViT_v1/base_layers.py
--rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras-vision-0.4.3/keras_vision/MobileViT_v1/configs.py
--rw-rw-rw-   0        0        0     8177 2024-05-05 18:59:51.000000 keras-vision-0.4.3/keras_vision/MobileViT_v1/mobile_vit_v1.py
--rw-rw-rw-   0        0        0    13452 2024-05-05 15:29:51.000000 keras-vision-0.4.3/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
--rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras-vision-0.4.3/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
--rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.4.3/keras_vision/MobileViT_v1/utils.py
--rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.4.3/keras_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:00:49.621153 keras-vision-0.4.3/keras_vision.egg-info/
--rw-rw-rw-   0        0        0     1396 2024-05-05 19:00:49.000000 keras-vision-0.4.3/keras_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-05 19:00:49.000000 keras-vision-0.4.3/keras_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:00:49.000000 keras-vision-0.4.3/keras_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-05 19:00:49.000000 keras-vision-0.4.3/keras_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-05 19:00:49.000000 keras-vision-0.4.3/keras_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 19:00:49.632152 keras-vision-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1832 2024-05-05 19:00:35.000000 keras-vision-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:45:48.011488 keras_vision-0.4.4/
+-rw-rw-rw-   0        0        0     1455 2024-05-07 20:45:48.009487 keras_vision-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-05-03 19:13:27.000000 keras_vision-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 20:45:47.982475 keras_vision-0.4.4/keras_vision/
+drwxrwxrwx   0        0        0        0 2024-05-07 20:45:48.006472 keras_vision-0.4.4/keras_vision/MobileViT_v1/
+-rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/__init__.py
+-rw-rw-rw-   0        0        0     4662 2024-05-07 20:24:40.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/base_layers.py
+-rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/configs.py
+-rw-rw-rw-   0        0        0     6418 2024-05-07 20:28:52.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/extras.py
+-rw-rw-rw-   0        0        0     8177 2024-05-07 11:37:39.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1.py
+-rw-rw-rw-   0        0        0    10286 2024-05-07 20:32:59.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
+-rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
+-rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras_vision-0.4.4/keras_vision/MobileViT_v1/utils.py
+-rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras_vision-0.4.4/keras_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:45:48.008478 keras_vision-0.4.4/keras_vision.egg-info/
+-rw-rw-rw-   0        0        0     1455 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       58 2024-05-07 20:45:47.000000 keras_vision-0.4.4/keras_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1322 2024-05-07 20:45:09.000000 keras_vision-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 20:45:48.012472 keras_vision-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1832 2024-05-07 20:35:22.000000 keras_vision-0.4.4/setup.py
```

### Comparing `keras-vision-0.4.3/PKG-INFO` & `keras_vision-0.4.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4.3
-Summary: Building Vision models in Keras3 for framework agnostic training and inference.
+Version: 0.4.4
+Summary: Building Vision models in Keras3 for framework-agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
-Author-email: vaibhav.singh.3001@gmail.com
-License: Apache 2.0
-Keywords: keras3 tensorflow Jax PyTorch Vision
+Author-email: Vaibhav Singh <vaibhav.singh.3001@gmail.com>
+Project-URL: Homepage, https://github.com/veb-101/keras-vision
+Keywords: keras3,tensorflow,Jax,PyTorch,Vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `keras-vision-0.4.3/keras_vision/MobileViT_v1/base_layers.py` & `keras_vision-0.4.4/keras_vision/MobileViT_v1/base_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
         if self.use_bn:
             self.bn = BatchNormalization(epsilon=1e-05, momentum=0.1)
 
         if self.use_activation:
             self.activation = Activation("swish")
 
+    def build(self, input_shape):
+        super().build(input_shape)
+
     def call(self, x, **kwargs):
         x = self.zero_pad(x)
         x = self.conv(x)
         if self.use_bn:
             x = self.bn(x)
 
         if self.use_activation:
@@ -100,14 +103,17 @@
 
         self.depthwise_conv_zero_pad = ZeroPadding2D(padding=(1, 1))
         self.depthwise_conv = DepthwiseConv2D(kernel_size=3, strides=self.depthwise_stride, padding="valid", use_bias=False)
         self.bn = BatchNormalization(epsilon=1e-05, momentum=0.1)
         self.activation = Activation("swish")
         self.out_conv_block = ConvLayer(num_filters=num_out_channels, kernel_size=1, strides=1, use_activation=False, use_bn=True)
 
+    def build(self, input_shape):
+        super().build(input_shape)
+
     def call(self, data, **kwargs):
         out = self.expansion_conv_block(data)
         out = self.depthwise_conv_zero_pad(out)
         out = self.depthwise_conv(out)
         out = self.bn(out)
         out = self.activation(out)
         out = self.out_conv_block(out)
```

### Comparing `keras-vision-0.4.3/keras_vision/MobileViT_v1/configs.py` & `keras_vision-0.4.4/keras_vision/MobileViT_v1/configs.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.3/keras_vision/MobileViT_v1/mobile_vit_v1.py` & `keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.3/keras_vision/MobileViT_v1/mobile_vit_v1_block.py` & `keras_vision-0.4.4/keras_vision/MobileViT_v1/mobile_vit_v1_block.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         hidden_features = int(self.embedding_dim * self.mlp_ratio)
 
         self.mlp_block_0 = Dense(hidden_features, activation="swish")
         self.mlp_block_1 = Dropout(self.linear_drop)
         self.mlp_block_2 = Dense(embedding_dim)
         self.mlp_block_3 = Dropout(dropout)
 
+    def build(self, input_shape):
+        super().build(input_shape)
+
     def call(self, x):
         x = x + self.attn(self.norm_1(x))
 
         mlp_block_out = self.mlp_block_0(self.norm_2(x))
         mlp_block_out = self.mlp_block_1(mlp_block_out)
         mlp_block_out = self.mlp_block_2(mlp_block_out)
         mlp_block_out = self.mlp_block_3(mlp_block_out)
@@ -70,59 +73,14 @@
                 "dropout": self.dropout,
                 "linear_drop": self.linear_drop,
                 "attention_drop": self.attention_drop,
             }
         )
         return config
 
-    @classmethod
-    def from_config(cls, config):
-        return cls(**config)
-
-
-# # https://github.com/apple/ml-cvnets/blob/84d992f413e52c0468f86d23196efd9dad885e6f/cvnets/modules/mobilevit_blockops.py#L186
-# def unfolding(
-#     x,
-#     B: int = 1,
-#     D: int = 144,
-#     patch_h: int = 2,
-#     patch_w: int = 2,
-#     num_patches_h: int = 10,
-#     num_patches_w: int = 10,
-# ):
-#     """
-#     ### Notations (wrt paper) ###
-#         B/b = batch
-#         P/p = patch_size
-#         N/n = number of patches
-#         D/d = embedding_dim
-
-#     H, W
-#     [                            [
-#         [1, 2, 3, 4],     Goal      [1, 3, 9, 11],
-#         [5, 6, 7, 8],     ====>     [2, 4, 10, 12],
-#         [9, 10, 11, 12],            [5, 7, 13, 15],
-#         [13, 14, 15, 16],           [6, 8, 14, 16]
-#     ]                            ]
-# #     """
-#     # print("B", B)
-#     # [B, H, W, D] --> [B*nh, ph, nw, pw*D]
-#     reshaped_fm = kops.reshape(x, (B * num_patches_h, patch_h, num_patches_w, patch_w * D))
-
-#     # [B*nh, ph, nw, pw*D] --> [B*nh, nw, ph, pw*D]
-#     transposed_fm = kops.transpose(reshaped_fm, axes=[0, 2, 1, 3])
-
-#     # [B*nh, nw, ph, pw*D] --> [B, N, P, D]
-#     reshaped_fm = kops.reshape(transposed_fm, (B, num_patches_h * num_patches_w, patch_h * patch_w, D))
-
-#     # [B, N, P, D] --> [B, P, N, D]
-#     transposed_fm = kops.transpose(reshaped_fm, axes=[0, 2, 1, 3])
-
-#     return transposed_fm
-
 
 class MobileViT_v1_Block(Layer):
     def __init__(
         self,
         out_filters: int = 64,
         embedding_dim: int = 90,
         patch_size: Union[int, tuple] = 2,
@@ -169,61 +127,42 @@
         self.concat = Concatenate(axis=-1)
         self.fuse_local_global = ConvLayer(num_filters=self.out_filters, kernel_size=3, strides=1, use_bn=True, use_activation=True)
 
     def build(self, input_shape):
         super().build(input_shape)
 
     def call(self, x):
-
-        fmH, fmW = kops.shape(x)[1], kops.shape(x)[2]
-
+        # Local Representation
         local_representation = self.local_rep_layer_1(x)
         local_representation = self.local_rep_layer_2(local_representation)
-        out_channels = local_representation.shape[-1]
 
         # Transformer as Convolution Steps
         # --------------------------------
         # # Unfolding
 
         unfolded, info_dict = self.unfolding(local_representation)
 
         # # Infomation sharing/mixing --> global representation
         for layer in self.transformer_layers:
             unfolded = layer(unfolded)
 
         global_representation = self.transformer_layer_norm(unfolded)
 
-        # #Folding
-        folded = self.folding(global_representation, info_dict=info_dict, outH=fmH, outW=fmW, outC=out_channels)
+        # # Folding
+        folded = self.folding(global_representation, info_dict=info_dict)
+        # --------------------------------
 
         # Fusion
         local_mix = self.local_features_3(folded)
         fusion = self.concat([x, local_mix])
         fusion = self.fuse_local_global(fusion)
 
         return fusion
 
-    def get_config(self):
-        config = super().get_config()
-        config.update(
-            {
-                "out_filters": self.out_filters,
-                "embedding_dim": self.embedding_dim,
-                "patch_size": self.patch_size,
-                "transformer_repeats": self.transformer_repeats,
-                "num_heads": self.num_heads,
-                "dropout": self.dropout,
-                "attention_drop": self.attention_drop,
-                "linear_drop": self.linear_drop,
-            }
-        )
-        return config
-
-    # https://github.com/apple/ml-cvnets/blob/84d992f413e52c0468f86d23196efd9dad885e6f/cvnets/modules/mobilevit_blockops.py#L186
-    def unfolding(self, feature_map):
+    def unfolding(self, x):
         """
         ### Notations (wrt paper) ###
             B/b = batch
             P/p = patch_size
             N/n = number of patches
             D/d = embedding_dim
 
@@ -233,111 +172,102 @@
             [5, 6, 7, 8],     ====>     [2, 4, 10, 12],
             [9, 10, 11, 12],            [5, 7, 13, 15],
             [13, 14, 15, 16],           [6, 8, 14, 16]
         ]                            ]
         """
 
         # Initially convert channel-last to channel-first for processing
-        shape = kops.shape(feature_map)
-        batch_size, orig_h, orig_w, in_channels = shape[0], shape[1], shape[2], shape[3]
-        feature_map = kops.transpose(feature_map, [0, 3, 1, 2])  # [B, H, W, C] -> [B, C, H, W]
+        shape = kops.shape(x)
+        batch_size, orig_h, orig_w, D = shape[0], shape[1], shape[2], shape[3]
 
         patch_area = self.patch_size_w * self.patch_size_h
 
         orig_h, orig_w = kops.cast(orig_h, dtype="int32"), kops.cast(orig_w, dtype="int32")
+        num_patches_h = orig_h // self.patch_size_h
+        num_patches_w = orig_w // self.patch_size_w
+        num_patches = kops.cast(num_patches_h * num_patches_w, dtype="int32")
 
-        h_ceil = kops.ceil(orig_h / self.patch_size_h)
-        w_ceil = kops.ceil(orig_w / self.patch_size_w)
+        # Handle dynamic shape multiplication
+        dynamic_shape_mul = kops.prod([batch_size, num_patches_h])
 
-        new_h = kops.cast(h_ceil * kops.cast(self.patch_size_h, dtype=h_ceil.dtype), dtype="int32")
-        new_w = kops.cast(w_ceil * kops.cast(self.patch_size_w, dtype=h_ceil.dtype), dtype="int32")
+        # [B, H, W, D] --> [B*nh, ph, nw, pw*D]
+        reshaped_fm = kops.reshape(x, (dynamic_shape_mul, self.patch_size_h, num_patches_w, self.patch_size_w * D))
 
-        # Condition to decide if resizing is necessary
-        resize_required = kops.logical_or(kops.not_equal(new_w, orig_w), kops.not_equal(new_h, orig_h))
-        feature_map = kops.cond(
-            resize_required,
-            true_fn=lambda: kops.image.resize(feature_map, [new_h, new_w], data_format="channels_first"),
-            false_fn=lambda: feature_map,
-        )
+        # [B * n_h, p_h, n_w, p_w*D] --> [B * n_h, n_w, p_h, p_w * D]
+        transposed_fm = kops.transpose(reshaped_fm, axes=[0, 2, 1, 3])
 
-        num_patch_h = new_h // self.patch_size_h
-        num_patch_w = new_w // self.patch_size_w
-        num_patches = num_patch_h * num_patch_w
+        # [B * n_h, n_w, p_h, p_w * D] --> [B, N, P, D] where P = p_h * p_w and N = n_h * n_w
+        reshaped_fm = kops.reshape(transposed_fm, (batch_size, num_patches, patch_area, D))
 
-        # Handle dynamic shape multiplication
-        dynamic_shape_mul = kops.prod([batch_size, in_channels * num_patch_h])
+        # [B, N, P, D] --> [B, P, N, D]
+        transposed_fm = kops.transpose(reshaped_fm, axes=[0, 2, 1, 3])
 
-        # Reshape and transpose to create patches
-        reshaped_fm = kops.reshape(feature_map, [dynamic_shape_mul, self.patch_size_h, num_patch_w, self.patch_size_w])
-        transposed_fm = kops.transpose(reshaped_fm, [0, 2, 1, 3])
-        reshaped_fm = kops.reshape(transposed_fm, [batch_size, in_channels, num_patches, patch_area])
-        transposed_fm = kops.transpose(reshaped_fm, [0, 3, 2, 1])
-        patches = kops.reshape(transposed_fm, [batch_size * patch_area, num_patches, in_channels])
+        # [B, P, N, D] -> [BP, N, D]
+        patches = kops.reshape(transposed_fm, [batch_size * patch_area, num_patches, D])
 
         info_dict = {
-            "orig_size": (orig_h, orig_w),
             "batch_size": batch_size,
-            "interpolate": resize_required,
             "total_patches": num_patches,
-            "num_patches_w": num_patch_w,
-            "num_patches_h": num_patch_h,
+            "num_patches_h": num_patches_h,
+            "num_patches_w": num_patches_w,
             "patch_area": patch_area,
         }
 
         return patches, info_dict
 
-    def folding(self, patches, info_dict, outH, outW, outC):
-        # Ensure the input patches tensor has the correct dimensions
-        assert len(patches.shape) == 3, f"Tensor should be of shape BPxNxC. Got: {patches.shape}"
-
-        # Reshape to [B, P, N, C]
-        patches = kops.reshape(patches, [info_dict["batch_size"], info_dict["patch_area"], info_dict["total_patches"], -1])
+    def folding(self, x, info_dict):
+        """
+        ### Notations (wrt paper) ###
+            B/b = batch
+            P/p = patch_size
+            N/n = number of patches
+            D/d = embedding_dim
+        """
 
         # Get shape parameters for further processing
-        shape = kops.shape(patches)
-        batch_size = shape[0]
-        channels = shape[3]
-
+        shape = kops.shape(x)
+        D = shape[2]
+        batch_size = info_dict["batch_size"]
+        num_patches = info_dict["total_patches"]
         num_patch_h = info_dict["num_patches_h"]
         num_patch_w = info_dict["num_patches_w"]
+        patch_area = info_dict["patch_area"]
 
-        # Transpose dimensions [B, P, N, C] --> [B, C, N, P]
-        patches = kops.transpose(patches, [0, 3, 2, 1])
+        # Reshape to [BP, N, D] -> [B, P, N, D]
+        x = kops.reshape(x, [batch_size, patch_area, num_patches, D])
 
-        # Calculate total elements dynamically
-        num_total_elements = batch_size * channels * num_patch_h
+        # [B, P, N D] --> [B, N, P, D]
+        x = kops.transpose(x, (0, 2, 1, 3))
 
-        # Reshape to match the size of the feature map before splitting into patches
-        # [B, C, N, P] --> [B*C*n_h, n_w, p_h, p_w]
-        feature_map = kops.reshape(patches, [num_total_elements, num_patch_w, self.patch_size_h, self.patch_size_w])
-
-        # Transpose to switch width and height axes [B*C*n_h, n_w, p_h, p_w] --> [B*C*n_h, p_h, n_w, p_w]
-        feature_map = kops.transpose(feature_map, [0, 2, 1, 3])
-
-        # Reshape back to the original image dimensions [B*C*n_h, p_h, n_w, p_w] --> [B, C, H, W]
-        # Reshape back to [B, C, H, W]
-        new_height = num_patch_h * self.patch_size_h
-        new_width = num_patch_w * self.patch_size_w
-        feature_map = kops.reshape(feature_map, [batch_size, -1, new_height, new_width])
-
-        # Conditional resizing using kops.cond
-        feature_map = kops.cond(
-            info_dict["interpolate"],
-            lambda: kops.image.resize(feature_map, info_dict["orig_size"], data_format="channels_first"),
-            lambda: feature_map,
-        )
+        # [B, N, P, D] --> [B *n_h, n_w, p_h, p_w * D]
+        x = kops.reshape(x, (batch_size * num_patch_h, num_patch_w, self.patch_size_h, self.patch_size_w * D))
 
-        feature_map = kops.transpose(feature_map, [0, 2, 3, 1])
-        feature_map = kops.reshape(feature_map, (batch_size, outH, outW, outC))
+        # [B *n_h, n_w, p_h, p_w * D] --> [B * n_h, p_h, n_w, p_w * D]
+        x = kops.transpose(x, (0, 2, 1, 3))
 
-        return feature_map
+        # [B * n_h, p_h, n_w, p_w * D] --> [B, n_h * p_h, n_w, p_w, D] --> [B, H, W, C]
+        x = kops.reshape(x, (batch_size, num_patch_h * self.patch_size_h, num_patch_w * self.patch_size_w, D))
 
-    @classmethod
-    def from_config(cls, config):
-        return cls(**config)
+        return x
+
+    def get_config(self):
+        config = super().get_config()
+        config.update(
+            {
+                "out_filters": self.out_filters,
+                "embedding_dim": self.embedding_dim,
+                "patch_size": self.patch_size,
+                "transformer_repeats": self.transformer_repeats,
+                "num_heads": self.num_heads,
+                "dropout": self.dropout,
+                "attention_drop": self.attention_drop,
+                "linear_drop": self.linear_drop,
+            }
+        )
+        return config
 
 
 if __name__ == "__main__":
     batch = 1
     H = W = 32
     C = 48
     P = 2 * 2
```

### Comparing `keras-vision-0.4.3/keras_vision/MobileViT_v1/multihead_self_attention_2D.py` & `keras_vision-0.4.4/keras_vision/MobileViT_v1/multihead_self_attention_2D.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.3/keras_vision/MobileViT_v1/utils.py` & `keras_vision-0.4.4/keras_vision/MobileViT_v1/utils.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.3/keras_vision.egg-info/PKG-INFO` & `keras_vision-0.4.4/keras_vision.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4.3
-Summary: Building Vision models in Keras3 for framework agnostic training and inference.
+Version: 0.4.4
+Summary: Building Vision models in Keras3 for framework-agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
-Author-email: vaibhav.singh.3001@gmail.com
-License: Apache 2.0
-Keywords: keras3 tensorflow Jax PyTorch Vision
+Author-email: Vaibhav Singh <vaibhav.singh.3001@gmail.com>
+Project-URL: Homepage, https://github.com/veb-101/keras-vision
+Keywords: keras3,tensorflow,Jax,PyTorch,Vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `keras-vision-0.4.3/setup.py` & `keras_vision-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 DESCRIPTION = "Building Vision models in Keras3 for framework agnostic training and inference."
 
 # Setting up
 setup(
     name="keras-vision",
     version=__version__,
     author="Vaibhav Singh",
```

