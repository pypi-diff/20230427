# Comparing `tmp/pystripe-1.2.2.tar.gz` & `tmp/pystripe-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pystripe-1.2.2.tar", last modified: Tue Mar 28 18:52:22 2023, max compression
+gzip compressed data, was "dist\pystripe-1.2.3.tar", last modified: Thu Apr 27 18:52:20 2023, max compression
```

## Comparing `pystripe-1.2.2.tar` & `pystripe-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 18:52:22.000000 pystripe-1.2.2/
--rw-rw-rw-   0        0        0     1087 2023-03-03 17:18:26.000000 pystripe-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     5302 2023-03-28 18:52:22.000000 pystripe-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4922 2023-03-03 17:18:26.000000 pystripe-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 18:52:22.000000 pystripe-1.2.2/pystripe/
--rw-rw-rw-   0        0        0      327 2023-03-03 17:18:26.000000 pystripe-1.2.2/pystripe/__init__.py
--rw-rw-rw-   0        0        0    34101 2023-03-28 18:50:56.000000 pystripe-1.2.2/pystripe/core.py
--rw-rw-rw-   0        0        0    10929 2023-03-03 17:18:26.000000 pystripe-1.2.2/pystripe/lightsheet_correct.py
--rw-rw-rw-   0        0        0     1668 2023-03-03 17:18:26.000000 pystripe-1.2.2/pystripe/raw.py
-drwxrwxrwx   0        0        0        0 2023-03-28 18:52:22.000000 pystripe-1.2.2/pystripe.egg-info/
--rw-rw-rw-   0        0        0     5302 2023-03-28 18:52:21.000000 pystripe-1.2.2/pystripe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-03-28 18:52:22.000000 pystripe-1.2.2/pystripe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 18:52:21.000000 pystripe-1.2.2/pystripe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-28 18:52:21.000000 pystripe-1.2.2/pystripe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-03-28 18:52:22.000000 pystripe-1.2.2/pystripe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-28 18:52:22.000000 pystripe-1.2.2/pystripe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-28 18:52:22.000000 pystripe-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      905 2023-03-28 18:51:27.000000 pystripe-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:52:20.000000 pystripe-1.2.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-27 18:51:02.000000 pystripe-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     5302 2023-04-27 18:52:20.000000 pystripe-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4922 2023-04-27 18:51:02.000000 pystripe-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 18:52:20.000000 pystripe-1.2.3/pystripe/
+-rw-rw-rw-   0        0        0      327 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/__init__.py
+-rw-rw-rw-   0        0        0    36593 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/core.py
+-rw-rw-rw-   0        0        0    10929 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/lightsheet_correct.py
+-rw-rw-rw-   0        0        0     1668 2023-04-27 18:51:02.000000 pystripe-1.2.3/pystripe/raw.py
+drwxrwxrwx   0        0        0        0 2023-04-27 18:52:20.000000 pystripe-1.2.3/pystripe.egg-info/
+-rw-rw-rw-   0        0        0     5302 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-04-27 18:52:20.000000 pystripe-1.2.3/pystripe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 18:52:19.000000 pystripe-1.2.3/pystripe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 18:52:20.000000 pystripe-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-04-27 18:51:02.000000 pystripe-1.2.3/setup.py
```

### Comparing `pystripe-1.2.2/LICENSE` & `pystripe-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.2/PKG-INFO` & `pystripe-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.2
+Version: 1.2.3
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.2/README.md` & `pystripe-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.2/pystripe/core.py` & `pystripe-1.2.3/pystripe/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 import multiprocessing
 import tqdm
 from dcimg import DCIMGFile
 from pystripe import raw
 from .lightsheet_correct import correct_lightsheet
 import warnings
 import shutil
+from typing import Optional
 warnings.filterwarnings("ignore")
 
 supported_extensions = ['.tif', '.tiff', '.raw', '.dcimg', '.png']
+supported_output_extensions = ['.tif', '.tiff', '.png']
 nb_retry = 10
 
 
 def _get_extension(path):
     """Extract the file extension from the provided path
 
     Parameters
@@ -56,14 +58,15 @@
     extension = _get_extension(path)
     if extension == '.raw':
         img = raw.raw_imread(path)
     elif extension == '.tif' or extension == '.tiff':
         img = tifffile.imread(path)
     elif extension == '.png':
         img = iio.imread(path)
+
     return img
 
 
 def imread_dcimg(path, z):
     """Load a slice from a DCIMG file
 
     Parameters
@@ -119,37 +122,59 @@
     start : int
         starting z position in tenths of micron
 
     """
     return int(os.path.basename(path).split('.')[0])
 
 
-def imsave(path, img, compression=1):
+def imsave(path, img, compression=1, output_format:Optional[str]=None):
     """Save an array as a tiff or raw image
 
     The file format will be inferred from the file extension in `path`
 
     Parameters
     ----------
     path : str
         path to tiff or raw image
     img : ndarray
         image as a numpy array
     compression : int
         compression level for tiff writing
-
+    output_format : Optional[str]
+        Desired format extension to save the image. Default: None
+        Accepted ['.tiff', '.tif', '.png']
     """
     extension = _get_extension(path)
-    if extension == '.raw' or extension == '.png':
-        # TODO: get raw writing to work
-        # raw.raw_imsave(path, img)
-        tifffile.imsave(os.path.splitext(path)[0]+'.tiff', img, compress=compression)
-    elif extension == '.tif' or extension == '.tiff':
-        tifffile.imsave(path, img, compress=compression)
 
+    if output_format is None:
+        # Saving any input format to tiff
+        if extension == '.raw' or extension == '.png':
+            # TODO: get raw writing to work
+            # raw.raw_imsave(path, img)
+            tifffile.imsave(os.path.splitext(path)[0]+'.tiff', img, compress=compression) # Use with versions <= 2020.9.3
+            # tifffile.imsave(os.path.splitext(path)[0]+'.tiff', img, compressionargs={'level': compression}) # Use with version 2023.03.21
+
+        elif extension == '.tif' or extension == '.tiff':
+            tifffile.imsave(path, img, compress=compression) # Use with versions <= 2020.9.3
+            # tifffile.imsave(path, img, compressionargs={'level': compression}) # Use with version 2023.03.21
+
+    else:
+        # Saving output images based on the output format
+        if output_format not in supported_output_extensions:
+            raise ValueError(f"Output format {output_format} is not valid! Supported extensions are: {supported_output_extensions}")
+
+        filename = os.path.splitext(path)[0] + output_format
+        if output_format == '.tif' or output_format == '.tiff':
+            tifffile.imsave(filename, img, compress=compression) # Use with versions <= 2020.9.3
+            # tifffile.imsave(path, img, compressionargs={'level': compression}) # Use with version 2023.03.21
+        
+        elif output_format == '.png':
+            # print(img.dtype)
+            iio.imwrite(filename, img, compress_level=compression) # Works fine up to version 2.15.0
+            # iio.v3.imwrite(filename, img, compress_level=compression) # version 2.27.0
 
 def wavedec(img, wavelet, level=None):
     """Decompose `img` using discrete (decimated) wavelet transform using `wavelet`
 
     Parameters
     ----------
     img : ndarray
@@ -419,15 +444,16 @@
 
     if threshold == -1:
         try:
             threshold = threshold_otsu(img)
         except ValueError:
             threshold = 1
 
-    img = np.array(img, dtype=np.float)
+    img = np.array(img, dtype=float) # np.float deprecated in version 1.20
+
     #
     # Need to pad image to multiple of 2
     #
     pady, padx = [_ % 2 for _ in img.shape]
     if pady == 1 or padx == 1:
         img = np.pad(img, ((0, pady), (0, padx)), mode="edge")
 
@@ -490,15 +516,15 @@
                      crossover=10, threshold=-1, compression=1,
                      flat=None, dark=0, z_idx=None, rotate=False,
                      lightsheet=False,
                      artifact_length=150,
                      background_window_size=200,
                      percentile=.25,
                      lightsheet_vs_background=2.0,
-                     dont_convert_16bit=False):
+                     dont_convert_16bit=False, output_format=None):
 
     """Convenience wrapper around filter streaks. Takes in a path to an image rather than an image array
 
     Note that the directory being written to must already exist before calling this function
 
     Parameters
     ----------
@@ -536,14 +562,16 @@
         Look at this size window around the pixel in x and y
     percentile : float
         Take this percentile as background with lightsheet
     lightsheet_vs_background : float
         weighting factor to use background or lightsheet background
     dont_convert_16bit : bool
         Flag for converting to 16-bit
+    output_format: str
+        Desired output format [.png, .tiff, .tif]. Default None
     """
 
     n = 3
     for i in range(n):
         try:
             if z_idx is None:
                 # Path must be TIFF or RAW
@@ -591,15 +619,15 @@
             lightsheet_vs_background=lightsheet_vs_background
             ).reshape(img.shape[0], img.shape[1])
         if flat is not None:
             fimg = apply_flat(fimg, flat)
     # Save image, retry if OSError for NAS
     for _ in range(nb_retry):
         try:
-            imsave(str(output_path), fimg.astype(dtype), compression=compression)
+            imsave(str(output_path), fimg.astype(dtype), compression=compression, output_format=output_format)
         except OSError:
             print('Retrying...')
             continue
         break
 
 
 def _read_filter_save(input_dict):
@@ -673,15 +701,16 @@
 def batch_filter(input_path, output_path, workers, chunks, sigma, auto_mode, level=0, wavelet='db3', crossover=10,
                  threshold=-1, compression=1, flat=None, dark=0, zstep=None, rotate=False,
                  lightsheet=False,
                  artifact_length=150,
                  background_window_size=200,
                  percentile=.25,
                  lightsheet_vs_background=2.0,
-                 dont_convert_16bit=False
+                 dont_convert_16bit=False,
+                 output_format=None
                  ):
     """Applies `streak_filter` to all images in `input_path` and write the results to `output_path`.
 
     Parameters
     ----------
     input_path : Path
         root directory to search for images to filter
@@ -709,14 +738,16 @@
         Intensity to subtract from the images for dark offset. Default is 0.
     zstep : int
         Zstep in tenths of micron. only used for DCIMG files.
     rotate : bool
         Flag for 90 degree rotation.
     dont_convert_16bit : bool
         Flag for converting to 16-bit
+    output_format: str
+        Desired output format [.png, .tiff, .tif]. Default None
     """
 
     error_path = os.path.join(output_path, 'destripe_log.txt')
     if os.path.exists(error_path):
         os.remove(error_path)
 
     if workers == 0:
@@ -773,34 +804,31 @@
             'z_idx': z_idx,
             'rotate': rotate,
             'lightsheet': lightsheet,
             'artifact_length': artifact_length,
             'background_window_size': background_window_size,
             'percentile': percentile,
             'lightsheet_vs_background': lightsheet_vs_background,
-            'dont_convert_16bit' : dont_convert_16bit
+            'dont_convert_16bit' : dont_convert_16bit,
+            'output_format': output_format
         }
         args.append(arg_dict)
     print('Pystripe batch processing progress:')
     with multiprocessing.Pool(workers) as pool:
         if auto_mode:
             list(tqdm.tqdm(
                 pool.imap(_read_filter_save, args, chunksize=chunks), 
                 total=len(args), 
                 ascii=True,
                 bar_format='{l_bar}{bar:60}{r_bar}{bar:-10b}'))
         else:
             list(tqdm.tqdm(pool.imap(_read_filter_save, args, chunksize=chunks), total=len(args), ascii=True))
-
     
     print('Done!')
 
-
-        
-
     if os.path.exists(error_path):
         with open(error_path, 'r') as fp:
             first_line = fp.readline()
             images = fp.readlines()
             for image_path in images:
                 interpolate(image_path, input_path, output_path)
             x = len(images)
@@ -840,14 +868,15 @@
     parser.add_argument("--rotate", "-r", help="Rotate output images 90 degrees counter-clockwise", action='store_true')
     parser.add_argument("--lightsheet", help="Use the lightsheet method", action="store_true")
     parser.add_argument("--artifact-length", help="Look for minimum in lightsheet direction over this length", default=150, type=int)
     parser.add_argument("--background-window-size", help="Size of window in x and y for background estimation", default=200, type=int)
     parser.add_argument("--percentile", help="The percentile at which to measure the background", type=float, default=.25)
     parser.add_argument("--lightsheet-vs-background", help="The background is multiplied by this weight when comparing lightsheet against background", type=float, default=2.0)
     parser.add_argument("--dont-convert-16bit", help="Is the output converted to 16-bit .tiff or not", action="store_true")
+    parser.add_argument("--output_format", "-of", help="Desired format output for the images", type=str, required=False, default=None)
     args = parser.parse_args()
     return args
 
 
 def interpolate(image_path, input_path, output_path):
     # print('Interpolate:\nimage_path: {}\ninput_path: {}\noutput_path: {}\n'.format(image_path, input_path, output_path))
     rel_path = Path(image_path).relative_to(input_path)
@@ -873,36 +902,38 @@
             # print(closest_image)
     new_file_name = str(image_num) + os.path.splitext(closest_image['name'])[1]
     try:
         shutil.copyfile(os.path.join(o_dir, closest_image['name']), os.path.join(o_dir, new_file_name))
     except Exception as e:
         # print(e)
         pass
-    
-    
-    
-    
-    
+
 
 def main():
     args = _parse_args()
     sigma = [args.sigma1, args.sigma2]
     input_path = Path(args.input)
 
     flat = None
     if args.flat is not None:
         flat = normalize_flat(imread(args.flat))
 
     zstep = None
     if args.zstep is not None:
         zstep = int(args.zstep * 10)
 
+    if args.output_format not in ['.png', '.tif', '.tiff']:
+        raise ValueError("Custom output format not supported.")
+
     if args.dark < 0:
         raise ValueError('Only positive values for dark offset are allowed')
 
+    if args.output_format is not None and args.output_format not in supported_output_extensions:
+        raise ValueError(f"Output format {args.output_format} is currently not supported! Supported formats are: {supported_output_extensions}")
+
     if input_path.is_file():  # single image
         if input_path.suffix not in supported_extensions:
             print('Input file was found but is not supported. Exiting...')
             return
         if args.output == '':
             output_path = Path(input_path.parent).joinpath(input_path.stem+'_destriped'+input_path.suffix)
         else:
@@ -923,15 +954,16 @@
                          dark=args.dark,
                          rotate=args.rotate,  # Does not work on DCIMG files
                          lightsheet=args.lightsheet,
                          artifact_length=args.artifact_length,
                          background_window_size=args.background_window_size,
                          percentile=args.percentile,
                          lightsheet_vs_background=args.lightsheet_vs_background,
-                         dont_convert_16bit=args.dont_convert_16bit
+                         dont_convert_16bit=args.dont_convert_16bit,
+                         output_format=args.output_format
                          )
 
     elif input_path.is_dir():  # batch processing
         if args.output == '':
             output_path = Path(input_path.parent).joinpath(str(input_path)+'_destriped')
         else:
             output_path = Path(args.output)
@@ -952,15 +984,16 @@
                      zstep=zstep,
                      rotate=args.rotate,
                      lightsheet=args.lightsheet,
                      artifact_length=args.artifact_length,
                      background_window_size=args.background_window_size,
                      percentile=args.percentile,
                      lightsheet_vs_background=args.lightsheet_vs_background,
-                     dont_convert_16bit=args.dont_convert_16bit
+                     dont_convert_16bit=args.dont_convert_16bit,
+                     output_format=args.output_format
                      )
     else:
         print('Cannot find input file or directory. Exiting...')
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pystripe-1.2.2/pystripe/lightsheet_correct.py` & `pystripe-1.2.3/pystripe/lightsheet_correct.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.2/pystripe/raw.py` & `pystripe-1.2.3/pystripe/raw.py`

 * *Files identical despite different names*

### Comparing `pystripe-1.2.2/pystripe.egg-info/PKG-INFO` & `pystripe-1.2.3/pystripe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystripe
-Version: 1.2.2
+Version: 1.2.3
 Summary: Stripe artifact filtering for SPIM images
 Home-page: https://github.com/LifeCanvas-Technologies/pystripe
 Author: LifeCanvas Technologies
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystripe-1.2.2/setup.py` & `pystripe-1.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
-version = "1.2.2"
+version = "1.2.3"
 
 with open("./README.md") as fd:
     long_description = fd.read()
 
 setup(
     name="pystripe",
     version=version,
     description=
     "Stripe artifact filtering for SPIM images",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        "numpy",
-        "scipy",
-        "scikit-image",
-        "tifffile",
-        "PyWavelets",
-        "tqdm",
-        "pathlib2",
-        "dcimg"
+        "numpy==1.19.5",
+        "scipy==1.5.4",
+        "scikit-image==0.17.2",
+        "tifffile==2020.9.3",
+        "PyWavelets==1.1.1",
+        "tqdm==4.64.1",
+        "pathlib2==2.3.7.post1",
+        "dcimg==0.6.0.post1"
     ],
     author="LifeCanvas Technologies",
     packages=["pystripe"],
     entry_points={ 'console_scripts': [
         'pystripe=pystripe.core:main',
     ]},
     url="https://github.com/LifeCanvas-Technologies/pystripe",
```

