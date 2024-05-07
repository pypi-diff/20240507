# Comparing `tmp/pssr-1.2.1.tar.gz` & `tmp/pssr-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.2.1.tar", max compression
+gzip compressed data, was "pssr-1.2.2.tar", max compression
```

## Comparing `pssr-1.2.1.tar` & `pssr-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.2.1/LICENSE
--rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.2.1/pssr/__init__.py
--rw-r--r--   0        0        0     4934 2024-05-01 03:00:25.746754 pssr-1.2.1/pssr/__main__.py
--rw-r--r--   0        0        0     4678 2024-05-02 02:57:56.749173 pssr-1.2.1/pssr/crappifiers.py
--rw-r--r--   0        0        0    32730 2024-05-01 17:09:11.249481 pssr-1.2.1/pssr/data.py
--rw-r--r--   0        0        0     2662 2024-05-02 00:48:45.425156 pssr-1.2.1/pssr/loss.py
--rw-r--r--   0        0        0       84 2024-05-02 16:17:46.536616 pssr-1.2.1/pssr/models/__init__.py
--rw-r--r--   0        0        0     4671 2024-05-02 16:04:40.293835 pssr-1.2.1/pssr/models/_blocks.py
--rw-r--r--   0        0        0     8046 2024-05-01 15:20:32.105611 pssr-1.2.1/pssr/models/_rdnet.py
--rw-r--r--   0        0        0     7617 2024-05-02 16:03:50.417239 pssr-1.2.1/pssr/models/rdresunet.py
--rw-r--r--   0        0        0     6955 2024-05-01 03:02:41.421290 pssr-1.2.1/pssr/models/resunet.py
--rw-r--r--   0        0        0    11138 2024-05-02 01:49:54.825731 pssr-1.2.1/pssr/predict.py
--rw-r--r--   0        0        0    13435 2024-05-02 16:31:42.218290 pssr-1.2.1/pssr/train.py
--rw-r--r--   0        0        0     1132 2024-05-02 16:16:58.819917 pssr-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 pssr-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.2.2/pssr/__init__.py
+-rw-r--r--   0        0        0     5574 2024-05-07 03:46:32.512042 pssr-1.2.2/pssr/__main__.py
+-rw-r--r--   0        0        0     4678 2024-05-02 02:57:56.749173 pssr-1.2.2/pssr/crappifiers.py
+-rw-r--r--   0        0        0    32650 2024-05-07 03:25:12.982266 pssr-1.2.2/pssr/data.py
+-rw-r--r--   0        0        0     2662 2024-05-02 00:48:45.425156 pssr-1.2.2/pssr/loss.py
+-rw-r--r--   0        0        0      111 2024-05-02 18:58:16.599258 pssr-1.2.2/pssr/models/__init__.py
+-rw-r--r--   0        0        0     4671 2024-05-02 16:04:40.293835 pssr-1.2.2/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     8046 2024-05-01 15:20:32.105611 pssr-1.2.2/pssr/models/_rdnet.py
+-rw-r--r--   0        0        0     7682 2024-05-06 03:52:11.907243 pssr-1.2.2/pssr/models/rdresunet.py
+-rw-r--r--   0        0        0     6955 2024-05-07 02:36:15.775241 pssr-1.2.2/pssr/models/resunet.py
+-rw-r--r--   0        0        0    34796 2024-05-07 03:10:57.785540 pssr-1.2.2/pssr/models/swinir.py
+-rw-r--r--   0        0        0    11516 2024-05-07 03:33:47.653002 pssr-1.2.2/pssr/predict.py
+-rw-r--r--   0        0        0    14608 2024-05-06 04:09:07.918747 pssr-1.2.2/pssr/train.py
+-rw-r--r--   0        0        0     1133 2024-05-07 03:47:03.696502 pssr-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 pssr-1.2.2/PKG-INFO
```

### Comparing `pssr-1.2.1/LICENSE` & `pssr-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.2.1/README.md` & `pssr-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pssr-1.2.1/pssr/__main__.py` & `pssr-1.2.2/pssr/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 sys.path.append("..")
 
 import torch, argparse
 from torch.nn import MSELoss
-from pssr.models import ResUNet, ResUNetA, RDResUNet, RDResUNetA
+from pssr.models import ResUNet, ResUNetA, RDResUNet, RDResUNetA, SwinIR
 from pssr.data import ImageDataset, SlidingDataset, PairedImageDataset, PairedSlidingDataset
 from pssr.crappifiers import MultiCrappifier, Poisson, AdditiveGaussian, SaltPepper
 from pssr.loss import SSIMLoss
 from pssr.train import train_paired
 from pssr.predict import predict_images, test_metrics
 
 def _handle_declaration(arg, defaults, req=None):
@@ -31,34 +31,36 @@
     parser.add_argument("-mp", "--model-path", type=str, help="specify model path")
 
     parser.add_argument("-e", "--epochs", type=int, default=10, help="specify number of training epochs")
     parser.add_argument("-b", "--batch-size", type=int, default=16, help="specify batch size")
     parser.add_argument("-lr", "--lr", type=float, default=1e-3, help="specify learning rate")
     parser.add_argument("-p", "--patience", type=int, default=3, help="specify learning rate decay patience")
     parser.add_argument("-mse", "--mse", action="store_true", help="use MSE loss instead of SSIM loss")
+
+    parser.add_argument("-cp", "--checkpoint", action="store_true", help="save model checkpoints during training")
     parser.add_argument("-sl", "--save-losses", action="store_true", help="save training losses")
 
     return parser
 
-def run():
+def main():
     parser = parse()
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         return
     args = parser.parse_args()
 
     if "Paired" not in args.data_type and args.data_path is None:
         print("--data-path(-dp) must be provided for semi-synthetic datasets")
         return
     
     if args.model_path is None and not args.train:
         print("--model-path(-mp) must be provided in predict mode")
         return
 
-    model = _handle_declaration(args.model_type, ["ResUNet", "RDResUNet"])
+    model = _handle_declaration(args.model_type, ["ResUNet", "ResUNetA", "RDResUNet", "RDResUNetA", "SwinIR"])
     dataset = _handle_declaration(args.data_type, ["ImageDataset", "SlidingDataset"], 
         req=[f"'{args.data_path}'"] if args.train else [f'''{f"'{args.data_path}', " if "Paired" not in args.data_type else ""}val_split=1'''])
     
     print(f"\nModel:\n{_tab_string(model.extra_repr())}")
     print(f"\nDataset:\n{_tab_string(str(dataset))}")
 
     if torch.cuda.is_available():
@@ -73,38 +75,47 @@
         pin_memory = True,
     )
 
     if args.train:
         loss_fn = MSELoss() if args.mse else SSIMLoss(mix=.8, ms=True)
         optim = torch.optim.AdamW(model.parameters(), lr=args.lr)
         scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optim, factor=0.1, patience=args.patience, threshold=5e-3, verbose=True)
+        checkpoint_dir = "checkpoints" if args.checkpoint else None
+
+        if args.model_path:
+            print(f"Loading {model.__class__.__name__} model from {args.model_path}")
+            model.load_state_dict(torch.load(args.model_path))
 
         print("\nTraining model...")
-        losses = train_paired(
+        train_losses, val_losses = train_paired(
             model=model,
             dataset=dataset,
             batch_size=args.batch_size,
             loss_fn=loss_fn,
             optim=optim,
             epochs=args.epochs,
             device=device,
             scheduler=scheduler,
             log_frequency=50,
+            checkpoint_dir=checkpoint_dir,
             dataloader_kwargs=kwargs,
         )
         print("\nTraining complete!")
 
-        model_path = args.model_path if args.model_path else f"{model.__class__.__name__}_{losses[-1]:.3f}.pth"
-        torch.save(model.state_dict(), model_path)
-        print(f"Saved trained model to {model_path}")
+        save_path = f"{model.__class__.__name__}_{val_losses[-1]:.4f}.pth"
+        torch.save(model.state_dict(), save_path)
+        print(f"Saved trained model to {save_path}")
 
         if args.save_losses:
-            with open("train_loss.txt", "w") as file:
-                for loss in losses:
-                    file.write(f"{loss}\n")
+            with open(f"{model.__class__.__name__}_train_losses.txt", "w") as file:
+                for loss in train_losses:
+                    file.write(f"{loss:.6f}\n")
+            with open(f"{model.__class__.__name__}_val_losses.txt", "w") as file:
+                for loss in val_losses:
+                    file.write(f"{loss:.6f}\n")
 
     else:
         model.load_state_dict(torch.load(args.model_path))
 
         print("\nPredicting images from low resolution...")
         predict_images(model, dataset, device, norm=not dataset.is_lr, out_dir="preds")
 
@@ -120,8 +131,8 @@
 
 def _tab_string(text):
     lines = text.split("\n")
     indented_lines = ["\t" + line for line in lines]
     return "\n".join(indented_lines)
 
 if __name__ == "__main__":
-    run()
+    main()
```

### Comparing `pssr-1.2.1/pssr/crappifiers.py` & `pssr-1.2.2/pssr/crappifiers.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.1/pssr/data.py` & `pssr-1.2.2/pssr/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class ImageDataset(Dataset):
     def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), n_frames : int = None, mode : str = "L", extension : str = "tif", val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
         r"""Training dataset for loading high-resolution images from individual files and returning high-low-resolution pairs, the latter receiving crappification.
 
         Dataset used for pre-tiled image files. For image sheets (e.g. .czi files), use :class:`SlidingDataset`.
 
         LR mode (dataset loads only unmodified low-resolution images for prediction) can be enabled by
-        either inputting images less than or equal to LR size (``hr_res``/``lr_scale``) or by setting ``lr_scale`` = 1 and ``hr_res`` = LR resolution.
+        either inputting images less than or equal to LR size (``hr_res``/``lr_scale``) or by setting ``lr_scale`` = None and ``hr_res`` = LR resolution.
 
         Args:
             path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
@@ -51,17 +51,17 @@
         self.slices, max_size = [], 0
         for image_idx in range(len(self.hr_files)):
             image = Image.open(Path(self.path, self.hr_files[image_idx]))
             self.slices.append(1 if self.n_frames is None else image.n_frames // self.n_frames[0])
             max_size = max(max(image.size), max_size)
 
         self.val_idx = _get_val_idx(self.slices, val_split, split_seed)
-        self.is_lr = max_size <= hr_res//lr_scale or (lr_scale == 1)
+        self.is_lr = max_size <= hr_res//lr_scale or (lr_scale == None)
         if self.is_lr: print("LR mode is enabled, dataset will load only unmodified low-resolution images.")
-        self.crop_res = min(hr_res, max_size) * (lr_scale if self.is_lr else 1)
+        self.crop_res = min(hr_res, max_size)
 
         self.hr_res = hr_res
         self.lr_scale = lr_scale
         self.crappifier = crappifier
         self.rotation = rotation
         self.transforms = transforms
 
@@ -91,15 +91,15 @@
 
 class SlidingDataset(Dataset):
     def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), overlap : int = 128, n_frames : int = None, stack : str = "TZ", mode : str = "L", extension : str = "czi", preload : bool = True, val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
         r"""Training dataset for loading high-resolution image tiles from image sheets and returning high-low-resolution pairs, the latter receiving crappification.
 
         Dataset used for image sheets (e.g. .czi files). For pre-tiled image files, use :class:`ImageDataset`.
 
-        LR mode (dataset loads only unmodified low-resolution images for prediction) can be enabled by setting ``lr_scale`` = 1 and ``hr_res`` = LR resolution.
+        LR mode (dataset loads only unmodified low-resolution images for prediction) can be enabled by setting ``lr_scale`` = None and ``hr_res`` = LR resolution.
 
         Args:
             path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
@@ -146,17 +146,17 @@
         for image_idx in range(len(self.hr_files)):
             image = self.preload[image_idx] if self.preload else _load_sheet(self.path, self.hr_files[image_idx], self.stack, self.mode)
             tiles_x, tiles_y = _n_tiles(image, hr_res, self.stride)
             self.tiles.append(tiles_x * tiles_y)
             self.slices.append(1 if self.n_frames is None else image.shape[0] // self.n_frames[0])
 
         self.val_idx = _get_val_idx(self.slices, val_split, split_seed, self.tiles)
-        self.is_lr = (lr_scale == 1)
+        self.is_lr = (lr_scale == None)
         if self.is_lr: print("LR mode is enabled, dataset will load only unmodified low-resolution images.")
-        self.crop_res = hr_res * (lr_scale if self.is_lr else 1)
+        self.crop_res = hr_res
 
         self.hr_res = hr_res
         self.lr_scale = lr_scale
         self.crappifier = crappifier
         self.rotation = rotation
         self.transforms = transforms
     
@@ -252,15 +252,15 @@
 
         return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, False if is_val else self.rotation, self.transforms, self.n_frames)
     
     def __len__(self):
         return sum(self.slices)
     
     def __repr__(self):
-        return f'PairedImageDataset from paths "{self.hr_path}" and "{self.lr_path}"\n{len(self.hr_files)+len(self.lr_files)} files with {len(self)} total frame slices'
+        return f'PairedImageDataset from paths "{self.hr_path}" and "{self.lr_path}"\n{len(self.hr_files)} paired files with {len(self)} total frame slices'
 
     def _get_name(self, idx):
         image_idx, idx = _get_image_idx(idx, self.slices)
         return self.lr_files[image_idx].split('.')[0] + (f"_{idx}" if self.n_frames is not None else "")
 
 class PairedSlidingDataset(Dataset):
     def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, overlap : int = 128, n_frames : int = None, stack : str = "TZ", mode : str = "L", extension : str = "czi", preload : bool = True, val_split : float = 1, rotation : bool = True, split_seed : int = None, transforms : list[torch.nn.Module] = None):
@@ -346,15 +346,15 @@
 
         return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, False if is_val else self.rotation, self.transforms, self.n_frames)
     
     def __len__(self):
         return sum([self.tiles[idx] * self.slices[idx] for idx in range(len(self.hr_files))])
     
     def __repr__(self):
-        return f'PairedSlidingDataset from paths "{self.hr_path}" and "{self.lr_path}"\n{len(self.hr_files)+len(self.lr_files)} files with {len(self)} total frame slices'
+        return f'PairedSlidingDataset from paths "{self.hr_path}" and "{self.lr_path}"\n{len(self.hr_files)} paired files with {len(self)} total frame slices'
     
     def _get_name(self, idx):
         image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
         return f"{self.lr_files[image_idx].split('.')[0]}_{idx}"
 
 def preprocess_dataset(dataset : Dataset, preprocess_hr : bool = False, out_dir : str = "preprocess"):
     r"""Saves processed frame slices from a given dataset, including processes such as crappification or cropping/padding.
```

### Comparing `pssr-1.2.1/pssr/loss.py` & `pssr-1.2.2/pssr/loss.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.1/pssr/models/_blocks.py` & `pssr-1.2.2/pssr/models/_blocks.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.1/pssr/models/_rdnet.py` & `pssr-1.2.2/pssr/models/_rdnet.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.1/pssr/models/rdresunet.py` & `pssr-1.2.2/pssr/models/rdresunet.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
             self.decoder.append(get_resblock(in_channels=layers[layer_idx]//self.ratios[layer_idx]**2+skips[layer_idx], out_channels=layers[layer_idx+1], dilations=dilations[layer_idx] if dilations else None, depth=depth))
 
         self.encoder_pool = PSP_Pooling(skips[0], pool_sizes) if pool_sizes and encoder_pool else None
         self.reconstruction_pool = PSP_Pooling(hidden[-1]//self.ratios[-1]**2, pool_sizes) if pool_sizes else None
 
         self.reconstruction = Reconstruction(channels[0], channels[1], hidden[-1]//self.ratios[-1]**2, scale)
 
+        self.skips = skips
+
     def forward(self, x):
         x = x / 128 - 1 # Scale input approx from [0, 255] to [-1, 1]
         if self.norm is not None:
             x = self.norm(x)
 
         skips = [x]
         skips.extend(self.encoder(x))
@@ -97,15 +99,15 @@
 
         x = self.reconstruction(x)
 
         x = x * 128 + 128 # Scale output approx from [-1, 1] to [0, 255]
         return x
 
     def extra_repr(self):
-        return f"{'Atrous ' if self.norm is None else ''}RDResUNet with {self.reconstruction.scale}x upscaling\n{len(self.decoder)} residual blocks with {self.decoder[0].depth} hidden layers each\nPSP pooling {'enabled' if self.reconstruction_pool else 'disabled'}"
+        return f"{'Atrous ' if self.norm is None else ''}RDResUNet with {self.reconstruction.scale}x upscaling\nSkip connection sizes: {self.skips}\n{len(self.decoder)} residual blocks with {self.decoder[0].depth} hidden layers each\nPSP pooling {'enabled' if self.reconstruction_pool else 'disabled'}"
 
 class RDResUNetA():
     def __new__(cls,
             channels : int = 1,
             hidden : list[int] = [1024, 1024, 512, 256],
             scale : int = 4,
             depth : int = 3,
```

### Comparing `pssr-1.2.1/pssr/models/resunet.py` & `pssr-1.2.2/pssr/models/resunet.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.1/pssr/predict.py` & `pssr-1.2.2/pssr/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 
             hr_hat = model(lr)
             hr_hat = _pred_array(hr_hat).squeeze(0)
             
             if norm:
                 _, hr_hat = normalize_preds(_pred_array(dataset[idx][0]), hr_hat)
 
-            hr_hat = hr_hat[:,:dataset.crop_res,:dataset.crop_res]
+            crop_res = dataset.crop_res if not dataset.is_lr else dataset.crop_res * (hr_hat.shape[-1]//lr.shape[-1])
+            hr_hat = hr_hat[:,:crop_res,:crop_res]
             outs.append(hr_hat)
 
     if out_dir:
         os.makedirs(out_dir, exist_ok=True)
         for idx, hr_hat in enumerate(outs):
             tifffile.imwrite(f"{out_dir}/{prefix+'_' if prefix else ''}{dataset._get_name(idx)}.tif", np.asarray(hr_hat))
     else:
@@ -75,30 +76,32 @@
 
         n_images (int) : Number of images to concatenate. Set to None to use all validation images, maximum 50. Default is None.
 
         prefix (str) : Prefix to append at the beginning the output file name. Default is None.
 
         out_dir (str) : Directory to save collage. Default is "preds".
     """
+    if dataset.is_lr: raise ValueError("Dataset cannot be in LR mode when creating a collage.")
+
     n_images = min(50, len(dataset)) if n_images is None else n_images
 
     model.to(device)
     model.eval()
 
     collage = Image.new("L", (dataset.crop_res*3, dataset.crop_res*n_images))
     with torch.no_grad():
         for idx, data_idx in enumerate(_RandomIterIdx(dataset.val_idx, seed=True)):
             hr, lr = dataset[data_idx]
             hr, lr = hr.to(device).unsqueeze(0), lr.to(device).unsqueeze(0)
 
             hr_hat = model(lr)
 
-            collage.paste(_collage_preds(lr, hr_hat, hr, norm, 1, dataset.crop_res), (0, dataset.crop_res*idx))
+            collage.paste(_collage_preds(lr, hr_hat, hr, norm, 1, dataset.crop_res, dataset.lr_scale), (0, dataset.crop_res*idx))
 
-            if idx >= n_images:
+            if idx >= n_images - 1:
                 break
 
     os.makedirs(out_dir, exist_ok=True)
     collage.save(f"{out_dir}/{prefix+'_' if prefix else ''}collage_{n_images}.png")
 
 def test_metrics(model : nn.Module, dataset : Dataset, device : str = "cpu", metrics : list[str] = ["mse", "pixel", "psnr", "ssim"], avg : bool = True, norm : bool = True):
     r"""Computes image restoration metrics of predicted vs ground truth images.
@@ -134,15 +137,18 @@
     with torch.no_grad():
         for idx in progress:
             hr, lr = dataset[0]
             hr, lr = hr.to(device).unsqueeze(0), lr.to(device).unsqueeze(0)
 
             hr_hat = model(lr)
 
-            hr, hr_hat = _pred_array(hr)[:,:,:dataset.crop_res,:dataset.crop_res], _pred_array(hr_hat)[:,:,:dataset.crop_res,:dataset.crop_res]
+            hr, hr_hat = _pred_array(hr), _pred_array(hr_hat)
+
+            crop_res = dataset.crop_res if not dataset.is_lr else dataset.crop_res * (hr_hat.shape[-1]//lr.shape[-1])
+            hr, hr_hat = hr[:,:,:crop_res,:crop_res], hr_hat[:,:,:crop_res,:crop_res]
 
             if norm:
                 hr, hr_hat = normalize_preds(hr, hr_hat)
 
             for idx in range(len(hr)):
                 mse = np.mean((hr[idx]/image_range-hr_hat[idx]/image_range)**2) if use_mse else None
 
@@ -207,17 +213,17 @@
 
         hr_norms.append(hr_norm)
         hr_hat_norms.append(hr_hat_norm)
     
     hr, hr_hat = np.asarray(hr_norms).clip(0, 255), np.asarray(hr_hat_norms).clip(0, 255)
     return hr.reshape(hr_shape).astype(np.uint8), hr_hat.reshape(hr_hat_shape).astype(np.uint8)
 
-def _collage_preds(lr, hr_hat, hr, norm : bool = True, max_images : int = 5, crop_res : int = None):
+def _collage_preds(lr, hr_hat, hr, norm : bool = True, max_images : int = 5, crop_res : int = None, lr_scale : int = 4):
     crop_res = hr.shape[-1] if crop_res is None else crop_res
-    lr, hr_hat, hr = _pred_array(lr)[:,:,:crop_res//4,:crop_res//4], _pred_array(hr_hat)[:,:,:crop_res,:crop_res], _pred_array(hr)[:,:,:crop_res,:crop_res]
+    lr, hr_hat, hr = _pred_array(lr)[:,:,:crop_res//lr_scale,:crop_res//lr_scale], _pred_array(hr_hat)[:,:,:crop_res,:crop_res], _pred_array(hr)[:,:,:crop_res,:crop_res]
 
     if norm:
         hr, hr_hat = normalize_preds(hr, hr_hat)
         _, lr = normalize_preds(hr, lr)
 
     lr = _image_stack(lr, max_images)
     hr_hat = _image_stack(hr_hat, max_images)
```

### Comparing `pssr-1.2.1/pssr/train.py` & `pssr-1.2.2/pssr/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,18 @@
         dataset : Dataset,
         batch_size : int,
         loss_fn : nn.Module,
         optim : torch.optim.Optimizer,
         epochs : int,
         device : str = "cpu",
         scheduler : torch.optim.lr_scheduler = None,
-        clamp : bool = False,
         log_frequency : int = 50,
-        collage_dir : str = "preds",
+        checkpoint_dir : str = None,
+        collage_dir : str = None,
+        clamp : bool = False,
         dataloader_kwargs = None
     ):
     r"""Trains model on paired high-low-resolution crappified data.
 
     Args:
         model (nn.Module) : Model to train on paired data.
 
@@ -45,34 +46,38 @@
 
         epochs (int) : Number of epochs to train model for.
 
         device (str) : Device to train model on. Default is "cpu".
 
         scheduler (LRScheduler) : Optional learning rate scheduler for training. Default is None.
 
-        clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
-
         log_frequency (int) : Frequency to log losses and recalculate metrics in steps. Default is 50.
 
-        collage_dir (str) : Directory to save validation collages. A value of None skips the collage. Default is "preds".
+        checkpoint_dir (str) : Directory to save model checkpoints each epoch. A value of None skips checkpointing. Default is None.
+
+        collage_dir (str) : Directory to save validation collages each epoch. A value of None skips the collage. Default is None.
+
+        clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
     Returns:
-        losses (list[float]) : List of losses during training.
+        train_losses (list[float]) : List of losses during training.
+
+        val_losses (list[float]) : Validation losses per epoch.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
     val_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(dataset.val_idx, seed=True), **dataloader_kwargs)
     include_metric = True if type(scheduler) == torch.optim.lr_scheduler.ReduceLROnPlateau else False
     image_range = 255
 
     model.to(device)
 
-    losses = []
+    train_losses, val_losses = [], []
     for epoch in range(epochs):
         # Train
         model.train()
         print(f"Epoch {epoch}:")
 
         progress = tqdm(train_dataloader)
         for batch_idx, (hr, lr) in enumerate(progress):
@@ -84,15 +89,15 @@
 
             loss = loss_fn(hr_hat/image_range, hr/image_range)
             loss.backward()
             optim.step()
             optim.zero_grad()
 
             if batch_idx % log_frequency == 0 or batch_idx == len(progress) - 1:
-                losses.append(loss.item())
+                train_losses.append(loss.item())
 
                 mse = nn.functional.mse_loss(hr_hat/image_range, hr/image_range)
                 progress.set_description(f"pixel[{pixel_metric(mse, image_range):.2f}], psnr[{_psnr_metric(mse):.2f}], ssim[{ssim(hr_hat, hr, data_range=image_range):.3f}]")
 
         # Validation
         model.eval()
 
@@ -106,44 +111,50 @@
 
                 hr_hat = model(lr)
                 if clamp:
                     hr_hat = torch.clamp(hr_hat, 0, image_range)
 
                 loss = loss_fn(hr_hat/image_range, hr/image_range)
                 val_loss.append(loss.item())
-        val_loss = sum(val_loss) / len(val_loss)
 
+        val_loss = sum(val_loss) / len(val_loss)
+        val_losses.append(val_loss)
         print(f"Epoch {epoch} validation loss: {val_loss:4f}\n")
 
+        if checkpoint_dir and epoch < epochs - 1:
+            os.makedirs(checkpoint_dir, exist_ok=True)
+            torch.save(model.state_dict(), f"{checkpoint_dir}/checkpoint{epoch}_{model.__class__.__name__}_{val_loss:.4f}.pth")
+
+        if collage_dir:
+            collage = _collage_preds(lr, hr_hat, hr, crop_res=dataset.crop_res, lr_scale=dataset.lr_scale)
+            os.makedirs(collage_dir, exist_ok=True)
+            collage.save(f"{collage_dir}/epoch{epoch}_loss{val_loss:.4f}.png")
+
         if scheduler:
             if include_metric:
                 scheduler.step(val_loss)
             else:
                 scheduler.step()
-        
-        if collage_dir:
-            collage = _collage_preds(lr, hr_hat, hr, crop_res=dataset.crop_res)
-            os.makedirs(collage_dir, exist_ok=True)
-            collage.save(f"{collage_dir}/epoch{epoch}_loss{val_loss:.3f}.png")
 
-    return losses
+    return train_losses, val_losses
 
 def train_crappifier(
         model : nn.Module,
         dataset : Dataset,
         batch_size : int,
         optim : torch.optim.Optimizer,
         epochs : int,
         sigma : int = 5,
         clip : float = 3,
         device : str = "cpu",
         scheduler : torch.optim.lr_scheduler = None,
-        clamp : bool = False,
         log_frequency : int = 50,
-        collage_dir : str = "preds",
+        checkpoint_dir : str = None,
+        collage_dir : str = None,
+        clamp : bool = False,
         dataloader_kwargs = None
     ):
     r"""EXPERIMENTAL, NOT CURRENTLY RECOMMENDED FOR MOST WORKFLOWS!
     
     Trains an :class:`nn.Module` model as a crappifier on high-low-resolution paired data.
     The model must output an image the same size as the input/have a `scale` value of 1.
     This is not necessary if you are using a :class:`Crappifier` instance as your crappifier.
@@ -163,38 +174,42 @@
 
         clip : (float) : Max gradient for gradient clipping. Use None for no clipping. Default is 3.
 
         device (str) : Device to train model on. Default is "cpu".
 
         scheduler (LRScheduler) : Optional learning rate scheduler for training. Default is None.
 
-        clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
-
         log_frequency (int) : Frequency to log losses and recalculate metrics in steps. Default is 50.
 
-        collage_dir (str) : Directory to save validation collages. A value of None skips the collage. Default is "preds".
+        checkpoint_dir (str) : Directory to save model checkpoints each epoch. A value of None skips checkpointing. Default is None.
+
+        collage_dir (str) : Directory to save validation collages each epoch. A value of None skips the collage. Default is None.
+
+        clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
     Returns:
-        losses (list[float]) : List of losses during training.
+        train_losses (list[float]) : List of losses during training.
+
+        val_losses (list[float]) : Validation losses per epoch.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
     val_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(dataset.val_idx, seed=True), **dataloader_kwargs)
     include_metric = True if type(scheduler) == torch.optim.lr_scheduler.ReduceLROnPlateau else False
 
     model.to(device)
     model.train()
 
     # Leave on cpu?
     hist_fn = GradHist(sigma=sigma)
     ssim_loss = SSIMLoss(ms=False)
 
-    losses = []
+    train_losses, val_losses = [], []
     for epoch in range(epochs):
         # Train
         model.train()
         print(f"Epoch {epoch}:")
 
         progress = tqdm(train_dataloader)
         for batch_idx, (hr, lr) in enumerate(progress):
@@ -212,17 +227,17 @@
             if clip is not None and clip > 0:
                 nn.utils.clip_grad_value_(model.parameters(), clip)
 
             optim.step()
             optim.zero_grad()
 
             if batch_idx % log_frequency == 0 or batch_idx == len(progress) - 1:
-                losses.append(loss.item())
+                train_losses.append(loss.item())
 
-                progress.set_description(f"loss[{loss.item():.5f}]")
+                progress.set_description(f"loss[{loss.item():.4f}]")
 
         # Validation
         model.eval()
 
         val_loss = []
         progress = tqdm(val_dataloader)
         progress.set_description(f"Epoch {epoch} validation...")
@@ -235,30 +250,35 @@
 
                 lr_hat = model(ds_hr)
                 if clamp:
                     lr_hat = torch.clamp(lr_hat, 0, 255)
 
                 loss = _crappifier_loss(lr.to(device), lr_hat, ds_hr, hist_fn, ssim_loss)
                 val_loss.append(loss.item())
-        val_loss = sum(val_loss) / len(val_loss)
 
+        val_loss = sum(val_loss) / len(val_loss)
+        val_losses.append(val_loss)
         print(f"Epoch {epoch} validation loss: {val_loss:4f}\n")
 
+        if checkpoint_dir and epoch < epochs - 1:
+            os.makedirs(checkpoint_dir, exist_ok=True)
+            torch.save(model.state_dict(), f"{checkpoint_dir}/checkpoint{epoch}_{model.__class__.__name__}_{val_loss:.4f}.pth")
+
+        if collage_dir:
+            collage = _collage_preds(lr, lr_hat, hr, crop_res=dataset.crop_res, lr_scale=dataset.lr_scale)
+            os.makedirs(collage_dir, exist_ok=True)
+            collage.save(f"{collage_dir}/epoch{epoch}_loss{val_loss:.4f}.png")
+
         if scheduler:
             if include_metric:
                 scheduler.step(val_loss)
             else:
                 scheduler.step()
 
-        if collage_dir:
-            collage = _collage_preds(lr, lr_hat, hr, crop_res=dataset.crop_res)
-            os.makedirs(collage_dir, exist_ok=True)
-            collage.save(f"{collage_dir}/pred{epoch}_loss{val_loss:.3f}.png")
-
-    return losses
+    return train_losses, val_losses
 
 def approximate_crappifier(crappifier : Crappifier, space : list[Dimension], dataset : Dataset, max_images = None, opt_kwargs = None):
     r"""Approximates :class:`Crappifier` parameters from ground truth paired images. Uses Bayesian optimization because Crappifier functions are not differentiable.
 
     Args:
         crappifier (Crappifier) : Crappifier whose parameter space will be optimized.
```

### Comparing `pssr-1.2.1/pyproject.toml` & `pssr-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pssr"
-version = "1.2.1"
+version = "1.2.2"
 description = "Point-Scanning Super-Resolution"
 authors = ["Hayden Stites"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ucsdmanorlab/PSSR"
 documentation = "https://ucsdmanorlab.github.io/PSSR/"
 classifiers = [
@@ -30,12 +30,12 @@
 scikit-optimize = ">=0.9.0"
 tqdm = "^4.0.0"
 pytorch-msssim = "^1.0.0"
 psutil = ">=5.0.0"
 timm = ">=0.8.0"
 
 [tool.poetry.scripts]
-pssr = "pssr.__main__:run"
+pssr = "pssr.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pssr-1.2.1/PKG-INFO` & `pssr-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.2.1
+Version: 1.2.2
 Summary: Point-Scanning Super-Resolution
 Home-page: https://github.com/ucsdmanorlab/PSSR
 License: MIT
 Author: Hayden Stites
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

