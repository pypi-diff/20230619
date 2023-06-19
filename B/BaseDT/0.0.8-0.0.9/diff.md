# Comparing `tmp/BaseDT-0.0.8.tar.gz` & `tmp/BaseDT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDT-0.0.8.tar", last modified: Fri Jun 16 06:29:18 2023, max compression
+gzip compressed data, was "dist/BaseDT-0.0.9.tar", last modified: Mon Jun 19 06:05:56 2023, max compression
```

## Comparing `BaseDT-0.0.8.tar` & `BaseDT-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-16 06:29:18.000000 BaseDT-0.0.8/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.8/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    31622 2023-06-07 06:26:00.000000 BaseDT-0.0.8/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.8/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    37236 2023-06-09 06:59:00.000000 BaseDT-0.0.8/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.8/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)    13050 2023-06-16 06:28:08.000000 BaseDT-0.0.8/BaseDT/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)     7577 2023-06-05 14:43:34.000000 BaseDT-0.0.8/BaseDT/utils.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.8/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.8/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-16 06:29:18.000000 BaseDT-0.0.8/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.8/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-16 06:29:18.000000 BaseDT-0.0.8/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-16 06:28:25.000000 BaseDT-0.0.8/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:05:56.000000 BaseDT-0.0.9/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-06-19 05:43:54.000000 BaseDT-0.0.9/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    35422 2023-06-19 05:49:30.000000 BaseDT-0.0.9/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-06-19 05:43:54.000000 BaseDT-0.0.9/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    37236 2023-06-09 06:59:00.000000 BaseDT-0.0.9/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-06-19 05:43:54.000000 BaseDT-0.0.9/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    15369 2023-06-19 05:48:40.000000 BaseDT-0.0.9/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    18654 2023-06-19 05:47:08.000000 BaseDT-0.0.9/BaseDT/utils.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-19 06:05:56.000000 BaseDT-0.0.9/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.9/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.9/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-19 06:05:56.000000 BaseDT-0.0.9/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.9/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-19 06:05:56.000000 BaseDT-0.0.9/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-19 06:05:36.000000 BaseDT-0.0.9/setup.py
```

### Comparing `BaseDT-0.0.8/BaseDT/data.py` & `BaseDT-0.0.9/BaseDT/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -336,23 +336,23 @@
             border_type[padding_mode],
             value=pad_val)
         self.value = img
 
     def _flip(self):
         pass
     
-    def imshow(self, raw = False):
+    def show(self, raw = False):
         if raw: img = self.raw_value
         else: img = self.value
         if len(img.shape) == 3:
             img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
         plt.imshow(img)
         plt.axis('off')
         plt.show()
-    
+       
     def map_orig_coords(self, boxes):
         #TODO 暂时只支持box的映射，后续应该支持单纯的坐标映射
         original_w, original_h = self.raw_value.shape[:2]
         processed_w, processed_h = self.value.shape[:2]
         sx, sy = original_w / processed_w, original_h / processed_h
         new_boxes = np.array([]).reshape(0, 5)
         for box in boxes:
@@ -368,15 +368,15 @@
         ax.axis(False)
 
         # remove white edges by set subplot margin
         fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
         canvas = FigureCanvasAgg(fig)
         return canvas, fig, ax
     
-    def show(self,
+    def imshow(self,
              drawn_img: Optional[np.ndarray] = None,
              win_name: str = 'image',
              wait_time: float = 0.,
              continue_key: str = ' ',
              backend: str = 'matplotlib') -> None:
         """Show the drawn image.
 
@@ -391,14 +391,15 @@
                 the space key.
             backend (str): The backend to show the image. Defaults to
                 'matplotlib'. `New in version 0.7.3.`
         """
         if backend == 'matplotlib':
             import matplotlib.pyplot as plt
             is_inline = 'inline' in plt.get_backend()
+
             img = self.get_image() if drawn_img is None else drawn_img
             self._init_manager(win_name)
             #fig = self.manager.canvas.figure
             # remove white edges by set subplot margin
             #fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
             #fig.clear()
             #ax = fig.add_subplot()
@@ -547,14 +548,103 @@
             poly,
             alpha=alpha,
             edge_colors=edge_colors,
             line_styles=line_styles,
             line_widths=line_widths,
             face_colors=face_colors)
     
+    def draw_lines(
+        self,
+        x_datas: np.ndarray,
+        y_datas: np.ndarray,
+        colors: Union[str, tuple, List[str], List[tuple]] = 'g',
+        line_styles: Union[str, List[str]] = '-',
+        line_widths: Union[Union[int, float], List[Union[int, float]]] = 2
+    ) -> 'Visualizer':
+        from matplotlib.collections import LineCollection
+        #check_type('x_datas', x_datas, (np.ndarray, torch.Tensor))
+        #x_datas = tensor2ndarray(x_datas)
+        #check_type('y_datas', y_datas, (np.ndarray, torch.Tensor))
+        #y_datas = tensor2ndarray(y_datas)
+        assert x_datas.shape == y_datas.shape, (
+            '`x_datas` and `y_datas` should have the same shape')
+        assert x_datas.shape[-1] == 2, (
+            f'The shape of `x_datas` should be (N, 2), but got {x_datas.shape}'
+        )
+        if len(x_datas.shape) == 1:
+            x_datas = x_datas[None]
+            y_datas = y_datas[None]
+        colors = color_val_matplotlib(colors)  # type: ignore
+        lines = np.concatenate(
+            (x_datas.reshape(-1, 2, 1), y_datas.reshape(-1, 2, 1)), axis=-1)
+        if not self._is_posion_valid(lines):
+            warnings.warn(
+                'Warning: The line is out of bounds,'
+                ' the drawn line may not be in the image', UserWarning)
+        line_collect = LineCollection(
+            lines.tolist(),
+            colors=colors,
+            linestyles=line_styles,
+            linewidths=line_widths)
+        self.ax_save.add_collection(line_collect)
+        return self
+    
+    def draw_circles(
+        self,
+        center: np.ndarray,
+        radius: np.ndarray,
+        edge_colors: Union[str, tuple, List[str], List[tuple]] = 'g',
+        line_styles: Union[str, List[str]] = '-',
+        line_widths: Union[Union[int, float], List[Union[int, float]]] = 2,
+        face_colors: Union[str, tuple, List[str], List[tuple]] = 'none',
+        alpha: Union[float, int] = 0.8,
+    ) -> 'Visualizer':
+        from matplotlib.collections import PatchCollection
+        from matplotlib.patches import Circle
+        #check_type('center', center, (np.ndarray, torch.Tensor))
+        #center = tensor2ndarray(center)
+        #check_type('radius', radius, (np.ndarray, torch.Tensor))
+        #radius = tensor2ndarray(radius)
+        if len(center.shape) == 1:
+            center = center[None]
+        assert center.shape == (radius.shape[0], 2), (
+            'The shape of `center` should be (radius.shape, 2), '
+            f'but got {center.shape}')
+        if not (self._is_posion_valid(center -
+                                      np.tile(radius.reshape((-1, 1)), (1, 2)))
+                and self._is_posion_valid(
+                    center + np.tile(radius.reshape((-1, 1)), (1, 2)))):
+            warnings.warn(
+                'Warning: The circle is out of bounds,'
+                ' the drawn circle may not be in the image', UserWarning)
+
+        center = center.tolist()
+        radius = radius.tolist()
+        edge_colors = color_val_matplotlib(edge_colors)  # type: ignore
+        face_colors = color_val_matplotlib(face_colors)  # type: ignore
+        circles = []
+        for i in range(len(center)):
+            circles.append(Circle(tuple(center[i]), radius[i]))
+
+        if isinstance(line_widths, (int, float)):
+            line_widths = [line_widths] * len(circles)
+        line_widths = [
+            min(max(linewidth, 1), self._default_font_size / 4)
+            for linewidth in line_widths
+        ]
+        p = PatchCollection(
+            circles,
+            alpha=alpha,
+            facecolors=face_colors,
+            edgecolors=edge_colors,
+            linewidths=line_widths,
+            linestyles=line_styles)
+        self.ax_save.add_collection(p)
+        return self
+    
     def color_val_matplotlib(
             colors: Union[str, tuple, List[Union[str, tuple]]]
             ) -> Union[str, tuple, List[Union[str, tuple]]]:
         if isinstance(colors, str):
             return colors
         elif isinstance(colors, tuple):
             assert len(colors) == 3
@@ -743,15 +833,15 @@
         sess = onnxruntime.InferenceSession(model_path)
         model_meta = sess.get_modelmeta()
         key='MODEL_INFO'
         if key in model_meta.custom_metadata_map:
             unicode_string = model_meta.custom_metadata_map[key]
             print(f'Success load model info generate by MMEdu>=0.1.15: {unicode_string[:100] + "..." if len(unicode_string) > 100 else unicode_string}')
         else:   
-            #print('Please input onnx model path convert by MMEdu>=0.1.15.')
+            print('Please input onnx model path convert by MMEdu>=0.1.15 for a better experience.')
             return ''
         #return json.loads(unicode_string)
         #print('ok')
         return json.loads(codecs.decode(unicode_string, 'unicode_escape'))
     def get_model_info(self):
         if self.model_info == '':
             #print('Please input onnx model path convert by MMEdu>=0.1.15.')
@@ -770,15 +860,15 @@
             else:
                 print(f'The model info does not contain key:{key}')
 
     def get_modelname(self):
         key = 'modelname'
         if self.model_info == '':
             #print('Please input onnx model path convert by MMEdu>=0.1.15.')
-            return 'MobileNet'
+            return ''
         else:
             if key in self.model_info:
                 return self.model_info[key]
             else:
                 print(f'The model info does not contain key:{key}')
 
     def get_labels(self):
```

### Comparing `BaseDT-0.0.8/BaseDT/data_image.py` & `BaseDT-0.0.9/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.8/BaseDT/dataset.py` & `BaseDT-0.0.9/BaseDT/dataset.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.8/BaseDT/io.py` & `BaseDT-0.0.9/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.8/BaseDT/plot.py` & `BaseDT-0.0.9/BaseDT/plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -242,20 +242,17 @@
     'bbox': dict(facecolor='black', alpha=0.5, boxstyle='Round'),
     'verticalalignment': 'top',
     'horizontalalignment': 'left',
 }
 def draw_single_cls(image, result):
     texts = []
     max_length = 12 # 文本长度限制
-    if '标签' in result:
-        texts.append('Pred_label: {}'.format(result['标签']))
-    if '置信度' in result:
-        texts.append('Pred_score: {:.2f}'.format(result['置信度']))
-    if '预测结果' in result:
-        texts.append('Pred_label: {}'.format(result['预测结果'][:max_length]))
+    texts.append('Pred_label: {}'.format(result['标签']))
+    texts.append('Pred_score: {:.2f}'.format(result['置信度']))
+    texts.append('Pred_label: {}'.format(result['预测结果'][:max_length]))
     text = '\n'.join(texts)
     #fig = plt.figure()
     image.init_plt()
     img_tmp = image._image
     img_scale = get_adaptive_scale(img_tmp.shape[:2])
     DEFAULT_TEXT_CFG['size'] = int(img_scale * 5)
     pos = np.array([[img_scale*5, img_scale*5]], dtype=int)
@@ -282,17 +279,18 @@
 # 将vis绘图内容与mmlab对齐
 def show_cls(images, results):
     # 探讨传入dt还是img_path
     # 判断是文件夹还是文件
     if isinstance(images, list) and isinstance(results, list):
         for image, result in zip(images, results):
             draw_single_cls(image, result)
-            image.show()
+            image.imshow()
     else:
         draw_single_cls(images, results)
+        images.imshow()
         
 
 def _get_adaptive_scales(areas: np.ndarray,
                          min_area: int = 800,
                          max_area: int = 30000) -> np.ndarray:
     scales = 0.5 + (areas - min_area) / (max_area - min_area)
     scales = np.clip(scales, 0.5, 1.0)
@@ -307,33 +305,29 @@
     assert len(dataset_palette) >= num_classes, \
         'The length of palette should not be less than `num_classes`.'
     return dataset_palette
 
 def draw_single_det(image, result, line_width: int =3) -> None:
     assert isinstance(result, list), "Expected 'result' to be a list"
     image.init_plt()
-    if len(result) == 0:
-        return
     bboxes = []
     labels = []
     label_texts = []
     for bbox in result:
         assert isinstance(bbox, dict), "Expected each element in 'result' to be a dictionary"
         assert '坐标' in bbox and '标签' in bbox, "Each dictionary in 'result' should have '坐标' and '标签' keys"
         
         coords = bbox['坐标']
         assert isinstance(coords, dict), "Expected '坐标' to be a dictionary"
         assert all(key in coords for key in ['x1', 'y1', 'x2', 'y2']), "The '坐标' dictionary should have 'x1', 'y1', 'x2', 'y2' keys"
         
         bboxes.append([coords['x1'], coords['y1'], coords['x2'], coords['y2']])
         labels.append(bbox['标签'])
-        if '预测结果' in bbox:
-            label_texts.append('{}:{}'.format(bbox['预测结果'],round(float(bbox['置信度']) * 100, 1)))
-        else:
-            label_texts.append('{}:{}'.format(bbox['标签'],round(float(bbox['置信度']) * 100, 1)))
+        label_texts.append('{}:{}'.format(bbox['预测结果'],round(float(bbox['置信度']) * 100, 1)))
+
     bboxes = np.array(bboxes)
     labels = np.array(labels)
 
 
     max_label = int(max(labels) if len(labels) > 0 else 0)
 
     bbox_palette = get_palette(max_label + 1)
@@ -358,10 +352,64 @@
                                 'edgecolor': 'none'
                             }])
 
 def show_det(images, results):
     if isinstance(images, list) and isinstance(results, list):
         for image, result in zip(images, results):
             draw_single_det(image=image, result= result)
-            image.show()
+            image.imshow()
+    else:
+        draw_single_det(image=images, result= results)
+        images.imshow()
+
+def draw_single_pose(image, result, thr=0.3) -> None:
+    image.init_plt()
+    keypoints = result['关键点']
+    scores = result['得分']
+    #result = {'关键点':keypoints, '得分':scores}
+    skeleton = [(15, 13), (13, 11), (16, 14), (14, 12), (11, 12), (5, 11),
+            (6, 12), (5, 6), (5, 7), (6, 8), (7, 9), (8, 10), (1, 2),
+            (0, 1), (0, 2), (1, 3), (2, 4), (3, 5), (4, 6)]
+    palette = [[51, 153, 255], [0, 255, 0], [255, 128, 0], [255, 255, 255],
+               [255, 153, 255], [102, 178, 255], [255, 51, 51]]
+    link_color = [
+        1, 1, 2, 2, 0, 0, 0, 0, 1, 2, 1, 2, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 2, 2,
+        2, 2, 2, 2, 2, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 1, 1, 1, 1, 2, 2, 2,
+        2, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 1, 1, 1, 1
+    ]
+    point_color = [
+        0, 0, 0, 0, 0, 1, 2, 1, 2, 1, 2, 1, 2, 1, 2, 1, 2, 2, 2, 2, 2, 2, 2, 3,
+        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
+        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3,
+        3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 2, 2, 2, 2,
+        4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 1, 1, 1, 1, 3, 2, 2, 2, 2, 4, 4, 4,
+        4, 5, 5, 5, 5, 6, 6, 6, 6, 1, 1, 1, 1
+    ]
+
+    # draw keypoints and skeleton
+    for kpts, score in zip(keypoints, scores):
+        for kpt, color in zip(kpts, point_color):
+            image.draw_circles(center=kpt,
+                                radius=np.array([1.5]),
+                                edge_colors=tuple(palette[color]))
+            #cv2.circle(img, tuple(kpt.astype(np.int32)), 1, palette[color], 1,
+            #           cv2.LINE_AA)
+        for (u, v), color in zip(skeleton, link_color):
+            if score[u] > thr and score[v] > thr:
+                x_data = [kpts[u][0], kpts[v][0]]
+                y_data = [kpts[u][1], kpts[v][1]]
+                image.draw_lines(x_datas=np.array(x_data),
+                                y_datas=np.array(y_data),
+                                colors=tuple(palette[color]))
+                #cv2.line(img, tuple(kpts[u].astype(np.int32)),
+                #         tuple(kpts[v].astype(np.int32)), palette[color], 2,
+                #         cv2.LINE_AA)
+    
+
+def show_pose(images, results):
+    if isinstance(images, list) and isinstance(results, list):
+        for image, result in zip(images, results):
+            draw_single_pose(image=image, result= result)
+            image.imshow()
     else:
-        draw_single_det(image=images, result= results)
+        draw_single_pose(image=images, result= results)
+        images.imshow()
```

### Comparing `BaseDT-0.0.8/setup.py` & `BaseDT-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.0.8',
+    version='0.0.9',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

