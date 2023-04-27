# Comparing `tmp/ms-mint-0.2.2.tar.gz` & `tmp/ms-mint-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-0.2.2.tar", last modified: Thu Mar  9 21:57:22 2023, max compression
+gzip compressed data, was "ms-mint-0.2.3.tar", last modified: Thu Apr 27 15:30:19 2023, max compression
```

## Comparing `ms-mint-0.2.2.tar` & `ms-mint-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 21:57:22.282462 ms-mint-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-03-09 21:57:11.000000 ms-mint-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-09 21:57:11.000000 ms-mint-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-03-09 21:57:22.282462 ms-mint-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-03-09 21:57:11.000000 ms-mint-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 21:57:22.282462 ms-mint-0.2.2/ms_mint/
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-09 21:57:22.282462 ms-mint-0.2.2/ms_mint/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/matplotlib_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/plotly_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-03-09 21:57:11.000000 ms-mint-0.2.2/ms_mint/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 21:57:22.282462 ms-mint-0.2.2/ms_mint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-03-09 21:57:22.000000 ms-mint-0.2.2/ms_mint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-09 21:57:22.000000 ms-mint-0.2.2/ms_mint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 21:57:22.000000 ms-mint-0.2.2/ms_mint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-09 21:57:22.000000 ms-mint-0.2.2/ms_mint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 21:57:22.000000 ms-mint-0.2.2/ms_mint.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      425 2023-03-09 21:57:22.282462 ms-mint-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1248 2023-03-09 21:57:11.000000 ms-mint-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-03-09 21:57:12.000000 ms-mint-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:30:19.840465 ms-mint-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-04-27 15:29:56.000000 ms-mint-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 15:29:56.000000 ms-mint-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-27 15:30:19.840465 ms-mint-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-04-27 15:29:56.000000 ms-mint-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:30:19.840465 ms-mint-0.2.3/ms_mint/
+-rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 15:30:19.840465 ms-mint-0.2.3/ms_mint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/matplotlib_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/plotly_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:30:19.840465 ms-mint-0.2.3/ms_mint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-04-27 15:30:19.840465 ms-mint-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1248 2023-04-27 15:29:56.000000 ms-mint-0.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-04-27 15:29:56.000000 ms-mint-0.2.3/versioneer.py
```

### Comparing `ms-mint-0.2.2/LICENSE` & `ms-mint-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.2/PKG-INFO` & `ms-mint-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.2
+Version: 0.2.3
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,27 +22,27 @@
 The `ms-mint` library is a tool designed to assist with targeted metabolomics studies, which involves the systematic analysis of small chemical compounds called metabolites that are present in biological samples. These metabolites can provide valuable information about the state of an organism, including indicators of disease or other physiological changes. In order to perform a targeted metabolomics study, researchers typically use liquid chromatography-mass spectrometry (LCMS) to identify and quantify specific metabolites of interest.
 
 The `ms-mint` library includes a range of functions for processing LCMS data from targeted metabolomics experiments, and it is particularly well-suited for handling large amounts of data (10,000+ files). To use `ms-mint`, you provide it with a target list of the specific metabolites you want to analyze, as well as the names of the mass spectrometry files containing the data. ms-mint then extracts peak intensities and other relevant information from the data, allowing you to gain insights into the concentrations and profiles of the metabolites in your samples. This information can be used to identify biomarkers, which are indicators of disease or other physiological changes that can be used in the development of diagnostic tests or other medical applications.
 
 ## Documentation
 The code documentation can be accessed [here](https://lewisresearchgroup.github.io/ms-mint/readme.html).
 
-## News
+## ms-mint application with graphical user iterface (GUI)
 MINT has been split into the Python library and the app. This repository contains the Python library. For the app follow [this link](https://github.com/LewisResearchGroup/ms-mint-app).
 
 ## Contributions
 All contributions, bug reports, code reviews, bug fixes, documentation improvements, enhancements, and ideas are welcome.
 Before you modify the code please reach out to us using the [issues](https://github.com/LewisResearchGroup/ms-mint/issues) page.
 
 ## Code standards
 The project follows PEP8 standard and uses Black and Flake8 to ensure a consistent code format throughout the project.
 
 ---
 
-# Usage
+## Usage
 
 To use the main class of the ms-mint library, you can import it into your code with the following command:
 
     from ms_mint.Mint import Mint
 
 This will import a lightweight version of the class with the essential functionality. If you want to use the ms-mint tool interactively in a Jupyter Notebook or JupyterLab, you can import the class with the following command:
 
@@ -155,28 +155,26 @@
     mint.run()
     mint.plot.peak_shapes(col_wrap=3)
 
 ![](notebooks/peak-shapes-after-opt.png)
 
 As you can see, the shapes of Xanthine, Succinate, Citrulline look much better.
 
-
 ## Plotting and data exploration
 
 The `Mint` class has a few convenient methods to visualize and explore the processed data. The results can be viewed directly in JupyterLab or stored to files using `matplotlib` and `seaborn` syntax. The figures are matplotlib objects and can be easily customised. 
 
 ## Plot peak shapes
 
 ![](notebooks/peak-shapes-after-opt.png)
 
     mint.plot.peak_shapes(col_wrap = 3)
 
 The method uses seaborn [sns.relplot()](https://seaborn.pydata.org/generated/seaborn.relplot.html) function and keyword arguments are passed on. 
 
-
 ## Hierarchical clustering
 Mint ca be used to cluster the extracted data. An agglomerative hierarchical clustering is a bottom-up clustering technique where each data point starts as its own cluster and then are merged with other clusters in a hierarchical manner based on their proximity or similarity until a single cluster is formed or a specified stopping criteria is met. The proximity is usually determined by a distance metric, such as Euclidean distance, and the similarity is usually determined by a linkage function, such as ward linkage or complete linkage. The result is a tree-like representation called a dendrogram, which can be used to determine the number of clusters and the cluster assignments of the data points.
 
 Mint uses `scipy.spartial.distance` to generate the distance matrix and `scipy.cluster.hierarchy.linkage` to perform the clustering. By default a 'cosine' metric is used to calculate the distances. Distances between row vectors and column vectors respectively can also be done using different metrics for each set. To do so a tuple with the names of the metrics has to be provided: `mint.hierarchical_clustering(metric=("euclidean", "cosine")`.
 
 Before clustering the data can be transformed and scaled. By default `log2p1(x) = log_2(x+1)` is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
 
@@ -198,15 +196,14 @@
         transform_filenames_func="basename",  # Transformation function to shorten filenames
         transposed=False,  # Transpose the plot     
         top_height=2,  # Height of the top-dendrogram
         left_width=2,  # Width of the left-dendrogram
         cmap=None  # Name of a matplotlib color map                
     )
 
-
 ![](notebooks/hierarchical_clustering.png)
 
 ## Principal Components Analysis
 
 Principal Component Analysis (PCA) is a widely used statistical technique for dimensionality reduction. It transforms the original high-dimensional data into a new set of linearly uncorrelated variables, called Principal Components (PCs), that capture the maximum variance in the data. The first PC accounts for the largest variance in the data, the second PC for the second largest variance, and so on. PCA is commonly used for data visualization, data compression, and noise reduction. By reducing the number of dimensions in the data, PCA allows us to more easily identify patterns and relationships in the data.
 
 Before clustering the data can be transformed and scaled. By default log2p1(x) = log_2(x+1) is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
@@ -215,49 +212,49 @@
     
 After running the PCA the results can be plotted with:    
     
     mint.pca.plot.pairplot(n_components=5, interactive=False)
     
 ![](notebooks/pca-pairplot.png)
 
-# FAQ
-## What is a target list
+## FAQ
+### What is a target list
 A target list is a pandas dataframe with specific columns. 
 
 -   **peak_label**: string, Label of the peak (must be unique).
 -   **mz_mean**: numeric value, theoretical m/z value of the target ion to extract.
 -   **mz_width**: numeric value, width of the peak in \[ppm\]. It is used to calculate the width of the mass window  according to the formula: `Δm = m/z * 1e-6 * mz_width`.
 -   **rt**: numeric value, (optional), expected time of the peak. This value is not used during processing, but it can inform the peak optimization procedure.
 -   **rt_min**: numeric value, starting time for peak integration.
 -   **rt_max**: numeric value, ending time for peak integration.
 -   **rt_unit**: one of `s` or `min` for seconds or minutes respectively.
 -   **intensity_threshold**: numeric value (>=0), minimum intensity value to include, serves as a noise filter. We recommend setting this to 0. 
 -   **target_filename**: string (optional), name of the target list file. It is not used for processing, just to keep track of what files were used.
 
 The target list can be stored as csv or Excel file. 
 
-## What input files can be used
+### What input files can be used
 `ms_mint` can be used with `mzXML`, `mzML`, `mzMLb` and experimental formats in `.feather` and `.parquet` format.
 
-## Which properties does ms-mint extract
-### Parameters from target list
+### Which properties does ms-mint extract
+#### Parameters from target list
 -   **ms_file**: Filename of MS-file
 -   **peak_label**: From target list
 -   **mz_mean**: From target list
 -   **mz_width**: From target list
 -   **rt**: From target list
 -   **rt_min**: From target list
 -   **rt_max**: From target list
 -   **rt_unit**: Unit of retention times, default is s (seconds), from [s, min]
 -   **intensity_threshold**: From target list
 -   **target_filename**: From target list
 
 ---
 
-### Results columns
+#### Results columns
 -   **peak_area**: The sum of all intensities in the extraction window
 -   **peak_area_top3**: The average of the 3 largest intensities in the extraction window
 -   **peak_n_datapoints**: Number of datapoints
 -   **peak_max**: Intensity of peak maximum
 -   **peak_rt_of_max**: Retentiontime of peak maximum
 -   **peak_min**: Minimum peak intensity (offset)
 -   **peak_median**: Median of all intensities 
@@ -270,13 +267,11 @@
 -   **peak_mass_diff_75pc**: 75th percentile between *mz_mean* minus m/z values of all datapoints
 -   **peak_score**: Score of peak quality (experimental)
 -   **total_intensity**: Sum of all intensities in the file
 -   **ms_path**: Path of the MS-file
 -   **ms_file_size**: Size of the MS-file in MB
 ---
 
+## Release Notes
 
-# Release Notes
-
-## 0.2.0 Milestones
+### 0.2.0 Milestones
     - peak_area_top3 comparable to El-Maven PeakAreaTop values
-
```

### Comparing `ms-mint-0.2.2/README.md` & `ms-mint-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 The `ms-mint` library is a tool designed to assist with targeted metabolomics studies, which involves the systematic analysis of small chemical compounds called metabolites that are present in biological samples. These metabolites can provide valuable information about the state of an organism, including indicators of disease or other physiological changes. In order to perform a targeted metabolomics study, researchers typically use liquid chromatography-mass spectrometry (LCMS) to identify and quantify specific metabolites of interest.
 
 The `ms-mint` library includes a range of functions for processing LCMS data from targeted metabolomics experiments, and it is particularly well-suited for handling large amounts of data (10,000+ files). To use `ms-mint`, you provide it with a target list of the specific metabolites you want to analyze, as well as the names of the mass spectrometry files containing the data. ms-mint then extracts peak intensities and other relevant information from the data, allowing you to gain insights into the concentrations and profiles of the metabolites in your samples. This information can be used to identify biomarkers, which are indicators of disease or other physiological changes that can be used in the development of diagnostic tests or other medical applications.
 
 ## Documentation
 The code documentation can be accessed [here](https://lewisresearchgroup.github.io/ms-mint/readme.html).
 
-## News
+## ms-mint application with graphical user iterface (GUI)
 MINT has been split into the Python library and the app. This repository contains the Python library. For the app follow [this link](https://github.com/LewisResearchGroup/ms-mint-app).
 
 ## Contributions
 All contributions, bug reports, code reviews, bug fixes, documentation improvements, enhancements, and ideas are welcome.
 Before you modify the code please reach out to us using the [issues](https://github.com/LewisResearchGroup/ms-mint/issues) page.
 
 ## Code standards
 The project follows PEP8 standard and uses Black and Flake8 to ensure a consistent code format throughout the project.
 
 ---
 
-# Usage
+## Usage
 
 To use the main class of the ms-mint library, you can import it into your code with the following command:
 
     from ms_mint.Mint import Mint
 
 This will import a lightweight version of the class with the essential functionality. If you want to use the ms-mint tool interactively in a Jupyter Notebook or JupyterLab, you can import the class with the following command:
 
@@ -141,28 +141,26 @@
     mint.run()
     mint.plot.peak_shapes(col_wrap=3)
 
 ![](notebooks/peak-shapes-after-opt.png)
 
 As you can see, the shapes of Xanthine, Succinate, Citrulline look much better.
 
-
 ## Plotting and data exploration
 
 The `Mint` class has a few convenient methods to visualize and explore the processed data. The results can be viewed directly in JupyterLab or stored to files using `matplotlib` and `seaborn` syntax. The figures are matplotlib objects and can be easily customised. 
 
 ## Plot peak shapes
 
 ![](notebooks/peak-shapes-after-opt.png)
 
     mint.plot.peak_shapes(col_wrap = 3)
 
 The method uses seaborn [sns.relplot()](https://seaborn.pydata.org/generated/seaborn.relplot.html) function and keyword arguments are passed on. 
 
-
 ## Hierarchical clustering
 Mint ca be used to cluster the extracted data. An agglomerative hierarchical clustering is a bottom-up clustering technique where each data point starts as its own cluster and then are merged with other clusters in a hierarchical manner based on their proximity or similarity until a single cluster is formed or a specified stopping criteria is met. The proximity is usually determined by a distance metric, such as Euclidean distance, and the similarity is usually determined by a linkage function, such as ward linkage or complete linkage. The result is a tree-like representation called a dendrogram, which can be used to determine the number of clusters and the cluster assignments of the data points.
 
 Mint uses `scipy.spartial.distance` to generate the distance matrix and `scipy.cluster.hierarchy.linkage` to perform the clustering. By default a 'cosine' metric is used to calculate the distances. Distances between row vectors and column vectors respectively can also be done using different metrics for each set. To do so a tuple with the names of the metrics has to be provided: `mint.hierarchical_clustering(metric=("euclidean", "cosine")`.
 
 Before clustering the data can be transformed and scaled. By default `log2p1(x) = log_2(x+1)` is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
 
@@ -184,15 +182,14 @@
         transform_filenames_func="basename",  # Transformation function to shorten filenames
         transposed=False,  # Transpose the plot     
         top_height=2,  # Height of the top-dendrogram
         left_width=2,  # Width of the left-dendrogram
         cmap=None  # Name of a matplotlib color map                
     )
 
-
 ![](notebooks/hierarchical_clustering.png)
 
 ## Principal Components Analysis
 
 Principal Component Analysis (PCA) is a widely used statistical technique for dimensionality reduction. It transforms the original high-dimensional data into a new set of linearly uncorrelated variables, called Principal Components (PCs), that capture the maximum variance in the data. The first PC accounts for the largest variance in the data, the second PC for the second largest variance, and so on. PCA is commonly used for data visualization, data compression, and noise reduction. By reducing the number of dimensions in the data, PCA allows us to more easily identify patterns and relationships in the data.
 
 Before clustering the data can be transformed and scaled. By default log2p1(x) = log_2(x+1) is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
@@ -201,49 +198,49 @@
     
 After running the PCA the results can be plotted with:    
     
     mint.pca.plot.pairplot(n_components=5, interactive=False)
     
 ![](notebooks/pca-pairplot.png)
 
-# FAQ
-## What is a target list
+## FAQ
+### What is a target list
 A target list is a pandas dataframe with specific columns. 
 
 -   **peak_label**: string, Label of the peak (must be unique).
 -   **mz_mean**: numeric value, theoretical m/z value of the target ion to extract.
 -   **mz_width**: numeric value, width of the peak in \[ppm\]. It is used to calculate the width of the mass window  according to the formula: `Δm = m/z * 1e-6 * mz_width`.
 -   **rt**: numeric value, (optional), expected time of the peak. This value is not used during processing, but it can inform the peak optimization procedure.
 -   **rt_min**: numeric value, starting time for peak integration.
 -   **rt_max**: numeric value, ending time for peak integration.
 -   **rt_unit**: one of `s` or `min` for seconds or minutes respectively.
 -   **intensity_threshold**: numeric value (>=0), minimum intensity value to include, serves as a noise filter. We recommend setting this to 0. 
 -   **target_filename**: string (optional), name of the target list file. It is not used for processing, just to keep track of what files were used.
 
 The target list can be stored as csv or Excel file. 
 
-## What input files can be used
+### What input files can be used
 `ms_mint` can be used with `mzXML`, `mzML`, `mzMLb` and experimental formats in `.feather` and `.parquet` format.
 
-## Which properties does ms-mint extract
-### Parameters from target list
+### Which properties does ms-mint extract
+#### Parameters from target list
 -   **ms_file**: Filename of MS-file
 -   **peak_label**: From target list
 -   **mz_mean**: From target list
 -   **mz_width**: From target list
 -   **rt**: From target list
 -   **rt_min**: From target list
 -   **rt_max**: From target list
 -   **rt_unit**: Unit of retention times, default is s (seconds), from [s, min]
 -   **intensity_threshold**: From target list
 -   **target_filename**: From target list
 
 ---
 
-### Results columns
+#### Results columns
 -   **peak_area**: The sum of all intensities in the extraction window
 -   **peak_area_top3**: The average of the 3 largest intensities in the extraction window
 -   **peak_n_datapoints**: Number of datapoints
 -   **peak_max**: Intensity of peak maximum
 -   **peak_rt_of_max**: Retentiontime of peak maximum
 -   **peak_min**: Minimum peak intensity (offset)
 -   **peak_median**: Median of all intensities 
@@ -256,13 +253,11 @@
 -   **peak_mass_diff_75pc**: 75th percentile between *mz_mean* minus m/z values of all datapoints
 -   **peak_score**: Score of peak quality (experimental)
 -   **total_intensity**: Sum of all intensities in the file
 -   **ms_path**: Path of the MS-file
 -   **ms_file_size**: Size of the MS-file in MB
 ---
 
+## Release Notes
 
-# Release Notes
-
-## 0.2.0 Milestones
+### 0.2.0 Milestones
     - peak_area_top3 comparable to El-Maven PeakAreaTop values
-
```

### Comparing `ms-mint-0.2.2/ms_mint/Mint.py` & `ms-mint-0.2.3/ms_mint/Mint.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     is_ms_file,
     get_ms_files_from_results,
     get_targets_from_results,
     scale_dataframe,
 )
 from .pca import PrincipalComponentsAnalyser
 from .plotting import MintPlotter
-#from .filter import Resampler
+
+# from .filter import Resampler
 from .chromatogram import Chromatogram, extract_chromatogram_from_ms1
 
 import ms_mint
 
 from tqdm import tqdm
 
 from typing import Callable
@@ -41,47 +42,33 @@
     :type verbose: bool
 
     :param progress_callback: A callback for a progress bar.
     :type progress_callback: Callable[]
 
     """
 
-    def __init__(self, verbose: bool = False, progress_callback=None, time_unit="s"):
-
-        self._verbose = verbose
+    def __init__(
+        self,
+        verbose: bool = False,
+        progress_callback: Callable = None,
+        time_unit: str = "s",
+    ):
+        self.verbose = verbose
         self._version = ms_mint.__version__
-        self._progress_callback = progress_callback
+        self.progress_callback = progress_callback
         self.reset()
         if self.verbose:
             print("Mint Version:", self.version, "\n")
         self.plot = MintPlotter(mint=self)
         self.opt = TargetOptimizer(mint=self)
         self.pca = PrincipalComponentsAnalyser(self)
         self.tqdm = tqdm
         self.meta = None
 
     @property
-    def verbose(self):
-        """
-        Get/set verbosity.
-
-        :getter: Get current verbosity.
-        :return: True or False
-        :rtype: bool
-        :setter: Sets verbosity.
-        :param value: True or False
-        :type value: bool
-        """
-        return self._verbose
-
-    @verbose.setter
-    def verbose(self, value: bool):
-        self._verbose = value
-
-    @property
     def version(self):
         """
         ms-mint version number.
 
         :return: Version string.
         :rtype: str
         """
@@ -129,78 +116,92 @@
 
         :param nthreads: Number of cores to use, defaults to None
         :type nthreads: int
                 * None - Run with min(n_cpus, c_files) CPUs
                 * 1: Run without multiprocessing on one CPU
                 * >1: Run with multiprocessing enabled using nthreads threads.
         :param mode: Compute mode ('standard' or 'express'), defaults to 'standard'
+        :type mode: str
                 * 'standard': calculates peak shaped projected to RT dimension
                 * 'express': omits calculation of other features, only peak_areas
         :param fn: Output filename to not keep results in memory.
         :type fn: str
-        :type mode: str
         :param kwargs: Arguments passed to the procesing function.
         """
         self._status = "running"
 
         if (self.n_files == 0) or (len(self.targets) == 0):
             return None
 
         targets = self.targets.reset_index()
+        self._set_rt_min_max(targets, rt_margin)
 
-        if "rt" in targets.columns:
-            ndx = (targets.rt_min.isna()) & (~targets.rt.isna())
-            targets.loc[ndx, "rt_min"] = targets.loc[ndx, "rt"] - rt_margin
-            ndx = (targets.rt_max.isna()) & (~targets.rt.isna())
-            targets.loc[ndx, "rt_max"] = targets.loc[ndx, "rt"] + rt_margin
-            del ndx
-
-        if nthreads is None:
-            nthreads = min(cpu_count(), self.n_files)
+        nthreads = self._determine_nthreads(nthreads)
 
         if self.verbose:
             print(f"Run MINT with {nthreads} processes:")
 
         start = time.time()
         if nthreads > 1:
-            self.__run_parallel__(nthreads=nthreads, mode=mode, fn=fn, **kwargs)
+            self._run_parallel(nthreads=nthreads, mode=mode, fn=fn, **kwargs)
         else:
-            results = []
-            for i, filename in enumerate(self.ms_files):
-                args = {
-                    "filename": filename,
-                    "targets": targets,
-                    "q": None,
-                    "mode": mode,
-                    "output_fn": None,
-                }
-                results.append(process_ms1_files_in_parallel(args))
-                self.progress = int(100 * (i / self.n_files))
-            self.results = pd.concat(results).reset_index(drop=True)
+            self._run_sequential(mode=mode, fn=fn, targets=targets)
 
         self.progress = 100
+        self._report_runtime(start)
 
+        self._status = "done"
+        assert self.progress == 100
+        return self
+
+    def _set_rt_min_max(self, targets, rt_margin):
+        if "rt" in targets.columns:
+            update_rt_min = (targets.rt_min.isna()) & (~targets.rt.isna())
+            targets.loc[update_rt_min, "rt_min"] = (
+                targets.loc[update_rt_min, "rt"] - rt_margin
+            )
+            update_rt_max = (targets.rt_max.isna()) & (~targets.rt.isna())
+            targets.loc[update_rt_max, "rt_max"] = (
+                targets.loc[update_rt_max, "rt"] + rt_margin
+            )
+
+    def _determine_nthreads(self, nthreads):
+        if nthreads is None:
+            nthreads = min(cpu_count(), self.n_files)
+        return nthreads
+
+    def _run_sequential(self, mode, fn, targets):
+        results = []
+        for i, filename in enumerate(self.ms_files):
+            args = {
+                "filename": filename,
+                "targets": targets,
+                "q": None,
+                "mode": mode,
+                "output_fn": None,
+            }
+            results.append(process_ms1_files_in_parallel(args))
+            self.progress = int(100 * (i / self.n_files))
+        self.results = pd.concat(results).reset_index(drop=True)
+
+    def _report_runtime(self, start):
         end = time.time()
         self.runtime = end - start
         self.runtime_per_file = self.runtime / self.n_files
         self.runtime_per_peak = self.runtime / self.n_files / len(self.targets)
 
         if self.verbose:
             print(f"Total runtime: {self.runtime:.2f}s")
             print(f"Runtime per file: {self.runtime_per_file:.2f}s")
             print(
                 f"Runtime per peak ({len(self.targets)}): {self.runtime_per_peak:.2f}s\n"
             )
             print("Results:", self.results)
 
-        self._status = "done"
-        assert self.progress == 100
-        return self
-
-    def __run_parallel__(
+    def _run_parallel(
         self, nthreads=1, mode="standard", maxtasksperchild=None, fn=None
     ):
         print(f"maxtasksperchild: {maxtasksperchild}")
         pool = Pool(processes=nthreads, maxtasksperchild=maxtasksperchild)
         m = Manager()
         q = m.Queue()
         args = []
@@ -217,33 +218,30 @@
                     "queue": q,
                     "mode": mode,
                     "output_fn": fn,
                 }
             )
 
         results = pool.map_async(process_ms1_files_in_parallel, args)
-
-        # monitor progress
-        while True:
-            if results.ready():
-                break
-            else:
-                size = q.qsize()
-                self.progress = 100 * size / self.n_files
-                time.sleep(1)
-
-        self.progress = 100
+        self._monitor_progress(results, q)
 
         pool.close()
         pool.join()
 
         if fn is None:
             results = results.get()
             self.results = pd.concat(results).reset_index(drop=True)
 
+    def _monitor_progress(self, results, q):
+        while not results.ready():
+            size = q.qsize()
+            self.progress = 100 * size / self.n_files
+            time.sleep(1)
+        self.progress = 100
+
     @property
     def status(self):
         """
         Returns current status of Mint instance.
 
         :return: ['waiting', 'running', 'done']
         :rtype: str
@@ -395,28 +393,14 @@
         if apply:
             df = df.apply(apply)
         if scaler:
             df = scale_dataframe(df, scaler=scaler)
         return df
 
     @property
-    def progress_callback(self):
-        """
-        Assigns a callback function to update a progress bar.
-
-        :getter: Returns the current callback function.
-        :setter: Sets the callback function.
-        """
-        return self._progress_callback
-
-    @progress_callback.setter
-    def progress_callback(self, func: Callable = None):
-        self._progress_callback = func
-
-    @property
     def progress(self):
         """
         Shows the current progress.
 
         :getter: Returns the current progress value.
         :setter: Set the progress to a value between 0 and 100 and calls the progress callback function.
         """
@@ -497,15 +481,15 @@
         if not isinstance(fns, list):
             fns = [fns]
 
         if peak_label is None:
             peak_label = self.peak_labels
 
         data = []
-        
+
         for fn in self.tqdm(fns):
             df = ms_file_to_df(fn)
             for label in peak_label:
                 mz_mean, mz_width, rt_min, rt_max = self.get_target_params(label)
                 chrom_raw = extract_chromatogram_from_ms1(
                     df, mz_mean=mz_mean, mz_width=mz_width
                 ).to_frame()
@@ -513,14 +497,14 @@
                     continue
                 chrom = Chromatogram(chrom_raw.index, chrom_raw.values)
                 chrom.apply_filter()
                 chrom_data = chrom.data
                 chrom_data["ms_file"] = fn
                 chrom_data["peak_label"] = label
                 chrom_data["rt_min"] = rt_min
-                chrom_data["rt_max"] = rt_min
+                chrom_data["rt_max"] = rt_max
                 data.append(chrom_data)
 
         data = pd.concat(data).reset_index()
 
         data["ms_file"] = data["ms_file"].apply(lambda x: P(x).with_suffix("").name)
         return data
```

### Comparing `ms-mint-0.2.2/ms_mint/chromatogram.py` & `ms-mint-0.2.3/ms_mint/chromatogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import pandas as pd
 import logging
 
 from matplotlib import pyplot as plt
 
 from .tools import find_peaks_in_timeseries, gaussian, mz_mean_width_to_min_max
 from .io import ms_file_to_df
-from .filter import Resampler, Smoother, GaussFilter
+from .filters import Resampler, Smoother, GaussFilter
 from .matplotlib_tools import plot_peaks
 
 
 class Chromatogram:
     def __init__(
-        self, scan_times=None, intensities=None, filter=None, expected_rt=None
+        self, scan_times=None, intensities=None, filters=None, expected_rt=None
     ):
         self.t = np.array([0])
         self.x = np.array([0])
         if scan_times is not None:
             self.t = np.append(self.t, scan_times)
         if intensities is not None:
             self.x = np.append(self.x, intensities)
         self.noise_level = None
-        if filter is None:
-            self.filter = [Resampler(), GaussFilter(), Smoother()]
+        if filters is None:
+            self.filters = [Resampler(), GaussFilter(), Smoother()]
         else:
-            self.filter = filter
+            self.filters = filters
         self.peaks = None
         self.selected_peak_ndxs = None
         if expected_rt is None and scan_times is not None:
             expected_rt = max(scan_times) // 2
         self.expected_rt = expected_rt
         self.weights = None
 
@@ -39,16 +39,16 @@
         if expected_rt is not None:
             self.expected_rt = expected_rt
 
     def estimate_noise_level(self, window=20):
         data = pd.Series(index=self.t, data=self.x)
         self.noise_level = data.rolling(window, center=True).std().median()
 
-    def apply_filter(self):
-        for filt in self.filter:
+    def apply_filters(self):
+        for filt in self.filters:
             self.t, self.x = filt.transform(self.t, self.x)
 
     def find_peaks(self, prominence=None, rel_height=0.9):
         self.estimate_noise_level()
         if prominence is None:
             prominence = self.noise_level * 3
         self.peaks = find_peaks_in_timeseries(
@@ -76,15 +76,14 @@
         peak_endings = find_peaks_in_timeseries(
             -diff.fillna(0).intensity, prominence=prominence, plot=plot
         )
         if plot:
             plt.show()
 
         for ndx, row in peaks.iterrows():
-
             new_rt_min = row.rt_min
             new_rt_max = row.rt_max
 
             candidates_rt_min = peak_startings[peak_startings.rt <= new_rt_min]
             candidates_rt_max = peak_endings[peak_endings.rt >= new_rt_max]
 
             if len(candidates_rt_min) > 0:
@@ -126,15 +125,15 @@
         self.weights = max(peaks.peak_height) * gaussian(x, expected_rt, sigma)
         selected_ndx = weighted_peaks.sort_values(ascending=False).index.values[0]
         self.selected_peak_ndxs = [selected_ndx]
         return self.selected_peaks
 
     @property
     def selected_peaks(self):
-        self.peaks.loc[self.selected_peak_ndxs]
+        return self.peaks.loc[self.selected_peak_ndxs]
 
     @property
     def data(self):
         df = pd.DataFrame(index=self.t, data={"intensity": self.x})
         df.index.name = "scan_time"
         return df
```

### Comparing `ms-mint-0.2.2/ms_mint/filelock.py` & `ms-mint-0.2.3/ms_mint/filelock.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,14 @@
     msvcrt = None
 
 try:
     import fcntl
 except ImportError:
     fcntl = None
 
-
-# Backward compatibility
-# ------------------------------------------------
-try:
-    TimeoutError
-except NameError:
-    TimeoutError = OSError
-
-
 # Data
 # ------------------------------------------------
 __all__ = [
     "Timeout",
     "BaseFileLock",
     "WindowsFileLock",
     "UnixFileLock",
@@ -101,14 +92,15 @@
         temp = "The file lock '{}' could not be acquired.".format(self.lock_file)
         return temp
 
 
 # Classes
 # ------------------------------------------------
 
+
 # This is a helper class which is returned by :meth:`BaseFileLock.acquire`
 # and wraps the lock to make sure __enter__ is not called twice when entering
 # the with statement.
 # If we would simply return *self*, the lock would be acquired again
 # in the *__enter__* method of the BaseFileLock, but not released again
 # automatically.
 #
@@ -306,15 +298,14 @@
         Also note, that the lock file itself is not automatically deleted.
 
         :arg bool force:
             If true, the lock counter is ignored and the lock is released in
             every case.
         """
         with self._thread_lock:
-
             if self.is_locked:
                 self._lock_counter -= 1
 
                 if self._lock_counter == 0 or force:
                     lock_id = id(self)
                     lock_filename = self._lock_file
```

### Comparing `ms-mint-0.2.2/ms_mint/filter.py` & `ms-mint-0.2.3/ms_mint/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,25 @@
 class Smoother:
     """
     Filter for time series that smoothes the
     x values by running one or more rolling
     averages.
     """
 
-    def __init__(self, windows=[30, 20]):
+    def __init__(self, windows=None):
         """
         Filter for time series that smoothes the
         x values by running one or more rolling
         averages.
 
         :param windows: Window sizes of rolling averages applied to time series, defaults to [30, 20]
         :type windows: : List[int], optional
         """
+        if windows is None:
+            windows = [30, 20]
         self.windows = windows
         self.name = "smoother"
 
     def transform(self, t, x):
         """
         Transformation method.
```

### Comparing `ms-mint-0.2.2/ms_mint/io.py` & `ms-mint-0.2.3/ms_mint/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 Funtions to read and write MINT files.
 """
 
 import pandas as pd
 import numpy as np
 import io
 import logging
-import pymzml
+
+import pathlib
+from typing import Union, Optional
 
 from pathlib import Path as P
 from datetime import date
 from pyteomics import mzxml, mzml
 
 try:
     from pyteomics import mzmlb
@@ -27,234 +29,205 @@
     "polarity",
     "scan_time",
     "mz",
     "intensity",
 ]
 
 
-def ms_file_to_df(fn, read_only: bool = False, time_unit="seconds"):
+def ms_file_to_df(fn, read_only: bool = False):
     """
     Read MS file and convert it to a pandas.DataFrame.
 
     :param fn: Filename
     :type fn: str or PosixPath
     :param read_only: Whether or not to apply convert to dataframe (for testing purposes), defaults to False
     :type read_only: bool, optional
-    :param time_unit: Time unit used in file, defaults to "seconds"
-    :type time_unit: str, ['seconds', 'minutes']
     :return: MS data as DataFrame
     :rtype: pandas.DataFrame
     """
 
-    assert time_unit in ["minutes", "seconds"]
     fn = str(fn)
 
     try:
         if fn.lower().endswith(".mzxml"):
             df = mzxml_to_df(fn, read_only=read_only)
         elif fn.lower().endswith(".mzml"):
-            df = mzml_to_df(fn, read_only=read_only, time_unit=time_unit)
+            df = mzml_to_df(fn, read_only=read_only)
         elif fn.lower().endswith("hdf"):
             df = pd.read_hdf(fn)
         elif fn.lower().endswith(".feather"):
             df = pd.read_feather(fn)
         elif fn.lower().endswith(".parquet"):
             df = read_parquet(fn, read_only=read_only)
         elif fn.lower().endswith(".mzmlb"):
             df = mzmlb_to_df__pyteomics(fn, read_only=read_only)
         else:
             logging.error(f"Cannot read file {fn} of type {type(fn)}")
     except IndexError as e:
         logging.warning(f"{e}: {fn}")
         return None
-    # Compatibility with old schema
     if not read_only:
+        # Compatibility with old schema
         df = df.rename(
             columns={
                 "retentionTime": "scan_time",
                 "intensity array": "intensity",
                 "m/z array": "mz",
             }
         )
+        # Set datatypes
+        set_dtypes(df)
+
+    # assert df.scan_id.dtype in [np.int32, np.int64], df.scan_id.dtype
+    # assert df.intensity.dtype == np.int64, df.intensity.dtype
+    # assert df.mz.dtype == np.float64, df.mz.dtype
+    # assert df.scan_time.dtype == np.float64, df.scan_time.dtype
+
     return df
 
 
-def mzxml_to_df(fn, read_only=False):
+def mzxml_to_df(
+    fn: Union[str, pathlib.Path],
+    read_only: bool = False,
+    time_unit_in_file: str = "min",
+) -> Optional[pd.DataFrame]:
     """
     Read mzXML file and convert it to pandas.DataFrame.
 
     :param fn: Filename
-    :type fn: str or PosixPath
+    :type fn: Union[str, pathlib.Path]
     :param read_only: Whether or not to convert to dataframe (for testing purposes), defaults to False
     :type read_only: bool, optional
+    :param time_unit_in_file: The time unit used in the mzXML file (either 'sec' or 'min'), defaults to 'min'
+    :type time_unit_in_file: str, optional
     :return: MS data
-    :rtype: pandas.DataFrame
+    :rtype: Optional[pd.DataFrame]
     """
 
+    assert str(fn).lower().endswith(".mzxml"), fn
+
     with mzxml.MzXML(fn) as ms_data:
         data = [x for x in ms_data]
 
     if read_only:
         return None
 
-    data = list(extract_mzxml(data))
-
-    df = (
-        pd.DataFrame.from_dict(data)
-        .set_index("retentionTime")
-        .apply(pd.Series.explode)
-        .reset_index()
-    )
-
-    df["retentionTime"] = df["retentionTime"].astype(np.float64) * 60.0
-    df["m/z array"] = df["m/z array"].astype(np.float64)
-    df["intensity array"] = df["intensity array"].astype(np.float64)
-
-    df = df.rename(
-        columns={
-            "num": "scan_id",
-            "msLevel": "ms_level",
-            "retentionTime": "scan_time",
-            "m/z array": "mz",
-            "intensity array": "intensity",
-        }
-    )
+    data = [_extract_mzxml(x) for x in data]
+    df = pd.json_normalize(data, sep="_")
 
-    df = df.reset_index(drop=True)
-    df = df[MS_FILE_COLUMNS]
-    return df
+    # Convert retention time to seconds
+    if time_unit_in_file == "min":
+        df["scan_time"] = df["scan_time"].astype(np.float64) * 60.0
+
+    df = df.explode(["mz", "intensity"])
+    set_dtypes(df)
+    return df.reset_index(drop=True)[MS_FILE_COLUMNS]
 
 
 def _extract_mzxml(data):
-    cols = [
-        "num",
-        "msLevel",
-        "polarity",
-        "retentionTime",
-        "m/z array",
-        "intensity array",
-    ]
-    return {c: data[c] for c in cols}
+    return {
+        "scan_id": data["num"],
+        "ms_level": data["msLevel"],
+        "polarity": data["polarity"],
+        "scan_time": data["retentionTime"],
+        "mz": np.array(data["m/z array"]),
+        "intensity": np.array(data["intensity array"]),
+    }
 
 
-extract_mzxml = np.vectorize(_extract_mzxml)
+def mzml_to_pandas_df_pyteomics(fn, **kwargs):
+    # warnings.warn("mzml_to_pandas_df_pyteomics() is deprecated use mzxml_to_df() instead", DeprecationWarning)
+    return mzml_to_df(fn, **kwargs)
 
 
-def mzml_to_pandas_df_pyteomics(fn, read_only=False):
+def mzml_to_df(fn, read_only=False):
     """
     Reads mzML file and returns a pandas.DataFrame
-    using the pyteomics library.
+    using the mzML library.
 
     :param fn: Filename
     :type fn: str or PosixPath
-    :param read_only: Whether or not to convert to dataframe, defaults to False
-    :type read_only: bool, optional
+    :param explode: Whether to explode the DataFrame, defaults to True
+    :type explode: bool, optional
     :return: MS data
     :rtype: pandas.DataFrame
     """
-    slices = []
-    with mzml.MzML(fn) as ms_data:
-
-        while True:
 
-            try:
-                data = ms_data.next()
-            except Exception as e:
-                logging.warning(e)
-                break
+    assert str(fn).lower().endswith(".mzml"), fn
 
-            scan = data["scanList"]["scan"][0]
-
-            if "positive scan" in data.keys():
-                data["polarity"] = "+"
-
-            elif "negative scan" in data.keys():
-                data["polarity"] = "-"
+  # Read mzML file using pyteomics
+    with mzml.read(str(fn)) as reader:
+        # Initialize empty lists for the slices and the attributes
+        slices = []
+        # Loop through the spectra and extract the data
+        for spectrum in reader:
+            time_unit = spectrum['scanList']['scan'][0]['scan start time'].unit_info
+            if read_only:
+                continue
+            # Extract the scan ID, retention time, m/z values, and intensity values
+            scan_id = int(spectrum["id"].split("scan=")[-1])
+            rt = spectrum["scanList"]["scan"][0]["scan start time"]
+            if time_unit == 'minute':
+                rt = rt * 60.
+            mz = np.array(spectrum["m/z array"], dtype=np.float64)
+            intensity = np.array(spectrum["intensity array"], dtype=np.float64)
+            if "positive scan" in spectrum.keys():
+                polarity = "+"
+            elif "negative scan" in spectrum.keys():
+                polarity = "-"
             else:
-                data["polarity"] = None
-
-            if "scan start time" in scan.keys():
-                data["scan_time"] = scan["scan start time"]
-
-            elif "scan time" in scan.keys():
-                data["scan_time"] = scan["scan time"]
-            else:
-                logging.error(f"No scan time identified \n{scan}")
-                break
-
-            del data["scanList"]
-            slices.append(pd.DataFrame(data))
-
-    df = pd.concat(slices)
-
-    df["scan_id"] = df["id"].apply(lambda x: int(x.split("scan=")[1].split(" ")[0]))
-    df_to_numeric(df)
-    df["intensity array"] = df["intensity array"].astype(int)
-
-    mapping = {
-        "m/z array": "mz",
-        "intensity array": "intensity",
-        "ms level": "ms_level",
-    }
-
-    df = df.rename(columns=mapping)
-    df = df.reset_index(drop=True)
-    df = df[MS_FILE_COLUMNS]
-    return df
-
-
-def mzml_to_df(fn, time_unit="seconds", read_only=False):
-    """
-    Reads mzML file and returns a pandas.DataFrame
-    using the mzML library.
-
-    :param fn: Filename
-    :type fn: str or PosixPath
-    :param read_only: Whether or not to convert to dataframe, defaults to False
-    :type read_only: bool, optional
-    :return: MS data
-    :rtype: pandas.DataFrame
-    """
-    with pymzml.run.Reader(fn) as ms_data:
-        data = [x for x in ms_data]
-
+                polarity = None
+            ms_level = spectrum["ms level"]
+            slices.append(
+                pd.DataFrame(
+                    {
+                        "scan_id": scan_id,
+                        "mz": mz,
+                        "intensity": intensity,
+                        "polarity": polarity,
+                        "ms_level": ms_level,
+                        "scan_time": rt,
+                    }
+                )
+            )
     if read_only:
         return None
+    df = pd.concat(slices)
+    df["intensity"] = df["intensity"].astype(int)
+    df = df[MS_FILE_COLUMNS].reset_index(drop=True)
+    set_dtypes(df)
+    return df
 
-    data = list(extract_mzml(data, time_unit=time_unit))
 
-    df = (
-        pd.DataFrame.from_dict(data)
-        .set_index(["scan_id", "ms_level", "polarity", "scan_time"])
-        .apply(pd.Series.explode)
-        .reset_index()
+def set_dtypes(df):
+    dtypes = dict(
+        mz=np.float32,
+        scan_id=np.int64,
+        ms_level=np.int8,
+        scan_time=np.float32,
+        intensity=np.int64,
     )
 
-    df["mz"] = df["mz"].astype("float64")
-    df["intensity"] = df["intensity"].astype("float64")
-    df["scan_time"] = df["scan_time"] * 60.0
+    for var, dtype in dtypes.items():
+        if not df[var].dtype == dtype:
+            df[var] = df[var].astype(dtype)
+
     return df
 
 
 def _extract_mzml(data, time_unit):
-    try:
-        RT = data.scan_time_in_minutes()
-    except Exception:
-        if time_unit == "seconds":
-            RT = data.scan_time[0]
-        elif time_unit == "minutes":
-            RT = data.scan_time[0] * 60.0
+    RT = data.scan_time_in_minutes() * 60
     peaks = data.peaks("centroided")
     return {
         "scan_id": data["id"],
         "ms_level": data.ms_level,
         "polarity": "+" if data["positive scan"] else "-",
         "scan_time": RT,
         "mz": peaks[:, 0].astype("float64"),
-        "intensity": peaks[:, 1].astype("float64"),
+        "intensity": peaks[:, 1].astype("int64"),
     }
 
 
 extract_mzml = np.vectorize(_extract_mzml)
 
 
 def read_parquet(fn, read_only=False):
@@ -295,14 +268,15 @@
                 "MsOrder": "ms_level",
                 "RetentionTime": "scan_time",
                 "Masses": "mz",
                 "Intensities": "intensity",
             }
         )
     )
+    df["scan_time"] = df["scan_time"]*60
     df["polarity"] = None
     df["intensity"] = df.intensity.astype(np.float64)
     df = df[MS_FILE_COLUMNS]
     return df
 
 
 def mzmlb_to_df__pyteomics(fn, read_only=False):
@@ -320,39 +294,40 @@
     with mzmlb.MzMLb(fn) as ms_data:
         data = [x for x in ms_data]
 
     if read_only:
         return None
 
     data = list(extract_mzmlb(data))
-
     df = (
         pd.DataFrame.from_dict(data)
-        .set_index("retentionTime")
+        .set_index(["index", "retentionTime"])
         .apply(pd.Series.explode)
         .reset_index()
         .rename(
             columns={
                 "index": "scan_id",
                 "retentionTime": "scan_time",
                 "m/z array": "mz",
                 "ms level": "ms_level",
                 "intensity array": "intensity",
             }
         )
     )
 
+    # mzMLb starts scan index with 0
+    df["scan_id"] = df["scan_id"] + 1
     df["polarity"] = None
     df = df[MS_FILE_COLUMNS]
     return df
 
 
 def _extract_mzmlb(data):
     cols = ["index", "ms level", "retentionTime", "m/z array", "intensity array"]
-    data["retentionTime"] = data["scanList"]["scan"][0]["scan start time"] / 60
+    data["retentionTime"] = data["scanList"]["scan"][0]["scan start time"] * 60
     return {c: data[c] for c in cols}
 
 
 extract_mzmlb = np.vectorize(_extract_mzmlb)
 
 
 def df_to_numeric(df):
```

### Comparing `ms-mint-0.2.2/ms_mint/matplotlib_tools.py` & `ms-mint-0.2.3/ms_mint/matplotlib_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,23 +188,23 @@
         peak_labels = R.peak_label.drop_duplicates().values
 
     if fns is not None:
         R = R[R.ms_file.isin(fns)]
 
     dfs = []
     for peak_label in peak_labels:
-        for ndx, row in R[
+        for _, row in R[
             (R.peak_label == peak_label) & (R.peak_n_datapoints > 1)
         ].iterrows():
             peak_rt = [float(i) for i in row.peak_shape_rt.split(",")]
             peak_int = [float(i) for i in row.peak_shape_int.split(",")]
             ms_file = row.ms_file
             mz = row.mz_mean
             rt = row.rt
-            
+
             df = pd.DataFrame(
                 {
                     "Scan time [s]": peak_rt,
                     "Intensity": peak_int,
                     "ms_file": ms_file,
                     "peak_label": peak_label + f"\nm/z={mz:.3f}",
                     "Expected Scan time [s]": rt,
@@ -261,15 +261,15 @@
     )
     if peaks is not None:
         series.iloc[peaks.ndxs].plot(
             label="Peaks", marker="x", y="intensity", lw=0, ax=ax
         )
         for i, (
             ndx,
-            (_, rt, rt_span, peak_base_height, peak_height, rt_min, rt_max),
+            (_, _, _, peak_base_height, _, rt_min, rt_max),
         ) in enumerate(peaks.iterrows()):
             if ndx in highlight:
                 plt.axvspan(rt_min, rt_max, color="green", alpha=0.25, label="Selected")
             plt.hlines(
                 peak_base_height,
                 rt_min,
                 rt_max,
@@ -298,15 +298,14 @@
     set_dim=True,
     cmap="jet",
     rt_range=None,
     mz_range=None,
     mz_bins=100,
     **kwargs,
 ):
-
     if set_dim:
         plt.figure(figsize=figsize, dpi=dpi)
 
     if mz_range is None:
         mz_range = (df.mz.min(), df.mz.max())
 
     if rt_range is None:
```

### Comparing `ms-mint-0.2.2/ms_mint/notebook.py` & `ms-mint-0.2.3/ms_mint/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 class Mint(_Mint_):
     """
     MINT with added functions for interactive use in Jupyter Notebook (experimental).
     """
 
     def __init__(self, *args, **kwargs):
-
         self.progress_callback = self._set_progress_
 
         super().__init__(progress_callback=self.progress_callback, *args, **kwargs)
 
         fc = FileChooser()
         fc.show_only_dirs = True
         fc.default_path = os.getcwd()
@@ -103,15 +102,15 @@
                 self.progress_bar,
             ]
         )
 
         self.tqdm = tqdm
 
     def _load_target_from_bytes_(self, value):
-        for fn, data in value["new"].items():
+        for data in value["new"].values():
             self.load(io.BytesIO(data["content"]))
         self._message_(f"{len(self.targets)} targets loaded.")
 
     @property
     def messages(self):
         return self._messages
 
@@ -138,15 +137,15 @@
 
         :return: IPython Widgets elements.
         """
         display(HTML("<style>textarea, input { font-family: monospace; }</style>"))
         return self.layout
 
     def _run_(self, b=None, **kwargs):
-        self.message(f"Start processing...")
+        self.message("Start processing...")
         self.progress = 0
         self.run(**kwargs)
         self.message("...finished processing.")
         if self.results is not None:
             self.download_button.style.button_color = "lightgreen"
 
     def _set_progress_(self, value):
```

### Comparing `ms-mint-0.2.2/ms_mint/pca.py` & `ms-mint-0.2.3/ms_mint/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,9 +163,9 @@
         return g
 
     def pairplot_plotly(self, df, **kwargs):
         color_col = "Label" if "Label" in df.columns else None
         fig = ff.create_scatterplotmatrix(df, index=color_col, **kwargs)
         # set the legendgroup equal to the marker color
         for t in fig.data:
-            t.legendgroup=t.marker.color
+            t.legendgroup = t.marker.color
         return fig
```

### Comparing `ms-mint-0.2.2/ms_mint/plotly_tools.py` & `ms-mint-0.2.3/ms_mint/plotly_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,26 +228,25 @@
     call_show=False,
 ):
     """
     Returns a plotly multiplost of all peak_shapes in mint.results
     grouped by peak_label.
     """
     mint_results = mint_results.copy()
-    
 
     if fns is not None:
         fns = [P(fn).name for fn in fns]
         mint_results = mint_results[mint_results.ms_file.isin(fns)]
 
     mint_results.ms_file = [P(fn).name for fn in mint_results.ms_file]
 
-    logging.warning('TEST')
+    logging.warning("TEST")
 
     res = mint_results[mint_results.peak_max > 0]
-    
+
     fns = list(res.ms_file.drop_duplicates())
     labels = list(mint_results.peak_label.drop_duplicates())
 
     res = res.set_index(["peak_label", "ms_file"]).sort_index()
 
     if isinstance(peak_labels, str):
         peak_labels = [peak_labels]
```

### Comparing `ms-mint-0.2.2/ms_mint/plotting.py` & `ms-mint-0.2.3/ms_mint/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         # Scale along peak_labels
         if scaler_peak_label is not None:
             tmp_data = scale_dataframe(tmp_data, scaler_peak_label)
 
         if transposed:
             tmp_data = tmp_data.T
 
-        clustered, fig, ndx_x, ndx_y = hierarchical_clustering(
+        _, fig, ndx_x, ndx_y = hierarchical_clustering(
             tmp_data,
             vmin=vmin,
             vmax=vmax,
             figsize=figsize,
             xmaxticks=xmaxticks,
             ymaxticks=ymaxticks,
             metric=metric,
@@ -277,27 +277,27 @@
         :type mz_width: int>0, optional
         :return: Plot of chromatogram(s)
         :rtype: matplotlib.Figure
         """
 
         if isinstance(fns, str):
             fns = [fns]
-        
+
         if fns is not None:
             fns = tuple(fns)
 
         if isinstance(peak_labels, str):
             peak_labels = [peak_labels]
 
         if peak_labels is None:
             peak_labels = self.mint.peak_labels
 
         if peak_labels is not None:
             peak_labels = tuple(peak_labels)
-        
+
         data = self.mint.get_chromatograms(fns=fns, peak_labels=peak_labels)
 
         if not interactive:
             params = dict(
                 x="scan_time",
                 y="intensity",
                 col="peak_label",
@@ -310,15 +310,15 @@
                 marker=".",
                 linewidth=0,
             )
             params.update(kwargs)
             g = sns.relplot(data=data, **params)
 
             for peak_label, ax in zip(peak_labels, g.axes.flatten()):
-                mz_mean, mz_width, rt_min, rt_max = self.mint.get_target_params(
+                _, _, rt_min, rt_max = self.mint.get_target_params(
                     peak_label
                 )
                 if rt_min is not None and rt_max is not None:
                     ax.axvspan(rt_min, rt_max, color="lightgreen", alpha=0.5, zorder=-1)
                 ax.ticklabel_format(
                     style="sci", axis="y", useOffset=False, scilimits=(0, 0)
                 )
```

### Comparing `ms-mint-0.2.2/ms_mint/processing.py` & `ms-mint-0.2.3/ms_mint/processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,29 +32,30 @@
     return chrom["intensity"]
 
 
 def process_ms1_files_in_parallel(args):
     """
     Pickleable function for (parallel) peak integration.
     """
-
     filename = args["filename"]
     targets = args["targets"]
     output_fn = args["output_fn"]
 
     if "queue" in args.keys():
         q = args["queue"]
         q.put("filename")
 
     try:
         results = process_ms1_file(filename=filename, targets=targets)
     except Exception as e:
         logging.error(f"process_ms1_files_in_parallel(): {e}")
         results = pd.DataFrame()
 
+    print(len(results))
+
     if (output_fn is not None) and (len(results) > 0):
         append_results(results, output_fn)
         return None
 
     return results
 
 
@@ -85,14 +86,15 @@
     df = ms_file_to_df(filename)
     results = process_ms1(df, targets)
     results["total_intensity"] = df["intensity"].sum()
     results["ms_file"] = os.path.basename(filename)
     results["ms_path"] = os.path.dirname(filename)
     results["ms_file_size"] = os.path.getsize(filename) / 1024 / 1024
     results["peak_score"] = score_peaks(results)
+    print(results)
     return results[MINT_RESULTS_COLUMNS]
 
 
 def process_ms1(df, targets):
     """
     Process MS-1 data with a target list.
 
@@ -116,16 +118,14 @@
         "mz_width",
         "rt_min",
         "rt_max",
         "intensity_threshold",
         "peak_label",
     ]
     array_peaks = targets[peak_cols].values
-    # if "ms_level" in df.columns:
-    #    df = df[df.ms_level == 1]
     array_data = df[["scan_time", "mz", "intensity"]].values
     result = process_ms1_from_numpy(array_data, array_peaks)
     return result
 
 
 def process_ms1_from_numpy(array, peaks):
     """
@@ -135,15 +135,15 @@
     :type array: numpy.Array
     :param peaks: Peak data np.array([[mz_mean_1, mz_width_1, rt_min_1, rt_max_1, intensity_threshold_1, peak_label_1], ...])
     :type peaks: numpy.Array
     :return: Extracted data.
     :rtype: list
     """
     results = []
-    for (mz_mean, mz_width, rt_min, rt_max, intensity_threshold, peak_label) in peaks:
+    for mz_mean, mz_width, rt_min, rt_max, intensity_threshold, peak_label in peaks:
         props = _process_ms1_from_numpy(
             array,
             mz_mean=mz_mean,
             mz_width=mz_width,
             rt_min=rt_min,
             rt_max=rt_max,
             intensity_threshold=intensity_threshold,
@@ -186,14 +186,23 @@
     :rtype: dict
     """
 
     float_list_to_comma_sep_str = lambda x: ",".join([str(np.round(i, 4)) for i in x])
     int_list_to_comma_sep_str = lambda x: ",".join([str(int(i)) for i in x])
 
     projection = pd.DataFrame(array[:, [0, 2]], columns=["rt", "int"])
+
+    print("DEBUG extract_ms1_properties")
+    print(array)
+    print(array.dtype)
+    print(array.shape)
+    print(len(projection))
+    print(projection)
+    print(projection.dtypes)
+
     projection["rt"] = projection["rt"].round(2)
     projection["int"] = projection["int"].astype(int)
     projection = projection.groupby("rt").max().reset_index().values
 
     times = array[:, 0]
     masses = array[:, 1]
     intensities = array[:, 2]
@@ -248,15 +257,15 @@
     peak_mass_diff_50pc /= 1e-6 * mz_mean
     peak_mass_diff_75pc /= 1e-6 * mz_mean
 
     peak_shape_rt = float_list_to_comma_sep_str(projection[:, 0])
     peak_shape_int = int_list_to_comma_sep_str(projection[:, 1])
 
     # Check that peak projection arrays (rt, int) have same number of elements
-    assert len(peak_shape_rt.split(',')) == len(peak_shape_int.split(','))
+    assert len(peak_shape_rt.split(",")) == len(peak_shape_int.split(","))
 
     return dict(
         peak_area=peak_area,
         peak_area_top3=peak_area_top3,
         peak_max=peak_max,
         peak_min=peak_min,
         peak_mean=peak_mean,
```

### Comparing `ms-mint-0.2.2/ms_mint/standards.py` & `ms-mint-0.2.3/ms_mint/standards.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.2/ms_mint/targets.py` & `ms-mint-0.2.3/ms_mint/targets.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,17 +186,17 @@
     """
     rt_cuts = np.arange(0, rt_max + dt, dt)
     targets = pd.DataFrame(index=rt_cuts, columns=masses).unstack().reset_index()
     del targets[0]
     targets.columns = ["mz_mean", "rt_min"]
     targets["rt_max"] = targets.rt_min + (1 * dt)
     targets["peak_label"] = (
-        targets.mz_mean.apply(lambda x: "{:.3f}".format(x))
+        targets.mz_mean.apply("{:.3f}".format)
         + "__"
-        + targets.rt_min.apply(lambda x: "{:2.2f}".format(x))
+        + targets.rt_min.apply("{:2.2f}".format)
     )
     targets["mz_width"] = mz_ppm
     targets["intensity_threshold"] = intensity_threshold
     targets["targets_name"] = "gen_target_grid"
     return targets
 
 
@@ -242,22 +242,21 @@
         self,
         fns=None,
         targets=None,
         peak_labels=None,
         minimum_intensity=1e4,
         plot=False,
         sigma=20,
-        filter=None,
+        filters=None,
         post_opt=False,
         post_opt_kwargs=None,
         rel_height=0.9,
         height=3,
         aspect=2,
         col_wrap=3,
-        verbose=False,
         **kwargs,
     ):
         """
         Optimize rt_min and rt_max values based on expected retention times (rt).
         For this optimization all rt values in the target list must be present.
 
         :param fns: List of filenames to use for optimization
@@ -268,16 +267,16 @@
         :type peak_labels: List[str or PosixPath], optional
         :param minimum_intensity: Minimum intensity required, otherwise skip target, defaults to 1e4
         :type minimum_intensity: float, optional
         :param plot: Whether or not to plot first 100 optimizations, defaults to True
         :type plot: bool, optional
         :param sigma: Sigma value for peak selection, defaults to 20
         :type sigma: float, optional
-        :param filter: Filter instances to apply in respective order, defaults to None
-        :type filter: ms_mint.filter.Filter, optional
+        :param filters: Filter instances to apply in respective order, defaults to None
+        :type filters: ms_mint.filters.Filter, optional
         :param post_opt: Optimize retention times after peak selection, defaults to False
         :type post_opt: bool, optional
         :param post_opt_kwargs: _description_, defaults to 20
         :type post_opt_kwargs: int, optional
         :return: (self, None) or (self, matplotlib.pyplot.Figure) if plot==True
         :rtype: tuple
         """
@@ -287,58 +286,46 @@
 
         if fns is None:
             fns = self.mint.ms_files
 
         if peak_labels is None:
             peak_labels = targets.peak_label.values
 
-        if verbose:
-            print(targets)
-            print(fns)
-            print(peak_labels)
-
         _targets = targets.set_index("peak_label").copy()
 
-        if verbose:
-            print(_targets)
-
-        print("Reading files...")
         ms1 = pd.concat([ms_file_to_df(fn) for fn in tqdm(fns)]).sort_values(
             ["scan_time", "mz"]
         )
 
         if plot:
             n_rows = int(np.ceil(len(peak_labels) / col_wrap))
             fig = plt.figure(figsize=(col_wrap * height * aspect, n_rows * height))
 
         i = 0
-        for (peak_label, row) in tqdm(_targets.iterrows(), total=len(targets)):
-
-            if verbose:
-                print(peak_label)
+        for peak_label, row in tqdm(_targets.iterrows(), total=len(targets)):
             if peak_label not in peak_labels:
                 logging.warning(f"{peak_label} not in {peak_labels}")
                 continue
 
             mz = row.mz_mean
             rt = row.rt
 
             _slice = extract_chromatogram_from_ms1(ms1, mz).groupby("scan_time").sum()
 
             chrom = Chromatogram(
-                _slice.index, _slice.values, expected_rt=rt, filter=filter
+                _slice.index, _slice.values, expected_rt=rt, filters=filters
             )
 
             if chrom.x.max() < minimum_intensity:
                 logging.warning(
                     f"Peak intensity for {peak_label} below threshold ({minimum_intensity})"
                 )
                 continue
 
-            chrom.apply_filter()
+            chrom.apply_filters()
             chrom.find_peaks(rel_height=rel_height)
             chrom.select_peak_with_gaussian_weight(rt, sigma)
 
             if post_opt:
                 if post_opt_kwargs is None:
                     post_opt_kwargs = {}
                 chrom.optimise_peak_times_with_diff(**post_opt_kwargs)
@@ -347,17 +334,14 @@
                 logging.warning(f"No peaks detected for {peak_label}")
                 continue
 
             ndx = chrom.selected_peak_ndxs[0]
             rt_min = chrom.peaks.at[ndx, "rt_min"]
             rt_max = chrom.peaks.at[ndx, "rt_max"]
 
-            if verbose:
-                print(ndx, peak_label, rt_min, rt_max)
-
             _targets.loc[peak_label, ["rt_min", "rt_max"]] = rt_min, rt_max
 
             if plot:
                 i += 1
 
                 if i <= 1000:
                     plt.subplot(n_rows, col_wrap, i)
```

### Comparing `ms-mint-0.2.2/ms_mint/tools.py` & `ms-mint-0.2.3/ms_mint/tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.2/ms_mint.egg-info/PKG-INFO` & `ms-mint-0.2.3/ms_mint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.2
+Version: 0.2.3
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,27 +22,27 @@
 The `ms-mint` library is a tool designed to assist with targeted metabolomics studies, which involves the systematic analysis of small chemical compounds called metabolites that are present in biological samples. These metabolites can provide valuable information about the state of an organism, including indicators of disease or other physiological changes. In order to perform a targeted metabolomics study, researchers typically use liquid chromatography-mass spectrometry (LCMS) to identify and quantify specific metabolites of interest.
 
 The `ms-mint` library includes a range of functions for processing LCMS data from targeted metabolomics experiments, and it is particularly well-suited for handling large amounts of data (10,000+ files). To use `ms-mint`, you provide it with a target list of the specific metabolites you want to analyze, as well as the names of the mass spectrometry files containing the data. ms-mint then extracts peak intensities and other relevant information from the data, allowing you to gain insights into the concentrations and profiles of the metabolites in your samples. This information can be used to identify biomarkers, which are indicators of disease or other physiological changes that can be used in the development of diagnostic tests or other medical applications.
 
 ## Documentation
 The code documentation can be accessed [here](https://lewisresearchgroup.github.io/ms-mint/readme.html).
 
-## News
+## ms-mint application with graphical user iterface (GUI)
 MINT has been split into the Python library and the app. This repository contains the Python library. For the app follow [this link](https://github.com/LewisResearchGroup/ms-mint-app).
 
 ## Contributions
 All contributions, bug reports, code reviews, bug fixes, documentation improvements, enhancements, and ideas are welcome.
 Before you modify the code please reach out to us using the [issues](https://github.com/LewisResearchGroup/ms-mint/issues) page.
 
 ## Code standards
 The project follows PEP8 standard and uses Black and Flake8 to ensure a consistent code format throughout the project.
 
 ---
 
-# Usage
+## Usage
 
 To use the main class of the ms-mint library, you can import it into your code with the following command:
 
     from ms_mint.Mint import Mint
 
 This will import a lightweight version of the class with the essential functionality. If you want to use the ms-mint tool interactively in a Jupyter Notebook or JupyterLab, you can import the class with the following command:
 
@@ -155,28 +155,26 @@
     mint.run()
     mint.plot.peak_shapes(col_wrap=3)
 
 ![](notebooks/peak-shapes-after-opt.png)
 
 As you can see, the shapes of Xanthine, Succinate, Citrulline look much better.
 
-
 ## Plotting and data exploration
 
 The `Mint` class has a few convenient methods to visualize and explore the processed data. The results can be viewed directly in JupyterLab or stored to files using `matplotlib` and `seaborn` syntax. The figures are matplotlib objects and can be easily customised. 
 
 ## Plot peak shapes
 
 ![](notebooks/peak-shapes-after-opt.png)
 
     mint.plot.peak_shapes(col_wrap = 3)
 
 The method uses seaborn [sns.relplot()](https://seaborn.pydata.org/generated/seaborn.relplot.html) function and keyword arguments are passed on. 
 
-
 ## Hierarchical clustering
 Mint ca be used to cluster the extracted data. An agglomerative hierarchical clustering is a bottom-up clustering technique where each data point starts as its own cluster and then are merged with other clusters in a hierarchical manner based on their proximity or similarity until a single cluster is formed or a specified stopping criteria is met. The proximity is usually determined by a distance metric, such as Euclidean distance, and the similarity is usually determined by a linkage function, such as ward linkage or complete linkage. The result is a tree-like representation called a dendrogram, which can be used to determine the number of clusters and the cluster assignments of the data points.
 
 Mint uses `scipy.spartial.distance` to generate the distance matrix and `scipy.cluster.hierarchy.linkage` to perform the clustering. By default a 'cosine' metric is used to calculate the distances. Distances between row vectors and column vectors respectively can also be done using different metrics for each set. To do so a tuple with the names of the metrics has to be provided: `mint.hierarchical_clustering(metric=("euclidean", "cosine")`.
 
 Before clustering the data can be transformed and scaled. By default `log2p1(x) = log_2(x+1)` is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
 
@@ -198,15 +196,14 @@
         transform_filenames_func="basename",  # Transformation function to shorten filenames
         transposed=False,  # Transpose the plot     
         top_height=2,  # Height of the top-dendrogram
         left_width=2,  # Width of the left-dendrogram
         cmap=None  # Name of a matplotlib color map                
     )
 
-
 ![](notebooks/hierarchical_clustering.png)
 
 ## Principal Components Analysis
 
 Principal Component Analysis (PCA) is a widely used statistical technique for dimensionality reduction. It transforms the original high-dimensional data into a new set of linearly uncorrelated variables, called Principal Components (PCs), that capture the maximum variance in the data. The first PC accounts for the largest variance in the data, the second PC for the second largest variance, and so on. PCA is commonly used for data visualization, data compression, and noise reduction. By reducing the number of dimensions in the data, PCA allows us to more easily identify patterns and relationships in the data.
 
 Before clustering the data can be transformed and scaled. By default log2p1(x) = log_2(x+1) is used to transform the data and the standard scaler (z-scores) is used to normalize the variables for each target.
@@ -215,49 +212,49 @@
     
 After running the PCA the results can be plotted with:    
     
     mint.pca.plot.pairplot(n_components=5, interactive=False)
     
 ![](notebooks/pca-pairplot.png)
 
-# FAQ
-## What is a target list
+## FAQ
+### What is a target list
 A target list is a pandas dataframe with specific columns. 
 
 -   **peak_label**: string, Label of the peak (must be unique).
 -   **mz_mean**: numeric value, theoretical m/z value of the target ion to extract.
 -   **mz_width**: numeric value, width of the peak in \[ppm\]. It is used to calculate the width of the mass window  according to the formula: `Δm = m/z * 1e-6 * mz_width`.
 -   **rt**: numeric value, (optional), expected time of the peak. This value is not used during processing, but it can inform the peak optimization procedure.
 -   **rt_min**: numeric value, starting time for peak integration.
 -   **rt_max**: numeric value, ending time for peak integration.
 -   **rt_unit**: one of `s` or `min` for seconds or minutes respectively.
 -   **intensity_threshold**: numeric value (>=0), minimum intensity value to include, serves as a noise filter. We recommend setting this to 0. 
 -   **target_filename**: string (optional), name of the target list file. It is not used for processing, just to keep track of what files were used.
 
 The target list can be stored as csv or Excel file. 
 
-## What input files can be used
+### What input files can be used
 `ms_mint` can be used with `mzXML`, `mzML`, `mzMLb` and experimental formats in `.feather` and `.parquet` format.
 
-## Which properties does ms-mint extract
-### Parameters from target list
+### Which properties does ms-mint extract
+#### Parameters from target list
 -   **ms_file**: Filename of MS-file
 -   **peak_label**: From target list
 -   **mz_mean**: From target list
 -   **mz_width**: From target list
 -   **rt**: From target list
 -   **rt_min**: From target list
 -   **rt_max**: From target list
 -   **rt_unit**: Unit of retention times, default is s (seconds), from [s, min]
 -   **intensity_threshold**: From target list
 -   **target_filename**: From target list
 
 ---
 
-### Results columns
+#### Results columns
 -   **peak_area**: The sum of all intensities in the extraction window
 -   **peak_area_top3**: The average of the 3 largest intensities in the extraction window
 -   **peak_n_datapoints**: Number of datapoints
 -   **peak_max**: Intensity of peak maximum
 -   **peak_rt_of_max**: Retentiontime of peak maximum
 -   **peak_min**: Minimum peak intensity (offset)
 -   **peak_median**: Median of all intensities 
@@ -270,13 +267,11 @@
 -   **peak_mass_diff_75pc**: 75th percentile between *mz_mean* minus m/z values of all datapoints
 -   **peak_score**: Score of peak quality (experimental)
 -   **total_intensity**: Sum of all intensities in the file
 -   **ms_path**: Path of the MS-file
 -   **ms_file_size**: Size of the MS-file in MB
 ---
 
+## Release Notes
 
-# Release Notes
-
-## 0.2.0 Milestones
+### 0.2.0 Milestones
     - peak_area_top3 comparable to El-Maven PeakAreaTop values
-
```

### Comparing `ms-mint-0.2.2/ms_mint.egg-info/SOURCES.txt` & `ms-mint-0.2.3/ms_mint.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 setup.py
 versioneer.py
 ms_mint/Mint.py
 ms_mint/__init__.py
 ms_mint/_version.py
 ms_mint/chromatogram.py
 ms_mint/filelock.py
-ms_mint/filter.py
+ms_mint/filters.py
 ms_mint/io.py
 ms_mint/matplotlib_tools.py
 ms_mint/notebook.py
 ms_mint/pca.py
 ms_mint/plotly_tools.py
 ms_mint/plotting.py
 ms_mint/processing.py
```

### Comparing `ms-mint-0.2.2/setup.py` & `ms-mint-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.2/versioneer.py` & `ms-mint-0.2.3/versioneer.py`

 * *Files identical despite different names*

