# Comparing `tmp/bacteria-0.1.7.tar.gz` & `tmp/bacteria-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.1.7.tar", last modified: Thu Apr 27 16:54:24 2023, max compression
+gzip compressed data, was "bacteria-0.1.8.tar", last modified: Thu Apr 27 17:04:28 2023, max compression
```

## Comparing `bacteria-0.1.7.tar` & `bacteria-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 16:54:24.097000 bacteria-0.1.7/
--rw-rw-rw-   0        0        0      593 2023-04-27 16:54:23.963000 bacteria-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2023-04-27 16:19:57.000000 bacteria-0.1.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-27 16:54:23.520000 bacteria-0.1.7/bacteria/
--rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-0.1.7/bacteria/__init__.py
--rw-rw-rw-   0        0        0   151173 2023-04-27 16:53:20.000000 bacteria-0.1.7/bacteria/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-27 16:54:23.865000 bacteria-0.1.7/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-04-27 16:54:22.000000 bacteria-0.1.7/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-27 16:54:22.000000 bacteria-0.1.7/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 16:54:22.000000 bacteria-0.1.7/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-27 16:54:22.000000 bacteria-0.1.7/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 16:54:22.000000 bacteria-0.1.7/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 16:54:24.069000 bacteria-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-04-27 16:53:42.000000 bacteria-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:04:28.514000 bacteria-0.1.8/
+-rw-rw-rw-   0        0        0      593 2023-04-27 17:04:28.403000 bacteria-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2023-04-27 16:19:57.000000 bacteria-0.1.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-27 17:04:27.993000 bacteria-0.1.8/bacteria/
+-rw-rw-rw-   0        0        0       34 2023-04-27 16:19:58.000000 bacteria-0.1.8/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   144470 2023-04-27 17:04:04.000000 bacteria-0.1.8/bacteria/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-27 17:04:28.372000 bacteria-0.1.8/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-04-27 17:04:27.000000 bacteria-0.1.8/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-27 17:04:27.000000 bacteria-0.1.8/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 17:04:27.000000 bacteria-0.1.8/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-27 17:04:27.000000 bacteria-0.1.8/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 17:04:27.000000 bacteria-0.1.8/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 17:04:28.462000 bacteria-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-04-27 17:04:22.000000 bacteria-0.1.8/setup.py
```

### Comparing `bacteria-0.1.7/PKG-INFO` & `bacteria-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.7
+Version: 0.1.8
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.7/README.rst` & `bacteria-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.7/bacteria/functions.py` & `bacteria-0.1.8/bacteria/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
     df_temp_2 = []
     df_temp_3 = []
 
     for idx,mat in enumerate(paths_xy,1):
         data_temp = scipy.io.loadmat(mat)
         data2D_temp = df_data2d(data_temp,fps=fps, const=const)
-        data3D_temp,_ = df_data3d(data_temp,fps = fps, filter = False, const = const)
+        data3D_temp,_ = df_data3d(data_temp,fps = fps, filters = False, const = const)
 
         if direct:
             data2D_temp['fov'] = 'xy' + str(idx)
             data3D_temp['fov'] = 'xy' + str(idx)
         else:
             data2D_temp['fov'] = mat.split('/')[-2]
             data3D_temp['fov'] = mat.split('/')[-2]
@@ -754,16 +754,14 @@
     ax : nd.array (optional)
         the ax position to plot
         
     Returns
     --------------
     None
     """
-    from sklearn import preprocessing as pre
-
     t_mother = pre.MinMaxScaler((0,1)).fit_transform(df_3d[df_3d['Cell ID'] == cell_id]['Time (Frames)'].values.reshape(-1, 1))
     # Plot mother fluorescence:
     plt.plot(t_mother,df_3d[df_3d['Cell ID'] == cell_id]['Fluor1 mean'],label = 'Mother ' + str(int(cell_id)))
 
     # Plot daughters fluorescence:
     color_add = 0
     if ax is None:
@@ -1061,148 +1059,14 @@
         ax[1].legend()
 
         plt.tight_layout()
         plt.show()
 
     return ci_low,ci_high
 
-def mean_vector_np(df, column_y ,column_x = 'Time (fps)', fps = 3, good_cells = None):
-    """
-    Calculate the mean vector for a column in time or volume
-    using numpy logic.
-    
-    Parameters
-    --------------
-    df : DataFrame
-        DataFrame of 3D data
-    column_y : str
-        Column to calculate the mean (y axis data)
-    column_x: str (optional)
-        x axis data, 'Volume' or 'Time (fps)'
-    fps : int (optional)
-        frames per second used in the experiment, default = 3
-    good_cells : List (optional)
-        List with cells to use 
-        if None good_cells = df['Cell ID'].values
-        
-    Returns
-    --------------
-    time :  nd.array
-        time array using column_x
-    vector : nd.array
-        mean of the vector from column_y
-    """
-    if good_cells is None: 
-        good_cells = list(set(df['Cell ID'].values))    
-    times = np.arange(df[column_x].min(),df[column_x].max()+fps,fps)
-    vector = np.zeros((len(good_cells),len(times)))
-
-    for idx,cell in enumerate(good_cells):
-        for _,data in enumerate(zip(df[df['Cell ID']==cell][column_x],df[df['Cell ID']==cell][column_y])):
-            vector[idx,np.where(times==data[0])[0][0]] = data[1]
-
-    return times, np.mean(vector,0)
-
-def mean_vector_df(df,id_vars = 'Time (fps)', value_vars = 'F/V', conf = 0.95, method = np.mean,fps = 3):
-    """
-    Calculate the mean vector for a column in time or volume
-    using pd.melt.
-    
-    Parameters
-    --------------
-    df : DataFrame
-        DataFrame of 3D data
-    id_vars : str (optional)
-        Column to do the melt, default 'Time (fps)'
-    value_vars : str (optional)
-        Column to calculate the mean, default 'F/V'
-    conf : float (optional)
-        confidence interval desired, default - 0.95
-    method : function (optional)
-        Method to use as basis for the boostrap,
-        default its np.mean. Other options are np.std
-        and stats.sem.
-    fps : int (optional)
-        frames per second used in the experiment, default = 3
-
-    Returns
-    --------------
-    time : nd.array
-        time array for the experiment (using 'Time (fps)')
-    mean_nd.array
-        mean values array
-    ci : nd.array
-        matrix with CI low and high (ci[:,0] = low, ci[:,1] = high)
-    """
-    
-    df_ratio = pd.melt(df, id_vars=[id_vars], value_vars=[value_vars]).sort_values(by=[id_vars])
-    time_frames = list(set(df_ratio['Time (fps)'].values))
-    mean_list = []
-    times = []
-    ci = np.zeros((len(range(1,len(time_frames)-2)),2))
-
-    for i in range(1,len(time_frames)-2):
-        mean_list.append(np.mean(df_ratio[df_ratio['Time (fps)'].isin(time_frames[i-1:i+2])]['value'].values))
-        times.append(time_frames[i])
-        ci[i-1,:] = ci_bootstrap(df_ratio[df_ratio['Time (fps)'].isin(time_frames[i-1:i+2])]['value'].values,
-                                 conf = conf, method = method, plot = False)
-
-    mean_list = np.asarray(mean_list)
-    times = np.asarray(times)
-
-    return times,mean_list,ci
-
-def plot_mean_vector_df(df, id_vars = 'Time (fps)', value_vars = 'F/V', conf = 0.95, method = np.mean, fps = 3, ax = None):
-    """
-    Plot the mean vector for the entire experiment.
-    Check also mean_vector_df().
-    
-    Parameters
-    --------------
-    df : DataFrame
-        DataFrame of 3D data
-    id_vars : str (optional)
-        Column to do the melt, default 'Time (fps)'
-    value_vars: str (optional)
-        Column to calculate the mean, default 'F/V'
-    conf : float (optional)
-        confidence interval desired, default - 0.95
-    method : function (optional)
-        Method to use as basis for the boostrap,
-        default its np.mean. Other options are np.std
-        and stats.sem.
-    fps : int (optional)
-        frames per second used in the experiment, default = 3
-    ax : nd.array (optional)
-        the ax position to plot
-        
-    Returns
-    --------------
-    None
-    """
-
-    times,mean_vector,ci = mean_vector_df(df,id_vars=id_vars,value_vars=value_vars,conf=conf,method=method,fps=fps)
-
-    if ax is None:
-        plt.plot(times,mean_vector)
-        plt.fill_between(times,ci[:,0],ci[:,1], alpha=.3)
-        plt.title(value_vars + ' mean', fontsize = 17)
-        plt.xlabel(id_vars, fontsize = 15)
-        plt.ylabel(value_vars + ' (a.u.)', fontsize = 15)
-        plt.show()
-
-    else:
-        out = ax.plot(times,mean_vector),\
-              ax.fill_between(times,ci[:,0],ci[:,1], alpha=.3),\
-              ax.set_xlabel(id_vars, fontsize = 15),\
-              ax.set_ylabel(value_vars + ' (a.u.)', fontsize = 15),\
-              ax.set_title(value_vars + ' mean', fontsize = 17)
-        
-        return out
-
 def instantaneous_measuraments(df,good_cells, column, fps = 3, minus = 1, plus = 2):
     """
     Calculate the instantaneous mesasurament for each cell 
     in the dataset using a window of 3 data points. 
     
     Parameters
     --------------
@@ -1255,79 +1119,14 @@
 
     for idx,cell in enumerate(good_cells):
         for _,data in enumerate(zip(time_dict[cell],gr_inst[cell])):
             im[idx,np.where(times==data[0])[0][0]] = data[1]
 
     return im,times
 
-def simple_bootstrap(arr, conf = 0.95,times = 10000):
-    """
-    Calculate the confidence interval (CI).By default 
-    the bootstrap is done for 10000 times. 
-    
-    Parameters
-    --------------
-    arr: nd.array
-        data to calculate the CI
-    conf : float (optional)
-        confidence interval desired, default - 0.95
-    times : int (optional)
-        Number of times to run the bootstrap
-
-    Returns
-    --------------
-    ci_low : float
-        Value for the lower CI (default 2.5%)
-    ci_high : float
-        Value for the higher CI (default 97.5%)
-    """
-    values = [np.random.choice(arr,size=len(arr),replace=True).mean() for i in range(times)] 
-    ci_low,ci_high = np.percentile(values,[100*(1-conf)/2,100*(1-(1-conf)/2)])
-    
-    return ci_low,ci_high
-
-def _progressbar(it, prefix="", size=60, out=sys.stdout):
-    """
-    Binarize the data and make the mean for each bin.
-    Suport function for fluor_lineage(). Bins are
-    calculated based on the time data (previous reshaped
-    and sclaed) using np.histogram(), default values for bins
-    is 10.
-    
-    Parameters
-    --------------
-    it : int
-        range of iterations (for size)
-    prefix : str
-        Term before the computation
-    size : int (optional)
-        progress bar size
-    out : function
-        show the bar in the console
-        
-    Returns
-    --------------
-    None
-
-    Author
-    --------------
-    https://stackoverflow.com/questions/3160699/python-progress-bar
-    """
-    import sys
-    count = len(it)
-    def show(j):
-        x = int(size*j/count)
-        print("{}[{}{}] {}/{}".format(prefix, "#"*x, "."*(size-x), j, count), 
-                end='\r', file=out, flush=True)
-    show(0)
-    for i, item in enumerate(it):
-        yield item
-        show(i+1)
-    print("\n", flush=True, file=out)
-
 def derivative(df_3d, column = 'Fluor1 sum',minus = 1, plus = 2, bar = True):
     """
     Calculate the derivatine of the fluor sum using
     a 3 slide window. Return a dataframe with the
     derivative, derivative normalized by volume,
     logrith
 
@@ -1486,34 +1285,34 @@
         1D time vector with the mean for 
         each time point
     ci : nd.array
         array(2,bins) with inferior Confidence
         Interval in the first column and the 
     """
     len_data = []
-    time = natsorted(set(df['Time (fps)'].values))
-    mean = np.zeros((len(time),))
-    ci = np.zeros((len(time),2))
+    times = natsorted(set(df['Time (fps)'].values))
+    mean = np.zeros((len(times),))
+    ci = np.zeros((len(times),2))
 
-    for idx,ts in enumerate(time):
+    for idx,ts in enumerate(times):
         temp = df[df['Time (fps)']==ts][column].values
         mean[idx] = np.mean(temp)
         len_data.append(len(df[df['Time (fps)']==ts][column].values))
         if len(temp) > 1:
             ci[idx,:] = ci_bootstrap(temp,conf = conf, method = method, plot = False)
         else:
             ci[idx,:] = [-temp[0],+temp[0]]
 
     if plot_hist:
         plt.hist(len_data)
         plt.ylabel('Amount of time points')
         plt.xlabel('len(derivative)')
         plt.show()
 
-    return time,mean,ci
+    return times,mean,ci
 
 def plot_column_mean(time,mean,ci,column,color = 'Orange', ax = None):
     """
     Plot the colunm mean for the entire experiment.
     Check also 'column_mean()'.
 
     Parameters
```

### Comparing `bacteria-0.1.7/bacteria.egg-info/PKG-INFO` & `bacteria-0.1.8/bacteria.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.7
+Version: 0.1.8
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.7/setup.py` & `bacteria-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.rst", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.1.7',      
+    version = '0.1.8',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

