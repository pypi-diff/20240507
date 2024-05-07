# Comparing `tmp/hidiffusion-0.1.6.tar.gz` & `tmp/hidiffusion-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidiffusion-0.1.6.tar", last modified: Thu Apr 25 18:12:24 2024, max compression
+gzip compressed data, was "hidiffusion-0.1.8.tar", last modified: Tue May  7 18:10:08 2024, max compression
```

## Comparing `hidiffusion-0.1.6.tar` & `hidiffusion-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    11357 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/LICENSE
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       35 2024-04-25 18:11:43.000000 hidiffusion-0.1.6/MANIFEST.in
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15091 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/PKG-INFO
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    14776 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/README.md
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/hidiffusion/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      118 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/__init__.py
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   105548 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/hidiffusion.py
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/hidiffusion/sd_module_key/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    30444 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/sd_module_key/sd15_module_key.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   100878 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/sd_module_key/sdxl_module_key.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      872 2024-04-25 18:10:50.000000 hidiffusion-0.1.6/hidiffusion/utils.py
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/hidiffusion.egg-info/
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15091 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/PKG-INFO
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      342 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)        1 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       12 2024-04-25 18:12:24.000000 hidiffusion-0.1.6/hidiffusion.egg-info/top_level.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       38 2024-04-25 18:12:24.690060 hidiffusion-0.1.6/setup.cfg
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      493 2024-04-25 18:11:34.000000 hidiffusion-0.1.6/setup.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-05-07 18:10:08.718584 hidiffusion-0.1.8/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    11357 2024-05-07 18:09:12.000000 hidiffusion-0.1.8/LICENSE
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       35 2024-05-07 18:09:08.000000 hidiffusion-0.1.8/MANIFEST.in
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    17736 2024-05-07 18:10:08.718584 hidiffusion-0.1.8/PKG-INFO
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    17421 2024-05-07 18:08:29.000000 hidiffusion-0.1.8/README.md
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-05-07 18:10:08.714584 hidiffusion-0.1.8/hidiffusion/
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)      118 2024-05-07 18:08:29.000000 hidiffusion-0.1.8/hidiffusion/__init__.py
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)   112975 2024-05-07 18:08:29.000000 hidiffusion-0.1.8/hidiffusion/hidiffusion.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-05-07 18:10:08.718584 hidiffusion-0.1.8/hidiffusion/sd_module_key/
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    30443 2024-05-07 18:08:29.000000 hidiffusion-0.1.8/hidiffusion/sd_module_key/sd15_module_key.txt
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)   100878 2024-05-07 18:08:29.000000 hidiffusion-0.1.8/hidiffusion/sd_module_key/sdxl_module_key.txt
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)      872 2024-05-07 18:08:29.000000 hidiffusion-0.1.8/hidiffusion/utils.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-05-07 18:10:08.718584 hidiffusion-0.1.8/hidiffusion.egg-info/
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    17736 2024-05-07 18:10:08.000000 hidiffusion-0.1.8/hidiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      342 2024-05-07 18:10:08.000000 hidiffusion-0.1.8/hidiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)        1 2024-05-07 18:10:08.000000 hidiffusion-0.1.8/hidiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       12 2024-05-07 18:10:08.000000 hidiffusion-0.1.8/hidiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       38 2024-05-07 18:10:08.718584 hidiffusion-0.1.8/setup.cfg
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)      493 2024-05-07 18:08:59.000000 hidiffusion-0.1.8/setup.py
```

### Comparing `hidiffusion-0.1.6/LICENSE` & `hidiffusion-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.6/PKG-INFO` & `hidiffusion-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: hidiffusion
-Version: 0.1.6
-Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
-Home-page: 
-Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- # 💡 HiDiffusion -->
 
 <div align="center">
   <img src="assets/hidiffusion_logo.jpg"  height=120>
 </div>
 
 ### <div align="center">💡 HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in Pretrained Diffusion Models</div> 
@@ -31,41 +22,57 @@
   <em>
       (Select HiDiffusion samples for various diffusion models, resolutions, and aspect ratios.) 
   </em>
 </div>
 <br>
 
 
-# 👉 Why HiDiffusion
+## 👉 Why HiDiffusion
 
 - A  **training-free method that increases the resolution and speed of pretrained diffusion models.**
 - Designed as a **plug-and-play implementation**. It can be integrated into diffusion pipelines by **only adding a single line of code**!
+- Supports various tasks, including **text-to-image, image-to-image, inpainting**.
 
 <div align="center">
   <img src="assets/quality_efficiency.jpg" width="800" ></img>
   <br>
   <em>
       (Faster, and better image details.) 
   </em>
 </div>
 <br>
 
+<div align="center">
+  <img src="assets/various_task.jpg" width="800" ></img>
+  <br>
+  <em>
+      (2K results of ControlNet and inpainting tasks.) 
+  </em>
+</div>
+<br>
+
+## 🔥 Update
+- 2024.5.7 - 💥 Support image-to-image task, see [here](#image-to-image-generation).
+
+- 2024.4.16 - 💥 Release source code.
+
+
 ## 📢 Supported Models
 
 - ✅ [Stable Diffusion XL](https://huggingface.co/papers/2307.01952)
 - ✅ [Stable Diffusion XL Turbo](https://huggingface.co/stabilityai/sdxl-turbo)
 - ✅ [Stable Diffusion v2](https://huggingface.co/stabilityai/stable-diffusion-2-1)
 - ✅ [Stable Diffusion v1](https://huggingface.co/runwayml/stable-diffusion-v1-5)
 
 **Note**: HiDiffusion also supports the downstream diffusion models based on these repositories, such as [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc.
 
 ## 💣 Supported Tasks
 
 - ✅ Text-to-image
-- ✅ ControlNet
+- ✅ ControlNet, including text-to-image, image-to-image
 - ✅ Inpainting
 
 
 ## 🔎 Main Requirements
 This repository is tested on
 * Python==3.8
 * torch==1.13.1
@@ -226,24 +233,25 @@
 
 ### Remove HiDiffusion
 
 If you want to remove HiDiiffusion, simply use `remove_hidiffusion(pipe)`.
 
 ## ControlNet
 
+### Text-to-image generation
 ```python
 from diffusers import StableDiffusionXLControlNetPipeline, ControlNetModel, DDIMScheduler
 import numpy as np
 import torch
 import cv2
 from PIL import Image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 # load Yoshua_Bengio.jpg in the assets file.
-path = 'Yoshua_Bengio.jpg'
+path = './assets/Yoshua_Bengio.jpg'
 image = Image.open(path)
 # get canny image
 image = np.array(image)
 image = cv2.Canny(image, 100, 200)
 image = image[:, :, None]
 image = np.concatenate([image, image, image], axis=2)
 canny_image = Image.fromarray(image)
@@ -279,14 +287,78 @@
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/controlnet_result.jpg" width="800" ></img>
 </div>
 </details>
 
+
+### Image-to-image generation
+```python
+import torch
+import numpy as np
+from PIL import Image
+from diffusers import ControlNetModel, StableDiffusionXLControlNetImg2ImgPipeline, DDIMScheduler
+from hidiffusion import apply_hidiffusion, remove_hidiffusion
+import cv2 
+
+controlnet = ControlNetModel.from_pretrained(
+    "diffusers/controlnet-canny-sdxl-1.0", torch_dtype=torch.float16, variant="fp16"
+).to("cuda")
+scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0", subfolder="scheduler")
+
+pipe = StableDiffusionXLControlNetImg2ImgPipeline.from_pretrained(
+    "stabilityai/stable-diffusion-xl-base-1.0",
+    controlnet=controlnet,
+    scheduler = scheduler,
+    torch_dtype=torch.float16,
+).to("cuda")
+
+# Apply hidiffusion with a single line of code.
+apply_hidiffusion(pipe)
+
+pipe.enable_model_cpu_offload()
+pipe.enable_xformers_memory_efficient_attention()
+
+path = './assets/lara.jpeg'
+ori_image = Image.open(path)
+# get canny image
+image = np.array(ori_image)
+image = cv2.Canny(image, 50, 120)
+image = image[:, :, None]
+image = np.concatenate([image, image, image], axis=2)
+canny_image = Image.fromarray(image)
+
+controlnet_conditioning_scale = 0.5  # recommended for good generalization
+prompt = "Lara Croft with brown hair, and is wearing a tank top, a brown backpack. The room is dark and has an old-fashioned decor with a patterned floor and a wall featuring a design with arches and a dark area on the right side, muted color, high detail, 8k high definition award winning"
+negative_prompt = "underexposed, poorly drawn hands, duplicate hands, overexposed, bad art, beginner, amateur, abstract, disfigured, deformed, close up, weird colors, watermark"
+
+image = pipe(prompt,
+    image=ori_image,
+    control_image=canny_image,
+    height=1536,
+    width=2048,
+    strength=0.99,
+    num_inference_steps=50,
+    controlnet_conditioning_scale=controlnet_conditioning_scale,
+    guidance_scale=12.5,
+    negative_prompt = negative_prompt,
+    eta=1.0
+).images[0]
+
+image.save("lara.jpg")
+```
+
+<details>
+<summary>Output:</summary>
+<div align="center">
+  <img src="assets/lara_result.jpg" width="800" ></img>
+</div>
+</details>
+
 ## Inpainting
 
 ```python
 import torch
 from diffusers import AutoPipelineForInpainting, DDIMScheduler
 from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
@@ -305,15 +377,15 @@
 # remove following line if xFormers is not installed
 pipeline.enable_xformers_memory_efficient_attention()
 
 # load base and mask image
 img_url = "https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/diffusers/sdxl-text2img.png"
 init_image = load_image(img_url)
 # load mask_image.jpg in the assets file.
-mask_image = Image.open("mask_image.png")
+mask_image = Image.open("./assets/mask_image.png")
 
 prompt =  "A steampunk explorer in a leather aviator cap and goggles, with a brass telescope in hand, stands amidst towering ancient trees, their roots entwined with intricate gears and pipes."
 
 negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image = pipeline(prompt=prompt, image=init_image, mask_image=mask_image, height=2048, width=2048, strength=0.85, guidance_scale=12.5, negative_prompt = negative_prompt, eta=1.0).images[0]
 image.save('steampunk_explorer.jpg')
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.6 Summary: HiDiffusion: A
-training-free method to increase the resolution and speed of diffusion models.
-Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
-Jiajun Liang Description-Content-Type: text/markdown License-File: LICENSE
                          [assets/hidiffusion_logo.jpg]
 ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
@@ -13,47 +9,54 @@
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_P_a_p_e_r_&_m_e_s_s_a_g_e_=_A_r_x_i_v_:
       _H_i_D_i_f_f_u_s_i_o_n_&_c_o_l_o_r_=_r_e_d_&_l_o_g_o_=_a_r_x_i_v_]  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
           _v_1_?_l_a_b_e_l_=_D_e_m_o_&_m_e_s_s_a_g_e_=_C_o_l_a_b_&_c_o_l_o_r_=_p_u_r_p_l_e_&_l_o_g_o_=_g_o_o_g_l_e_c_o_l_a_b_] 
                           [assets/image_gallery.jpg]
   ((SSeelleecctt HHiiDDiiffffuussiioonn ssaammpplleess ffoorr vvaarriioouuss ddiiffffuussiioonn mmooddeellss,, rreessoolluuttiioonnss,, aanndd
                                 aassppeecctt rraattiiooss..))
 
-# ð Why HiDiffusion - A **training-free method that increases the resolution
-and speed of pretrained diffusion models.** - Designed as a **plug-and-play
-implementation**. It can be integrated into diffusion pipelines by **only
-adding a single line of code**!
+## ð Why HiDiffusion - A **training-free method that increases the
+resolution and speed of pretrained diffusion models.** - Designed as a **plug-
+and-play implementation**. It can be integrated into diffusion pipelines by
+**only adding a single line of code**! - Supports various tasks, including
+**text-to-image, image-to-image, inpainting**.
                         [assets/quality_efficiency.jpg]
                       ((FFaasstteerr,, aanndd bbeetttteerr iimmaaggee ddeettaaiillss..))
 
-## ð¢ Supported Models - â [Stable Diffusion XL](https://huggingface.co/
-papers/2307.01952) - â [Stable Diffusion XL Turbo](https://huggingface.co/
+                           [assets/various_task.jpg]
+               ((22KK rreessuullttss ooff CCoonnttrroollNNeett aanndd iinnppaaiinnttiinngg ttaasskkss..))
+
+## ð¥ Update - 2024.5.7 - ð¥ Support image-to-image task, see [here]
+(#image-to-image-generation). - 2024.4.16 - ð¥ Release source code. ## ð¢
+Supported Models - â [Stable Diffusion XL](https://huggingface.co/papers/
+2307.01952) - â [Stable Diffusion XL Turbo](https://huggingface.co/
 stabilityai/sdxl-turbo) - â [Stable Diffusion v2](https://huggingface.co/
 stabilityai/stable-diffusion-2-1) - â [Stable Diffusion v1](https://
 huggingface.co/runwayml/stable-diffusion-v1-5) **Note**: HiDiffusion also
 supports the downstream diffusion models based on these repositories, such as
 [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion),
 [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-
-aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
-â Inpainting ## ð Main Requirements This repository is tested on *
-Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
-accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
-installing the packages in the [main requirements](#-main-requirements),
-install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
-source Alternatively, you can install from github source. Clone the repository
-and install: ```bash git clone https://github.com/megvii-model/HiDiffusion.git
-cd HiDiffusion python3 setup.py install ``` ## ð Usage Generating outputs
-with HiDiffusion is super easy based on ð¤ [diffusers](https://github.com/
-huggingface/diffusers/tree/main). **You just need to add a single line of
-code**. ## Text-to-image generation ### Stable Diffusion XL ```python from
-hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
-StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
-"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
-DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
-StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
-scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
+aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet,
+including text-to-image, image-to-image - â Inpainting ## ð Main
+Requirements This repository is tested on * Python==3.8 * torch==1.13.1 *
+diffusers==0.27.0 * transformers==4.27.4 * accelerate==0.18.0 *
+xformers==0.0.16rc425 ## ð Install HiDiffusion After installing the packages
+in the [main requirements](#-main-requirements), install HiDiffusion: ```shell
+pip3 install hidiffusion ``` ### Installing from source Alternatively, you can
+install from github source. Clone the repository and install: ```bash git clone
+https://github.com/megvii-model/HiDiffusion.git cd HiDiffusion python3 setup.py
+install ``` ## ð Usage Generating outputs with HiDiffusion is super easy
+based on ð¤ [diffusers](https://github.com/huggingface/diffusers/tree/main).
+**You just need to add a single line of code**. ## Text-to-image generation ###
+Stable Diffusion XL ```python from hidiffusion import apply_hidiffusion,
+remove_hidiffusion from diffusers import StableDiffusionXLPipeline,
+DDIMScheduler import torch pretrain_model = "stabilityai/stable-diffusion-xl-
+base-1.0" scheduler = DDIMScheduler.from_pretrained(pretrain_model,
+subfolder="scheduler") pipe = StableDiffusionXLPipeline.from_pretrained
+(pretrain_model, scheduler = scheduler, torch_dtype=torch.float16,
+variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
 with a single line of code. apply_hidiffusion(pipe) prompt = "Standing tall
 amidst the ruins, a stone golem awakens, vines and flowers sprouting from the
 crevices in its body." negative_prompt = "blurry, ugly, duplicate, poorly drawn
@@ -113,54 +116,85 @@
 negative_prompt = "ugly, tiling, poorly drawn face, out of frame, disfigured,
 deformed, blurry, bad anatomy, blurred." image = pipe(prompt,
 guidance_scale=7.5, height=1024, width=1024, eta=1.0,
 negative_prompt=negative_prompt).images[0] image.save(f"fox.jpg") ``` Output:
                                [assets/sd15.jpg]
 Set height = 2048, width = 2048, and you can get output with 2048x2048
 resolution. ### Remove HiDiffusion If you want to remove HiDiiffusion, simply
-use `remove_hidiffusion(pipe)`. ## ControlNet ```python from diffusers import
-StableDiffusionXLControlNetPipeline, ControlNetModel, DDIMScheduler import
-numpy as np import torch import cv2 from PIL import Image from hidiffusion
-import apply_hidiffusion, remove_hidiffusion # load Yoshua_Bengio.jpg in the
-assets file. path = 'Yoshua_Bengio.jpg' image = Image.open(path) # get canny
-image image = np.array(image) image = cv2.Canny(image, 100, 200) image = image
-[:, :, None] image = np.concatenate([image, image, image], axis=2) canny_image
-= Image.fromarray(image) # initialize the models and pipeline
-controlnet_conditioning_scale = 0.5 # recommended for good generalization
-controlnet = ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-
-1.0", torch_dtype=torch.float16, variant="fp16" ) scheduler =
+use `remove_hidiffusion(pipe)`. ## ControlNet ### Text-to-image generation
+```python from diffusers import StableDiffusionXLControlNetPipeline,
+ControlNetModel, DDIMScheduler import numpy as np import torch import cv2 from
+PIL import Image from hidiffusion import apply_hidiffusion, remove_hidiffusion
+# load Yoshua_Bengio.jpg in the assets file. path = './assets/
+Yoshua_Bengio.jpg' image = Image.open(path) # get canny image image = np.array
+(image) image = cv2.Canny(image, 100, 200) image = image[:, :, None] image =
+np.concatenate([image, image, image], axis=2) canny_image = Image.fromarray
+(image) # initialize the models and pipeline controlnet_conditioning_scale =
+0.5 # recommended for good generalization controlnet =
+ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-1.0",
+torch_dtype=torch.float16, variant="fp16" ) scheduler =
 DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
 subfolder="scheduler") pipe =
 StableDiffusionXLControlNetPipeline.from_pretrained( "stabilityai/stable-
 diffusion-xl-base-1.0", controlnet=controlnet, torch_dtype=torch.float16,
 scheduler = scheduler ) # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
 pipe.enable_xformers_memory_efficient_attention() prompt = "The Joker, high
 face detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
 duplicate, poorly drawn, deformed, mosaic." image = pipe( prompt,
 controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
 height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt,
 eta=1.0 ).images[0] image.save('joker.jpg') ``` Output:
                         [assets/controlnet_result.jpg]
+### Image-to-image generation ```python import torch import numpy as np from
+PIL import Image from diffusers import ControlNetModel,
+StableDiffusionXLControlNetImg2ImgPipeline, DDIMScheduler from hidiffusion
+import apply_hidiffusion, remove_hidiffusion import cv2 controlnet =
+ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-1.0",
+torch_dtype=torch.float16, variant="fp16" ).to("cuda") scheduler =
+DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
+subfolder="scheduler") pipe =
+StableDiffusionXLControlNetImg2ImgPipeline.from_pretrained( "stabilityai/
+stable-diffusion-xl-base-1.0", controlnet=controlnet, scheduler = scheduler,
+torch_dtype=torch.float16, ).to("cuda") # Apply hidiffusion with a single line
+of code. apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
+pipe.enable_xformers_memory_efficient_attention() path = './assets/lara.jpeg'
+ori_image = Image.open(path) # get canny image image = np.array(ori_image)
+image = cv2.Canny(image, 50, 120) image = image[:, :, None] image =
+np.concatenate([image, image, image], axis=2) canny_image = Image.fromarray
+(image) controlnet_conditioning_scale = 0.5 # recommended for good
+generalization prompt = "Lara Croft with brown hair, and is wearing a tank top,
+a brown backpack. The room is dark and has an old-fashioned decor with a
+patterned floor and a wall featuring a design with arches and a dark area on
+the right side, muted color, high detail, 8k high definition award winning"
+negative_prompt = "underexposed, poorly drawn hands, duplicate hands,
+overexposed, bad art, beginner, amateur, abstract, disfigured, deformed, close
+up, weird colors, watermark" image = pipe(prompt, image=ori_image,
+control_image=canny_image, height=1536, width=2048, strength=0.99,
+num_inference_steps=50,
+controlnet_conditioning_scale=controlnet_conditioning_scale,
+guidance_scale=12.5, negative_prompt = negative_prompt, eta=1.0 ).images[0]
+image.save("lara.jpg") ``` Output:
+                           [assets/lara_result.jpg]
 ## Inpainting ```python import torch from diffusers import
 AutoPipelineForInpainting, DDIMScheduler from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion from PIL import
 Image scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-
 xl-base-1.0", subfolder="scheduler") pipeline =
 AutoPipelineForInpainting.from_pretrained( "diffusers/stable-diffusion-xl-1.0-
 inpainting-0.1", torch_dtype=torch.float16, variant="fp16", scheduler=scheduler
 ) # Apply hidiffusion with a single line of code. apply_hidiffusion(pipeline)
 pipeline.enable_model_cpu_offload() # remove following line if xFormers is not
 installed pipeline.enable_xformers_memory_efficient_attention() # load base and
 mask image img_url = "https://huggingface.co/datasets/huggingface/
 documentation-images/resolve/main/diffusers/sdxl-text2img.png" init_image =
 load_image(img_url) # load mask_image.jpg in the assets file. mask_image =
-Image.open("mask_image.png") prompt = "A steampunk explorer in a leather
-aviator cap and goggles, with a brass telescope in hand, stands amidst towering
-ancient trees, their roots entwined with intricate gears and pipes."
+Image.open("./assets/mask_image.png") prompt = "A steampunk explorer in a
+leather aviator cap and goggles, with a brass telescope in hand, stands amidst
+towering ancient trees, their roots entwined with intricate gears and pipes."
 negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image = pipeline(prompt=prompt, image=init_image, mask_image=mask_image,
 height=2048, width=2048, strength=0.85, guidance_scale=12.5, negative_prompt =
 negative_prompt, eta=1.0).images[0] image.save('steampunk_explorer.jpg') ```
 Output:
                         [assets/inpainting_result.jpg]
 ## Integration into downstream models HiDiffusion supports models based on
```

### Comparing `hidiffusion-0.1.6/README.md` & `hidiffusion-0.1.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: hidiffusion
+Version: 0.1.8
+Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
+Home-page: 
+Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!-- # 💡 HiDiffusion -->
 
 <div align="center">
   <img src="assets/hidiffusion_logo.jpg"  height=120>
 </div>
 
 ### <div align="center">💡 HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in Pretrained Diffusion Models</div> 
@@ -22,41 +31,57 @@
   <em>
       (Select HiDiffusion samples for various diffusion models, resolutions, and aspect ratios.) 
   </em>
 </div>
 <br>
 
 
-# 👉 Why HiDiffusion
+## 👉 Why HiDiffusion
 
 - A  **training-free method that increases the resolution and speed of pretrained diffusion models.**
 - Designed as a **plug-and-play implementation**. It can be integrated into diffusion pipelines by **only adding a single line of code**!
+- Supports various tasks, including **text-to-image, image-to-image, inpainting**.
 
 <div align="center">
   <img src="assets/quality_efficiency.jpg" width="800" ></img>
   <br>
   <em>
       (Faster, and better image details.) 
   </em>
 </div>
 <br>
 
+<div align="center">
+  <img src="assets/various_task.jpg" width="800" ></img>
+  <br>
+  <em>
+      (2K results of ControlNet and inpainting tasks.) 
+  </em>
+</div>
+<br>
+
+## 🔥 Update
+- 2024.5.7 - 💥 Support image-to-image task, see [here](#image-to-image-generation).
+
+- 2024.4.16 - 💥 Release source code.
+
+
 ## 📢 Supported Models
 
 - ✅ [Stable Diffusion XL](https://huggingface.co/papers/2307.01952)
 - ✅ [Stable Diffusion XL Turbo](https://huggingface.co/stabilityai/sdxl-turbo)
 - ✅ [Stable Diffusion v2](https://huggingface.co/stabilityai/stable-diffusion-2-1)
 - ✅ [Stable Diffusion v1](https://huggingface.co/runwayml/stable-diffusion-v1-5)
 
 **Note**: HiDiffusion also supports the downstream diffusion models based on these repositories, such as [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc.
 
 ## 💣 Supported Tasks
 
 - ✅ Text-to-image
-- ✅ ControlNet
+- ✅ ControlNet, including text-to-image, image-to-image
 - ✅ Inpainting
 
 
 ## 🔎 Main Requirements
 This repository is tested on
 * Python==3.8
 * torch==1.13.1
@@ -217,24 +242,25 @@
 
 ### Remove HiDiffusion
 
 If you want to remove HiDiiffusion, simply use `remove_hidiffusion(pipe)`.
 
 ## ControlNet
 
+### Text-to-image generation
 ```python
 from diffusers import StableDiffusionXLControlNetPipeline, ControlNetModel, DDIMScheduler
 import numpy as np
 import torch
 import cv2
 from PIL import Image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 # load Yoshua_Bengio.jpg in the assets file.
-path = 'Yoshua_Bengio.jpg'
+path = './assets/Yoshua_Bengio.jpg'
 image = Image.open(path)
 # get canny image
 image = np.array(image)
 image = cv2.Canny(image, 100, 200)
 image = image[:, :, None]
 image = np.concatenate([image, image, image], axis=2)
 canny_image = Image.fromarray(image)
@@ -270,14 +296,78 @@
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/controlnet_result.jpg" width="800" ></img>
 </div>
 </details>
 
+
+### Image-to-image generation
+```python
+import torch
+import numpy as np
+from PIL import Image
+from diffusers import ControlNetModel, StableDiffusionXLControlNetImg2ImgPipeline, DDIMScheduler
+from hidiffusion import apply_hidiffusion, remove_hidiffusion
+import cv2 
+
+controlnet = ControlNetModel.from_pretrained(
+    "diffusers/controlnet-canny-sdxl-1.0", torch_dtype=torch.float16, variant="fp16"
+).to("cuda")
+scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0", subfolder="scheduler")
+
+pipe = StableDiffusionXLControlNetImg2ImgPipeline.from_pretrained(
+    "stabilityai/stable-diffusion-xl-base-1.0",
+    controlnet=controlnet,
+    scheduler = scheduler,
+    torch_dtype=torch.float16,
+).to("cuda")
+
+# Apply hidiffusion with a single line of code.
+apply_hidiffusion(pipe)
+
+pipe.enable_model_cpu_offload()
+pipe.enable_xformers_memory_efficient_attention()
+
+path = './assets/lara.jpeg'
+ori_image = Image.open(path)
+# get canny image
+image = np.array(ori_image)
+image = cv2.Canny(image, 50, 120)
+image = image[:, :, None]
+image = np.concatenate([image, image, image], axis=2)
+canny_image = Image.fromarray(image)
+
+controlnet_conditioning_scale = 0.5  # recommended for good generalization
+prompt = "Lara Croft with brown hair, and is wearing a tank top, a brown backpack. The room is dark and has an old-fashioned decor with a patterned floor and a wall featuring a design with arches and a dark area on the right side, muted color, high detail, 8k high definition award winning"
+negative_prompt = "underexposed, poorly drawn hands, duplicate hands, overexposed, bad art, beginner, amateur, abstract, disfigured, deformed, close up, weird colors, watermark"
+
+image = pipe(prompt,
+    image=ori_image,
+    control_image=canny_image,
+    height=1536,
+    width=2048,
+    strength=0.99,
+    num_inference_steps=50,
+    controlnet_conditioning_scale=controlnet_conditioning_scale,
+    guidance_scale=12.5,
+    negative_prompt = negative_prompt,
+    eta=1.0
+).images[0]
+
+image.save("lara.jpg")
+```
+
+<details>
+<summary>Output:</summary>
+<div align="center">
+  <img src="assets/lara_result.jpg" width="800" ></img>
+</div>
+</details>
+
 ## Inpainting
 
 ```python
 import torch
 from diffusers import AutoPipelineForInpainting, DDIMScheduler
 from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
@@ -296,15 +386,15 @@
 # remove following line if xFormers is not installed
 pipeline.enable_xformers_memory_efficient_attention()
 
 # load base and mask image
 img_url = "https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/diffusers/sdxl-text2img.png"
 init_image = load_image(img_url)
 # load mask_image.jpg in the assets file.
-mask_image = Image.open("mask_image.png")
+mask_image = Image.open("./assets/mask_image.png")
 
 prompt =  "A steampunk explorer in a leather aviator cap and goggles, with a brass telescope in hand, stands amidst towering ancient trees, their roots entwined with intricate gears and pipes."
 
 negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image = pipeline(prompt=prompt, image=init_image, mask_image=mask_image, height=2048, width=2048, strength=0.85, guidance_scale=12.5, negative_prompt = negative_prompt, eta=1.0).images[0]
 image.save('steampunk_explorer.jpg')
 ```
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.8 Summary: HiDiffusion: A
+training-free method to increase the resolution and speed of diffusion models.
+Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
+Jiajun Liang Description-Content-Type: text/markdown License-File: LICENSE
                          [assets/hidiffusion_logo.jpg]
 ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
@@ -9,47 +13,54 @@
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_P_a_p_e_r_&_m_e_s_s_a_g_e_=_A_r_x_i_v_:
       _H_i_D_i_f_f_u_s_i_o_n_&_c_o_l_o_r_=_r_e_d_&_l_o_g_o_=_a_r_x_i_v_]  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
           _v_1_?_l_a_b_e_l_=_D_e_m_o_&_m_e_s_s_a_g_e_=_C_o_l_a_b_&_c_o_l_o_r_=_p_u_r_p_l_e_&_l_o_g_o_=_g_o_o_g_l_e_c_o_l_a_b_] 
                           [assets/image_gallery.jpg]
   ((SSeelleecctt HHiiDDiiffffuussiioonn ssaammpplleess ffoorr vvaarriioouuss ddiiffffuussiioonn mmooddeellss,, rreessoolluuttiioonnss,, aanndd
                                 aassppeecctt rraattiiooss..))
 
-# ð Why HiDiffusion - A **training-free method that increases the resolution
-and speed of pretrained diffusion models.** - Designed as a **plug-and-play
-implementation**. It can be integrated into diffusion pipelines by **only
-adding a single line of code**!
+## ð Why HiDiffusion - A **training-free method that increases the
+resolution and speed of pretrained diffusion models.** - Designed as a **plug-
+and-play implementation**. It can be integrated into diffusion pipelines by
+**only adding a single line of code**! - Supports various tasks, including
+**text-to-image, image-to-image, inpainting**.
                         [assets/quality_efficiency.jpg]
                       ((FFaasstteerr,, aanndd bbeetttteerr iimmaaggee ddeettaaiillss..))
 
-## ð¢ Supported Models - â [Stable Diffusion XL](https://huggingface.co/
-papers/2307.01952) - â [Stable Diffusion XL Turbo](https://huggingface.co/
+                           [assets/various_task.jpg]
+               ((22KK rreessuullttss ooff CCoonnttrroollNNeett aanndd iinnppaaiinnttiinngg ttaasskkss..))
+
+## ð¥ Update - 2024.5.7 - ð¥ Support image-to-image task, see [here]
+(#image-to-image-generation). - 2024.4.16 - ð¥ Release source code. ## ð¢
+Supported Models - â [Stable Diffusion XL](https://huggingface.co/papers/
+2307.01952) - â [Stable Diffusion XL Turbo](https://huggingface.co/
 stabilityai/sdxl-turbo) - â [Stable Diffusion v2](https://huggingface.co/
 stabilityai/stable-diffusion-2-1) - â [Stable Diffusion v1](https://
 huggingface.co/runwayml/stable-diffusion-v1-5) **Note**: HiDiffusion also
 supports the downstream diffusion models based on these repositories, such as
 [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion),
 [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-
-aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
-â Inpainting ## ð Main Requirements This repository is tested on *
-Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
-accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
-installing the packages in the [main requirements](#-main-requirements),
-install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
-source Alternatively, you can install from github source. Clone the repository
-and install: ```bash git clone https://github.com/megvii-model/HiDiffusion.git
-cd HiDiffusion python3 setup.py install ``` ## ð Usage Generating outputs
-with HiDiffusion is super easy based on ð¤ [diffusers](https://github.com/
-huggingface/diffusers/tree/main). **You just need to add a single line of
-code**. ## Text-to-image generation ### Stable Diffusion XL ```python from
-hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
-StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
-"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
-DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
-StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
-scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
+aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet,
+including text-to-image, image-to-image - â Inpainting ## ð Main
+Requirements This repository is tested on * Python==3.8 * torch==1.13.1 *
+diffusers==0.27.0 * transformers==4.27.4 * accelerate==0.18.0 *
+xformers==0.0.16rc425 ## ð Install HiDiffusion After installing the packages
+in the [main requirements](#-main-requirements), install HiDiffusion: ```shell
+pip3 install hidiffusion ``` ### Installing from source Alternatively, you can
+install from github source. Clone the repository and install: ```bash git clone
+https://github.com/megvii-model/HiDiffusion.git cd HiDiffusion python3 setup.py
+install ``` ## ð Usage Generating outputs with HiDiffusion is super easy
+based on ð¤ [diffusers](https://github.com/huggingface/diffusers/tree/main).
+**You just need to add a single line of code**. ## Text-to-image generation ###
+Stable Diffusion XL ```python from hidiffusion import apply_hidiffusion,
+remove_hidiffusion from diffusers import StableDiffusionXLPipeline,
+DDIMScheduler import torch pretrain_model = "stabilityai/stable-diffusion-xl-
+base-1.0" scheduler = DDIMScheduler.from_pretrained(pretrain_model,
+subfolder="scheduler") pipe = StableDiffusionXLPipeline.from_pretrained
+(pretrain_model, scheduler = scheduler, torch_dtype=torch.float16,
+variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
 with a single line of code. apply_hidiffusion(pipe) prompt = "Standing tall
 amidst the ruins, a stone golem awakens, vines and flowers sprouting from the
 crevices in its body." negative_prompt = "blurry, ugly, duplicate, poorly drawn
@@ -109,54 +120,85 @@
 negative_prompt = "ugly, tiling, poorly drawn face, out of frame, disfigured,
 deformed, blurry, bad anatomy, blurred." image = pipe(prompt,
 guidance_scale=7.5, height=1024, width=1024, eta=1.0,
 negative_prompt=negative_prompt).images[0] image.save(f"fox.jpg") ``` Output:
                                [assets/sd15.jpg]
 Set height = 2048, width = 2048, and you can get output with 2048x2048
 resolution. ### Remove HiDiffusion If you want to remove HiDiiffusion, simply
-use `remove_hidiffusion(pipe)`. ## ControlNet ```python from diffusers import
-StableDiffusionXLControlNetPipeline, ControlNetModel, DDIMScheduler import
-numpy as np import torch import cv2 from PIL import Image from hidiffusion
-import apply_hidiffusion, remove_hidiffusion # load Yoshua_Bengio.jpg in the
-assets file. path = 'Yoshua_Bengio.jpg' image = Image.open(path) # get canny
-image image = np.array(image) image = cv2.Canny(image, 100, 200) image = image
-[:, :, None] image = np.concatenate([image, image, image], axis=2) canny_image
-= Image.fromarray(image) # initialize the models and pipeline
-controlnet_conditioning_scale = 0.5 # recommended for good generalization
-controlnet = ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-
-1.0", torch_dtype=torch.float16, variant="fp16" ) scheduler =
+use `remove_hidiffusion(pipe)`. ## ControlNet ### Text-to-image generation
+```python from diffusers import StableDiffusionXLControlNetPipeline,
+ControlNetModel, DDIMScheduler import numpy as np import torch import cv2 from
+PIL import Image from hidiffusion import apply_hidiffusion, remove_hidiffusion
+# load Yoshua_Bengio.jpg in the assets file. path = './assets/
+Yoshua_Bengio.jpg' image = Image.open(path) # get canny image image = np.array
+(image) image = cv2.Canny(image, 100, 200) image = image[:, :, None] image =
+np.concatenate([image, image, image], axis=2) canny_image = Image.fromarray
+(image) # initialize the models and pipeline controlnet_conditioning_scale =
+0.5 # recommended for good generalization controlnet =
+ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-1.0",
+torch_dtype=torch.float16, variant="fp16" ) scheduler =
 DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
 subfolder="scheduler") pipe =
 StableDiffusionXLControlNetPipeline.from_pretrained( "stabilityai/stable-
 diffusion-xl-base-1.0", controlnet=controlnet, torch_dtype=torch.float16,
 scheduler = scheduler ) # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
 pipe.enable_xformers_memory_efficient_attention() prompt = "The Joker, high
 face detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
 duplicate, poorly drawn, deformed, mosaic." image = pipe( prompt,
 controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
 height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt,
 eta=1.0 ).images[0] image.save('joker.jpg') ``` Output:
                         [assets/controlnet_result.jpg]
+### Image-to-image generation ```python import torch import numpy as np from
+PIL import Image from diffusers import ControlNetModel,
+StableDiffusionXLControlNetImg2ImgPipeline, DDIMScheduler from hidiffusion
+import apply_hidiffusion, remove_hidiffusion import cv2 controlnet =
+ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-1.0",
+torch_dtype=torch.float16, variant="fp16" ).to("cuda") scheduler =
+DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
+subfolder="scheduler") pipe =
+StableDiffusionXLControlNetImg2ImgPipeline.from_pretrained( "stabilityai/
+stable-diffusion-xl-base-1.0", controlnet=controlnet, scheduler = scheduler,
+torch_dtype=torch.float16, ).to("cuda") # Apply hidiffusion with a single line
+of code. apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
+pipe.enable_xformers_memory_efficient_attention() path = './assets/lara.jpeg'
+ori_image = Image.open(path) # get canny image image = np.array(ori_image)
+image = cv2.Canny(image, 50, 120) image = image[:, :, None] image =
+np.concatenate([image, image, image], axis=2) canny_image = Image.fromarray
+(image) controlnet_conditioning_scale = 0.5 # recommended for good
+generalization prompt = "Lara Croft with brown hair, and is wearing a tank top,
+a brown backpack. The room is dark and has an old-fashioned decor with a
+patterned floor and a wall featuring a design with arches and a dark area on
+the right side, muted color, high detail, 8k high definition award winning"
+negative_prompt = "underexposed, poorly drawn hands, duplicate hands,
+overexposed, bad art, beginner, amateur, abstract, disfigured, deformed, close
+up, weird colors, watermark" image = pipe(prompt, image=ori_image,
+control_image=canny_image, height=1536, width=2048, strength=0.99,
+num_inference_steps=50,
+controlnet_conditioning_scale=controlnet_conditioning_scale,
+guidance_scale=12.5, negative_prompt = negative_prompt, eta=1.0 ).images[0]
+image.save("lara.jpg") ``` Output:
+                           [assets/lara_result.jpg]
 ## Inpainting ```python import torch from diffusers import
 AutoPipelineForInpainting, DDIMScheduler from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion from PIL import
 Image scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-
 xl-base-1.0", subfolder="scheduler") pipeline =
 AutoPipelineForInpainting.from_pretrained( "diffusers/stable-diffusion-xl-1.0-
 inpainting-0.1", torch_dtype=torch.float16, variant="fp16", scheduler=scheduler
 ) # Apply hidiffusion with a single line of code. apply_hidiffusion(pipeline)
 pipeline.enable_model_cpu_offload() # remove following line if xFormers is not
 installed pipeline.enable_xformers_memory_efficient_attention() # load base and
 mask image img_url = "https://huggingface.co/datasets/huggingface/
 documentation-images/resolve/main/diffusers/sdxl-text2img.png" init_image =
 load_image(img_url) # load mask_image.jpg in the assets file. mask_image =
-Image.open("mask_image.png") prompt = "A steampunk explorer in a leather
-aviator cap and goggles, with a brass telescope in hand, stands amidst towering
-ancient trees, their roots entwined with intricate gears and pipes."
+Image.open("./assets/mask_image.png") prompt = "A steampunk explorer in a
+leather aviator cap and goggles, with a brass telescope in hand, stands amidst
+towering ancient trees, their roots entwined with intricate gears and pipes."
 negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image = pipeline(prompt=prompt, image=init_image, mask_image=mask_image,
 height=2048, width=2048, strength=0.85, guidance_scale=12.5, negative_prompt =
 negative_prompt, eta=1.0).images[0] image.save('steampunk_explorer.jpg') ```
 Output:
                         [assets/inpainting_result.jpg]
 ## Integration into downstream models HiDiffusion supports models based on
```

### Comparing `hidiffusion-0.1.6/hidiffusion/hidiffusion.py` & `hidiffusion-0.1.8/hidiffusion/hidiffusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                                'up_blocks.1.attentions.1.transformer_blocks.1', 
                                'up_blocks.1.attentions.2.transformer_blocks.0', 
                                'up_blocks.1.attentions.2.transformer_blocks.1']
     
     return modified_key
 
 # supported official model. If you use non-official model based on the following models/pipelines, hidiffusion will automatically select the best strategy to fit it. 
-surppoted_official_model = [
+supported_official_model = [
     'runwayml/stable-diffusion-v1-5', 'stabilityai/stable-diffusion-2-1-base',
     'stabilityai/stable-diffusion-xl-base-1.0', 'diffusers/stable-diffusion-xl-1.0-inpainting-0.1',
     'stabilityai/sdxl-turbo'
 ]
 
 
 # T1_ratio: see T1 introduced in the main paper. T1 = number_inference_step * T1_ratio. A higher T1_ratio can better mitigate object duplication. We set T1_ratio=0.4 by default. You'd better adjust it to fit your prompt. Only active when apply_raunet=True.
@@ -85,15 +85,15 @@
     'sd15_1024': {'T1_ratio': 0.4, 'T2_ratio': 0.0},
     'sd15_2048': {'T1_ratio': 0.7, 'T2_ratio': 0.3},
     'sdxl_2048': {'T1_ratio': 0.4, 'T2_ratio': 0.0},
     'sdxl_4096': {'T1_ratio': 0.7, 'T2_ratio': 0.3},
     'sdxl_turbo_1024': {'T1_ratio': 0.5, 'T2_ratio': 0.0},
 }
 
-controlnet_switching_threshold_ratio_dict = {
+text_to_img_controlnet_switching_threshold_ratio_dict = {
     'sdxl_2048': {'T1_ratio': 0.5, 'T2_ratio': 0.0},
 }
 controlnet_apply_steps_rate = 0.6
 
 is_aggressive_raunet = True
 aggressive_step = 8
 
@@ -106,185 +106,160 @@
     sd15_module_key = f.read().splitlines()
     
 with open(os.path.join(module_key_path, 'sdxl_module_key.txt'), 'r') as f:
     sdxl_module_key = f.read().splitlines()
 
 def make_diffusers_sdxl_contrtolnet_ppl(block_class):
 
-    EXAMPLE_DOC_STRING = """
-        Examples:
-            ```py
-            >>> # !pip install opencv-python transformers accelerate
-            >>> from diffusers import StableDiffusionXLControlNetPipeline, ControlNetModel, AutoencoderKL
-            >>> from diffusers.utils import load_image
-            >>> import numpy as np
-            >>> import torch
-
-            >>> import cv2
-            >>> from PIL import Image
-
-            >>> prompt = "aerial view, a futuristic research complex in a bright foggy jungle, hard lighting"
-            >>> negative_prompt = "low quality, bad quality, sketches"
-
-            >>> # download an image
-            >>> image = load_image(
-            ...     "https://hf.co/datasets/hf-internal-testing/diffusers-images/resolve/main/sd_controlnet/hf-logo.png"
-            ... )
-
-            >>> # initialize the models and pipeline
-            >>> controlnet_conditioning_scale = 0.5  # recommended for good generalization
-            >>> controlnet = ControlNetModel.from_pretrained(
-            ...     "diffusers/controlnet-canny-sdxl-1.0", torch_dtype=torch.float16
-            ... )
-            >>> vae = AutoencoderKL.from_pretrained("madebyollin/sdxl-vae-fp16-fix", torch_dtype=torch.float16)
-            >>> pipe = StableDiffusionXLControlNetPipeline.from_pretrained(
-            ...     "stabilityai/stable-diffusion-xl-base-1.0", controlnet=controlnet, vae=vae, torch_dtype=torch.float16
-            ... )
-            >>> pipe.enable_model_cpu_offload()
-
-            >>> # get canny image
-            >>> image = np.array(image)
-            >>> image = cv2.Canny(image, 100, 200)
-            >>> image = image[:, :, None]
-            >>> image = np.concatenate([image, image, image], axis=2)
-            >>> canny_image = Image.fromarray(image)
-
-            >>> # generate image
-            >>> image = pipe(
-            ...     prompt, controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image
-            ... ).images[0]
-            ```
-    """
     
     class sdxl_contrtolnet_ppl(block_class):
         # Save for unpatching later
         _parent = block_class
         
         @torch.no_grad()
-        @replace_example_docstring(EXAMPLE_DOC_STRING)
         def __call__(
             self,
             prompt: Union[str, List[str]] = None,
             prompt_2: Optional[Union[str, List[str]]] = None,
             image: PipelineImageInput = None,
+            control_image: PipelineImageInput = None,
             height: Optional[int] = None,
             width: Optional[int] = None,
+            strength: float = 0.8,
             num_inference_steps: int = 50,
             guidance_scale: float = 5.0,
             negative_prompt: Optional[Union[str, List[str]]] = None,
             negative_prompt_2: Optional[Union[str, List[str]]] = None,
             num_images_per_prompt: Optional[int] = 1,
             eta: float = 0.0,
             generator: Optional[Union[torch.Generator, List[torch.Generator]]] = None,
             latents: Optional[torch.FloatTensor] = None,
             prompt_embeds: Optional[torch.FloatTensor] = None,
             negative_prompt_embeds: Optional[torch.FloatTensor] = None,
             pooled_prompt_embeds: Optional[torch.FloatTensor] = None,
             negative_pooled_prompt_embeds: Optional[torch.FloatTensor] = None,
-            ip_adapter_image: Optional[PipelineImageInput] = None,
             output_type: Optional[str] = "pil",
             return_dict: bool = True,
             cross_attention_kwargs: Optional[Dict[str, Any]] = None,
-            controlnet_conditioning_scale: Union[float, List[float]] = 1.0,
+            controlnet_conditioning_scale: Union[float, List[float]] = 0.8,
             guess_mode: bool = False,
             control_guidance_start: Union[float, List[float]] = 0.0,
             control_guidance_end: Union[float, List[float]] = 1.0,
             original_size: Tuple[int, int] = None,
             crops_coords_top_left: Tuple[int, int] = (0, 0),
             target_size: Tuple[int, int] = None,
             negative_original_size: Optional[Tuple[int, int]] = None,
             negative_crops_coords_top_left: Tuple[int, int] = (0, 0),
             negative_target_size: Optional[Tuple[int, int]] = None,
+            aesthetic_score: float = 6.0,
+            negative_aesthetic_score: float = 2.5,
             clip_skip: Optional[int] = None,
             callback_on_step_end: Optional[Callable[[int, int, Dict], None]] = None,
             callback_on_step_end_tensor_inputs: List[str] = ["latents"],
             **kwargs,
         ):
             r"""
-            The call function to the pipeline for generation.
+            Function invoked when calling the pipeline for generation.
 
             Args:
                 prompt (`str` or `List[str]`, *optional*):
-                    The prompt or prompts to guide image generation. If not defined, you need to pass `prompt_embeds`.
+                    The prompt or prompts to guide the image generation. If not defined, one has to pass `prompt_embeds`.
+                    instead.
                 prompt_2 (`str` or `List[str]`, *optional*):
-                    The prompt or prompts to be sent to `tokenizer_2` and `text_encoder_2`. If not defined, `prompt` is
-                    used in both text-encoders.
+                    The prompt or prompts to be sent to the `tokenizer_2` and `text_encoder_2`. If not defined, `prompt` is
+                    used in both text-encoders
                 image (`torch.FloatTensor`, `PIL.Image.Image`, `np.ndarray`, `List[torch.FloatTensor]`, `List[PIL.Image.Image]`, `List[np.ndarray]`,:
                         `List[List[torch.FloatTensor]]`, `List[List[np.ndarray]]` or `List[List[PIL.Image.Image]]`):
-                    The ControlNet input condition to provide guidance to the `unet` for generation. If the type is
-                    specified as `torch.FloatTensor`, it is passed to ControlNet as is. `PIL.Image.Image` can also be
-                    accepted as an image. The dimensions of the output image defaults to `image`'s dimensions. If height
-                    and/or width are passed, `image` is resized accordingly. If multiple ControlNets are specified in
-                    `init`, images must be passed as a list such that each element of the list can be correctly batched for
-                    input to a single ControlNet.
-                height (`int`, *optional*, defaults to `self.unet.config.sample_size * self.vae_scale_factor`):
+                    The initial image will be used as the starting point for the image generation process. Can also accept
+                    image latents as `image`, if passing latents directly, it will not be encoded again.
+                control_image (`torch.FloatTensor`, `PIL.Image.Image`, `np.ndarray`, `List[torch.FloatTensor]`, `List[PIL.Image.Image]`, `List[np.ndarray]`,:
+                        `List[List[torch.FloatTensor]]`, `List[List[np.ndarray]]` or `List[List[PIL.Image.Image]]`):
+                    The ControlNet input condition. ControlNet uses this input condition to generate guidance to Unet. If
+                    the type is specified as `Torch.FloatTensor`, it is passed to ControlNet as is. `PIL.Image.Image` can
+                    also be accepted as an image. The dimensions of the output image defaults to `image`'s dimensions. If
+                    height and/or width are passed, `image` is resized according to them. If multiple ControlNets are
+                    specified in init, images must be passed as a list such that each element of the list can be correctly
+                    batched for input to a single controlnet.
+                height (`int`, *optional*, defaults to the size of control_image):
                     The height in pixels of the generated image. Anything below 512 pixels won't work well for
                     [stabilityai/stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)
                     and checkpoints that are not specifically fine-tuned on low resolutions.
-                width (`int`, *optional*, defaults to `self.unet.config.sample_size * self.vae_scale_factor`):
+                width (`int`, *optional*, defaults to the size of control_image):
                     The width in pixels of the generated image. Anything below 512 pixels won't work well for
                     [stabilityai/stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)
                     and checkpoints that are not specifically fine-tuned on low resolutions.
                 num_inference_steps (`int`, *optional*, defaults to 50):
                     The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                     expense of slower inference.
-                guidance_scale (`float`, *optional*, defaults to 5.0):
-                    A higher guidance scale value encourages the model to generate images closely linked to the text
-                    `prompt` at the expense of lower image quality. Guidance scale is enabled when `guidance_scale > 1`.
+                strength (`float`, *optional*, defaults to 0.3):
+                    Conceptually, indicates how much to transform the reference `image`. Must be between 0 and 1. `image`
+                    will be used as a starting point, adding more noise to it the larger the `strength`. The number of
+                    denoising steps depends on the amount of noise initially added. When `strength` is 1, added noise will
+                    be maximum and the denoising process will run for the full number of iterations specified in
+                    `num_inference_steps`.
+                guidance_scale (`float`, *optional*, defaults to 7.5):
+                    Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
+                    `guidance_scale` is defined as `w` of equation 2. of [Imagen
+                    Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
+                    1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
+                    usually at the expense of lower image quality.
                 negative_prompt (`str` or `List[str]`, *optional*):
-                    The prompt or prompts to guide what to not include in image generation. If not defined, you need to
-                    pass `negative_prompt_embeds` instead. Ignored when not using guidance (`guidance_scale < 1`).
+                    The prompt or prompts not to guide the image generation. If not defined, one has to pass
+                    `negative_prompt_embeds` instead. Ignored when not using guidance (i.e., ignored if `guidance_scale` is
+                    less than `1`).
                 negative_prompt_2 (`str` or `List[str]`, *optional*):
-                    The prompt or prompts to guide what to not include in image generation. This is sent to `tokenizer_2`
-                    and `text_encoder_2`. If not defined, `negative_prompt` is used in both text-encoders.
+                    The prompt or prompts not to guide the image generation to be sent to `tokenizer_2` and
+                    `text_encoder_2`. If not defined, `negative_prompt` is used in both text-encoders
                 num_images_per_prompt (`int`, *optional*, defaults to 1):
                     The number of images to generate per prompt.
                 eta (`float`, *optional*, defaults to 0.0):
-                    Corresponds to parameter eta (η) from the [DDIM](https://arxiv.org/abs/2010.02502) paper. Only applies
-                    to the [`~schedulers.DDIMScheduler`], and is ignored in other schedulers.
+                    Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
+                    [`schedulers.DDIMScheduler`], will be ignored for others.
                 generator (`torch.Generator` or `List[torch.Generator]`, *optional*):
-                    A [`torch.Generator`](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make
-                    generation deterministic.
+                    One or a list of [torch generator(s)](https://pytorch.org/docs/stable/generated/torch.Generator.html)
+                    to make generation deterministic.
                 latents (`torch.FloatTensor`, *optional*):
-                    Pre-generated noisy latents sampled from a Gaussian distribution, to be used as inputs for image
+                    Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
                     generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
-                    tensor is generated by sampling using the supplied random `generator`.
+                    tensor will ge generated by sampling using the supplied random `generator`.
                 prompt_embeds (`torch.FloatTensor`, *optional*):
-                    Pre-generated text embeddings. Can be used to easily tweak text inputs (prompt weighting). If not
-                    provided, text embeddings are generated from the `prompt` input argument.
+                    Pre-generated text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt weighting. If not
+                    provided, text embeddings will be generated from `prompt` input argument.
                 negative_prompt_embeds (`torch.FloatTensor`, *optional*):
-                    Pre-generated negative text embeddings. Can be used to easily tweak text inputs (prompt weighting). If
-                    not provided, `negative_prompt_embeds` are generated from the `negative_prompt` input argument.
+                    Pre-generated negative text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt
+                    weighting. If not provided, negative_prompt_embeds will be generated from `negative_prompt` input
+                    argument.
                 pooled_prompt_embeds (`torch.FloatTensor`, *optional*):
-                    Pre-generated pooled text embeddings. Can be used to easily tweak text inputs (prompt weighting). If
-                    not provided, pooled text embeddings are generated from `prompt` input argument.
+                    Pre-generated pooled text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt weighting.
+                    If not provided, pooled text embeddings will be generated from `prompt` input argument.
                 negative_pooled_prompt_embeds (`torch.FloatTensor`, *optional*):
-                    Pre-generated negative pooled text embeddings. Can be used to easily tweak text inputs (prompt
-                    weighting). If not provided, pooled `negative_prompt_embeds` are generated from `negative_prompt` input
-                    argument.
-                ip_adapter_image: (`PipelineImageInput`, *optional*): Optional image input to work with IP Adapters.
+                    Pre-generated negative pooled text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt
+                    weighting. If not provided, pooled negative_prompt_embeds will be generated from `negative_prompt`
+                    input argument.
                 output_type (`str`, *optional*, defaults to `"pil"`):
-                    The output format of the generated image. Choose between `PIL.Image` or `np.array`.
+                    The output format of the generate image. Choose between
+                    [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
                 return_dict (`bool`, *optional*, defaults to `True`):
                     Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                     plain tuple.
                 cross_attention_kwargs (`dict`, *optional*):
-                    A kwargs dictionary that if specified is passed along to the [`AttentionProcessor`] as defined in
-                    [`self.processor`](https://github.com/huggingface/diffusers/blob/main/src/diffusers/models/attention_processor.py).
+                    A kwargs dictionary that if specified is passed along to the `AttentionProcessor` as defined under
+                    `self.processor` in
+                    [diffusers.models.attention_processor](https://github.com/huggingface/diffusers/blob/main/src/diffusers/models/attention_processor.py).
                 controlnet_conditioning_scale (`float` or `List[float]`, *optional*, defaults to 1.0):
-                    The outputs of the ControlNet are multiplied by `controlnet_conditioning_scale` before they are added
-                    to the residual in the original `unet`. If multiple ControlNets are specified in `init`, you can set
-                    the corresponding scale as a list.
+                    The outputs of the controlnet are multiplied by `controlnet_conditioning_scale` before they are added
+                    to the residual in the original unet. If multiple ControlNets are specified in init, you can set the
+                    corresponding scale as a list.
                 guess_mode (`bool`, *optional*, defaults to `False`):
-                    The ControlNet encoder tries to recognize the content of the input image even if you remove all
-                    prompts. A `guidance_scale` value between 3.0 and 5.0 is recommended.
+                    In this mode, the ControlNet encoder will try best to recognize the content of the input image even if
+                    you remove all prompts. The `guidance_scale` between 3.0 and 5.0 is recommended.
                 control_guidance_start (`float` or `List[float]`, *optional*, defaults to 0.0):
-                    The percentage of total steps at which the ControlNet starts applying.
+                    The percentage of total steps at which the controlnet starts applying.
                 control_guidance_end (`float` or `List[float]`, *optional*, defaults to 1.0):
-                    The percentage of total steps at which the ControlNet stops applying.
+                    The percentage of total steps at which the controlnet stops applying.
                 original_size (`Tuple[int]`, *optional*, defaults to (1024, 1024)):
                     If `original_size` is not the same as `target_size` the image will appear to be down- or upsampled.
                     `original_size` defaults to `(height, width)` if not specified. Part of SDXL's micro-conditioning as
                     explained in section 2.2 of
                     [https://huggingface.co/papers/2307.01952](https://huggingface.co/papers/2307.01952).
                 crops_coords_top_left (`Tuple[int]`, *optional*, defaults to (0, 0)):
                     `crops_coords_top_left` can be used to generate an image that appears to be "cropped" from the position
@@ -306,14 +281,22 @@
                     [https://huggingface.co/papers/2307.01952](https://huggingface.co/papers/2307.01952). For more
                     information, refer to this issue thread: https://github.com/huggingface/diffusers/issues/4208.
                 negative_target_size (`Tuple[int]`, *optional*, defaults to (1024, 1024)):
                     To negatively condition the generation process based on a target image resolution. It should be as same
                     as the `target_size` for most cases. Part of SDXL's micro-conditioning as explained in section 2.2 of
                     [https://huggingface.co/papers/2307.01952](https://huggingface.co/papers/2307.01952). For more
                     information, refer to this issue thread: https://github.com/huggingface/diffusers/issues/4208.
+                aesthetic_score (`float`, *optional*, defaults to 6.0):
+                    Used to simulate an aesthetic score of the generated image by influencing the positive text condition.
+                    Part of SDXL's micro-conditioning as explained in section 2.2 of
+                    [https://huggingface.co/papers/2307.01952](https://huggingface.co/papers/2307.01952).
+                negative_aesthetic_score (`float`, *optional*, defaults to 2.5):
+                    Part of SDXL's micro-conditioning as explained in section 2.2 of
+                    [https://huggingface.co/papers/2307.01952](https://huggingface.co/papers/2307.01952). Can be used to
+                    simulate an aesthetic score of the generated image by influencing the negative text condition.
                 clip_skip (`int`, *optional*):
                     Number of layers to be skipped from CLIP while computing the prompt embeddings. A value of 1 means that
                     the output of the pre-final layer will be used for computing the prompt embeddings.
                 callback_on_step_end (`Callable`, *optional*):
                     A function that calls at the end of each denoising steps during the inference. The function is called
                     with the following arguments: `callback_on_step_end(self: DiffusionPipeline, step: int, timestep: int,
                     callback_kwargs: Dict)`. `callback_kwargs` will include a list of all tensors as specified by
@@ -323,18 +306,26 @@
                     will be passed as `callback_kwargs` argument. You will only be able to include variables listed in the
                     `._callback_tensor_inputs` attribute of your pipeine class.
 
             Examples:
 
             Returns:
                 [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
-                    If `return_dict` is `True`, [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] is returned,
-                    otherwise a `tuple` is returned containing the output images.
+                [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple`
+                containing the output images.
             """
-
+            
+            # convert image to control_image to fit sdxl_controlnet ppl. 
+            if control_image is None:
+                control_image = image 
+                image = None 
+                self.info['text_to_img_controlnet'] = True 
+            else:
+                self.info['text_to_img_controlnet'] = False 
+            
             callback = kwargs.pop("callback", None)
             callback_steps = kwargs.pop("callback_steps", None)
 
             if callback is not None:
                 deprecate(
                     "callback",
                     "1.0.0",
@@ -358,50 +349,94 @@
                 mult = len(controlnet.nets) if isinstance(controlnet, MultiControlNetModel) else 1
                 control_guidance_start, control_guidance_end = (
                     mult * [control_guidance_start],
                     mult * [control_guidance_end],
                 )
 
             # 1. Check inputs. Raise error if not correct
-            if old_diffusers:
-                self.check_inputs(
-                    prompt,
-                    prompt_2,
-                    image,
-                    callback_steps,
-                    negative_prompt,
-                    negative_prompt_2,
-                    prompt_embeds,
-                    negative_prompt_embeds,
-                    pooled_prompt_embeds,
-                    negative_pooled_prompt_embeds,
-                    controlnet_conditioning_scale,
-                    control_guidance_start,
-                    control_guidance_end,
-                    callback_on_step_end_tensor_inputs,
-                )
+            if image is not None:
+                # image-to-image controlnet
+                if old_diffusers:
+                    self.check_inputs(
+                        prompt,
+                        prompt_2,
+                        control_image,
+                        strength,
+                        num_inference_steps,
+                        callback_steps,
+                        negative_prompt,
+                        negative_prompt_2,
+                        prompt_embeds,
+                        negative_prompt_embeds,
+                        pooled_prompt_embeds,
+                        negative_pooled_prompt_embeds,
+                        controlnet_conditioning_scale,
+                        control_guidance_start,
+                        control_guidance_end,
+                        callback_on_step_end_tensor_inputs,
+                    )
+                else:
+                    self.check_inputs(
+                        prompt,
+                        prompt_2,
+                        control_image,
+                        strength,
+                        num_inference_steps,
+                        callback_steps,
+                        negative_prompt,
+                        negative_prompt_2,
+                        prompt_embeds,
+                        negative_prompt_embeds,
+                        pooled_prompt_embeds,
+                        negative_pooled_prompt_embeds,
+                        None,
+                        None,
+                        controlnet_conditioning_scale,
+                        control_guidance_start,
+                        control_guidance_end,
+                        callback_on_step_end_tensor_inputs,
+                    )
             else:
-                self.check_inputs(
-                    prompt,
-                    prompt_2,
-                    image,
-                    callback_steps,
-                    negative_prompt,
-                    negative_prompt_2,
-                    prompt_embeds,
-                    negative_prompt_embeds,
-                    pooled_prompt_embeds,
-                    None,
-                    None,
-                    negative_pooled_prompt_embeds,
-                    controlnet_conditioning_scale,
-                    control_guidance_start,
-                    control_guidance_end,
-                    callback_on_step_end_tensor_inputs,
-                )
+                # text-to-image controlnet
+                if old_diffusers:
+                    self.check_inputs(
+                        prompt,
+                        prompt_2,
+                        control_image,
+                        callback_steps,
+                        negative_prompt,
+                        negative_prompt_2,
+                        prompt_embeds,
+                        negative_prompt_embeds,
+                        pooled_prompt_embeds,
+                        negative_pooled_prompt_embeds,
+                        controlnet_conditioning_scale,
+                        control_guidance_start,
+                        control_guidance_end,
+                        callback_on_step_end_tensor_inputs,
+                    )
+                else:
+                    self.check_inputs(
+                        prompt,
+                        prompt_2,
+                        control_image,
+                        callback_steps,
+                        negative_prompt,
+                        negative_prompt_2,
+                        prompt_embeds,
+                        negative_prompt_embeds,
+                        pooled_prompt_embeds,
+                        None,
+                        None,
+                        negative_pooled_prompt_embeds,
+                        controlnet_conditioning_scale,
+                        control_guidance_start,
+                        control_guidance_end,
+                        callback_on_step_end_tensor_inputs,
+                    )
 
             self._guidance_scale = guidance_scale
             self._clip_skip = clip_skip
             self._cross_attention_kwargs = cross_attention_kwargs
 
             # 2. Define call parameters
             if prompt is not None and isinstance(prompt, str):
@@ -419,15 +454,15 @@
             global_pool_conditions = (
                 controlnet.config.global_pool_conditions
                 if isinstance(controlnet, ControlNetModel)
                 else controlnet.nets[0].config.global_pool_conditions
             )
             guess_mode = guess_mode or global_pool_conditions
 
-            # 3.1 Encode input prompt
+            # 3. Encode input prompt
             text_encoder_lora_scale = (
                 self.cross_attention_kwargs.get("scale", None) if self.cross_attention_kwargs is not None else None
             )
             (
                 prompt_embeds,
                 negative_prompt_embeds,
                 pooled_prompt_embeds,
@@ -444,150 +479,238 @@
                 negative_prompt_embeds=negative_prompt_embeds,
                 pooled_prompt_embeds=pooled_prompt_embeds,
                 negative_pooled_prompt_embeds=negative_pooled_prompt_embeds,
                 lora_scale=text_encoder_lora_scale,
                 clip_skip=self.clip_skip,
             )
 
-            # 3.2 Encode ip_adapter_image
-            if ip_adapter_image is not None:
-                output_hidden_state = False if isinstance(self.unet.encoder_hid_proj, ImageProjection) else True
-                image_embeds, negative_image_embeds = self.encode_image(
-                    ip_adapter_image, device, num_images_per_prompt, output_hidden_state
-                )
-                if self.do_classifier_free_guidance:
-                    image_embeds = torch.cat([negative_image_embeds, image_embeds])
-
-            # 4. Prepare image
-            if isinstance(controlnet, ControlNetModel):
-                image = self.prepare_image(
-                    image=image,
-                    width=width,
-                    height=height,
-                    batch_size=batch_size * num_images_per_prompt,
-                    num_images_per_prompt=num_images_per_prompt,
-                    device=device,
-                    dtype=controlnet.dtype,
-                    do_classifier_free_guidance=self.do_classifier_free_guidance,
-                    guess_mode=guess_mode,
-                )
-                height, width = image.shape[-2:]
-            elif isinstance(controlnet, MultiControlNetModel):
-                images = []
-
-                for image_ in image:
-                    image_ = self.prepare_image(
-                        image=image_,
+            # 4. Prepare image and controlnet_conditioning_image
+            if image is not None:
+                image = self.image_processor.preprocess(image, height=height, width=width).to(dtype=torch.float32)
+                if isinstance(controlnet, ControlNetModel):
+                    control_image = self.prepare_control_image(
+                        image=control_image,
                         width=width,
                         height=height,
                         batch_size=batch_size * num_images_per_prompt,
                         num_images_per_prompt=num_images_per_prompt,
                         device=device,
                         dtype=controlnet.dtype,
                         do_classifier_free_guidance=self.do_classifier_free_guidance,
                         guess_mode=guess_mode,
                     )
+                    height, width = control_image.shape[-2:]
+                elif isinstance(controlnet, MultiControlNetModel):
+                    control_images = []
+
+                    for control_image_ in control_image:
+                        control_image_ = self.prepare_control_image(
+                            image=control_image_,
+                            width=width,
+                            height=height,
+                            batch_size=batch_size * num_images_per_prompt,
+                            num_images_per_prompt=num_images_per_prompt,
+                            device=device,
+                            dtype=controlnet.dtype,
+                            do_classifier_free_guidance=self.do_classifier_free_guidance,
+                            guess_mode=guess_mode,
+                        )
 
-                    images.append(image_)
+                        control_images.append(control_image_)
 
-                image = images
-                height, width = image[0].shape[-2:]
+                    control_image = control_images
+                    height, width = control_image[0].shape[-2:]
+                else:
+                    assert False
             else:
-                assert False
+                if isinstance(controlnet, ControlNetModel):
+                    control_image = self.prepare_image(
+                        image=control_image,
+                        width=width,
+                        height=height,
+                        batch_size=batch_size * num_images_per_prompt,
+                        num_images_per_prompt=num_images_per_prompt,
+                        device=device,
+                        dtype=controlnet.dtype,
+                        do_classifier_free_guidance=self.do_classifier_free_guidance,
+                        guess_mode=guess_mode,
+                    )
+                    height, width = control_image.shape[-2:]
+                elif isinstance(controlnet, MultiControlNetModel):
+                    images = []
+
+                    for image_ in control_image:
+                        image_ = self.prepare_image(
+                            image=image_,
+                            width=width,
+                            height=height,
+                            batch_size=batch_size * num_images_per_prompt,
+                            num_images_per_prompt=num_images_per_prompt,
+                            device=device,
+                            dtype=controlnet.dtype,
+                            do_classifier_free_guidance=self.do_classifier_free_guidance,
+                            guess_mode=guess_mode,
+                        )
+
+                        images.append(image_)
 
+                    control_image = images
+                    height, width = image[0].shape[-2:]
+                else:
+                    assert False
             # 5. Prepare timesteps
             self.scheduler.set_timesteps(num_inference_steps, device=device)
-            timesteps = self.scheduler.timesteps
+            if image is not None:
+                timesteps, num_inference_steps = self.get_timesteps(num_inference_steps, strength, device)
+                latent_timestep = timesteps[:1].repeat(batch_size * num_images_per_prompt)
+            else:
+                timesteps = self.scheduler.timesteps
             self._num_timesteps = len(timesteps)
 
             # 6. Prepare latent variables
-            num_channels_latents = self.unet.config.in_channels
-            latents = self.prepare_latents(
-                batch_size * num_images_per_prompt,
-                num_channels_latents,
-                height,
-                width,
-                prompt_embeds.dtype,
-                device,
-                generator,
-                latents,
-            )
+            if image is not None:
+                # image-to-image controlnet
+                latents = self.prepare_latents(
+                    image,
+                    latent_timestep,
+                    batch_size,
+                    num_images_per_prompt,
+                    prompt_embeds.dtype,
+                    device,
+                    generator,
+                    True,
+                )
+            else:
+                # text-to-image controlnet
+                num_channels_latents = self.unet.config.in_channels
+                latents = self.prepare_latents(
+                    batch_size * num_images_per_prompt,
+                    num_channels_latents,
+                    height,
+                    width,
+                    prompt_embeds.dtype,
+                    device,
+                    generator,
+                    latents,
+                )
+                # num_channels_latents = self.unet.config.in_channels
+                # shape = (batch_size * num_images_per_prompt, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
+                # if isinstance(generator, list) and len(generator) != batch_size:
+                #     raise ValueError(
+                #         f"You have passed a list of generators of length {len(generator)}, but requested an effective batch"
+                #         f" size of {batch_size}. Make sure the batch size matches the length of the generators."
+                #     )
+
+                # if latents is None:
+                #     latents = randn_tensor(shape, generator=generator, device=device, dtype=dtype)
+                # else:
+                #     latents = latents.to(device)
 
-            # 6.5 Optionally get Guidance Scale Embedding
-            timestep_cond = None
-            if self.unet.config.time_cond_proj_dim is not None:
-                guidance_scale_tensor = torch.tensor(self.guidance_scale - 1).repeat(batch_size * num_images_per_prompt)
-                timestep_cond = self.get_guidance_scale_embedding(
-                    guidance_scale_tensor, embedding_dim=self.unet.config.time_cond_proj_dim
-                ).to(device=device, dtype=latents.dtype)
+                # # scale the initial noise by the standard deviation required by the scheduler
+                # latents = latents * self.scheduler.init_noise_sigma
 
             # 7. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
             extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
             # 7.1 Create tensor stating which controlnets to keep
             controlnet_keep = []
             for i in range(len(timesteps)):
                 keeps = [
                     1.0 - float(i / len(timesteps) < s or (i + 1) / len(timesteps) > e)
                     for s, e in zip(control_guidance_start, control_guidance_end)
                 ]
                 controlnet_keep.append(keeps[0] if isinstance(controlnet, ControlNetModel) else keeps)
 
             # 7.2 Prepare added time ids & embeddings
-            if isinstance(image, list):
-                original_size = original_size or image[0].shape[-2:]
-            else:
-                original_size = original_size or image.shape[-2:]
-            target_size = target_size or (height, width)
+            if image is not None:
+                if isinstance(control_image, list):
+                    original_size = original_size or control_image[0].shape[-2:]
+                else:
+                    original_size = original_size or control_image.shape[-2:]
+                target_size = target_size or (height, width)
 
-            add_text_embeds = pooled_prompt_embeds
-            if self.text_encoder_2 is None:
-                text_encoder_projection_dim = int(pooled_prompt_embeds.shape[-1])
-            else:
-                text_encoder_projection_dim = self.text_encoder_2.config.projection_dim
+                if negative_original_size is None:
+                    negative_original_size = original_size
+                if negative_target_size is None:
+                    negative_target_size = target_size
+                add_text_embeds = pooled_prompt_embeds
 
-            add_time_ids = self._get_add_time_ids(
-                original_size,
-                crops_coords_top_left,
-                target_size,
-                dtype=prompt_embeds.dtype,
-                text_encoder_projection_dim=text_encoder_projection_dim,
-            )
+                if self.text_encoder_2 is None:
+                    text_encoder_projection_dim = int(pooled_prompt_embeds.shape[-1])
+                else:
+                    text_encoder_projection_dim = self.text_encoder_2.config.projection_dim
 
-            if negative_original_size is not None and negative_target_size is not None:
-                negative_add_time_ids = self._get_add_time_ids(
+                add_time_ids, add_neg_time_ids = self._get_add_time_ids(
+                    original_size,
+                    crops_coords_top_left,
+                    target_size,
+                    aesthetic_score,
+                    negative_aesthetic_score,
                     negative_original_size,
                     negative_crops_coords_top_left,
                     negative_target_size,
                     dtype=prompt_embeds.dtype,
                     text_encoder_projection_dim=text_encoder_projection_dim,
                 )
+                add_time_ids = add_time_ids.repeat(batch_size * num_images_per_prompt, 1)
+
+                if self.do_classifier_free_guidance:
+                    prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds], dim=0)
+                    add_text_embeds = torch.cat([negative_pooled_prompt_embeds, add_text_embeds], dim=0)
+                    add_neg_time_ids = add_neg_time_ids.repeat(batch_size * num_images_per_prompt, 1)
+                    add_time_ids = torch.cat([add_neg_time_ids, add_time_ids], dim=0)
+
+                prompt_embeds = prompt_embeds.to(device)
+                add_text_embeds = add_text_embeds.to(device)
+                add_time_ids = add_time_ids.to(device)
             else:
-                negative_add_time_ids = add_time_ids
+                if isinstance(control_image, list):
+                    original_size = original_size or control_image[0].shape[-2:]
+                else:
+                    original_size = original_size or control_image.shape[-2:]
+                target_size = target_size or (height, width)
+
+                add_text_embeds = pooled_prompt_embeds
+                if self.text_encoder_2 is None:
+                    text_encoder_projection_dim = int(pooled_prompt_embeds.shape[-1])
+                else:
+                    text_encoder_projection_dim = self.text_encoder_2.config.projection_dim
+
+                add_time_ids = self._get_add_time_ids(
+                    original_size,
+                    crops_coords_top_left,
+                    target_size,
+                    dtype=prompt_embeds.dtype,
+                    text_encoder_projection_dim=text_encoder_projection_dim,
+                )
+
+                if negative_original_size is not None and negative_target_size is not None:
+                    negative_add_time_ids = self._get_add_time_ids(
+                        negative_original_size,
+                        negative_crops_coords_top_left,
+                        negative_target_size,
+                        dtype=prompt_embeds.dtype,
+                        text_encoder_projection_dim=text_encoder_projection_dim,
+                    )
+                else:
+                    negative_add_time_ids = add_time_ids
 
-            if self.do_classifier_free_guidance:
-                prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds], dim=0)
-                add_text_embeds = torch.cat([negative_pooled_prompt_embeds, add_text_embeds], dim=0)
-                add_time_ids = torch.cat([negative_add_time_ids, add_time_ids], dim=0)
-
-            prompt_embeds = prompt_embeds.to(device)
-            add_text_embeds = add_text_embeds.to(device)
-            add_time_ids = add_time_ids.to(device).repeat(batch_size * num_images_per_prompt, 1)
+                if self.do_classifier_free_guidance:
+                    prompt_embeds = torch.cat([negative_prompt_embeds, prompt_embeds], dim=0)
+                    add_text_embeds = torch.cat([negative_pooled_prompt_embeds, add_text_embeds], dim=0)
+                    add_time_ids = torch.cat([negative_add_time_ids, add_time_ids], dim=0)
+
+                prompt_embeds = prompt_embeds.to(device)
+                add_text_embeds = add_text_embeds.to(device)
+                add_time_ids = add_time_ids.to(device).repeat(batch_size * num_images_per_prompt, 1)
 
             # 8. Denoising loop
             num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
-            is_unet_compiled = is_compiled_module(self.unet)
-            is_controlnet_compiled = is_compiled_module(self.controlnet)
-            is_torch_higher_equal_2_1 = is_torch_version(">=", "2.1")
             with self.progress_bar(total=num_inference_steps) as progress_bar:
                 for i, t in enumerate(timesteps):
-                    # Relevant thread:
-                    # https://dev-discuss.pytorch.org/t/cudagraphs-in-pytorch-2-0/1428
-                    if (is_unet_compiled and is_controlnet_compiled) and is_torch_higher_equal_2_1:
-                        torch._inductor.cudagraph_mark_step_begin()
                     # expand the latents if we are doing classifier free guidance
                     latent_model_input = torch.cat([latents] * 2) if self.do_classifier_free_guidance else latents
                     latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
                     added_cond_kwargs = {"text_embeds": add_text_embeds, "time_ids": add_time_ids}
 
                     # controlnet(s) inference
@@ -609,67 +732,65 @@
                         cond_scale = [c * s for c, s in zip(controlnet_conditioning_scale, controlnet_keep[i])]
                     else:
                         controlnet_cond_scale = controlnet_conditioning_scale
                         if isinstance(controlnet_cond_scale, list):
                             controlnet_cond_scale = controlnet_cond_scale[0]
                         cond_scale = controlnet_cond_scale * controlnet_keep[i]
 
+                    
                     if i < controlnet_apply_steps_rate * num_inference_steps:
+                        
                         original_h, original_w = (128,128)
                         _, _, model_input_h, model_input_w = control_model_input.shape
-                        downsample_factor = math.ceil(max(model_input_h/original_h, model_input_w/original_w))
-                        downsample_size = (model_input_h//downsample_factor, model_input_w//downsample_factor)
+                        downsample_factor = max(model_input_h/original_h, model_input_w/original_w)
+                        downsample_size = (int(model_input_h//downsample_factor)//8*8, int(model_input_w//downsample_factor)//8*8)
                         
-                        original_pixel_h, original_pixel_w = (1024,1024)
-                        _, _, pixel_h, pixel_w = image.shape
-                        downsample_pixel_factor = math.ceil(max(pixel_h/original_pixel_h, pixel_w/original_pixel_w))
-                        downsample_pixel_size = (pixel_h//downsample_pixel_factor, pixel_w//downsample_pixel_factor)
+                        # original_pixel_h, original_pixel_w = (1024,1024)
+                        # _, _, pixel_h, pixel_w = control_image.shape
+                        # downsample_pixel_factor = max(pixel_h/original_pixel_h, pixel_w/original_pixel_w)
+                        # downsample_pixel_size = (int(pixel_h//downsample_pixel_factor)//8*8, int(pixel_w//downsample_pixel_factor)//8*8)
+                        downsample_pixel_size = [downsample_size[0]*8, downsample_size[1]*8]
                         
                         down_block_res_samples, mid_block_res_sample = self.controlnet(
                             F.interpolate(control_model_input, downsample_size),
                             # control_model_input,
                             t,
                             encoder_hidden_states=controlnet_prompt_embeds,
-                            # controlnet_cond=image,
-                            controlnet_cond=F.interpolate(image, downsample_pixel_size),
+                            controlnet_cond=F.interpolate(control_image, downsample_pixel_size),
+                            # controlnet_cond=control_image,
                             conditioning_scale=cond_scale,
                             guess_mode=guess_mode,
                             added_cond_kwargs=controlnet_added_cond_kwargs,
                             return_dict=False,
                         )
 
                     if guess_mode and self.do_classifier_free_guidance:
                         # Infered ControlNet only for the conditional batch.
                         # To apply the output of ControlNet to both the unconditional and conditional batches,
                         # add 0 to the unconditional batch to keep it unchanged.
                         down_block_res_samples = [torch.cat([torch.zeros_like(d), d]) for d in down_block_res_samples]
                         mid_block_res_sample = torch.cat([torch.zeros_like(mid_block_res_sample), mid_block_res_sample])
 
-                    if ip_adapter_image is not None:
-                        added_cond_kwargs["image_embeds"] = image_embeds
-
                     # predict the noise residual
                     if i < controlnet_apply_steps_rate * num_inference_steps:
                         noise_pred = self.unet(
                             latent_model_input,
                             t,
                             encoder_hidden_states=prompt_embeds,
-                            timestep_cond=timestep_cond,
                             cross_attention_kwargs=self.cross_attention_kwargs,
                             down_block_additional_residuals=down_block_res_samples,
                             mid_block_additional_residual=mid_block_res_sample,
                             added_cond_kwargs=added_cond_kwargs,
                             return_dict=False,
                         )[0]
                     else:
                         noise_pred = self.unet(
                             latent_model_input,
                             t,
                             encoder_hidden_states=prompt_embeds,
-                            timestep_cond=timestep_cond,
                             cross_attention_kwargs=self.cross_attention_kwargs,
                             down_block_additional_residuals=None,
                             mid_block_additional_residual=None,
                             added_cond_kwargs=added_cond_kwargs,
                             return_dict=False,
                         )[0]
 
@@ -694,18 +815,20 @@
                     # call the callback, if provided
                     if i == len(timesteps) - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0):
                         progress_bar.update()
                         if callback is not None and i % callback_steps == 0:
                             step_idx = i // getattr(self.scheduler, "order", 1)
                             callback(step_idx, t, latents)
 
+            # If we do sequential model offloading, let's offload unet and controlnet
             # manually for max memory savings
-            if self.vae.dtype == torch.float16 and self.vae.config.force_upcast:
-                self.upcast_vae()
-                latents = latents.to(next(iter(self.vae.post_quant_conv.parameters())).dtype)
+            if hasattr(self, "final_offload_hook") and self.final_offload_hook is not None:
+                self.unet.to("cpu")
+                self.controlnet.to("cpu")
+                torch.cuda.empty_cache()
 
             if not output_type == "latent":
                 # make sure the VAE is in float32 mode, as it overflows in float16
                 needs_upcasting = self.vae.dtype == torch.float16 and self.vae.config.force_upcast
 
                 if needs_upcasting:
                     self.upcast_vae()
@@ -714,21 +837,21 @@
                 image = self.vae.decode(latents / self.vae.config.scaling_factor, return_dict=False)[0]
 
                 # cast back to fp16 if needed
                 if needs_upcasting:
                     self.vae.to(dtype=torch.float16)
             else:
                 image = latents
+                return StableDiffusionXLPipelineOutput(images=image)
 
-            if not output_type == "latent":
-                # apply watermark if available
-                if self.watermark is not None:
-                    image = self.watermark.apply_watermark(image)
+            # apply watermark if available
+            if self.watermark is not None:
+                image = self.watermark.apply_watermark(image)
 
-                image = self.image_processor.postprocess(image, output_type=output_type)
+            image = self.image_processor.postprocess(image, output_type=output_type)
 
             # Offload all models
             self.maybe_free_model_hooks()
 
             if not return_dict:
                 return (image,)
 
@@ -1357,26 +1480,26 @@
             encoder_hidden_states: Optional[torch.FloatTensor] = None,
             attention_mask: Optional[torch.FloatTensor] = None,
             cross_attention_kwargs: Optional[Dict[str, Any]] = None,
             encoder_attention_mask: Optional[torch.FloatTensor] = None,
             additional_residuals: Optional[torch.FloatTensor] = None,
         ) -> Tuple[torch.FloatTensor, Tuple[torch.FloatTensor, ...]]:
             
-            self.max_timestep = len(self.info['scheduler'].timesteps)
-            
+            self.max_timestep = self.info['pipeline']._num_timesteps
+            # self.max_timestep = len(self.info['scheduler'].timesteps)
             ori_H, ori_W = self.info['size']
             if self.model == 'sd15':
                 if ori_H < 256 or ori_W < 256:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_1024'][self.switching_threshold_ratio]
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_2048'][self.switching_threshold_ratio]
             elif self.model == 'sdxl':
                 if ori_H < 512 or ori_W < 512:
-                    if self.info['use_controlnet']:
-                        self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
+                    if self.info['text_to_img_controlnet']:
+                        self.T1_ratio = text_to_img_controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                         
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
                     elif self.info['is_playground']:
                         self.aggressive_raunet = playground_is_aggressive_raunet
@@ -1487,26 +1610,27 @@
             temb: Optional[torch.FloatTensor] = None,
             encoder_hidden_states: Optional[torch.FloatTensor] = None,
             cross_attention_kwargs: Optional[Dict[str, Any]] = None,
             upsample_size: Optional[int] = None,
             attention_mask: Optional[torch.FloatTensor] = None,
             encoder_attention_mask: Optional[torch.FloatTensor] = None,
         ) -> torch.FloatTensor:
-            self.max_timestep = len(self.info['scheduler'].timesteps)
             
+            self.max_timestep = self.info['pipeline']._num_timesteps
+            # self.max_timestep = len(self.info['scheduler'].timesteps)
             ori_H, ori_W = self.info['size']
             if self.model == 'sd15':
                 if ori_H < 256 or ori_W < 256:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_1024'][self.switching_threshold_ratio]
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_2048'][self.switching_threshold_ratio]
             elif self.model == 'sdxl':
                 if ori_H < 512 or ori_W < 512:
-                    if self.info['use_controlnet']:
-                        self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
+                    if self.info['text_to_img_controlnet']:
+                        self.T1_ratio = text_to_img_controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                         
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
                     elif self.info['is_playground']:
                         self.aggressive_raunet = playground_is_aggressive_raunet
@@ -1623,25 +1747,26 @@
         T1_ratio = 0
         T1 = 0
         timestep = 0
         aggressive_raunet = False
         max_timestep = 50
         
         def forward(self, hidden_states: torch.Tensor, scale = 1.0) -> torch.Tensor:
-            self.max_timestep = len(self.info['scheduler'].timesteps)
+            self.max_timestep = self.info['pipeline']._num_timesteps
+            # self.max_timestep = len(self.info['scheduler'].timesteps)
             ori_H, ori_W = self.info['size']
             if self.model == 'sd15':
                 if ori_H < 256 or ori_W < 256:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_1024'][self.switching_threshold_ratio]
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_2048'][self.switching_threshold_ratio]
             elif self.model == 'sdxl':
                 if ori_H < 512 or ori_W < 512:
-                    if self.info['use_controlnet']:
-                        self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
+                    if self.info['text_to_img_controlnet']:
+                        self.T1_ratio = text_to_img_controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                         
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
                     elif self.info['is_playground']:
                         self.aggressive_raunet = playground_is_aggressive_raunet
@@ -1711,26 +1836,26 @@
         T1_ratio = 0
         T1 = 0
         timestep = 0
         aggressive_raunet = False
         max_timestep = 50
         
         def forward(self, hidden_states: torch.Tensor, scale = 1.0) -> torch.Tensor:
-            self.max_timestep = len(self.info['scheduler'].timesteps)
-
+            self.max_timestep = self.info['pipeline']._num_timesteps
+            # self.max_timestep = len(self.info['scheduler'].timesteps)
             ori_H, ori_W = self.info['size']
             if self.model == 'sd15':
                 if ori_H < 256 or ori_W < 256:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_1024'][self.switching_threshold_ratio]
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_2048'][self.switching_threshold_ratio]
             elif self.model == 'sdxl':
                 if ori_H < 512 or ori_W < 512:
-                    if self.info['use_controlnet']:
-                        self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
+                    if self.info['text_to_img_controlnet']:
+                        self.T1_ratio = text_to_img_controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                         
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
                     elif self.info['is_playground']:
                         self.aggressive_raunet = playground_is_aggressive_raunet
@@ -1800,41 +1925,45 @@
 
     # Make sure the module is not currently patched
     remove_hidiffusion(model)
 
     is_diffusers = isinstance_str(model, "DiffusionPipeline") or isinstance_str(model, "ModelMixin")
 
     if not is_diffusers:
-        # if not hasattr(model, "model") or not hasattr(model.model, "diffusion_model"):
-        #     # Provided model not supported
-        #     raise RuntimeError("Provided model was not a Stable Diffusion / Latent Diffusion model, as expected.")
-        # diffusion_model = model.model.diffusion_model
         raise RuntimeError("Provided model was not a diffusers model/pipeline, as expected.")
     else:
         if hasattr(model, 'controlnet'):
             make_ppl_fn = make_diffusers_sdxl_contrtolnet_ppl
             model.__class__ = make_ppl_fn(model.__class__)
             
             make_block_fn = make_diffusers_unet_2d_condition
             model.unet.__class__ = make_block_fn(model.unet.__class__)
         diffusion_model = model.unet if hasattr(model, "unet") else model
 
+    # force forward_upsample_size=True, see unet_2d_condition.py in diffusers
+    diffusion_model.num_upsamplers += 2
     
     name_or_path = model.name_or_path
     diffusion_model_module_key = []
-    if name_or_path not in surppoted_official_model:
+    if name_or_path not in supported_official_model:
         for key, module in diffusion_model.named_modules():
             diffusion_model_module_key.append(key)
         if set(sd15_module_key) < set(diffusion_model_module_key):
             name_or_path = 'runwayml/stable-diffusion-v1-5'
         elif set(sdxl_module_key) < set(diffusion_model_module_key):
             name_or_path = 'stabilityai/stable-diffusion-xl-base-1.0'
 
-    diffusion_model.info = {'size': None, 'hooks': [], 'scheduler': model.scheduler, 'use_controlnet': hasattr(model, 'controlnet'),
-                            'is_inpainting_task': 'inpainting' in model.name_or_path, 'is_playground': 'playground' in model.name_or_path}
+    diffusion_model.info = {
+        'size': None, 
+        'hooks': [], 
+        'text_to_img_controlnet': hasattr(model, 'controlnet'),
+        'is_inpainting_task': 'inpainting' in model.name_or_path, 
+        'is_playground': 'playground' in model.name_or_path,
+        'pipeline': model}
+    model.info = diffusion_model.info
     hook_diffusion_model(diffusion_model)
     
     if name_or_path in ['runwayml/stable-diffusion-v1-5', 'stabilityai/stable-diffusion-2-1-base']:
         modified_key = sd15_hidiffusion_key()
         for key, module in diffusion_model.named_modules():
             if apply_raunet and key in modified_key['down_module_key']:
                 make_block_fn = make_diffusers_downsampler_block
```

### Comparing `hidiffusion-0.1.6/hidiffusion/sd_module_key/sd15_module_key.txt` & `hidiffusion-0.1.8/hidiffusion/sd_module_key/sd15_module_key.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -678,8 +678,8 @@
 mid_block.resnets.1.norm1
 mid_block.resnets.1.conv1
 mid_block.resnets.1.time_emb_proj
 mid_block.resnets.1.norm2
 mid_block.resnets.1.dropout
 mid_block.resnets.1.conv2
 conv_norm_out
-conv_out
+conv_out
```

### Comparing `hidiffusion-0.1.6/hidiffusion/sd_module_key/sdxl_module_key.txt` & `hidiffusion-0.1.8/hidiffusion/sd_module_key/sdxl_module_key.txt`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.6/hidiffusion/utils.py` & `hidiffusion-0.1.8/hidiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.6/hidiffusion.egg-info/PKG-INFO` & `hidiffusion-0.1.8/hidiffusion.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hidiffusion
-Version: 0.1.6
+Version: 0.1.8
 Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
 Home-page: 
 Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- # 💡 HiDiffusion -->
@@ -31,41 +31,57 @@
   <em>
       (Select HiDiffusion samples for various diffusion models, resolutions, and aspect ratios.) 
   </em>
 </div>
 <br>
 
 
-# 👉 Why HiDiffusion
+## 👉 Why HiDiffusion
 
 - A  **training-free method that increases the resolution and speed of pretrained diffusion models.**
 - Designed as a **plug-and-play implementation**. It can be integrated into diffusion pipelines by **only adding a single line of code**!
+- Supports various tasks, including **text-to-image, image-to-image, inpainting**.
 
 <div align="center">
   <img src="assets/quality_efficiency.jpg" width="800" ></img>
   <br>
   <em>
       (Faster, and better image details.) 
   </em>
 </div>
 <br>
 
+<div align="center">
+  <img src="assets/various_task.jpg" width="800" ></img>
+  <br>
+  <em>
+      (2K results of ControlNet and inpainting tasks.) 
+  </em>
+</div>
+<br>
+
+## 🔥 Update
+- 2024.5.7 - 💥 Support image-to-image task, see [here](#image-to-image-generation).
+
+- 2024.4.16 - 💥 Release source code.
+
+
 ## 📢 Supported Models
 
 - ✅ [Stable Diffusion XL](https://huggingface.co/papers/2307.01952)
 - ✅ [Stable Diffusion XL Turbo](https://huggingface.co/stabilityai/sdxl-turbo)
 - ✅ [Stable Diffusion v2](https://huggingface.co/stabilityai/stable-diffusion-2-1)
 - ✅ [Stable Diffusion v1](https://huggingface.co/runwayml/stable-diffusion-v1-5)
 
 **Note**: HiDiffusion also supports the downstream diffusion models based on these repositories, such as [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion), [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-aesthetic), etc.
 
 ## 💣 Supported Tasks
 
 - ✅ Text-to-image
-- ✅ ControlNet
+- ✅ ControlNet, including text-to-image, image-to-image
 - ✅ Inpainting
 
 
 ## 🔎 Main Requirements
 This repository is tested on
 * Python==3.8
 * torch==1.13.1
@@ -226,24 +242,25 @@
 
 ### Remove HiDiffusion
 
 If you want to remove HiDiiffusion, simply use `remove_hidiffusion(pipe)`.
 
 ## ControlNet
 
+### Text-to-image generation
 ```python
 from diffusers import StableDiffusionXLControlNetPipeline, ControlNetModel, DDIMScheduler
 import numpy as np
 import torch
 import cv2
 from PIL import Image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 # load Yoshua_Bengio.jpg in the assets file.
-path = 'Yoshua_Bengio.jpg'
+path = './assets/Yoshua_Bengio.jpg'
 image = Image.open(path)
 # get canny image
 image = np.array(image)
 image = cv2.Canny(image, 100, 200)
 image = image[:, :, None]
 image = np.concatenate([image, image, image], axis=2)
 canny_image = Image.fromarray(image)
@@ -279,14 +296,78 @@
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/controlnet_result.jpg" width="800" ></img>
 </div>
 </details>
 
+
+### Image-to-image generation
+```python
+import torch
+import numpy as np
+from PIL import Image
+from diffusers import ControlNetModel, StableDiffusionXLControlNetImg2ImgPipeline, DDIMScheduler
+from hidiffusion import apply_hidiffusion, remove_hidiffusion
+import cv2 
+
+controlnet = ControlNetModel.from_pretrained(
+    "diffusers/controlnet-canny-sdxl-1.0", torch_dtype=torch.float16, variant="fp16"
+).to("cuda")
+scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0", subfolder="scheduler")
+
+pipe = StableDiffusionXLControlNetImg2ImgPipeline.from_pretrained(
+    "stabilityai/stable-diffusion-xl-base-1.0",
+    controlnet=controlnet,
+    scheduler = scheduler,
+    torch_dtype=torch.float16,
+).to("cuda")
+
+# Apply hidiffusion with a single line of code.
+apply_hidiffusion(pipe)
+
+pipe.enable_model_cpu_offload()
+pipe.enable_xformers_memory_efficient_attention()
+
+path = './assets/lara.jpeg'
+ori_image = Image.open(path)
+# get canny image
+image = np.array(ori_image)
+image = cv2.Canny(image, 50, 120)
+image = image[:, :, None]
+image = np.concatenate([image, image, image], axis=2)
+canny_image = Image.fromarray(image)
+
+controlnet_conditioning_scale = 0.5  # recommended for good generalization
+prompt = "Lara Croft with brown hair, and is wearing a tank top, a brown backpack. The room is dark and has an old-fashioned decor with a patterned floor and a wall featuring a design with arches and a dark area on the right side, muted color, high detail, 8k high definition award winning"
+negative_prompt = "underexposed, poorly drawn hands, duplicate hands, overexposed, bad art, beginner, amateur, abstract, disfigured, deformed, close up, weird colors, watermark"
+
+image = pipe(prompt,
+    image=ori_image,
+    control_image=canny_image,
+    height=1536,
+    width=2048,
+    strength=0.99,
+    num_inference_steps=50,
+    controlnet_conditioning_scale=controlnet_conditioning_scale,
+    guidance_scale=12.5,
+    negative_prompt = negative_prompt,
+    eta=1.0
+).images[0]
+
+image.save("lara.jpg")
+```
+
+<details>
+<summary>Output:</summary>
+<div align="center">
+  <img src="assets/lara_result.jpg" width="800" ></img>
+</div>
+</details>
+
 ## Inpainting
 
 ```python
 import torch
 from diffusers import AutoPipelineForInpainting, DDIMScheduler
 from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
@@ -305,15 +386,15 @@
 # remove following line if xFormers is not installed
 pipeline.enable_xformers_memory_efficient_attention()
 
 # load base and mask image
 img_url = "https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/diffusers/sdxl-text2img.png"
 init_image = load_image(img_url)
 # load mask_image.jpg in the assets file.
-mask_image = Image.open("mask_image.png")
+mask_image = Image.open("./assets/mask_image.png")
 
 prompt =  "A steampunk explorer in a leather aviator cap and goggles, with a brass telescope in hand, stands amidst towering ancient trees, their roots entwined with intricate gears and pipes."
 
 negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image = pipeline(prompt=prompt, image=init_image, mask_image=mask_image, height=2048, width=2048, strength=0.85, guidance_scale=12.5, negative_prompt = negative_prompt, eta=1.0).images[0]
 image.save('steampunk_explorer.jpg')
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.6 Summary: HiDiffusion: A
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.8 Summary: HiDiffusion: A
 training-free method to increase the resolution and speed of diffusion models.
 Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
 Jiajun Liang Description-Content-Type: text/markdown License-File: LICENSE
                          [assets/hidiffusion_logo.jpg]
 ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
@@ -13,47 +13,54 @@
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_P_a_p_e_r_&_m_e_s_s_a_g_e_=_A_r_x_i_v_:
       _H_i_D_i_f_f_u_s_i_o_n_&_c_o_l_o_r_=_r_e_d_&_l_o_g_o_=_a_r_x_i_v_]  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
           _v_1_?_l_a_b_e_l_=_D_e_m_o_&_m_e_s_s_a_g_e_=_C_o_l_a_b_&_c_o_l_o_r_=_p_u_r_p_l_e_&_l_o_g_o_=_g_o_o_g_l_e_c_o_l_a_b_] 
                           [assets/image_gallery.jpg]
   ((SSeelleecctt HHiiDDiiffffuussiioonn ssaammpplleess ffoorr vvaarriioouuss ddiiffffuussiioonn mmooddeellss,, rreessoolluuttiioonnss,, aanndd
                                 aassppeecctt rraattiiooss..))
 
-# ð Why HiDiffusion - A **training-free method that increases the resolution
-and speed of pretrained diffusion models.** - Designed as a **plug-and-play
-implementation**. It can be integrated into diffusion pipelines by **only
-adding a single line of code**!
+## ð Why HiDiffusion - A **training-free method that increases the
+resolution and speed of pretrained diffusion models.** - Designed as a **plug-
+and-play implementation**. It can be integrated into diffusion pipelines by
+**only adding a single line of code**! - Supports various tasks, including
+**text-to-image, image-to-image, inpainting**.
                         [assets/quality_efficiency.jpg]
                       ((FFaasstteerr,, aanndd bbeetttteerr iimmaaggee ddeettaaiillss..))
 
-## ð¢ Supported Models - â [Stable Diffusion XL](https://huggingface.co/
-papers/2307.01952) - â [Stable Diffusion XL Turbo](https://huggingface.co/
+                           [assets/various_task.jpg]
+               ((22KK rreessuullttss ooff CCoonnttrroollNNeett aanndd iinnppaaiinnttiinngg ttaasskkss..))
+
+## ð¥ Update - 2024.5.7 - ð¥ Support image-to-image task, see [here]
+(#image-to-image-generation). - 2024.4.16 - ð¥ Release source code. ## ð¢
+Supported Models - â [Stable Diffusion XL](https://huggingface.co/papers/
+2307.01952) - â [Stable Diffusion XL Turbo](https://huggingface.co/
 stabilityai/sdxl-turbo) - â [Stable Diffusion v2](https://huggingface.co/
 stabilityai/stable-diffusion-2-1) - â [Stable Diffusion v1](https://
 huggingface.co/runwayml/stable-diffusion-v1-5) **Note**: HiDiffusion also
 supports the downstream diffusion models based on these repositories, such as
 [Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion),
 [Playground](https://huggingface.co/playgroundai/playground-v2-1024px-
-aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
-â Inpainting ## ð Main Requirements This repository is tested on *
-Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
-accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
-installing the packages in the [main requirements](#-main-requirements),
-install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
-source Alternatively, you can install from github source. Clone the repository
-and install: ```bash git clone https://github.com/megvii-model/HiDiffusion.git
-cd HiDiffusion python3 setup.py install ``` ## ð Usage Generating outputs
-with HiDiffusion is super easy based on ð¤ [diffusers](https://github.com/
-huggingface/diffusers/tree/main). **You just need to add a single line of
-code**. ## Text-to-image generation ### Stable Diffusion XL ```python from
-hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
-StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
-"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
-DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
-StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
-scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
+aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet,
+including text-to-image, image-to-image - â Inpainting ## ð Main
+Requirements This repository is tested on * Python==3.8 * torch==1.13.1 *
+diffusers==0.27.0 * transformers==4.27.4 * accelerate==0.18.0 *
+xformers==0.0.16rc425 ## ð Install HiDiffusion After installing the packages
+in the [main requirements](#-main-requirements), install HiDiffusion: ```shell
+pip3 install hidiffusion ``` ### Installing from source Alternatively, you can
+install from github source. Clone the repository and install: ```bash git clone
+https://github.com/megvii-model/HiDiffusion.git cd HiDiffusion python3 setup.py
+install ``` ## ð Usage Generating outputs with HiDiffusion is super easy
+based on ð¤ [diffusers](https://github.com/huggingface/diffusers/tree/main).
+**You just need to add a single line of code**. ## Text-to-image generation ###
+Stable Diffusion XL ```python from hidiffusion import apply_hidiffusion,
+remove_hidiffusion from diffusers import StableDiffusionXLPipeline,
+DDIMScheduler import torch pretrain_model = "stabilityai/stable-diffusion-xl-
+base-1.0" scheduler = DDIMScheduler.from_pretrained(pretrain_model,
+subfolder="scheduler") pipe = StableDiffusionXLPipeline.from_pretrained
+(pretrain_model, scheduler = scheduler, torch_dtype=torch.float16,
+variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
 with a single line of code. apply_hidiffusion(pipe) prompt = "Standing tall
 amidst the ruins, a stone golem awakens, vines and flowers sprouting from the
 crevices in its body." negative_prompt = "blurry, ugly, duplicate, poorly drawn
@@ -113,54 +120,85 @@
 negative_prompt = "ugly, tiling, poorly drawn face, out of frame, disfigured,
 deformed, blurry, bad anatomy, blurred." image = pipe(prompt,
 guidance_scale=7.5, height=1024, width=1024, eta=1.0,
 negative_prompt=negative_prompt).images[0] image.save(f"fox.jpg") ``` Output:
                                [assets/sd15.jpg]
 Set height = 2048, width = 2048, and you can get output with 2048x2048
 resolution. ### Remove HiDiffusion If you want to remove HiDiiffusion, simply
-use `remove_hidiffusion(pipe)`. ## ControlNet ```python from diffusers import
-StableDiffusionXLControlNetPipeline, ControlNetModel, DDIMScheduler import
-numpy as np import torch import cv2 from PIL import Image from hidiffusion
-import apply_hidiffusion, remove_hidiffusion # load Yoshua_Bengio.jpg in the
-assets file. path = 'Yoshua_Bengio.jpg' image = Image.open(path) # get canny
-image image = np.array(image) image = cv2.Canny(image, 100, 200) image = image
-[:, :, None] image = np.concatenate([image, image, image], axis=2) canny_image
-= Image.fromarray(image) # initialize the models and pipeline
-controlnet_conditioning_scale = 0.5 # recommended for good generalization
-controlnet = ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-
-1.0", torch_dtype=torch.float16, variant="fp16" ) scheduler =
+use `remove_hidiffusion(pipe)`. ## ControlNet ### Text-to-image generation
+```python from diffusers import StableDiffusionXLControlNetPipeline,
+ControlNetModel, DDIMScheduler import numpy as np import torch import cv2 from
+PIL import Image from hidiffusion import apply_hidiffusion, remove_hidiffusion
+# load Yoshua_Bengio.jpg in the assets file. path = './assets/
+Yoshua_Bengio.jpg' image = Image.open(path) # get canny image image = np.array
+(image) image = cv2.Canny(image, 100, 200) image = image[:, :, None] image =
+np.concatenate([image, image, image], axis=2) canny_image = Image.fromarray
+(image) # initialize the models and pipeline controlnet_conditioning_scale =
+0.5 # recommended for good generalization controlnet =
+ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-1.0",
+torch_dtype=torch.float16, variant="fp16" ) scheduler =
 DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
 subfolder="scheduler") pipe =
 StableDiffusionXLControlNetPipeline.from_pretrained( "stabilityai/stable-
 diffusion-xl-base-1.0", controlnet=controlnet, torch_dtype=torch.float16,
 scheduler = scheduler ) # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
 pipe.enable_xformers_memory_efficient_attention() prompt = "The Joker, high
 face detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
 duplicate, poorly drawn, deformed, mosaic." image = pipe( prompt,
 controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
 height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt,
 eta=1.0 ).images[0] image.save('joker.jpg') ``` Output:
                         [assets/controlnet_result.jpg]
+### Image-to-image generation ```python import torch import numpy as np from
+PIL import Image from diffusers import ControlNetModel,
+StableDiffusionXLControlNetImg2ImgPipeline, DDIMScheduler from hidiffusion
+import apply_hidiffusion, remove_hidiffusion import cv2 controlnet =
+ControlNetModel.from_pretrained( "diffusers/controlnet-canny-sdxl-1.0",
+torch_dtype=torch.float16, variant="fp16" ).to("cuda") scheduler =
+DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
+subfolder="scheduler") pipe =
+StableDiffusionXLControlNetImg2ImgPipeline.from_pretrained( "stabilityai/
+stable-diffusion-xl-base-1.0", controlnet=controlnet, scheduler = scheduler,
+torch_dtype=torch.float16, ).to("cuda") # Apply hidiffusion with a single line
+of code. apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
+pipe.enable_xformers_memory_efficient_attention() path = './assets/lara.jpeg'
+ori_image = Image.open(path) # get canny image image = np.array(ori_image)
+image = cv2.Canny(image, 50, 120) image = image[:, :, None] image =
+np.concatenate([image, image, image], axis=2) canny_image = Image.fromarray
+(image) controlnet_conditioning_scale = 0.5 # recommended for good
+generalization prompt = "Lara Croft with brown hair, and is wearing a tank top,
+a brown backpack. The room is dark and has an old-fashioned decor with a
+patterned floor and a wall featuring a design with arches and a dark area on
+the right side, muted color, high detail, 8k high definition award winning"
+negative_prompt = "underexposed, poorly drawn hands, duplicate hands,
+overexposed, bad art, beginner, amateur, abstract, disfigured, deformed, close
+up, weird colors, watermark" image = pipe(prompt, image=ori_image,
+control_image=canny_image, height=1536, width=2048, strength=0.99,
+num_inference_steps=50,
+controlnet_conditioning_scale=controlnet_conditioning_scale,
+guidance_scale=12.5, negative_prompt = negative_prompt, eta=1.0 ).images[0]
+image.save("lara.jpg") ``` Output:
+                           [assets/lara_result.jpg]
 ## Inpainting ```python import torch from diffusers import
 AutoPipelineForInpainting, DDIMScheduler from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion from PIL import
 Image scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-
 xl-base-1.0", subfolder="scheduler") pipeline =
 AutoPipelineForInpainting.from_pretrained( "diffusers/stable-diffusion-xl-1.0-
 inpainting-0.1", torch_dtype=torch.float16, variant="fp16", scheduler=scheduler
 ) # Apply hidiffusion with a single line of code. apply_hidiffusion(pipeline)
 pipeline.enable_model_cpu_offload() # remove following line if xFormers is not
 installed pipeline.enable_xformers_memory_efficient_attention() # load base and
 mask image img_url = "https://huggingface.co/datasets/huggingface/
 documentation-images/resolve/main/diffusers/sdxl-text2img.png" init_image =
 load_image(img_url) # load mask_image.jpg in the assets file. mask_image =
-Image.open("mask_image.png") prompt = "A steampunk explorer in a leather
-aviator cap and goggles, with a brass telescope in hand, stands amidst towering
-ancient trees, their roots entwined with intricate gears and pipes."
+Image.open("./assets/mask_image.png") prompt = "A steampunk explorer in a
+leather aviator cap and goggles, with a brass telescope in hand, stands amidst
+towering ancient trees, their roots entwined with intricate gears and pipes."
 negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image = pipeline(prompt=prompt, image=init_image, mask_image=mask_image,
 height=2048, width=2048, strength=0.85, guidance_scale=12.5, negative_prompt =
 negative_prompt, eta=1.0).images[0] image.save('steampunk_explorer.jpg') ```
 Output:
                         [assets/inpainting_result.jpg]
 ## Integration into downstream models HiDiffusion supports models based on
```

