# Comparing `tmp/cellmap-1.0.1.dev202304260830-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304270154-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1392785 bytes, number of entries: 6
+Zip file size: 1393257 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    78094 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304260830.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304260830.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304260830.dist-info/RECORD
-6 files, 4527490 bytes uncompressed, 1391899 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    80570 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304270154.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304270154.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304270154.dist-info/RECORD
+6 files, 4529966 bytes uncompressed, 1392371 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304260830.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304270154.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304260830.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304270154.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304260830.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304270154.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1464,15 +1464,15 @@
             y_data = np.vstack((y_data,data_exp[pi]))
 
         X = x_data[:, np.newaxis]
         poly = PolynomialFeatures(degree=10)
         X_poly = poly.fit_transform(X)
         model = LinearRegression()
         model.fit(X_poly, y_data)
-        plot_x = np.linspace(0,1,n_div)
+        plot_x = np.linspace(0,1,n_div+1)
         gene_dynamics_[source_cluster+'_'+target_clusters[i]] = model.predict(poly.fit_transform(plot_x[:, np.newaxis]))
     adata.uns[gene_dynamics_key] = gene_dynamics_
     print('Done the computation of gene dynamics')
     
 
 
 
@@ -1525,14 +1525,16 @@
 
 
 
 def gene_dynamics_DEG(
         adata,
         source_cluster,
         target_clusters,
+        path_key = 'path',
+        exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
         target_genes = [],
         n_div = 100,
         fontsize_label = 14,
         fontsize_text = 12,
         fontsize_nDEG = 18,
         fontsize_legend = 10,
@@ -1588,15 +1590,15 @@
     #     plt.fill([-0.01*max_val_, DEG_min, DEG_min, -0.01*max_val_], [-0.01*max_val_, -0.01*max_val_, DEG_min, DEG_min], facecolor='lightgray', alpha=0.5,zorder=0)
     #     plt.xlabel(target_clusters[i],fontsize=fontsize_label,color=cmap_(i), fontweight="bold")
     #     plt.ylabel(target_clusters[j],fontsize=fontsize_label,color=cmap_(j), fontweight="bold")
     #     plt.xlim(lim)
     #     plt.ylim(lim)
     #     plt.grid(ls='--')
     def update(t,name_i_,name_j_,max_val_,lim,i,j,k):
-        print('\rcomputing %s vs %s (%d/%d) %d/%d' % (target_clusters[i],target_clusters[j],k,n_plot_,t+1,n_div),end='')
+        print('\rcomputing %s vs %s (%d/%d) %d/%d' % (target_clusters[i],target_clusters[j],k,n_plot_,t+1,n_div+1),end='')
         idx_DEG_i_ = np.arange(adata.shape[1])[(gene_dynamics_[name_j_][t] < gene_dynamics_[name_i_][t] - DEG_rate) & (gene_dynamics_[name_i_][t] > DEG_min)]
         idx_DEG_j_ = np.arange(adata.shape[1])[(gene_dynamics_[name_i_][t] < gene_dynamics_[name_j_][t] - DEG_rate) & (gene_dynamics_[name_j_][t] > DEG_min)]
         idx_DEG_i_ = idx_DEG_i_[np.argsort(gene_dynamics_[name_i_][t][idx_DEG_i_]- DEG_rate - gene_dynamics_[name_j_][t][idx_DEG_i_])[::-1]]
         idx_DEG_j_ = idx_DEG_j_[np.argsort(gene_dynamics_[name_j_][t][idx_DEG_j_]- DEG_rate - gene_dynamics_[name_i_][t][idx_DEG_j_])[::-1]]
         if len(idx_DEG_i_) > max_num_annotations:
             idx_DEG_ann_i_ = idx_DEG_i_[:max_num_annotations]
         else:
@@ -1629,40 +1631,92 @@
             texts = np.append(texts,tx_)
         if len(target_genes):
             for gene_ in target_genes:
                 idx_gene_ = adata.var.index == gene_
                 ax[0].scatter(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],s=20,color="red",zorder=2)
                 tx_ = ax[0].text(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],gene_,color="r",zorder=2,fontsize=fontsize_text)
                 texts = np.append(texts,tx_)
-        legend_i_ = target_clusters[i]+'\n'
+        legend_i_ = ''
         for g in np.arange(adata.shape[1])[idx_DEG_leg_i_]: legend_i_ += '(%.02f, %.02f)  %s\n' % (gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g])
-        legend_j_ = target_clusters[j]+'\n'
+        legend_j_ = ''
         for g in np.arange(adata.shape[1])[idx_DEG_leg_j_]: legend_j_ += '(%.02f, %.02f)  %s\n' % (gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g])
         if adjusttext: adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'),ax=ax[0])
         ax[0].text(0.9*(lim[1]-lim[0])+lim[0], 0.1*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_i_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(i), fontweight="bold",zorder=3)
         ax[0].text(0.1*(lim[1]-lim[0])+lim[0], 0.9*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_j_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(j), fontweight="bold",zorder=3)
         ax[0].fill_between(lim, lim-DEG_rate, lim+DEG_rate, facecolor='lightgray',  alpha=0.5,zorder=0)
         ax[0].fill([-0.01*max_val_, DEG_min, DEG_min, -0.01*max_val_], [-0.01*max_val_, -0.01*max_val_, DEG_min, DEG_min], facecolor='lightgray', alpha=0.5,zorder=0)
         ax[0].set_xlabel(target_clusters[i],fontsize=fontsize_label,color=cmap_(i), fontweight="bold")
         ax[0].set_ylabel(target_clusters[j],fontsize=fontsize_label,color=cmap_(j), fontweight="bold")
         ax[0].set_xlim(lim)
         ax[0].set_ylim(lim)
         ax[0].grid(ls='--')
-        ax[1].text(0.0,1,legend_i_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3)
-        ax[1].axis('off')
-        ax[1].text(0.5,1,legend_j_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3)
+        ax[1].text(0.0,1,target_clusters[i], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3, fontweight="bold")
+        ax[1].text(0.0,0.97,legend_i_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3)
+        ax[1].text(0.5,1,target_clusters[j], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3, fontweight="bold")
+        ax[1].text(0.5,0.97,legend_j_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3)
         ax[1].axis('off')
     k = 0
     for i in range(len(target_clusters)):
         for j in range(i+1,len(target_clusters)):
             name_i_ = source_cluster+'_'+target_clusters[i]
             name_j_ = source_cluster+'_'+target_clusters[j]
             fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
             max_val_ = max(np.max(gene_dynamics_[name_i_]),np.max(gene_dynamics_[name_j_]))
             lim = np.array([-0.01*max_val_,1.01*max_val_])
             k = k+1
-            ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div)
+            ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
             file_name = 'DEG_anoime_%s_%s.gif' % (target_clusters[i],target_clusters[j]) if save_dir == None else '%s/DEG_anoime_%s_%s.gif' % (save_dir,target_clusters[i],target_clusters[j])
             IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
             print('\nSaving gif animation as %s' % file_name)
             ani.save(file_name)
-            plt.close()
+            plt.close()
+
+def bifurcation_diagram(
+        adata,
+        source_cluster,
+        target_clusters,
+        path_key = 'path',
+        exp_key = None,
+        gene_dynamics_key = 'gene_dynamics',
+        n_div = 100,
+        fontsize_label = 14,
+        adjusttext =False,
+    ):
+
+    if gene_dynamics_key not in adata.uns.keys():
+        gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
+
+
+    vlines = [0,0.2,0.4,0.6,0.8,1]
+    vline_labels = np.append(np.append('Source (0)',np.array(vlines)[1:-1]),'Target (1)')
+
+    name_i_ = source_cluster + '_' + target_clusters[0]
+    samples_ = np.empty([len(target_clusters),adata.uns['gene_dynamics'][name_i_].shape[0],adata.uns['gene_dynamics'][name_i_].shape[1]],dtype=float)
+    for i in range(len(target_clusters)):
+        name_i_ = source_cluster + '_' + target_clusters[i]
+        samples_[i] = adata.uns['gene_dynamics'][name_i_]
+    samples_pca_ = sklearn.decomposition.PCA().fit_transform(np.concatenate(samples_))
+    # for i in range(n_div):
+    #     idx_ = np.arange(i,len(target_clusters)*n_div,n_div)
+    #     samples_pca_[idx_] = samples_pca_[idx_] - samples_pca_[i]
+
+    fig,ax = plt.subplots(figsize=(12,4))
+    ax.text(0,samples_pca_[0,0],source_cluster+' ',fontsize=fontsize_label,va='center',ha='right')
+    texts = []
+    for j in range(len(target_clusters)):
+        y_ = samples_pca_[j*n_div:(j+1)*n_div,1]
+        # y_[0] = 0
+        ax.plot(np.linspace(0,1,n_div),y_,lw=5,zorder=2)
+        texts = np.append(texts,ax.text(1,y_[-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left'))
+    if adjusttext: adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'))
+    for vl in vlines:
+        ax.axvline(vl,color='k',ls='--',lw=1,zorder=0)
+    ax.tick_params(axis='x', which='both', top=True)
+    ax.spines['right'].set_visible(False)
+    ax.spines['left'].set_visible(False)
+    ax.spines['top'].set_visible(False)
+    ax.spines['bottom'].set_visible(False)
+    ax.xaxis.set_label_position('top')
+    ax.xaxis.tick_top()
+    ax.yaxis.set_visible(False)
+    ax.set_xticks(vlines)
+    ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
```

## Comparing `cellmap-1.0.1.dev202304260830.dist-info/METADATA` & `cellmap-1.0.1.dev202304270154.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304260830
+Version: 1.0.1.dev202304270154
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

