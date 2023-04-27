# Comparing `tmp/pymef-1.3.4.tar.gz` & `tmp/pymef-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymef-1.3.4.tar", last modified: Wed Mar  2 14:06:15 2022, max compression
+gzip compressed data, was "pymef-1.3.5.tar", last modified: Thu Apr 27 07:10:52 2023, max compression
```

## Comparing `pymef-1.3.4.tar` & `pymef-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-03-02 14:06:15.465401 pymef-1.3.4/
--rw-r--r--   0 runner     (501) staff       (20)     1073 2022-03-02 14:05:48.000000 pymef-1.3.4/LICENSE.txt
--rw-r--r--   0 runner     (501) staff       (20)      732 2022-03-02 14:06:15.464985 pymef-1.3.4/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-03-02 14:06:15.460492 pymef-1.3.4/pymef/
--rw-r--r--   0 runner     (501) staff       (20)       35 2022-03-02 14:05:48.000000 pymef-1.3.4/pymef/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11175 2022-03-02 14:05:48.000000 pymef-1.3.4/pymef/mef_constants.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-03-02 14:06:15.463903 pymef-1.3.4/pymef/mef_file/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-03-02 14:05:48.000000 pymef-1.3.4/pymef/mef_file/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)   172459 2022-03-02 14:05:48.000000 pymef-1.3.4/pymef/mef_file/pymef3_file.c
--rw-r--r--   0 runner     (501) staff       (20)    64395 2022-03-02 14:05:48.000000 pymef-1.3.4/pymef/mef_session.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-03-02 14:06:15.463097 pymef-1.3.4/pymef.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      732 2022-03-02 14:06:15.000000 pymef-1.3.4/pymef.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      325 2022-03-02 14:06:15.000000 pymef-1.3.4/pymef.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-03-02 14:06:15.000000 pymef-1.3.4/pymef.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-03-02 14:06:15.000000 pymef-1.3.4/pymef.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)        6 2022-03-02 14:06:15.000000 pymef-1.3.4/pymef.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2022-03-02 14:06:15.000000 pymef-1.3.4/pymef.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      116 2022-03-02 14:05:48.000000 pymef-1.3.4/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-03-02 14:06:15.465522 pymef-1.3.4/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1692 2022-03-02 14:05:48.000000 pymef-1.3.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 07:10:52.154392 pymef-1.3.5/
+-rw-r--r--   0 runner     (501) staff       (20)     1073 2023-04-27 07:10:19.000000 pymef-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner     (501) staff       (20)      732 2023-04-27 07:10:52.153990 pymef-1.3.5/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 07:10:52.147986 pymef-1.3.5/pymef/
+-rw-r--r--   0 runner     (501) staff       (20)       35 2023-04-27 07:10:19.000000 pymef-1.3.5/pymef/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11175 2023-04-27 07:10:19.000000 pymef-1.3.5/pymef/mef_constants.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 07:10:52.152217 pymef-1.3.5/pymef/mef_file/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-27 07:10:19.000000 pymef-1.3.5/pymef/mef_file/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)   172529 2023-04-27 07:10:19.000000 pymef-1.3.5/pymef/mef_file/pymef3_file.c
+-rw-r--r--   0 runner     (501) staff       (20)    66373 2023-04-27 07:10:19.000000 pymef-1.3.5/pymef/mef_session.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-27 07:10:52.151363 pymef-1.3.5/pymef.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      732 2023-04-27 07:10:51.000000 pymef-1.3.5/pymef.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      325 2023-04-27 07:10:52.000000 pymef-1.3.5/pymef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-27 07:10:51.000000 pymef-1.3.5/pymef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-27 07:10:51.000000 pymef-1.3.5/pymef.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)        6 2023-04-27 07:10:51.000000 pymef-1.3.5/pymef.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2023-04-27 07:10:51.000000 pymef-1.3.5/pymef.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      116 2023-04-27 07:10:19.000000 pymef-1.3.5/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-27 07:10:52.154520 pymef-1.3.5/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2023-04-27 07:10:19.000000 pymef-1.3.5/setup.py
```

### Comparing `pymef-1.3.4/LICENSE.txt` & `pymef-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymef-1.3.4/PKG-INFO` & `pymef-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymef
-Version: 1.3.4
+Version: 1.3.5
 Summary: Wrapper for MEF (multiscale electrophysiology format)
 Home-page: https://github.com/msel-source/pymef
 Author: Jan Cimbalnik
 Author-email: jan.cimbalnik@fnusa.cz, jan.cimbalnik@mayo.edu
 License: Apache 2.0
 Description: UNKNOWN
 Keywords: MEF Mayo electrophysiology
```

### Comparing `pymef-1.3.4/pymef/mef_constants.py` & `pymef-1.3.5/pymef/mef_constants.py`

 * *Files identical despite different names*

### Comparing `pymef-1.3.4/pymef/mef_file/pymef3_file.c` & `pymef-1.3.5/pymef/mef_file/pymef3_file.c`

 * *Files 1% similar despite different names*

```diff
@@ -2581,14 +2581,15 @@
     PyArrayObject *py_array_out;
 
     // Helpers
     TIME_SERIES_INDEX     *tsi;
 
     si8     number_of_entries;
     si8     prev_time, prev_sample, start_time, start_sample, samp_time_diff, seg_start_sample;
+    ui4     n_samples;
     sf8     fs;
     si8     *numpy_arr_data;
     npy_intp dims[2];
 
     si4     i;
     
     // initialize Numpy
@@ -2610,28 +2611,29 @@
 
     for(i = 0; i < number_of_entries; i++){
 
 
         start_time = tsi->start_time;
         start_sample = tsi->start_sample;
         start_sample += seg_start_sample;
+        n_samples = tsi->number_of_samples;
 
         // Have we found a discontinuity?
         numpy_arr_data = (si8 *) PyArray_GETPTR2(py_array_out, 0, i);
         samp_time_diff = (si8) (((start_time - prev_time) - (1e6 * (start_sample - prev_sample)) / fs));
         if (samp_time_diff < (si8) (1e6/fs))
             samp_time_diff = 0;
         if  ((samp_time_diff != 0) | (i == 0)) // First entry is dicontinuity by definition
             *numpy_arr_data = 1;
         else
             *numpy_arr_data = 0;
 
-        // Discontinuity duration
+        // Number of samples of the block
         numpy_arr_data = (si8 *) PyArray_GETPTR2(py_array_out, 1, i);
-        *numpy_arr_data = (si8) samp_time_diff;
+        *numpy_arr_data = (si8) n_samples;
 
         // Start sample
         numpy_arr_data = (si8 *) PyArray_GETPTR2(py_array_out, 2, i);
         *numpy_arr_data = (si8) start_sample;
 
         // Start time
         numpy_arr_data = (si8 *) PyArray_GETPTR2(py_array_out, 3, i);
```

### Comparing `pymef-1.3.4/pymef/mef_session.py` & `pymef-1.3.5/pymef/mef_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,37 +360,37 @@
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
 
             if 'text' in record.keys():
                 record_str = record['text']+'\0'
                 body_dtype = create_note_dtype(len(record_str))
                 body_arr = np.zeros(1, body_dtype)
-                body_arr['text'] = record_str.encode()
+                body_arr['text'] = record_str.encode('utf8') + b'\x00'
 
         elif record_type == 'SyLg':
             hdr_arr['type_string'] = b'SyLg'
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
 
             if 'text' in record.keys():
                 record_str = record['text']+'\0'
                 body_dtype = create_sylg_dtype(len(record_str))
                 body_arr = np.zeros(1, body_dtype)
-                body_arr['text'] = record_str.encode()
+                body_arr['text'] = record_str.encode('utf8') + b'\x00'
 
         elif record_type == 'EDFA':
             hdr_arr['type_string'] = b'EDFA'
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
 
             if 'text' in record.keys():
                 record_str = record['text']+'\0'
                 body_dtype = create_edfa_dtype(len(record_str))
                 body_arr = np.zeros(1, body_dtype)
-                body_arr['text'] = record_str.encode()
+                body_arr['text'] = record_str.encode('utf8') + b'\x00'
             if 'duration' in record.keys():
                 body_arr['duration'] = record['duration']
 
         elif record_type == 'LNTP':
             hdr_arr['type_string'] = b'LNTP'
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
@@ -409,15 +409,15 @@
             body_dtype = create_csti_dtype()
             d_type_keys = [x[0] for x in body_dtype.descr]
             body_arr = np.zeros(1, body_dtype)
             for key in record.keys():
                 if key in ['type', 'time']:
                     continue
                 if isinstance(record[key], str):
-                    body_arr[key] = record[key].encode()
+                    body_arr[key] = record[key].encode('utf8') + b'\x00'
                 else:
                     body_arr[key] = record[key]
 
         elif record_type == 'ESti':
             hdr_arr['type_string'] = b'ESti'
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
@@ -425,15 +425,15 @@
             body_dtype = create_esti_dtype()
             d_type_keys = [x[0] for x in body_dtype.descr]
             body_arr = np.zeros(1, body_dtype)
             for key in record.keys():
                 if key in ['type', 'time']:
                     continue
                 if isinstance(record[key], str):
-                    body_arr[key] = record[key].encode()
+                    body_arr[key] = record[key].encode('utf8') + b'\x00'
                 else:
                     body_arr[key] = record[key]
 
         elif record_type == 'Seiz':
             hdr_arr['type_string'] = b'Seiz'
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
@@ -449,15 +449,15 @@
                     subbody_arr = np.zeros(len(record['channels']),
                                            subbody_dtype)
                     subbody_arr['name'] = [x['name'] for x in channels]
                     subbody_arr['onset'] = [x['onset'] for x in channels]
                     subbody_arr['offset'] = [x['offset'] for x in channels]
                 else:
                     if isinstance(record[key], str):
-                        body_arr[key] = record[key].encode()
+                        body_arr[key] = record[key].encode('utf8') + b'\x00'
                     else:
                         body_arr[key] = record[key]
 
         elif record_type == 'Curs':
             hdr_arr['type_string'] = b'Curs'
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
@@ -465,15 +465,15 @@
             body_dtype = create_curs_dtype()
             d_type_keys = [x[0] for x in body_dtype.descr]
             body_arr = np.zeros(1, body_dtype)
             for key in record.keys():
                 if key in ['type', 'time']:
                     continue
                 if isinstance(record[key], str):
-                    body_arr[key] = record[key].encode()
+                    body_arr[key] = record[key].encode('utf8') + b'\x00'
                 else:
                     body_arr[key] = record[key]
 
         elif record_type == 'Epoc':
             hdr_arr['type_string'] = b'Epoc'
             if 'time' in record.keys():
                 hdr_arr['time'] = record['time']
@@ -481,15 +481,15 @@
             body_dtype = create_epoc_dtype()
             d_type_keys = [x[0] for x in body_dtype.descr]
             body_arr = np.zeros(1, body_dtype)
             for key in record.keys():
                 if key in ['type', 'time']:
                     continue
                 if isinstance(record[key], str):
-                    body_arr[key] = record[key].encode()
+                    body_arr[key] = record[key].encode('utf8') + b'\x00'
                 else:
                     body_arr[key] = record[key]
 
         else:
             raise ValueError("Unrecognized record type:'%s'" % record_type)
 
         record_np_dict = {'record_header': hdr_arr,
@@ -924,72 +924,109 @@
         if not any([isinstance(x, int) for x in slice_start_stop]):
             raise ValueError("Start and stop must be integers.")
 
         channels_dict = self.session_md['time_series_channels']
 
         segment_n = 0
         for channel, ch_md in channels_dict.items():
+            
+            toc = self.get_channel_toc(channel)
+            
+            toc_start_idx = np.where(toc[0] == 1)[0]
+            toc_start_times = toc[-1, toc_start_idx]
+            toc_stop_times = toc[-1, toc_start_idx[1:]-1] + ((toc[1, toc_start_idx[1:]-1]/5000)*1e6).astype(int)
+            toc_stop_times = np.concatenate([toc_stop_times, self.session_md['session_specific_metadata']['latest_end_time']])
+            
+            toc_slices = np.stack([toc_start_times, toc_stop_times], axis=1)
+            toc_slices = toc_slices[((toc_slices[:, 1] > slice_start_stop[0])
+                                     & (toc_slices[:, 0] < slice_start_stop[1]))]
+            
+            toc_slices[0, 0] = slice_start_stop[0]
+            toc_slices[-1, 1] = slice_start_stop[1]
 
             segment_path = (slice_session_path+channel+'.timd/'
                             + channel+'-'+str(segment_n).zfill(6)+'.segd/')
+            
+            os.makedirs(segment_path, exist_ok=True)
 
             tmet_path = (segment_path+channel+'-'+str(segment_n).zfill(6)
                          + '.tmet')
 
             if os.path.exists(tmet_path):
                 raise RuntimeError('Metadata file '+tmet_path
                                    + ' already exists!')
 
-            os.makedirs(segment_path, exist_ok=True)
-
             section_2 = ch_md['section_2'].copy()
 
-            # Zero out the machine generated fields
-            section_2['maximum_native_sample_value'] = 0.0
-            section_2['minimum_native_sample_value'] = 0.0
-            section_2['number_of_blocks'] = 0
-            section_2['maximum_block_bytes'] = 0
-            section_2['maximum_block_samples'] = 0
-            section_2['maximum_difference_bytes'] = 0
-            section_2['block_interval'] = 0
-            section_2['maximum_contiguous_blocks'] = 0
-            section_2['maximum_contiguous_block_bytes'] = 0
-            section_2['maximum_contiguous_samples'] = 0
-            section_2['number_of_samples'] = 0
-
-            section_3 = ch_md['section_3'].copy()
-
-            write_mef_ts_metadata(segment_path,
-                                  password_1,
-                                  password_2,
-                                  slice_start_stop[0],
-                                  slice_start_stop[1],
-                                  section_2,
-                                  section_3)
-
-            data = self.read_ts_channels_uutc(channel, slice_start_stop)
-
-            tdat_path = (segment_path+channel+'-'+str(segment_n).zfill(6)
-                         + '.tdat')
-
-            if os.path.exists(tdat_path):
-                raise RuntimeError('Data file '+tdat_path+' already exists!')
-
             if samps_per_mef_block is None:
                 spmb = int(section_2['sampling_frequency'][0])
             else:
                 spmb = samps_per_mef_block
 
-            # lossy compression flag - not used
-            write_mef_ts_data_and_indices(segment_path,
+            is_first_write = True
+            
+            for ss in toc_slices:
+
+                if is_first_write is True:
+                
+                    # Zero out the machine generated fields
+                    section_2['maximum_native_sample_value'] = 0.0
+                    section_2['minimum_native_sample_value'] = 0.0
+                    section_2['number_of_blocks'] = 0
+                    section_2['maximum_block_bytes'] = 0
+                    section_2['maximum_block_samples'] = 0
+                    section_2['maximum_difference_bytes'] = 0
+                    section_2['block_interval'] = 0
+                    section_2['maximum_contiguous_blocks'] = 0
+                    section_2['maximum_contiguous_block_bytes'] = 0
+                    section_2['maximum_contiguous_samples'] = 0
+                    section_2['number_of_samples'] = 0
+                
+                    section_3 = ch_md['section_3'].copy()
+                    section_3['recording_time_offset'] = slice_start_stop[0]    
+                
+                    write_mef_ts_metadata(segment_path,
                                           password_1,
                                           password_2,
-                                          spmb,
-                                          data.astype('int32'),
-                                          0)
+                                          slice_start_stop[0],
+                                          slice_start_stop[1],
+                                          section_2,
+                                          section_3)
+                
+                    data = self.read_ts_channels_uutc(channel, [int(x) for x in ss])
+                
+                    tdat_path = (segment_path+channel+'-'+str(segment_n).zfill(6)
+                                 + '.tdat')
+                
+                    if os.path.exists(tdat_path):
+                        raise RuntimeError('Data file '+tdat_path+' already exists!')
+                
+                    
+                
+                    # lossy compression flag - not used
+                    write_mef_ts_data_and_indices(segment_path,
+                                                  password_1,
+                                                  password_2,
+                                                  spmb,
+                                                  data.astype('int32'),
+                                                  0)
+                    
+                    is_first_write = False
+                        
+                else:
+                    
+                    data = self.read_ts_channels_uutc(channel, [int(x) for x in ss])
+                    append_ts_data_and_indices(segment_path,
+                                               password_1,
+                                               password_2,
+                                               int(ss[0]),
+                                               int(ss[1]),
+                                               spmb,
+                                               data.astype('int32'),
+                                               True)
 
     # ----- Data reading functions -----
     def _create_dict_record(self, np_record):
         """
         Create python dictionary from record dictionary with numpy arrays.
 
         Parameters
@@ -1184,35 +1221,31 @@
             Channel to calculate TOC on
 
         Returns
         -------
         TOC: np.array
             Array with
               - [0,:] = discontinuity flags
-              - [1,:] = discont lengths
+              - [1,:] = n block samples
               - [2,:] = start samples
               - [3,:] = start uutc times
         """
 
         channel_md = self.session_md['time_series_channels'][channel]
         toc = np.empty([4, 0], dtype='int64')
-        fsamp = channel_md['section_2']['sampling_frequency']
 
         # Sort the segments to eliminate dictionary randomness
         segs = list(channel_md['segments'].keys())
         segs.sort()
         for segment_name in segs:
             seg_toc = channel_md['segments'][segment_name]['TOC']
 
             # Join into channel TOC
             toc = np.concatenate([toc, seg_toc], axis=1)
 
-        # Once we have all segments get lenghts (differnces between segments)
-        toc[1, 1::] = (((np.diff(toc[3, :]) / 1e6)
-                        - (np.diff(toc[2, :]) / fsamp)) * 1e6)
 
         return toc
 
     def read_ts_channels_sample(self, channel_map, sample_map, process_n=None):
         """
         Reads desired channels in desired sample segment
```

### Comparing `pymef-1.3.4/pymef.egg-info/PKG-INFO` & `pymef-1.3.5/pymef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymef
-Version: 1.3.4
+Version: 1.3.5
 Summary: Wrapper for MEF (multiscale electrophysiology format)
 Home-page: https://github.com/msel-source/pymef
 Author: Jan Cimbalnik
 Author-email: jan.cimbalnik@fnusa.cz, jan.cimbalnik@mayo.edu
 License: Apache 2.0
 Description: UNKNOWN
 Keywords: MEF Mayo electrophysiology
```

### Comparing `pymef-1.3.4/setup.py` & `pymef-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # the c extension module
 MEF_FILE_EXT = Extension("pymef.mef_file.pymef3_file",
                          ["pymef/mef_file/pymef3_file.c"],
                          include_dirs=["meflib/meflib"],
                          extra_compile_args=['-O3'])
 
 setup(name="pymef",
-      version='1.3.4',
+      version='1.3.5',
       description='Wrapper for MEF (multiscale electrophysiology format)',
       url='https://github.com/msel-source/pymef',
       author='Jan Cimbalnik',
       author_email='jan.cimbalnik@fnusa.cz, jan.cimbalnik@mayo.edu',
       license='Apache 2.0',
       platforms=['Linux', 'MaxOSX', 'Windows'],
       keywords='MEF Mayo electrophysiology',
```

