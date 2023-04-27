# Comparing `tmp/cellmap-1.0.1.dev202304260816-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304260830-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1392757 bytes, number of entries: 6
+Zip file size: 1392785 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    78052 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304260816.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304260816.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304260816.dist-info/RECORD
-6 files, 4527448 bytes uncompressed, 1391871 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    78094 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304260830.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304260830.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304260830.dist-info/RECORD
+6 files, 4527490 bytes uncompressed, 1391899 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304260816.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304260830.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304260816.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304260830.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304260816.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304260830.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1513,15 +1513,15 @@
                     y_data = np.append(y_data,data_exp[:,adata.var.index==gene][pi])
                 plt.scatter(x_data, y_data,color=cmap_(i),alpha=0.05,zorder=0)
                 dynamics_ = adata.uns[gene_dynamics_key][name_][:,adata.var.index==gene]
                 plot_x = np.linspace(0,1,len(dynamics_))
                 plt.plot(plot_x, dynamics_,color='w',lw=8,zorder=1)
                 plt.plot(plot_x, dynamics_,color=cmap_(i),lw=5,label=target_clusters[i],zorder=2)
             plt.legend(bbox_to_anchor=(1.05, 0.5), loc='center left', borderaxespad=0,title='Target', fontsize=fontsize_legend, title_fontsize=fontsize_legend)
-            plt.xticks([0,1],['Source\n(%s)' % source_cluster,'Target'],fontsize=fontsize_label)
+            plt.xticks([0,0.25,0.5,0.75,1],['Source (0)\n(%s)' % source_cluster,'0.25','0.5','0.75','Target (1)'],fontsize=fontsize_label)
             plt.title(gene,fontsize=fontsize_title)
             plt.show()
         else:
             print('Gene \"%s\" was not found' % gene)
```

## Comparing `cellmap-1.0.1.dev202304260816.dist-info/METADATA` & `cellmap-1.0.1.dev202304260830.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304260816
+Version: 1.0.1.dev202304260830
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

