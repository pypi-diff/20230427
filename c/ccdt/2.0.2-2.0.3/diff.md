# Comparing `tmp/ccdt-2.0.2.tar.gz` & `tmp/ccdt-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.0.2.tar", last modified: Tue Apr 25 10:50:03 2023, max compression
+gzip compressed data, was "ccdt-2.0.3.tar", last modified: Thu Apr 27 07:14:14 2023, max compression
```

## Comparing `ccdt-2.0.2.tar` & `ccdt-2.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.253633 ccdt-2.0.2/
--rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     4319 2023-04-25 10:50:03.252635 ccdt-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.200773 ccdt-2.0.2/ccdt/
--rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.2/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.219722 ccdt-2.0.2/ccdt/dataset/
--rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.2/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.223740 ccdt-2.0.2/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.2/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.2/ccdt/dataset/base_coco/coco.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.230692 ccdt-2.0.2/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.2/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.2/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    59802 2023-04-25 06:24:11.000000 ccdt-2.0.2/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.233688 ccdt-2.0.2/ccdt/dataset/logs/
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.2/ccdt/dataset/logs/__init__.py
--rw-rw-rw-   0        0        0    10717 2023-04-25 08:57:24.000000 ccdt-2.0.2/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.242660 ccdt-2.0.2/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      200 2023-04-17 07:06:14.000000 ccdt-2.0.2/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.2/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    10182 2023-04-25 10:32:57.000000 ccdt-2.0.2/ccdt/dataset/utils/labelme_load.py
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.2/ccdt/dataset/utils/logs.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.249668 ccdt-2.0.2/ccdt/video_tool/
--rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.2/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.2/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.2/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:50:03.214737 ccdt-2.0.2/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4319 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 10:50:03.000000 ccdt-2.0.2/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 10:50:03.254628 ccdt-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2278 2023-04-25 10:49:25.000000 ccdt-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.304269 ccdt-2.0.3/
+-rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4319 2023-04-27 07:14:14.303272 ccdt-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.270364 ccdt-2.0.3/ccdt/
+-rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.3/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.282329 ccdt-2.0.3/ccdt/dataset/
+-rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.3/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.285333 ccdt-2.0.3/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.3/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.3/ccdt/dataset/base_coco/coco.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.290310 ccdt-2.0.3/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.3/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.3/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    60692 2023-04-27 02:23:46.000000 ccdt-2.0.3/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.291310 ccdt-2.0.3/ccdt/dataset/logs/
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.3/ccdt/dataset/logs/__init__.py
+-rw-rw-rw-   0        0        0    11356 2023-04-27 01:34:21.000000 ccdt-2.0.3/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.297289 ccdt-2.0.3/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      200 2023-04-17 07:06:14.000000 ccdt-2.0.3/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.3/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    10182 2023-04-25 10:32:57.000000 ccdt-2.0.3/ccdt/dataset/utils/labelme_load.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.3/ccdt/dataset/utils/logs.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.302251 ccdt-2.0.3/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.3/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.3/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.3/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.279336 ccdt-2.0.3/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4319 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 07:14:14.304269 ccdt-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2278 2023-04-27 06:57:07.000000 ccdt-2.0.3/setup.py
```

### Comparing `ccdt-2.0.2/LICENSE` & `ccdt-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/PKG-INFO` & `ccdt-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.2
+Version: 2.0.3
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.2/README.md` & `ccdt-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/ccdt/dataset/base_coco/coco.py` & `ccdt-2.0.3/ccdt/dataset/base_coco/coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.0.3/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.0.3/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         """
         传参初始化labelme数据集对象
         """
         self.datasets = args[0]
         self.check_error_dataset = list()  # 存储错误图像数据变量列表
         self.error_output_path = ''  # 定义全局错误输出路径变量
         self.error_image_path = ''  # 定义全局图像路径变量
+        self.automatic_correction = list()  # 定义存放逻辑处理后封装数据的存放列表
+        self.output_dir = ''  # 自定义数据保存输入目录，用于传参时灵活使用
 
     def save_labelme(self, output_dir, index, custom_label):
         """
         保存数据功能，主要实现图片拷贝、json文件重写
         使用异步编程：Python的asyncio模块提供了异步编程的支持，可以在执行IO操作期间允许程序在其他任务中并行执行。
         :param output_dir: 形参变量，传递列表、字符串、None
         :param index: 形参变量，传递索引数字、bool值
@@ -150,15 +152,15 @@
         num_images = 0  # 计数image_file
         num_background = 0  # 计数labelme_info为空并且image_file不为空.有图片没有标注的算背景，有json文件就算背景不对
         property_tb = pt.PrettyTable(['label_name', 'shape_type_name', 'flags_name'])
         num_tb = pt.PrettyTable(['num_images', 'num_labelme', 'num_background'])
         label_value = []
         print_data = list()
         title = ''
-        # print(f'筛选及重组满足打印条件的labelme数据集')
+        print(f'筛选及重组满足打印条件的labelme数据集')
         for data_info in tqdm(self.datasets):
             title = data_info.get('input_dir')
             if data_info.get('image_file') and data_info.get('labelme_info') is None:
                 num_background += 1
             if data_info.get('image_file'):
                 num_images += 1
             if data_info.get('image_file') and data_info.get('labelme_info'):
@@ -175,25 +177,25 @@
                         print_data.append(rebuild_shape)
         num_tb.add_row([num_images, num_labelme, num_background])
         # print(f'打印满足重组条件的labelme数据集')
         for data in print_data:
             property_tb.add_row([data.get('label'), data.get('shape_type'), data.get('flags')])
         # print(property_tb)
         # print(num_tb)
-        # print(num_tb.get_string(title=title))
-        # print(property_tb.get_string(title=title))
+        print(num_tb.get_string(title=title))
+        print(property_tb.get_string(title=title))
 
     def split_list(self, parameter):
         """
         将列表平均分成 extract_amount 份
         :param parameter: 指定份数
         """
         random.shuffle(self.datasets)
         avg = len(self.datasets) / float(parameter.extract_portion)
-        result = []  # 分好后追加列表又会导致内存里面多了一份数据集
+        # result = []  # 分好后追加列表又会导致内存里面多了一份数据集
         last = 0.0
         index = 0
         while last < len(self.datasets):
             # result.append(self.datasets[int(last):int(last + avg)])
             # 直接传递列表到，save_labelme方法进行迭代后保存，省去了重写保存方法
             self.save_labelme(self.datasets[int(last):int(last + avg)], index, parameter.label_name)
             last += avg
@@ -551,25 +553,14 @@
             # 再确定左下角和右上角
             vertices = [
                 [x_min, y_min],  # 左上角
                 [x_max, y_min],  # 右上角
                 [x_max, y_max],  # 右下角
                 [x_min, y_max],  # 左下角
             ]
-            # ==============错误计算======================
-            # left_top = rectangle['points'][0]  # 左上角坐标
-            # right_bottom = rectangle['points'][1]  # 右下角坐标
-            # # 计算矩形框的左下角和右上角顶点坐标
-            # left_bottom = (left_top[0], right_bottom[1])
-            # right_top = (right_bottom[0], left_top[1])
-            # # 按照左上、右上、右下、左下的顺序排列4个顶点
-            # vertices = [tuple(left_top), right_top, tuple(right_bottom), left_bottom]
-            # ==============错误计算======================
-            # 输出结果
-            # print(vertices)
             # 按照左上、右上、右下、左下的顺序排列4个顶点，并返回列表
             return vertices
         else:
             points = rectangle['points']
             print(f'矩形框标注点的数量不对{points}，请核对数据{file_path}')
 
     @staticmethod
@@ -577,55 +568,29 @@
         """
         找到多边形，左上、右上、右下、左下的顺序排列4个顶点
         这个算法的时间复杂度为 O(n)，其中n 是多边形的点数。
         :param polygon:
         :param file_path:
         """
         if len(polygon.get('points')) == 4:
-            # 定义多边形的点集
-            points = [[polygon['points'][0][0], polygon['points'][0][1]],
-                      [polygon['points'][1][0], polygon['points'][1][1]],
-                      [polygon['points'][2][0], polygon['points'][2][1]],
-                      [polygon['points'][3][0], polygon['points'][3][1]]]
-            # 找到最左、最右、最上、最下的坐标点
-            leftmost = min(points, key=lambda x: x[0])
-            rightmost = max(points, key=lambda x: x[0])
-            topmost = min(points, key=lambda x: x[1])
-            bottommost = max(points, key=lambda x: x[1])
-            # 确定四个角的点
-            top_left = None  # 左上
-            top_right = None  # 右上
-            bottom_right = None  # 右下
-            bottom_left = None  # 左下
-            for point in points:
-                if point == leftmost:
-                    if top_left is None or point[1] < top_left[1]:
-                        top_left = point
-                    if bottom_left is None or point[1] > bottom_left[1]:
-                        bottom_left = point
-                elif point == rightmost:
-                    if top_right is None or point[1] < top_right[1]:
-                        top_right = point
-                    if bottom_right is None or point[1] > bottom_right[1]:
-                        bottom_right = point
-                elif point == topmost:
-                    if top_left is None or point[0] > top_left[0]:
-                        top_left = point
-                    if top_right is None or point[0] < top_right[0]:
-                        top_right = point
-                elif point == bottommost:
-                    if bottom_left is None or point[0] > bottom_left[0]:
-                        bottom_left = point
-                    if bottom_right is None or point[0] < bottom_right[0]:
-                        bottom_right = point
-            # 按照左上、右上、右下、左下的顺序排列4个顶点
-            vertices = [top_left, top_right, bottom_right, bottom_left]
-            # 输出结果
-            # print(vertices)
-            return vertices
+            # 初始化最左、最右、最上和最下的点为多边形的第一个点
+            leftmost, rightmost, topmost, bottommost = polygon.get('points')[0], polygon.get('points')[0], \
+                                                       polygon.get('points')[0], polygon.get('points')[0]
+
+            # 遍历多边形的每一个点，并更新最左、最右、最上和最下的点的坐标值
+            for point in polygon.get('points'):
+                if point[0] < leftmost[0]:
+                    leftmost = point
+                if point[0] > rightmost[0]:
+                    rightmost = point
+                if point[1] < topmost[1]:
+                    topmost = point
+                if point[1] > bottommost[1]:
+                    bottommost = point
+            return [leftmost, topmost, rightmost, bottommost]
         else:
             points = polygon.get('points')
             print(f'多边形标注点不为4个点{points}，请核对数据{file_path}')
 
     def intercept_coordinates(self):
         """
         根据矩形框截取图像，并保存矩形框内包含的多边形标注属性
@@ -816,138 +781,135 @@
                                     print(f'车牌号未填写{file_path}')
                                     self.error_dataset_handle(dataset)
         if isinstance(parameter.judging_cross_the_border, str):
             print(f'检查标注坐标位置，是否超越原始图像宽高边界')
             for dataset in tqdm(self.datasets):
                 if dataset.get('background') is False:
                     for shape in dataset.get('labelme_info').get('shapes'):
-                        self.rectangle_cross_the_border(shape, dataset)
+                        self.rectangle_cross_the_border(shape, dataset, parameter.automatic_correction)
         if self.check_error_dataset:  # 如果有值才保存，否则会保存出错
             # 保存合并后的数据集
             print(f'保存出错数据集，需要人工矫正')
             self.save_labelme(self.check_error_dataset, self.error_output_path, None)
 
     def sort_correct_labelme(self, parameter):
         """
         通过坐标点排序后，抠出车牌，并对倾斜的车牌进行矫正
+        也可以对原始标注进行截取
         :param parameter:
         """
         print(f'更新多边形标注坐标的排序顺序')
         for dataset in tqdm(self.datasets):
             if dataset.get('background') is False:
                 for shape in dataset.get('labelme_info').get('shapes'):
                     if shape.get('shape_type') == 'polygon':
-                        # 找到多边形，左上、右上、右下、左下的顺序排列4个顶点
-                        # crop_img = self.mask_img(shape, dataset.get('full_path'), dataset)
-                        # 按照原始图像进行
-                        # crop_img = self.original_shape_cutout(shape, dataset.get('full_path'))
-
-                        if shape.get('text'):
-                            crop_img = self.main(shape, dataset.get('full_path'))
-                            obj = Path(dataset.get('full_path'))
-
-                            file_name = obj.stem + '_' + shape.get('text') + obj.suffix
-                            save_dir = os.path.join(dataset.get('output_dir'), file_name)
-                            os.makedirs(dataset.get('error_path'), exist_ok=True)
-                            cv2.imwrite(save_dir, crop_img)
-                        # else:
-                        # print(dataset)
-
-                        # poly_sequential_coordinates = self.find_poly_sequential_coordinates(shape,
-                        # dataset.get('full_path'))
-                        # shape['points'] = poly_sequential_coordinates
-        print(f'保存排序后的labelme数据集')
-        # self.save_labelme(None, None, None)e
-
-    # @staticmethod
-    def mask_img(self, shape, image_path, dataset):
-        """
-        截取多边形图像，补充黑边
-        :param shape:
-        :param image_path:
-        :return:
-        """
-
-        # 获取按顺序排列的多边形坐标点
-        # sort_poly_point = self.find_poly_sequential_coordinates(shape, image_path)
-        # 获取多边形坐标点的宽高
-        points = np.array(shape['points'])
-        point_min, point_max = points.min(axis=0), points.max(axis=0)
-        w, h = point_max - point_min
-        # 读取原始图像
-        img = cv2.imread(image_path)
-
-        # 定义标记多边形的对应点
-        poly = np.array(shape['points'], np.int32)
-
-        # 创建一个全0矩阵作为掩模（mask）
-        mask = np.zeros(img.shape[:2], dtype=np.uint8)
-
-        # 以四元组（x，y）的形式构造点集合
-        # pts = np.array(shape['points'], dtype=np.int32)
-
-        # 将多边形的点集合打包为适当的数据类型
-        # pts = poly.reshape((-1, 1, 2))
-
-        # 调用cv2.fillPoly()函数
-        # cv2.fillPoly(mask, pts, color=(255, 255, 255))
-        # 将多边形区域填充为白色（255），注意这里需要将多边形点坐标先转置（即x,y变为y,x）再传入fillPoly函数
-        cv2.fillPoly(mask, [poly], 255)
-
-        # 根据掩模mask对原始图像进行位运算，提取多边形区域
-        res = cv2.bitwise_and(img, img, mask=mask)
-
-        # 提取多边形四个顶点的坐标，并按顺时针方向排列
-        rect = cv2.minAreaRect(poly)
-        src_sort = cv2.boxPoints(rect)
-        # dst_sort = np.int0(src_sort)
-
-        # 计算变换矩阵和输出图像大小
-        src_pts = src_sort.astype("float32")
-        # 注意，这几个点的顺序要按照顺时针或逆时针方向给出
-        # dst_pts = np.array(dst_sort, dtype="float32")
-
-        # 获取新坐标点
-        left_top = points[0]
-        right_top = [points[0][0] + w, points[0][1] + 0]
-        right_down = [points[0][0] + w, points[0][1] + h]
-        left_down = [points[0][0] + 0, points[0][1] + h]
-        # dst_pts = np.array([left_top, right_top, right_down, left_down], dtype=np.float32)
-        dst_pts = np.array([right_top, right_down, left_down, left_top], dtype=np.float32)
-
-        # 计算透视变换矩阵，src_pts是源图像上的四个点的坐标，它们需要按照逆时针方向给出；dst_pts是目标图像上的四个点的坐标，也需要按照逆时针方向给出。
-        perspective_transformation = cv2.getPerspectiveTransform(src_pts, dst_pts)
-        # 将原始图像res应用透视变换, perspective_transformation为透视变换矩阵，(w, h)是输出图像的大小，它表示输出图像的宽度和高度
-        warp = cv2.warpPerspective(res, perspective_transformation,
-                                   (dataset.get('image_width'), dataset.get('image_height')))
-        a = warp[int(min(dst_pts[:, 1])):int(max(dst_pts[:, 1])), int(min(dst_pts[:, 0])):int(max(dst_pts[:, 0])), :]
-        # 显示原图和处理后图像
-        # cv2.imshow("Original Image", img)
-        # cv2.imshow("Mask", mask)
-        # cv2.imshow("Result", res)
-        # cv2.imshow("Warped", warp)
-        # cv2.waitKey(0)
-        # cv2.destroyAllWindows()
-        return a
+                        if parameter.function == 'correct':
+                            if shape.get('text'):  # 有车牌的才进行截取图像并矫正车牌
+                                if shape.get('flags').get('double'):  # 双层车牌
+                                    crop_img = self.correct_shape_cutout(shape, dataset.get('full_path'))
+                                    self.save_poly_cut_img(crop_img, dataset, shape, 'double')
+                                else:  # 单层车牌
+                                    crop_img = self.correct_shape_cutout(shape, dataset.get('full_path'))
+                                    self.save_poly_cut_img(crop_img, dataset, shape, 'single')
+                        if parameter.function == 'original':
+                            if shape.get('text'):  # 有车牌的才进行截取图像
+                                if shape.get('flags').get('double'):  # 双层车牌
+                                    crop_img = self.original_shape_cutout(shape, dataset.get('full_path'))
+                                    self.save_poly_cut_img(crop_img, dataset, shape, 'double')
+                                else:  # 单层车牌
+                                    crop_img = self.original_shape_cutout(shape, dataset.get('full_path'))
+                                    self.save_poly_cut_img(crop_img, dataset, shape, 'single')
+
+    # # @staticmethod
+    # def mask_img(self, shape, image_path, dataset):
+    #     """
+    #     截取多边形图像，补充黑边
+    #     :param shape:
+    #     :param image_path:
+    #     :return:
+    #     """
+    #
+    #     # 获取按顺序排列的多边形坐标点
+    #     # sort_poly_point = self.find_poly_sequential_coordinates(shape, image_path)
+    #     # 获取多边形坐标点的宽高
+    #     points = np.array(shape['points'])
+    #     point_min, point_max = points.min(axis=0), points.max(axis=0)
+    #     w, h = point_max - point_min
+    #     # 读取原始图像
+    #     img = cv2.imread(image_path)
+    #
+    #     # 定义标记多边形的对应点
+    #     poly = np.array(shape['points'], np.int32)
+    #
+    #     # 创建一个全0矩阵作为掩模（mask）
+    #     mask = np.zeros(img.shape[:2], dtype=np.uint8)
+    #
+    #     # 以四元组（x，y）的形式构造点集合
+    #     # pts = np.array(shape['points'], dtype=np.int32)
+    #
+    #     # 将多边形的点集合打包为适当的数据类型
+    #     # pts = poly.reshape((-1, 1, 2))
+    #
+    #     # 调用cv2.fillPoly()函数
+    #     # cv2.fillPoly(mask, pts, color=(255, 255, 255))
+    #     # 将多边形区域填充为白色（255），注意这里需要将多边形点坐标先转置（即x,y变为y,x）再传入fillPoly函数
+    #     cv2.fillPoly(mask, [poly], 255)
+    #
+    #     # 根据掩模mask对原始图像进行位运算，提取多边形区域
+    #     res = cv2.bitwise_and(img, img, mask=mask)
+    #
+    #     # 提取多边形四个顶点的坐标，并按顺时针方向排列
+    #     rect = cv2.minAreaRect(poly)
+    #     src_sort = cv2.boxPoints(rect)
+    #     # dst_sort = np.int0(src_sort)
+    #
+    #     # 计算变换矩阵和输出图像大小
+    #     src_pts = src_sort.astype("float32")
+    #     # 注意，这几个点的顺序要按照顺时针或逆时针方向给出
+    #     # dst_pts = np.array(dst_sort, dtype="float32")
+    #
+    #     # 获取新坐标点
+    #     left_top = points[0]
+    #     right_top = [points[0][0] + w, points[0][1] + 0]
+    #     right_down = [points[0][0] + w, points[0][1] + h]
+    #     left_down = [points[0][0] + 0, points[0][1] + h]
+    #     # dst_pts = np.array([left_top, right_top, right_down, left_down], dtype=np.float32)
+    #     dst_pts = np.array([right_top, right_down, left_down, left_top], dtype=np.float32)
+    #
+    #     # 计算透视变换矩阵，src_pts是源图像上的四个点的坐标，它们需要按照逆时针方向给出；dst_pts是目标图像上的四个点的坐标，也需要按照逆时针方向给出。
+    #     perspective_transformation = cv2.getPerspectiveTransform(src_pts, dst_pts)
+    #     # 将原始图像res应用透视变换, perspective_transformation为透视变换矩阵，(w, h)是输出图像的大小，它表示输出图像的宽度和高度
+    #     warp = cv2.warpPerspective(res, perspective_transformation,
+    #                                (dataset.get('image_width'), dataset.get('image_height')))
+    #     a = warp[int(min(dst_pts[:, 1])):int(max(dst_pts[:, 1])), int(min(dst_pts[:, 0])):int(max(dst_pts[:, 0])), :]
+    #     # 显示原图和处理后图像
+    #     # cv2.imshow("Original Image", img)
+    #     # cv2.imshow("Mask", mask)
+    #     # cv2.imshow("Result", res)
+    #     # cv2.imshow("Warped", warp)
+    #     # cv2.waitKey(0)
+    #     # cv2.destroyAllWindows()
+    #     return a
 
     def error_dataset_handle(self, dataset):
         """
         判断追加的封装数据是否重复，如果重复就不继续追加
         :param dataset:
         """
         # 如果同一张图像分组出现多次错误，只追加一次dataset
         if dataset not in self.check_error_dataset:
             self.error_output_path = dataset.get('group_error_path')
             self.check_error_dataset.append(dataset)
 
-    def rectangle_cross_the_border(self, bbox, dataset):
+    def rectangle_cross_the_border(self, bbox, dataset, automatic_correction):
         """
         标注坐标超越原始图像边界逻辑实现
         :param bbox:
         :param dataset:
+        :param automatic_correction:自动矫正越界标注参数
         :return:
         """
         self.error_image_path = dataset.get('full_path')
         if isinstance(bbox, list):
             x1 = bbox[0][0]
             y1 = bbox[0][1]
             x2 = bbox[1][0]
@@ -968,17 +930,29 @@
                     x1 = bbox.get('points')[0][0]
                     y1 = bbox.get('points')[0][1]
                     x2 = bbox.get('points')[1][0]
                     y2 = bbox.get('points')[1][1]
                     if x1 < 0 or y1 < 0 or x2 < 0 or y2 < 0 or x1 > dataset.get('image_width') or \
                             y1 > dataset.get('image_height') or x2 > dataset.get('image_width') or \
                             y2 > dataset.get('image_height'):
-                        print(f'标注的矩形框已经超越图像边界{self.error_image_path}')
-                        print(bbox)
-                        self.error_dataset_handle(dataset)
+                        if automatic_correction:  # 自动矫正越界标注形状
+                            clamp_x1 = np.clip(x1, 0, dataset.get('image_width'))
+                            clamp_y1 = np.clip(y1, 0, dataset.get('image_height'))
+                            clamp_x2 = np.clip(x2, 0, dataset.get('image_width'))
+                            clamp_y2 = np.clip(y2, 0, dataset.get('image_height'))
+                            # 替换
+                            bbox.get('points')[0][0] = clamp_x1
+                            bbox.get('points')[0][1] = clamp_y1
+                            bbox.get('points')[1][0] = clamp_x2
+                            bbox.get('points')[1][1] = clamp_y2
+                            self.output_dir = dataset.get('output_dir')
+                            self.automatic_correction.append(dataset)
+                        else:
+                            print(f'标注的矩形框已经超越图像边界{self.error_image_path}')
+                            self.error_dataset_handle(dataset)
                 else:
                     print(f'标注的矩形框坐标点不对，保存到错误数据集')
                     self.error_dataset_handle(dataset)
             if bbox.get('shape_type') == 'polygon':
                 if len(bbox.get('points')) == 4:
                     x1 = bbox.get('points')[0][0]
                     y1 = bbox.get('points')[0][1]
@@ -989,113 +963,143 @@
                     x4 = bbox.get('points')[3][0]
                     y4 = bbox.get('points')[3][1]
                     if x1 < 0 or y1 < 0 or x2 < 0 or y2 < 0 or x3 < 0 or y3 < 0 or x4 < 0 or y4 < 0 or \
                             x1 > dataset.get('image_width') or y1 > dataset.get('image_height') or \
                             x2 > dataset.get('image_width') or y2 > dataset.get('image_height') or \
                             x3 > dataset.get('image_width') or y3 > dataset.get('image_height') or \
                             x4 > dataset.get('image_width') or y4 > dataset.get('image_height'):
-                        print(f'标注的多边形框已经超越图像边界{self.error_image_path}')
-                        self.error_dataset_handle(dataset)
+                        if automatic_correction:  # 自动矫正越界标注形状
+                            clamp_x1 = np.clip(x1, 0, dataset.get('image_width'))
+                            clamp_y1 = np.clip(y1, 0, dataset.get('image_height'))
+                            clamp_x2 = np.clip(x2, 0, dataset.get('image_width'))
+                            clamp_y2 = np.clip(y2, 0, dataset.get('image_height'))
+                            # 替换
+                            bbox.get('points')[0][0] = clamp_x1
+                            bbox.get('points')[0][1] = clamp_y1
+                            bbox.get('points')[1][0] = clamp_x2
+                            bbox.get('points')[1][1] = clamp_y2
+                            self.output_dir = dataset.get('output_dir')
+                            self.automatic_correction.append(dataset)
+                        else:
+                            print(f'标注的多边形框已经超越图像边界{self.error_image_path}')
+                            self.error_dataset_handle(dataset)
                 else:
                     print(f'标注的多边形坐标点不为4个，保存到错误数据集')
                     self.error_dataset_handle(dataset)
 
+    def correct_shape_cutout(self, shape, image_path):
+        points = self.sort_lmks(np.array(shape['points']))  # 把传入的列表坐标转成numpy，然后进行排序，左上、右上、右下、左下的顺序排列4个顶点
+        # 读取原始图像
+        img = cv2.imread(image_path)
+        xmax, ymax = np.max(points, axis=0)
+        point_max = np.array([xmax, ymax])
+        w = int(abs(points[0][0] - point_max[0]))
+        h = int(abs(points[0][1] - point_max[1]))
+        # 获取新坐标点
+        left_top = points[0]
+        right_top = [points[0][0] + w, points[0][1] + 0]
+        right_down = [points[0][0] + w, points[0][1] + h]
+        left_down = [points[0][0] + 0, points[0][1] + h]
+
+        new_points = np.array([left_top, right_top, right_down, left_down], dtype=np.float32)
+        points = points.astype(np.float32)
+        # 透视变换
+        mat = cv2.getPerspectiveTransform(points, new_points)
+        plate_img = cv2.warpPerspective(img, mat, (img.shape[1], img.shape[0]))[int(points[0][1]):int(points[0][1] + h),
+                    int(points[0][0]):int(points[0][0] + w), :]
+        return plate_img
+
+    def sort_lmks(self, landmarks):
+        """
+        多边形标注排序，左上、右上、右下、左下的顺序排列
+        :param landmarks:
+        :return:
+        """
+        assert len(landmarks) == 4
+        x = list(copy.copy(landmarks[:, 0]))
+        y = list(copy.copy(landmarks[:, 1]))
+        points = landmarks
+        x.sort()
+        y.sort()
+        if abs(x[0] - x[1]) < abs(np.mean(x[:2]) - np.mean(x[2:])) and abs(x[2] - x[3]) < abs(
+                np.mean(x[:2]) - np.mean(x[2:])):
+            l_t, other = self.sort_x(np.array(points).reshape(-1, 2), x)
+        elif abs(y[0] - y[1]) < abs(np.mean(y[:2]) - np.mean(y[2:])) and abs(y[2] - y[3]) < abs(
+                np.mean(y[:2]) - np.mean(y[2:])):
+            l_t, other = self.sort_y(np.array(points).reshape(-1, 2), y)
+        else:
+            print(landmarks)
+        cos_key = lambda points_distance: (points_distance[0] - l_t[0]) / (
+            np.sqrt((points_distance[0] - l_t[0]) ** 2 + (points_distance[1] - l_t[1]) ** 2))
+        other.sort(key=cos_key, reverse=True)
+        other.insert(0, l_t)
+        # lmkds = list(np.array(other).reshape(-1))
+        lmkds = np.array(other)
+        return lmkds
+
+    @staticmethod
+    def sort_y(points, y):
+        l_t = points[np.isin(points[:, 1], np.array(y[:2]))]
+        l_t = l_t[np.where(l_t[:, 0] == np.min(l_t[:, 0]))]
+        l_t = np.squeeze(l_t)
+        return l_t, [point for point in points if (point != l_t).any()]
+
+    @staticmethod
+    def sort_x(points, x):
+        l_t = points[np.isin(points[:, 0], np.array(x[:2]))]
+        l_t = l_t[np.where(l_t[:, 1] == np.min(l_t[:, 1]))]
+        l_t = np.squeeze(l_t)
+        return l_t, [point for point in points if (point != l_t).any()]
+
     @staticmethod
     def original_shape_cutout(shape, image_path):
         """
-        按照原始标注形状截取图像
+        直接根据多边形坐标进行截取，不做矫正，只填写黑边
         :param shape:
         :param image_path:
         :return:
         """
+        coordinates = list()
         img = cv2.imread(image_path)
-        # 井的四个顶点
         points = np.array(shape['points'])
         a = points[0]
         b = points[1]
         c = points[2]
         d = points[3]
         bbox = [int(np.min(points[:, 0])), int(np.min(points[:, 1])), int(np.max(points[:, 0])),
                 int(np.max(points[:, 1]))]
         coordinate = [[[int(a[0]), int(a[1])], [int(b[0]), int(b[1])], [int(c[0]), int(c[1])], [int(d[0]), int(d[1])]]]
-        coordinates = []
         coordinates.append(np.array(coordinate))
-
-        # 获取车牌四个顶点e
-        '''a = points.split('_')[0]
-        b = points.split('_')[1]
-        c = points.split('_')[2]
-        d = points.split('_')[3]
-        coordinate = [[[int(a.split('&')[0]), int(a.split('&')[1])], [int(b.split('&')[0]), int(b.split('&')[1])], [int(c.split('&')[0]), int(c.split('&')[1])], [int(d.split('&')[0]), int(d.split('&')[1])]]]
-        coordinates = []
-        coordinates.append(np.array(coordinate))'''
-
         # 抠出车牌
         mask = np.zeros(img.shape[:2], dtype=np.int8)
         mask = cv2.fillPoly(mask, coordinates, 255)
         bbox_mask = mask
-        # color_mask = np.array([0, 0, 255], dtype=np.uint8)
         bbox_mask = bbox_mask.astype(np.bool_)
         temp_img = copy.deepcopy(img)
         for i in range(3):
             temp_img[:, :, i] *= bbox_mask
         crop_img = temp_img[bbox[1]:bbox[3], bbox[0]:bbox[2], :]
         return crop_img
 
     @staticmethod
-    def main(shape, image_path):
-        img = cv2.imread(image_path)
-        # img = copy.deepcopy(img0)
-        points = np.array(shape['points']).astype(np.float32)
-
-        # 获取最小外接矩阵，中心点坐标，宽高，旋转角度
-        rect = cv2.minAreaRect(points)
-        # 获取矩形四个顶点，浮点型
-        box_float = cv2.boxPoints(rect)
-        # 取整
-        box_int = np.int0(box_float)
-
-        # 获取四个顶点坐标
-        left_point_x = np.min(box_int[:, 0])
-        right_point_x = np.max(box_int[:, 0])
-        top_point_y = np.min(box_int[:, 1])
-        bottom_point_y = np.max(box_int[:, 1])
-
-        rect_w = right_point_x - left_point_x
-        rect_h = bottom_point_y - top_point_y
-
-        left_point_y = box_int[:, 1][np.where(box_int[:, 0] == left_point_x)][0]
-        right_point_y = box_int[:, 1][np.where(box_int[:, 0] == right_point_x)][0]
-        top_point_x = box_int[:, 0][np.where(box_int[:, 1] == top_point_y)][0]
-        bottom_point_x = box_int[:, 0][np.where(box_int[:, 1] == bottom_point_y)][0]
-        # 上下左右四个点坐标
-        vertices = np.array([[top_point_x, top_point_y], [bottom_point_x, bottom_point_y], [left_point_x, left_point_y],
-                             [right_point_x, right_point_y]])
-        # print(vertices)
-        # 畸变情况1
-        if rect[2] > -45:
-            new_right_point_x = vertices[0, 0]
-            new_right_point_y = int(vertices[1, 1] - (vertices[0, 0] - vertices[1, 0]) / (vertices[3, 0] - vertices[1, 0] + 0.00000001) * (vertices[1, 1] - vertices[3, 1]))
-            new_left_point_x = vertices[1, 0]
-            new_left_point_y = int(vertices[0, 1] + (vertices[0, 0] - vertices[1, 0]) / (vertices[0, 0] - vertices[2, 0] + 0.00000001) * (vertices[2, 1] - vertices[0, 1]))
-            # 校正后的四个顶点坐标
-            point_set_1 = np.float32([[rect_w, 0], [0, 0], [0, rect_h], [rect_w, rect_h]])
-        # 畸变情况2
-        elif rect[2] < -45:
-            new_right_point_x = vertices[1, 0]
-            new_right_point_y = int(vertices[0, 1] + (vertices[1, 0] - vertices[0, 0]) / (vertices[3, 0] - vertices[0, 0]) * (vertices[3, 1] - vertices[0, 1]))
-            new_left_point_x = vertices[0, 0]
-            new_left_point_y = int(vertices[1, 1] - (vertices[1, 0] - vertices[0, 0]) / (vertices[1, 0] - vertices[2, 0]) * (vertices[1, 1] - vertices[2, 1]))
-            # 校正后的四个顶点坐标
-            point_set_1 = np.float32([[0, 0], [0, rect_h], [rect_w, rect_h], [rect_w, 0]])
-
-        # 校正前平行四边形四个顶点坐标
-        new_box = np.array([(vertices[0, 0], vertices[0, 1]), (new_left_point_x, new_left_point_y), (vertices[1, 0], vertices[1, 1]),(new_right_point_x, new_right_point_y)])
-
-        point_set_0 = np.float32(new_box)
-
-        # 变换矩阵
-        mat = cv2.getPerspectiveTransform(point_set_0, point_set_1)
-        # 投影变换
-        lic = cv2.warpPerspective(img, mat, (rect_w, rect_h))
+    def save_poly_cut_img(crop_img, dataset, shape, single_double):
+        """
+        保存多边形截取图像
+        :param crop_img:
+        :param dataset:
+        :param shape:
+        :param single_double:单双车牌传参
+        """
+        obj = Path(dataset.get('full_path'))
+        file_name = obj.stem + '_' + shape.get('text') + obj.suffix
+        save_dir = os.path.join(dataset.get('output_dir'), single_double, file_name)
+        os.makedirs(os.path.dirname(save_dir), exist_ok=True)
+        cv2.imwrite(save_dir, crop_img)
 
-        return lic
+    def cross_boundary_correction(self, parameter):
+        print(f'程序自动矫正，标注形状超越图像边界情况')
+        for dataset in tqdm(self.datasets):
+            if dataset.get('background') is False:
+                for shape in dataset.get('labelme_info').get('shapes'):
+                    self.rectangle_cross_the_border(shape, dataset, parameter.automatic_correction)
+        print(f'保存标注超越图像边界，矫正后的数据')
+        self.save_labelme(self.automatic_correction, self.output_dir, None)
```

### Comparing `ccdt-2.0.2/ccdt/dataset/main.py` & `ccdt-2.0.3/ccdt/dataset/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     parser.add_argument('--min-pixel', type=int, default=512, help='最小像素截图设置，默认512像素。即大于512像素的矩形框才进行截图')
     parser.add_argument('--judging-group', type=int, help='默认值为2个shape元素为一组，用于判断分组元素的数量')
     # parser.add_argument('--judging-flags', type=json.loads, help="检查flags默认标注属性，是否符合标注准则")
     parser.add_argument('--judging-flags', type=ast.literal_eval, help="检查flags默认标注属性，是否符合标注准则")
     parser.add_argument('--judging-polygon', type=int, help='检查多边形标注的点是否超出预期数量，比如4个点的多边形，不能出现5个')
     parser.add_argument('--judging-cross-the-border', type=str, help="检查标注形状是否超越原始图像边界")
     parser.add_argument('--point-number', type=int, help='点标注的数量，用于标注点排序时，追加标注点到列表中然后判断，是否满足标注规则')
+    parser.add_argument('--automatic-correction', action="store_true", help="默认False，是否自动矫正标注形状超越图像边界情况。是为True，否为False")
 
     args = parser.parse_args()
     if args.function == 'filter_positive':  # 筛选正样本
         return args
     elif args.function == 'filter_negative':  # 筛选负样本
         return args
     elif args.function == 'filter_label':  # 筛选负样本
@@ -88,15 +89,17 @@
         return args
     elif args.function == 'duplicate':  # 对数据集去重
         return args
     elif args.function == 'compress':  # 对抽取数据集进行压缩
         return args
     elif args.function == 'check':  # 检查分组标注常见错误，包含：一组标注少一个标注框或点，一组标注的group_id值不对。
         return args
-    elif args.function == 'correct':  # 对多边形车牌标注进行排序，截取图像，矫正形状摆放位置
+    elif args.function == 'correct' or args.function == 'original':  # 对多边形车牌标注进行排序，截取图像，矫正形状摆放位置
+        return args
+    elif args.function == 'cross':  # 针对标注形状超越图像边界情况，使用程序自动矫正
         return args
     else:
         assert not args.function, '传入的操作功能参数不对:{}'.format(args.function)
 
 
 def main():
     args = parser_args()
@@ -145,13 +148,16 @@
             dataset.save_labelme(args.output_dir, None, None)
         elif args.function == 'extract':  # 抽取labelme数据集功能，指定份数抽取，只允许拷贝；指定图像张数抽取，允许剪切、拷贝
             dataset.extract_labelme(args)
         elif args.function == 'relation':  # 寻找标注形状包含关系，进行自动打组
             dataset.relation_labelme(args)
         elif args.function == 'check':  # 检查分组标注常见错误，包含：一组标注少一个标注框或点，一组标注的group_id值不对。
             dataset.check_group_labelme(args)
-        elif args.function == 'correct':  # 排序，按照多边形，左上、右上、右下、左下的顺序排列4个顶点，截取图像，矫正形状摆放位置
+        # correct为排序并矫正后的车牌截取，original为不排序也不矫正的车牌截取
+        elif args.function == 'correct' or args.function == 'original':  # 排序，按照多边形，左上、右上、右下、左下的顺序排列4个顶点，截取图像，矫正形状摆放位置
             dataset.sort_correct_labelme(args)
+        elif args.function == 'cross':  # 针对标注形状超越图像边界情况，使用程序自动矫正
+            dataset.cross_boundary_correction(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ccdt-2.0.2/ccdt/dataset/utils/encoder.py` & `ccdt-2.0.3/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.0.3/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/ccdt/video_tool/split.py` & `ccdt-2.0.3/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/ccdt/video_tool/video_main.py` & `ccdt-2.0.3/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/ccdt.egg-info/PKG-INFO` & `ccdt-2.0.3/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.2
+Version: 2.0.3
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.2/ccdt.egg-info/SOURCES.txt` & `ccdt-2.0.3/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.2/setup.py` & `ccdt-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.0.2',
+    version='2.0.3',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

