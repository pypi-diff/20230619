# Comparing `tmp/custom_diffusion-0.1.5.tar.gz` & `tmp/custom_diffusion-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.1.5.tar", last modified: Tue Jun 13 10:47:42 2023, max compression
+gzip compressed data, was "custom_diffusion-0.1.6.tar", last modified: Mon Jun 19 20:35:29 2023, max compression
```

## Comparing `custom_diffusion-0.1.5.tar` & `custom_diffusion-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.100524 custom_diffusion-0.1.5/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3110 2023-06-13 10:47:42.100524 custom_diffusion-0.1.5/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2062 2023-06-12 22:10:36.000000 custom_diffusion-0.1.5/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.093857 custom_diffusion-0.1.5/custom_diffusion/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      326 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2112 2023-06-13 10:35:42.000000 custom_diffusion-0.1.5/custom_diffusion/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.097191 custom_diffusion-0.1.5/custom_diffusion/pipelines/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7258 2023-06-13 10:47:00.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_img2img.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6684 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7401 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_pipeline.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8950 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/preprocces.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.100524 custom_diffusion-0.1.5/custom_diffusion/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2330 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1759 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/utils/downloads.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      811 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/utils/model_list.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1268 2023-06-13 10:06:55.000000 custom_diffusion-0.1.5/custom_diffusion/utils/scheduler_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3545 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/utils/video_utils.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.097191 custom_diffusion-0.1.5/custom_diffusion.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3110 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      785 2023-06-13 10:47:42.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      175 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       17 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      113 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      359 2023-06-13 10:47:42.103857 custom_diffusion-0.1.5/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2151 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.444764 custom_diffusion-0.1.6/
+-rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3489 2023-06-19 20:35:29.445763 custom_diffusion-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2322 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.364748 custom_diffusion-0.1.6/custom_diffusion/
+-rw-rw-rw-   0        0        0      317 2023-06-19 20:35:18.000000 custom_diffusion-0.1.6/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0     1538 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/demo.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.424760 custom_diffusion-0.1.6/custom_diffusion/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     7349 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_img2img.py
+-rw-rw-rw-   0        0        0     7320 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_inpaint.py
+-rw-rw-rw-   0        0        0     7136 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_pipeline.py
+-rw-rw-rw-   0        0        0     6354 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_img2img.py
+-rw-rw-rw-   0        0        0     6414 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_instruct_pix2pix.py
+-rw-rw-rw-   0        0        0     4598 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_text2image.py
+-rw-rw-rw-   0        0        0     6361 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_upscale.py
+-rw-rw-rw-   0        0        0     8950 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.443764 custom_diffusion-0.1.6/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2330 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1759 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0      811 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/model_list.py
+-rw-rw-rw-   0        0        0     1268 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3584 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.402755 custom_diffusion-0.1.6/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     3489 2023-06-19 20:35:28.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1008 2023-06-19 20:35:29.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:35:28.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-06-19 20:35:29.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 20:35:29.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-06-10 22:16:53.000000 custom_diffusion-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-19 20:35:29.448766 custom_diffusion-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/setup.py
```

### Comparing `custom_diffusion-0.1.5/LICENSE` & `custom_diffusion-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.5/README.md` & `custom_diffusion-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
 <h2>
-     Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
+     Custom Diffusion: Creating Video from Frame Using Diffusion
 </h2>
 <div>
     <a href="https://pepy.tech/project/custom_diffusion"><img src="https://pepy.tech/badge/custom_diffusion" alt="downloads"></a>
     <a href="https://badge.fury.io/py/custom_diffusion"><img src="https://badge.fury.io/py/custom_diffusion.svg" alt="pypi version"></a>
     <a href="https://huggingface.co/spaces/ArtGAN/Stable-Diffusion-ControlNet-WebUI"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 </div>
 </div>
@@ -14,34 +14,40 @@
 ```bash
 pip install custom_diffusion
 ```
 
 ### Usage
 ```python
 
+# Importing the required libraries
+
+from custom_diffusion.utils.data_utils import load_images_from_folder
+from custom_diffusion import StableDiffusionControlNetGenerator
+from custom_diffusion.utils.video_utils import convert_images_to_video
+from custom_diffusion.demo import video_pipeline
+
+# Creating a video from a video file
 frames_path = video_pipeline(
-    video_url="https://huggingface.co/spaces/kadirnar/torchyolo/resolve/main/testv2.mp4",
-    youtube=False,
-    output_path="output",
-    filename="test.mp4",
-    quality="720p",
+    video_path="test.mp4",
+    output_path="output.mp4",
     start_time=0,
-    end_time=2,
+    end_time=5,
     frame_rate=1,
 )
 
+# Creating a video from a folder of images
 images_list = load_images_from_folder(frames_path)
-image_grid(images_list, rows=5, cols=5)
 
 prompt = "a anime boy"
 negative_prompt = "bad"
 
 list_prompt = [prompt] * len(images_list)
 list_negative_prompt = [negative_prompt] * len(images_list)
 
+# Generating images from a list of images
 generator = StableDiffusionControlNetGenerator()
 
 generated_image_list = generator.generate_image(
     stable_model_path="andite/anything-v4.0",
     controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
     scheduler_name="EulerAncestralDiscrete",
     images_list=images_list,
@@ -56,15 +62,14 @@
     controlnet_conditioning_scale=1.0,
     generator_seed=0,
     preprocess_type="Canny",
     resize_type="center_crop_and_resize",
     crop_size=512,
 )
 
-frame2video = frames_to_video(
-    folder_path=generated_image_list,
-    output_folder="output",
-    output_video_name="frame2video.mp4",
-    duration=5,
+# Converting the generated images to a video
+frame2video = convert_images_to_video(
+    image_list=generated_image_list,
+    output_file="output.mp4",
+    frame_rate=5,
 )
-
 ```
```

#### html2text {}

```diff
@@ -1,21 +1,24 @@
-  ***** Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
-                                     *****
+    ***** Custom Diffusion: Creating Video from Frame Using Diffusion *****
                 [downloads] [pypi_version] [HuggingFace_Spaces]
-### Installation ```bash pip install custom_diffusion ``` ### Usage ```python
-frames_path = video_pipeline( video_url="https://huggingface.co/spaces/
-kadirnar/torchyolo/resolve/main/testv2.mp4", youtube=False,
-output_path="output", filename="test.mp4", quality="720p", start_time=0,
-end_time=2, frame_rate=1, ) images_list = load_images_from_folder(frames_path)
-image_grid(images_list, rows=5, cols=5) prompt = "a anime boy" negative_prompt
-= "bad" list_prompt = [prompt] * len(images_list) list_negative_prompt =
-[negative_prompt] * len(images_list) generator =
-StableDiffusionControlNetGenerator() generated_image_list =
+### Installation ```bash pip install custom_diffusion ``` ### Usage ```python #
+Importing the required libraries from custom_diffusion.utils.data_utils import
+load_images_from_folder from custom_diffusion import
+StableDiffusionControlNetGenerator from custom_diffusion.utils.video_utils
+import convert_images_to_video from custom_diffusion.demo import video_pipeline
+# Creating a video from a video file frames_path = video_pipeline
+( video_path="test.mp4", output_path="output.mp4", start_time=0, end_time=5,
+frame_rate=1, ) # Creating a video from a folder of images images_list =
+load_images_from_folder(frames_path) prompt = "a anime boy" negative_prompt =
+"bad" list_prompt = [prompt] * len(images_list) list_negative_prompt =
+[negative_prompt] * len(images_list) # Generating images from a list of images
+generator = StableDiffusionControlNetGenerator() generated_image_list =
 generator.generate_image( stable_model_path="andite/anything-v4.0",
 controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
 scheduler_name="EulerAncestralDiscrete", images_list=images_list,
 prompt=list_prompt, negative_prompt=list_negative_prompt, height=512,
 width=512, guess_mode=False, num_images_per_prompt=1, num_inference_steps=30,
 guidance_scale=7.0, controlnet_conditioning_scale=1.0, generator_seed=0,
 preprocess_type="Canny", resize_type="center_crop_and_resize", crop_size=512, )
-frame2video = frames_to_video( folder_path=generated_image_list,
-output_folder="output", output_video_name="frame2video.mp4", duration=5, ) ```
+# Converting the generated images to a video frame2video =
+convert_images_to_video( image_list=generated_image_list,
+output_file="output.mp4", frame_rate=5, ) ```
```

### Comparing `custom_diffusion-0.1.5/custom_diffusion/demo.py` & `custom_diffusion-0.1.6/custom_diffusion/demo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,8 @@
 from custom_diffusion.pipelines.controlnet_pipeline import StableDiffusionControlNetGenerator
-from custom_diffusion.utils.data_utils import load_images_from_folder
-from custom_diffusion.utils.video_utils import frames_to_video, trim_video, video_to_frames
-
-
-def video_pipeline(
-    video_path: str = "test.mp4",
-    output_path: str = "output",
-    start_time: int = 0,
-    end_time: int = 5,
-    frame_rate: int = 1,
-):
-    edit_video = trim_video(video_path=video_path, output_path=output_path, start_time=start_time, end_time=end_time)
-    video2frame = video_to_frames(video_path=edit_video, output_path=output_path, frame_rate=frame_rate)
-
-    return video2frame
 
 
 def main(
     stable_model_path: str = "runwayml/stable-diffusion-v1-5",
     controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny",
     scheduler_name: str = "DDIM",
     image_path: str = "test.png",
```

### Comparing `custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_img2img.py` & `custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_img2img.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         return generator
 
     def generate_image(
         self,
         stable_model_path: str = "runwayml/stable-diffusion-v1-5",
         controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny",
         scheduler_name: str = "DDIM",
-        images_list: List[str] = ["test.png"],
+        images_path_list: List[str] = ["test.png"],
         prompt: List[str] = ["A photo of a cat."],
         negative_prompt: List[str] = ["bad"],
         height: int = 512,
         width: int = 512,
         guess_mode: bool = False,
         num_images_per_prompt: int = 1,
         num_inference_steps: int = 20,
@@ -158,20 +158,22 @@
         generator_seed (int): The seed for the random generator.
         preprocess_type (str): The type of preprocessing to apply.
 
         Returns:
         output: The generated image.
         """
         control_image_list = []
-        for image_path in images_list:
+        read_image_list = []
+        for image_path in images_path_list:
             read_image = self.load_and_resize_image(
                 image_path=image_path, resize_type=resize_type, height=height, width=width, crop_size=crop_size
             )
             control_image = preprocces_dicts[preprocess_type](read_image)
             control_image_list.append(control_image)
+            read_image_list.append(read_image)
 
         pipe = self.load_model(
             stable_model_path=stable_model_path,
             controlnet_model_path=controlnet_model_path,
             scheduler_name=scheduler_name,
         )
 
@@ -179,15 +181,15 @@
 
         output = pipe(
             prompt=prompt,
             height=height,
             width=width,
             guess_mode=guess_mode,
             control_image=control_image_list,
-            image=read_image,
+            image=read_image_list,
             strength=strength,
             negative_prompt=negative_prompt,
             num_images_per_prompt=num_images_per_prompt,
             num_inference_steps=num_inference_steps,
             guidance_scale=guidance_scale,
             controlnet_conditioning_scale=float(controlnet_conditioning_scale),
             generator=generator,
```

### Comparing `custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py` & `custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_inpaint.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,59 +68,67 @@
             self.pipe.enable_xformers_memory_efficient_attention()
 
             self.model_cache[model_key] = self.pipe
 
         return self.model_cache[model_key]
 
     def load_and_resize_image(
-        self, image: Image, resize_type: str, crop_size: Optional[int], height: Optional[int], width: Optional[int]
+        self,
+        image_path: str = "test.png",
+        resize_type: str = "center_crop_and_resize",
+        crop_size: Optional[int] = 512,
+        height: Optional[int] = 512,
+        width: Optional[int] = 512,
     ):
         """
-        This function loads and resizes an image to a specified size.
+        This function loads and resizes the image.
 
         Args:
-        image (Image): The PIL Image object.
+        image_path (str): Path to the image.
+        resize_type (str): The type of resizing to apply.
+        crop_size (int): The size of the crop.
+        height (int): The height of the image to generate.
+        width (int): The width of the image to generate.
 
         Returns:
         Image: The resized and loaded PIL Image.
         """
-        image = image.convert("RGB")
+        image = Image.open(image_path)
 
         if resize_type == "center_crop_and_resize":
             image = center_crop_and_resize(image, crop_size=crop_size, height=height, width=width)
 
         elif resize_type == "resize":
             image = image.resize((height, width))
 
         else:
             raise ValueError("Invalid resize type.")
 
-        image = np.array(image)
-
-        return Image.fromarray(image)
+        return image
 
     def _setup_generator(self, generator_seed):
         if generator_seed == 0:
             random_seed = torch.randint(0, 1000000, (1,))
             generator = torch.manual_seed(random_seed)
         else:
             generator = torch.manual_seed(generator_seed)
         return generator
 
     def generate_image(
         self,
         stable_model_path: str,
         controlnet_model_path: str,
         scheduler_name: str,
-        image_paths: str,
+        images_path_list: str,
+        mask_path_list: str,
         prompt: str,
         negative_prompt: str,
         height: int,
         width: int,
-        strength: int,
+        strength: float,
         guess_mode: bool,
         num_images_per_prompt: int,
         num_inference_steps: int,
         guidance_scale: int,
         controlnet_conditioning_scale: int,
         generator_seed: int,
         preprocess_type: str,
@@ -147,40 +155,49 @@
         generator_seed (int): The seed for the random generator.
         preprocess_type (str): The type of preprocessing to apply.
         resize_type (str): The type of resizing to apply.
 
         Returns:
         output: The generated image.
         """
-        normal_image = self.load_and_resize_image(
-            image=image_paths["image"], resize_type=resize_type, height=height, width=width
-        )
-        mask_image = self.load_and_resize_image(
-            image=image_paths["mask"], resize_type=resize_type, height=height, width=width
-        )
-
-        control_image = preprocces_dicts[preprocess_type](normal_image)
+        control_image_list = []
+        mask_image_list = []
+        image_path_list = []
+
+        for image_path in images_path_list:
+            normal_image = self.load_and_resize_image(
+                image=image_path, resize_type=resize_type, height=height, width=width
+            )
+            control_image = preprocces_dicts[preprocess_type](normal_image)
+            control_image_list.append(control_image)
+            image_path_list.append(image_path)
+
+        for mask_path in mask_path_list:
+            mask_image = self.load_and_resize_image(
+                image=mask_path, resize_type=resize_type, height=height, width=width
+            )
+            mask_image_list.append(mask_image)
 
         pipe = self.load_model(
             stable_model_path=stable_model_path,
             controlnet_model_path=controlnet_model_path,
             scheduler_name=scheduler_name,
         )
 
         generator = self._setup_generator(generator_seed)
 
         output = pipe(
             prompt=prompt,
-            image=normal_image,
+            image=image_path_list,
             height=height,
             width=width,
-            mask_image=mask_image,
+            mask_image=mask_image_list,
             strength=strength,
             guess_mode=guess_mode,
-            control_image=control_image,
+            control_image=control_image_list,
             negative_prompt=negative_prompt,
             num_images_per_prompt=num_images_per_prompt,
             num_inference_steps=num_inference_steps,
             guidance_scale=guidance_scale,
             controlnet_conditioning_scale=float(controlnet_conditioning_scale),
             generator=generator,
         ).images
```

### Comparing `custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_pipeline.py` & `custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import torch
 from diffusers import ControlNetModel, StableDiffusionControlNetPipeline
 from PIL import Image
 
 from custom_diffusion.preprocces import preprocces_dicts
 from custom_diffusion.utils.data_utils import center_crop_and_resize
 from custom_diffusion.utils.scheduler_utils import get_scheduler
-from custom_diffusion.utils.video_utils import video_pipeline
 
 
 class StableDiffusionControlNetGenerator:
     """
     A class to handle image generation using stable diffusion and control net models.
     """
 
@@ -119,30 +118,28 @@
         return generator
 
     def generate_image(
         self,
         stable_model_path: str = "runwayml/stable-diffusion-v1-5",
         controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny",
         scheduler_name: str = "DDIM",
-        video_path: str = "test.mp4",
+        image_list: List[str] = ["test.png"],
         prompt: List[str] = ["A photo of a cat."],
         negative_prompt: List[str] = ["bad"],
         height: int = 512,
         width: int = 512,
         guess_mode: bool = False,
         num_images_per_prompt: int = 1,
         num_inference_steps: int = 20,
         guidance_scale: int = 7.0,
         controlnet_conditioning_scale: int = 1.0,
         generator_seed: int = 0,
         preprocess_type: str = "Canny",
         resize_type: str = "center_crop_and_resize",
         crop_size: int = 512,
-        start_time: int = 0,
-        end_time: int = 10,
     ):
         """
         This function generates an image based on the given parameters.
 
         Args:
         stable_model_path (str): Path to the stable model.
         controlnet_model_path (str): Path to the controlnet model.
@@ -160,19 +157,16 @@
         generator_seed (int): The seed for the random generator.
         preprocess_type (str): The type of preprocessing to apply.
 
         Returns:
         output: The generated image.
         """
 
-        video_path = video_pipeline(
-            video_path=video_path, output_path="output", filename="output.mp4", start_time=0, end_time=10
-        )
         control_image_list = []
-        for image_path in images_list:
+        for image_path in image_list:
             read_image = self.load_and_resize_image(
                 image_path=image_path, resize_type=resize_type, height=height, width=width, crop_size=crop_size
             )
             control_image = preprocces_dicts[preprocess_type](read_image)
             control_image_list.append(control_image)
 
         pipe = self.load_model(
```

### Comparing `custom_diffusion-0.1.5/custom_diffusion/preprocces.py` & `custom_diffusion-0.1.6/custom_diffusion/preprocces.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.5/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.1.6/custom_diffusion/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.5/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.1.6/custom_diffusion/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.5/custom_diffusion/utils/model_list.py` & `custom_diffusion-0.1.6/custom_diffusion/utils/model_list.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.5/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.1.6/custom_diffusion/utils/scheduler_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.5/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.1.6/custom_diffusion/utils/video_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     # Load the video
     clip = VideoFileClip(video_path)
 
     # Trim the video
     trimmed_clip = clip.subclip(start_time, end_time)
 
     # Write the result to a file (without processing audio)
+    output_path = output_path + ".mp4"
     trimmed_clip.write_videofile(output_path, audio=True)
 
     print("Video trimmed successfully!")
 
     return output_path
```

### Comparing `custom_diffusion-0.1.5/setup.py` & `custom_diffusion-0.1.6/setup.py`

 * *Files identical despite different names*

