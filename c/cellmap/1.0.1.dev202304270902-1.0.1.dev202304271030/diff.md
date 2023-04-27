# Comparing `tmp/cellmap-1.0.1.dev202304270902-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304271030-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1393280 bytes, number of entries: 6
+Zip file size: 1393782 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    80674 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304270902.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304270902.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304270902.dist-info/RECORD
-6 files, 4530070 bytes uncompressed, 1392394 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    85581 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1817 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271030.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304271030.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304271030.dist-info/RECORD
+6 files, 4534977 bytes uncompressed, 1392896 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304270902.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304271030.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304270902.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304271030.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304270902.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304271030.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -258,35 +258,23 @@
     # edge_vel = np.sum(0.5*(V1_p+V2_p),axis=1)/Dis/np.sum(idx_vel)
     edge_vel = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis/np.sum(idx_vel)
     if normalization:
         edge_vel_norm = np.linalg.norm(edge_vel)
         if edge_vel_norm > 0: edge_vel= edge_vel/edge_vel_norm
     return edge_vel
 
-def solve_vorticity_streamline(
-    div_mat,
-    edge_vel,
-    vorticity_key = 'vorticity',
-    stream_key = 'stream_line',
-):
-    vorticity_ = np.dot(div_mat,edge_vel)
-    stream_line_ = -np.dot(lap_inv,vorticity_)
-    adata.obs[vorticity_key] = vorticity_
-    adata.obs[stream_key] = stream_line_-np.min(stream_line_)
-
-
 def Hodge_decomposition(
     adata,
     basis = 'umap',
     vkey  = 'velocity',
     exp_key = None,
     potential_key = 'potential',
     rotation_key = 'rotation',
     vorticity_key = 'vorticity',
-    streamline_key = 'stream_line',
+    streamfunc_key = 'streamfunc',
     graph_key = 'CellMap_graph',
     edge_vel_key = 'edge_velocity',
     graph_method = 'Delauney',
     HD_rate = 0.0,
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
@@ -309,19 +297,19 @@
     exp_key,vkey,basis = kwargs_arg['exp_key'],kwargs_arg['vkey'],kwargs_arg['basis']
     
     exp_2d_key_ = 'X_%s' % basis
     vel_2d_key_ = '%s_%s' % (vkey,basis)
     pot_vkey_ = '%s_%s_%s' % (potential_key,vkey,basis)
     rot_vkey_ = '%s_%s_%s' % (rotation_key,vkey,basis)
     vor_key_ = '%s_%s' % (vorticity_key,basis)
-    sl_key_ = '%s_%s' % (streamline_key,basis)
+    sl_key_ = '%s_%s' % (streamfunc_key,basis)
     pot_vor_key_ = '%s_%s_%s' % (potential_key,vorticity_key,basis)
-    pot_sl_key_ = '%s_%s_%s' % (potential_key,streamline_key,basis)
+    pot_sl_key_ = '%s_%s_%s' % (potential_key,streamfunc_key,basis)
     rot_vor_key_ = '%s_%s_%s' % (rotation_key,vorticity_key,basis)
-    rot_sl_key_ = '%s_%s_%s' % (rotation_key,streamline_key,basis)
+    rot_sl_key_ = '%s_%s_%s' % (rotation_key,streamfunc_key,basis)
     
     if exp_key == None:
         if scipy.sparse.issparse(adata.X):
             exp_HD = adata.X.toarray()
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
@@ -424,34 +412,34 @@
     #     lap[i,:] = 0
     #     lap[i,i] = 1
     # lap_inv_ = np.linalg.pinv(lap)
     ## Solve vorticity & stream line
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target,normalization=False))
     source_term_ = vorticity_
     # source_term_[idx_bd_] = 100
-    stream_line_ = -np.dot(lap_inv_,source_term_)
-    # vorticity_ = -np.dot(lap,stream_line_)
+    streamfunc_ = -np.dot(lap_inv_,source_term_)
+    # vorticity_ = -np.dot(lap,streamfunc_)
     adata.obs[vor_key_] = vorticity_
-    adata.obs[sl_key_]  = stream_line_-np.min(stream_line_)
+    adata.obs[sl_key_]  = streamfunc_-np.min(streamfunc_)
 
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target,normalization=False))
     source_term_ = vorticity_
     # source_term_[idx_bd_] = 100
-    stream_line_ = -np.dot(lap_inv_,source_term_)
-    # vorticity_ = -np.dot(lap,stream_line_)
+    streamfunc_ = -np.dot(lap_inv_,source_term_)
+    # vorticity_ = -np.dot(lap,streamfunc_)
     adata.obs[pot_vor_key_] = vorticity_
-    adata.obs[pot_sl_key_] = stream_line_-np.min(stream_line_)
+    adata.obs[pot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target,normalization=False))
     source_term_ = vorticity_
     # source_term_[idx_bd_] = 100
-    stream_line_ = -np.dot(lap_inv_,source_term_)
-    # vorticity_ = -np.dot(lap,stream_line_)
+    streamfunc_ = -np.dot(lap_inv_,source_term_)
+    # vorticity_ = -np.dot(lap,streamfunc_)
     adata.obs[rot_vor_key_] = vorticity_
-    adata.obs[rot_sl_key_] = stream_line_-np.min(stream_line_)
+    adata.obs[rot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
     adata.obs[rotation_key] = np.array([np.mean(np.hstack((rot_flow_[source==i],-rot_flow_[target==i]))) for i in range(adata.shape[0])])
 
     ## Contribution ratio
     log_ = {}
     log_["Contribution_ratio"] = {}
     norm_grad = np.linalg.norm(pot_flow_)
@@ -720,15 +708,15 @@
             texts.append(txt)
         # adjust_text(texts)
 
 
 def view_stream_line(
     adata,
     basis = 'umap',
-    contour_key = 'stream_line',
+    contour_key = 'streamfunc',
     cluster_key = 'clusters',
     potential_key = 'potential',
     rotation_key = 'rotation',
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
@@ -1166,15 +1154,15 @@
     filename = 'CellMap',
     basis = 'umap',
     vkey  = 'velocity',
     exp_key = None,
     potential_key = 'potential',
     rotation_key = 'rotation',
     vorticity_key = 'vorticity',
-    streamline_key = 'stream_line',
+    streamfunc_key = 'streamfunc',
     cluster_key = 'clusters',
     obs_key = None,
     genes = None,
     use_HVG = True,
     n_HVG = 10,
 ):
     kwargs = check_arguments(adata,basis=basis,potential_key=potential_key,cluster_key=cluster_key,obs_key=obs_key,genes=genes,expression_key=exp_key)
@@ -1182,19 +1170,19 @@
     basis_key = 'X_%s' % basis
     vkey_ = '%s_%s' % (vkey,basis)
     pot_key_ = '%s' % (potential_key)
     rot_key_ = '%s' % (rotation_key)
     pot_vkey_ = '%s_%s_%s' % (potential_key,vkey,basis)
     rot_vkey_ = '%s_%s_%s' % (rotation_key,vkey,basis)
     vol_key_ = '%s_%s_%s' % (potential_key,vorticity_key,basis)
-    sl_key_ = '%s_%s_%s' % (potential_key,streamline_key,basis)
+    sl_key_ = '%s_%s_%s' % (potential_key,streamfunc_key,basis)
     pot_vol_key_ = '%s_%s_%s' % (potential_key,vorticity_key,basis)
-    pot_sl_key_ = '%s_%s_%s' % (potential_key,streamline_key,basis)
+    pot_sl_key_ = '%s_%s_%s' % (potential_key,streamfunc_key,basis)
     rot_vol_key_ = '%s_%s_%s' % (rotation_key,vorticity_key,basis)
-    rot_sl_key_ = '%s_%s_%s' % (rotation_key,streamline_key,basis)
+    rot_sl_key_ = '%s_%s_%s' % (rotation_key,streamfunc_key,basis)
     
     
     if exp_key == None:
         if scipy.sparse.issparse(adata.X): data_exp = adata.X.toarray()
         else: data_exp = adata.X
     else:
         data_exp = adata.layers[exp_key]
@@ -1330,37 +1318,42 @@
 
 
 def view_trajectory(
     adata,
     source_cluster,
     target_clusters,
     n_cells = 50,
-    register = 100,
+    register = 1,
     basis = 'umap',
     potential_key = 'potential',
     cluster_key = 'clusters',
+    streamfunc_key = 'streamfunc',
     graph_method = 'Delauney',
     path_key = 'path',
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
+    figsize = (10,8),
 ):
 
     kwargs_arg = check_arguments(adata, verbose = True, basis=basis)
     basis = kwargs_arg['basis']
 
     if sum(adata.obs[cluster_key].values == source_cluster) == 0:
         raise KeyError('Cluster %s was not found' % source_cluster)
     for trg_ in target_clusters:
         if sum(adata.obs[cluster_key].values == source_cluster) == 0:
             raise KeyError('Cluster %s was not found' % trg_)
 
     basis_key = 'X_%s' % basis
+    pot_sl_key_ = '%s_%s_%s' % (potential_key,streamfunc_key,basis)
+
     data_pos = adata.obsm[basis_key]
+    streamfunc_ = adata.obs[pot_sl_key_]
 
     ## Compute graph and edge velocities
     if graph_method == 'Delauney':
         tri_ = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='triangles')[0]
         source, target = create_graph(data_pos,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='edges')
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
@@ -1369,34 +1362,25 @@
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
         distances, indices = distances[:,1:], indices[:,1:]
         source = np.ravel(np.repeat(np.arange(data_pos.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
     
-    G = nx.Graph()
-    for i in range(len(source)):
-        G.add_edge(source[i],target[i],w=np.linalg.norm(data_pos[source[i]]-data_pos[target[i]]))
-    degree_centrality = nx.degree_centrality(G)
+    # def cost(data_pos,s,t,g,trg_,reg):
+    #     return np.exp(-g*reg)*np.linalg.norm(data_pos[s]-data_pos[t])*np.exp(np.linalg.norm(data_pos[s]-data_pos[t])/dis_mean)
 
     G = nx.DiGraph()
-    dis_mean = np.mean(np.linalg.norm(data_pos[source]-data_pos[target],axis=1))
+    G.add_weighted_edges_from([(int(s),int(t),1) for s,t in np.vstack((source,target)).T])
+    G.add_weighted_edges_from([(int(t),int(s),-1) for s,t in np.vstack((source,target)).T])
+    edges_ = np.array(list(G.edges))
+    weights_ = np.array([G[u][v]['weight'] for u, v in edges_])
 
-    def cost(data_pos,s,t,g,reg):
-        # return np.exp(-g*reg*(degree_centrality[s]+degree_centrality[t]))*np.linalg.norm(data_pos[s]-data_pos[t])
-        return np.exp(-g*reg)*np.linalg.norm(data_pos[s]-data_pos[t])*np.exp(np.linalg.norm(data_pos[s]-data_pos[t])/dis_mean)
-    
-    grad_ = adata.obs[potential_key][source].values - adata.obs[potential_key][target].values
-    G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
-    G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
-    G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
-    G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
-    
+    dis_mean = np.mean(np.linalg.norm(data_pos[source]-data_pos[target],axis=1))
     cmap_ = plt.get_cmap("tab10")
-    figsize = (10,8)
     fig,ax = plt.subplots(figsize=figsize)
     ax.triplot(tri_,color='gray',zorder=0,alpha=0.2,lw=1)
     clusters_ = adata.obs[cluster_key]
     idx_ = clusters_ == source_cluster
     ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color='gray',zorder=10,marker='D',alpha=0.2,s=5,label=source_cluster+' (source)')
     for i_trg_ in range(len(target_clusters)):
         idx_ = clusters_ == target_clusters[i_trg_]
@@ -1415,31 +1399,100 @@
         n_cells_ = np.min([n_cells,sum(adata.obs[cluster_key].values == source_cluster),sum(adata.obs[cluster_key].values == target_cluster)])
         data_trg_ = data_pos[adata.obs[cluster_key].values == target_cluster]
         center_trg_ = np.mean(data_trg_,axis=0)
         centrality_trg_ = np.linalg.norm(data_trg_-center_trg_,axis=1)
         n_trg_ = sum(adata.obs[cluster_key].values == target_cluster)
         idx_trg_ = np.arange(0,n_trg_,int(n_trg_/n_cells_))[:n_cells_]
         trg_set_ = np.arange(adata.shape[0])[adata.obs[cluster_key].values == target_cluster][np.argsort(centrality_trg_)][idx_trg_]
-        idx_src_ = np.arange(0,n_src_,int(n_src_/n_cells_))[:n_cells_]
+        idx_src_= np.array([np.argmin(np.abs(streamfunc_[trg__] - streamfunc_[src_set_all_].values)) for trg__ in trg_set_])
+        # idx_src_ = np.arange(0,n_src_,int(n_src_/n_cells_))[:n_cells_]
         src_set_ = src_set_all_[idx_src_]
 
         pathes,edges,weights,dists  = [],[],[],[]
         for src_,trg_ in np.vstack((src_set_,trg_set_)).T:
+            # G.add_weighted_edges_from([(int(s),int(t),np.exp(-g*register)*np.linalg.norm(streamfunc_[trg_]-streamfunc_[int(t)])*np.exp(np.linalg.norm(data_pos[int(s)]-data_pos[int(t)])/dis_mean)) for s,t,g in np.vstack((source,target,grad_)).T])
+            # G.add_weighted_edges_from([(int(t),int(s), np.exp(g*register)*np.linalg.norm(streamfunc_[trg_]-streamfunc_[int(t)])*np.exp(np.linalg.norm(data_pos[int(s)]-data_pos[int(t)])/dis_mean)) for s,t,g in np.vstack((source,target,grad_)).T])
+            # weights_ = np.hstack((np.exp(-grad_*register)*np.abs(streamfunc_[trg_]-streamfunc_[target])*np.exp(np.linalg.norm(data_pos[source]-data_pos[target],axis=1)/dis_mean),np.exp(grad_*register)*np.abs(streamfunc_[trg_]-streamfunc_[target])*np.exp(np.linalg.norm(data_pos[source]-data_pos[target],axis=1)/dis_mean)))
+            weights_i_ = np.exp(-weights_*(adata.obs[potential_key][edges_[:,0]].values - adata.obs[potential_key][edges_[:,1]].values)*register)*np.abs(streamfunc_[trg_]-streamfunc_[edges_[:,1]])*np.exp(np.linalg.norm(data_pos[edges_[:,0]]-data_pos[edges_[:,1]],axis=1)/dis_mean)
+            nx.set_edge_attributes(G, values=dict(zip(G.edges(), weights_i_)), name='weight')
             path = nx.dijkstra_path(G, source=src_, target=trg_, weight='weight')
             pathes.append(path)
             edges.append(np.array([[path[i], path[i+1]] for i in range(len(path)-1)]))
             weights.append((sum([G[path[i]][path[i+1]]['weight'] for i in range(len(path)-1)]))/sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
             dists.append(sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
         path_all[source_cluster+'_'+target_clusters[i_trg_]] = pathes
-        ax.scatter(data_pos[trg_set_,0],data_pos[trg_set_,1],color=cmap_(i_trg_),zorder=20,marker='o',s=20)
+        ax.scatter(data_pos[trg_set_,0],data_pos[trg_set_,1],color=cmap_(i_trg_),zorder=20,marker='o',s=30)
+        ax.scatter(data_pos[src_set_,0],data_pos[src_set_,1],color='gray',zorder=20,marker='D',s=30)
         for i in range(n_cells_):
-            ax.plot(data_pos[pathes[i],0],data_pos[pathes[i],1],color=cmap_(i_trg_),zorder=10,ls=':')
-    ax.scatter(data_pos[src_set_,0],data_pos[src_set_,1],color='gray',zorder=20,marker='D',s=30)
+            ax.plot(data_pos[pathes[i],0],data_pos[pathes[i],1],color=cmap_(i_trg_),zorder=10,ls='-',lw=2,alpha=0.3)
     ax.axis('off')
     adata.uns[path_key] = path_all
+    # G = nx.Graph()
+    # for i in range(len(source)):
+    #     G.add_edge(source[i],target[i],w=np.linalg.norm(data_pos[source[i]]-data_pos[target[i]]))
+    # degree_centrality = nx.degree_centrality(G)
+
+    # G = nx.DiGraph()
+    # dis_mean = np.mean(np.linalg.norm(data_pos[source]-data_pos[target],axis=1))
+
+    # def cost(data_pos,s,t,g,reg):
+    #     # return np.exp(-g*reg*(degree_centrality[s]+degree_centrality[t]))*np.linalg.norm(data_pos[s]-data_pos[t])
+    #     return np.exp(-g*reg)*np.linalg.norm(data_pos[s]-data_pos[t])*np.exp(np.linalg.norm(data_pos[s]-data_pos[t])/dis_mean)
+    
+    # grad_ = adata.obs[potential_key][source].values - adata.obs[potential_key][target].values
+    # G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
+    # G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_>0],target[grad_>0],grad_[grad_>0])).T])
+    # G.add_weighted_edges_from([(int(t),int(s),cost(data_pos,int(s),int(t),-g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
+    # G.add_weighted_edges_from([(int(s),int(t),cost(data_pos,int(s),int(t),g,register)) for s,t,g in np.vstack((source[grad_<0],target[grad_<0],grad_[grad_<0])).T])
+    
+    # cmap_ = plt.get_cmap("tab10")
+    # figsize = (10,8)
+    # fig,ax = plt.subplots(figsize=figsize)
+    # ax.triplot(tri_,color='gray',zorder=0,alpha=0.2,lw=1)
+    # clusters_ = adata.obs[cluster_key]
+    # idx_ = clusters_ == source_cluster
+    # ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color='gray',zorder=10,marker='D',alpha=0.2,s=5,label=source_cluster+' (source)')
+    # for i_trg_ in range(len(target_clusters)):
+    #     idx_ = clusters_ == target_clusters[i_trg_]
+    #     ax.scatter(data_pos[idx_,0],data_pos[idx_,1],color=cmap_(i_trg_),zorder=10,marker='o',alpha=0.2,s=5,label=target_clusters[i_trg_]+' (target)')
+    # leg = ax.legend(bbox_to_anchor=(1.05, 0.5), loc='center left', borderaxespad=0, fontsize=12,markerscale=3)
+    # for lh in leg.legend_handles: lh.set_alpha(1)
+
+    # data_src_ = data_pos[adata.obs[cluster_key].values == source_cluster]
+    # center_src_ = np.mean(data_src_,axis=0)
+    # centrality_src_ = np.linalg.norm(data_src_-center_src_,axis=1)
+    # src_set_all_ = np.arange(adata.shape[0])[adata.obs[cluster_key].values == source_cluster][np.argsort(centrality_src_)]
+    # n_src_ = sum(adata.obs[cluster_key].values == source_cluster)
+    # path_all = {}
+    # for i_trg_ in range(len(target_clusters)):
+    #     target_cluster = target_clusters[i_trg_]
+    #     n_cells_ = np.min([n_cells,sum(adata.obs[cluster_key].values == source_cluster),sum(adata.obs[cluster_key].values == target_cluster)])
+    #     data_trg_ = data_pos[adata.obs[cluster_key].values == target_cluster]
+    #     center_trg_ = np.mean(data_trg_,axis=0)
+    #     centrality_trg_ = np.linalg.norm(data_trg_-center_trg_,axis=1)
+    #     n_trg_ = sum(adata.obs[cluster_key].values == target_cluster)
+    #     idx_trg_ = np.arange(0,n_trg_,int(n_trg_/n_cells_))[:n_cells_]
+    #     trg_set_ = np.arange(adata.shape[0])[adata.obs[cluster_key].values == target_cluster][np.argsort(centrality_trg_)][idx_trg_]
+    #     idx_src_ = np.arange(0,n_src_,int(n_src_/n_cells_))[:n_cells_]
+    #     src_set_ = src_set_all_[idx_src_]
+
+    #     pathes,edges,weights,dists  = [],[],[],[]
+    #     for src_,trg_ in np.vstack((src_set_,trg_set_)).T:
+    #         path = nx.dijkstra_path(G, source=src_, target=trg_, weight='weight')
+    #         pathes.append(path)
+    #         edges.append(np.array([[path[i], path[i+1]] for i in range(len(path)-1)]))
+    #         weights.append((sum([G[path[i]][path[i+1]]['weight'] for i in range(len(path)-1)]))/sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
+    #         dists.append(sum([np.linalg.norm(data_pos[path[i]]-data_pos[path[i+1]]) for i in range(len(path)-1)]))
+    #     path_all[source_cluster+'_'+target_clusters[i_trg_]] = pathes
+    #     ax.scatter(data_pos[trg_set_,0],data_pos[trg_set_,1],color=cmap_(i_trg_),zorder=20,marker='o',s=20)
+    #     for i in range(n_cells_):
+    #         ax.plot(data_pos[pathes[i],0],data_pos[pathes[i],1],color=cmap_(i_trg_),zorder=10,ls=':')
+    # ax.scatter(data_pos[src_set_,0],data_pos[src_set_,1],color='gray',zorder=20,marker='D',s=30)
+    # ax.axis('off')
+    # adata.uns[path_key] = path_all
 
 
 def gene_dynamics(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
@@ -1678,14 +1731,15 @@
         target_clusters,
         path_key = 'path',
         exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
         n_div = 100,
         fontsize_label = 14,
         adjusttext =False,
+        PC = 0,
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
         gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
 
 
     vlines = [0,0.2,0.4,0.6,0.8,1]
@@ -1701,15 +1755,15 @@
     #     idx_ = np.arange(i,len(target_clusters)*n_div,n_div)
     #     samples_pca_[idx_] = samples_pca_[idx_] - samples_pca_[i]
 
     fig,ax = plt.subplots(figsize=(12,4))
     ax.text(0,samples_pca_[0,0],source_cluster+' ',fontsize=fontsize_label,va='center',ha='right')
     texts = []
     for j in range(len(target_clusters)):
-        y_ = samples_pca_[j*(n_div+1):(j+1)*(n_div+1),0]
+        y_ = samples_pca_[j*(n_div+1):(j+1)*(n_div+1),PC]
         ax.plot(np.linspace(0,1,n_div),y_,lw=5,zorder=2)
         texts = np.append(texts,ax.text(1,y_[-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left'))
     if adjusttext: adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'))
     for vl in vlines:
         ax.axvline(vl,color='k',ls='--',lw=1,zorder=0)
     ax.tick_params(axis='x', which='both', top=True)
     ax.spines['right'].set_visible(False)
```

## Comparing `cellmap-1.0.1.dev202304270902.dist-info/METADATA` & `cellmap-1.0.1.dev202304271030.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304270902
+Version: 1.0.1.dev202304271030
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

