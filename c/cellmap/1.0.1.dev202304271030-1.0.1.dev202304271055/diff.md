# Comparing `tmp/cellmap-1.0.1.dev202304271030-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304271055-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1393782 bytes, number of entries: 6
+Zip file size: 1393806 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    85581 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271030.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271030.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304271030.dist-info/RECORD
-6 files, 4534977 bytes uncompressed, 1392896 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    85706 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271055.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271055.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304271055.dist-info/RECORD
+6 files, 4535102 bytes uncompressed, 1392920 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304271030.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304271055.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304271030.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304271055.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304271030.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304271055.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1731,40 +1731,42 @@
         target_clusters,
         path_key = 'path',
         exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
         n_div = 100,
         fontsize_label = 14,
         adjusttext =False,
-        PC = 0,
+        PC = 1,
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
         gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
 
 
     vlines = [0,0.2,0.4,0.6,0.8,1]
     vline_labels = np.append(np.append('Source (0)',np.array(vlines)[1:-1]),'Target (1)')
 
     name_i_ = source_cluster + '_' + target_clusters[0]
     samples_ = np.empty([len(target_clusters),adata.uns['gene_dynamics'][name_i_].shape[0],adata.uns['gene_dynamics'][name_i_].shape[1]],dtype=float)
     for i in range(len(target_clusters)):
         name_i_ = source_cluster + '_' + target_clusters[i]
         samples_[i] = adata.uns['gene_dynamics'][name_i_]
-    samples_pca_ = sklearn.decomposition.PCA(n_components=2).fit_transform(np.concatenate(samples_))
+    # samples_pca_ = sklearn.decomposition.PCA(n_components=2).fit_transform(np.concatenate(samples_))
+    pca_ = sklearn.decomposition.PCA().fit(samples_[:,-1])
+    samples_pca_ = pca_.transform(np.concatenate(samples_))
     # for i in range(n_div):
     #     idx_ = np.arange(i,len(target_clusters)*n_div,n_div)
     #     samples_pca_[idx_] = samples_pca_[idx_] - samples_pca_[i]
 
     fig,ax = plt.subplots(figsize=(12,4))
     ax.text(0,samples_pca_[0,0],source_cluster+' ',fontsize=fontsize_label,va='center',ha='right')
     texts = []
     for j in range(len(target_clusters)):
-        y_ = samples_pca_[j*(n_div+1):(j+1)*(n_div+1),PC]
-        ax.plot(np.linspace(0,1,n_div),y_,lw=5,zorder=2)
+        y_ = samples_pca_[j*(n_div+1):(j+1)*(n_div+1),PC-1]
+        ax.plot(np.linspace(0,1,n_div+1),y_,lw=5,zorder=2)
         texts = np.append(texts,ax.text(1,y_[-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left'))
     if adjusttext: adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'))
     for vl in vlines:
         ax.axvline(vl,color='k',ls='--',lw=1,zorder=0)
     ax.tick_params(axis='x', which='both', top=True)
     ax.spines['right'].set_visible(False)
     ax.spines['left'].set_visible(False)
```

## Comparing `cellmap-1.0.1.dev202304271030.dist-info/METADATA` & `cellmap-1.0.1.dev202304271055.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304271030
+Version: 1.0.1.dev202304271055
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

