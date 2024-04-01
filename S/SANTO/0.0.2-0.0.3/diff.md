# Comparing `tmp/SANTO-0.0.2.tar.gz` & `tmp/SANTO-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SANTO-0.0.2.tar", last modified: Tue Dec  5 14:44:53 2023, max compression
+gzip compressed data, was "SANTO-0.0.3.tar", last modified: Mon Apr  1 11:24:24 2024, max compression
```

## Comparing `SANTO-0.0.2.tar` & `SANTO-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 haoyangli   (501) staff       (20)        0 2023-12-05 14:44:53.422991 SANTO-0.0.2/
--rw-r--r--   0 haoyangli   (501) staff       (20)     1071 2023-12-01 10:50:23.000000 SANTO-0.0.2/LICENSE
--rw-r--r--   0 haoyangli   (501) staff       (20)      467 2023-12-05 14:44:53.422617 SANTO-0.0.2/PKG-INFO
-drwxr-xr-x   0 haoyangli   (501) staff       (20)        0 2023-12-05 14:44:53.416250 SANTO-0.0.2/SANTO.egg-info/
--rw-r--r--   0 haoyangli   (501) staff       (20)      467 2023-12-05 14:44:52.000000 SANTO-0.0.2/SANTO.egg-info/PKG-INFO
--rw-r--r--   0 haoyangli   (501) staff       (20)      222 2023-12-05 14:44:53.000000 SANTO-0.0.2/SANTO.egg-info/SOURCES.txt
--rw-r--r--   0 haoyangli   (501) staff       (20)        1 2023-12-05 14:44:52.000000 SANTO-0.0.2/SANTO.egg-info/dependency_links.txt
--rw-r--r--   0 haoyangli   (501) staff       (20)      157 2023-12-05 14:44:53.000000 SANTO-0.0.2/SANTO.egg-info/requires.txt
--rw-r--r--   0 haoyangli   (501) staff       (20)        6 2023-12-05 14:44:53.000000 SANTO-0.0.2/SANTO.egg-info/top_level.txt
-drwxr-xr-x   0 haoyangli   (501) staff       (20)        0 2023-12-05 14:44:53.421471 SANTO-0.0.2/santo/
--rw-r--r--   0 haoyangli   (501) staff       (20)       67 2023-12-05 13:17:39.000000 SANTO-0.0.2/santo/__init__.py
--rw-r--r--   0 haoyangli   (501) staff       (20)     3034 2023-12-04 11:57:32.000000 SANTO-0.0.2/santo/data.py
--rw-r--r--   0 haoyangli   (501) staff       (20)     7467 2023-12-05 11:16:38.000000 SANTO-0.0.2/santo/model.py
--rw-r--r--   0 haoyangli   (501) staff       (20)    15142 2023-12-05 14:39:42.000000 SANTO-0.0.2/santo/utils.py
--rw-r--r--   0 haoyangli   (501) staff       (20)       38 2023-12-05 14:44:53.423162 SANTO-0.0.2/setup.cfg
--rw-r--r--   0 haoyangli   (501) staff       (20)      845 2023-12-05 14:40:28.000000 SANTO-0.0.2/setup.py
+drwxr-xr-x   0 haoyangli   (501) staff       (20)        0 2024-04-01 11:24:24.337638 SANTO-0.0.3/
+-rw-r--r--   0 haoyangli   (501) staff       (20)     1071 2023-12-01 10:50:23.000000 SANTO-0.0.3/LICENSE
+-rw-r--r--   0 haoyangli   (501) staff       (20)      468 2024-04-01 11:24:24.337362 SANTO-0.0.3/PKG-INFO
+drwxr-xr-x   0 haoyangli   (501) staff       (20)        0 2024-04-01 11:24:24.331733 SANTO-0.0.3/SANTO.egg-info/
+-rw-r--r--   0 haoyangli   (501) staff       (20)      468 2024-04-01 11:24:23.000000 SANTO-0.0.3/SANTO.egg-info/PKG-INFO
+-rw-r--r--   0 haoyangli   (501) staff       (20)      222 2024-04-01 11:24:24.000000 SANTO-0.0.3/SANTO.egg-info/SOURCES.txt
+-rw-r--r--   0 haoyangli   (501) staff       (20)        1 2024-04-01 11:24:23.000000 SANTO-0.0.3/SANTO.egg-info/dependency_links.txt
+-rw-r--r--   0 haoyangli   (501) staff       (20)      117 2024-04-01 11:24:24.000000 SANTO-0.0.3/SANTO.egg-info/requires.txt
+-rw-r--r--   0 haoyangli   (501) staff       (20)        6 2024-04-01 11:24:24.000000 SANTO-0.0.3/SANTO.egg-info/top_level.txt
+drwxr-xr-x   0 haoyangli   (501) staff       (20)        0 2024-04-01 11:24:24.336661 SANTO-0.0.3/santo/
+-rw-r--r--   0 haoyangli   (501) staff       (20)       67 2023-12-05 13:17:39.000000 SANTO-0.0.3/santo/__init__.py
+-rw-r--r--   0 haoyangli   (501) staff       (20)     3034 2024-03-07 13:40:26.000000 SANTO-0.0.3/santo/data.py
+-rw-r--r--   0 haoyangli   (501) staff       (20)     7645 2024-04-01 10:34:59.000000 SANTO-0.0.3/santo/model.py
+-rw-r--r--   0 haoyangli   (501) staff       (20)    15247 2024-04-01 10:46:28.000000 SANTO-0.0.3/santo/utils.py
+-rw-r--r--   0 haoyangli   (501) staff       (20)       38 2024-04-01 11:24:24.337727 SANTO-0.0.3/setup.cfg
+-rw-r--r--   0 haoyangli   (501) staff       (20)      770 2024-04-01 11:06:26.000000 SANTO-0.0.3/setup.py
```

### Comparing `SANTO-0.0.2/LICENSE` & `SANTO-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SANTO-0.0.2/santo/data.py` & `SANTO-0.0.3/santo/data.py`

 * *Files identical despite different names*

### Comparing `SANTO-0.0.2/santo/model.py` & `SANTO-0.0.3/santo/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,17 @@
     inner = -2 * torch.matmul(x.transpose(2, 1).contiguous(), x)
     xx = torch.sum(x ** 2, dim=1, keepdim=True)
     pairwise_distance = -xx - inner - xx.transpose(2, 1).contiguous()
     idx = pairwise_distance.topk(k=k, dim=-1)[1]  # (batch_size, num_points, k)
     return idx
 
 
-def get_graph_feature(x, k=3):
+def get_graph_feature(x, k=3, device='cpu'):
     idx = knn(x, k=k)  # (batch_size, num_points, k)
     batch_size, num_points, _ = idx.size()
-    device = torch.device('cuda')
     idx_base = torch.arange(0, batch_size, device=device).view(-1, 1, 1) * num_points
     idx = idx + idx_base
     idx = idx.view(-1)
     _, num_dims, _ = x.size()
     x = x.transpose(2,
                     1).contiguous()  # (batch_size, num_points, num_dims)  -> (batch_size*num_points, num_dims) #   batch_size * num_points * k + range(0, batch_size*num_points)
     feature = x.view(batch_size * num_points, -1)[idx, :]
@@ -37,61 +36,63 @@
     x = x.view(batch_size, num_points, 1, num_dims).repeat(1, 1, k, 1)
     feature = torch.cat((feature, x), dim=3).permute(0, 3, 1, 2)
     return feature
 
 
 
 class DGCNN_cor(nn.Module):
-    def __init__(self, cor_dim = 2, k =3):
+    def __init__(self, cor_dim = 2, k =3, device = 'cpu'):
         super(DGCNN_cor, self).__init__()
         self.k = k
-        self.conv1 = nn.Conv2d(cor_dim*2, 32, kernel_size=1, bias=False) # input: 2*2 or 3*2
-        self.conv2 = nn.Conv2d(32, 64, kernel_size=1, bias=False)
-        self.conv3 = nn.Conv2d(64, 128, kernel_size=1, bias=False)
-        self.conv4 = nn.Conv2d(128, 256, kernel_size=1, bias=False)
-        self.conv5 = nn.Conv2d(32+64+128+256, 512, kernel_size=1, bias=False)
-        self.bn1 = nn.BatchNorm2d(32)
-        self.bn2 = nn.BatchNorm2d(64)
-        self.bn3 = nn.BatchNorm2d(128)
-        self.bn4 = nn.BatchNorm2d(256)
-        self.bn5 = nn.BatchNorm2d(512)
+        self.device = device
+        self.conv1 = nn.Conv2d(cor_dim*2, 8, kernel_size=1, bias=False) # input: 2*2 or 3*2
+        self.conv2 = nn.Conv2d(8, 16, kernel_size=1, bias=False)
+        self.conv3 = nn.Conv2d(16, 32, kernel_size=1, bias=False)
+        self.conv4 = nn.Conv2d(32, 64, kernel_size=1, bias=False)
+        self.conv5 = nn.Conv2d(8+16+32+64, 128, kernel_size=1, bias=False)
+        self.bn1 = nn.BatchNorm2d(8)
+        self.bn2 = nn.BatchNorm2d(16)
+        self.bn3 = nn.BatchNorm2d(32)
+        self.bn4 = nn.BatchNorm2d(64)
+        self.bn5 = nn.BatchNorm2d(128)
 
     def forward(self, x):
         batch_size, num_dims, num_points = x.size()
-        x = get_graph_feature(x,self.k)
+        x = get_graph_feature(x, self.k, self.device)
         x = F.relu(self.bn1(self.conv1(x)))
         x1 = x.max(dim=-1, keepdim=True)[0]
         x = F.relu(self.bn2(self.conv2(x)))
         x2 = x.max(dim=-1, keepdim=True)[0]
         x = F.relu(self.bn3(self.conv3(x)))
         x3 = x.max(dim=-1, keepdim=True)[0]
         x = F.relu(self.bn4(self.conv4(x)))
         x4 = x.max(dim=-1, keepdim=True)[0]
         x = torch.cat((x1, x2, x3, x4), dim=1)
         x = F.relu(self.bn5(self.conv5(x))).view(batch_size, -1, num_points)
         return x
 
 class DGCNN_exp(nn.Module):
-    def __init__(self, exp_dim = 1000, k=3):
+    def __init__(self, exp_dim = 1000, k=3, device = 'cpu'):
         super(DGCNN_exp, self).__init__()
         self.k = k
-        self.conv1 = nn.Conv2d(2*exp_dim, 64, kernel_size=1, bias=False)
-        self.conv2 = nn.Conv2d(64, 128, kernel_size=1, bias=False)
-        self.conv3 = nn.Conv2d(128, 256, kernel_size=1, bias=False)
-        self.conv4 = nn.Conv2d(256, 512, kernel_size=1, bias=False)
-        self.conv5 = nn.Conv2d(64+128+256+512, 1024, kernel_size=1, bias=False)
-        self.bn1 = nn.BatchNorm2d(64)
-        self.bn2 = nn.BatchNorm2d(128)
-        self.bn3 = nn.BatchNorm2d(256)
-        self.bn4 = nn.BatchNorm2d(512)
-        self.bn5 = nn.BatchNorm2d(1024)
+        self.device = device
+        self.conv1 = nn.Conv2d(exp_dim*2, 32, kernel_size=1, bias=False) # input: 2*2 or 3*2
+        self.conv2 = nn.Conv2d(32, 64, kernel_size=1, bias=False)
+        self.conv3 = nn.Conv2d(64, 128, kernel_size=1, bias=False)
+        self.conv4 = nn.Conv2d(128, 256, kernel_size=1, bias=False)
+        self.conv5 = nn.Conv2d(32+64+128+256, 512, kernel_size=1, bias=False)
+        self.bn1 = nn.BatchNorm2d(32)
+        self.bn2 = nn.BatchNorm2d(64)
+        self.bn3 = nn.BatchNorm2d(128)
+        self.bn4 = nn.BatchNorm2d(256)
+        self.bn5 = nn.BatchNorm2d(512)
 
     def forward(self, x):
         batch_size, num_dims, num_points = x.size()
-        x = get_graph_feature(x,self.k)
+        x = get_graph_feature(x,self.k, self.device)
         x = F.relu(self.bn1(self.conv1(x)))
         x1 = x.max(dim=-1, keepdim=True)[0]
         x = F.relu(self.bn2(self.conv2(x)))
         x2 = x.max(dim=-1, keepdim=True)[0]
         x = F.relu(self.bn3(self.conv3(x)))
         x3 = x.max(dim=-1, keepdim=True)[0]
         x = F.relu(self.bn4(self.conv4(x)))
@@ -153,16 +154,17 @@
 class Model(nn.Module):
     def __init__(self, args):
         super(Model, self).__init__()
 
         self.exp_dim = args.exp_dim
         self.dimension = args.dimension
         self.k = args.k
-        self.cor_emb_nn = DGCNN_cor(cor_dim = self.dimension,k=args.k)
-        self.exp_emb_nn = DGCNN_exp(exp_dim = self.exp_dim,k=args.k)
+        self.device = args.device
+        self.cor_emb_nn = DGCNN_cor(cor_dim = self.dimension,k=args.k, device = self.device)
+        self.exp_emb_nn = DGCNN_exp(exp_dim = self.exp_dim,k=args.k, device = self.device)
         self.head = SVDHead(args=args)
 
     def forward(self, *input):
         src_cor = input[0].transpose(2,1).contiguous() # (Batch_size, Feature, num_point)
         src_exp = input[1].transpose(2,1).contiguous() # (Batch_size, Feature, num_point)
         tgt_cor = input[2].transpose(2,1).contiguous() # (Batch_size, Feature, num_point)
         tgt_exp = input[3].transpose(2,1).contiguous() # (Batch_size, Feature, num_point)
```

### Comparing `SANTO-0.0.2/santo/utils.py` & `SANTO-0.0.3/santo/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import anndata as ad
 import ruptures as rpt
 from scipy.spatial import cKDTree
 import gc
 import scanpy as sc
 import torch.optim as optim
 from torch.optim.lr_scheduler import MultiStepLR
-from .model import Model
-from .data import intersect, combine_training_data, STDataset
+from model import Model
+from data import intersect, combine_training_data, STDataset
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 import matplotlib.pyplot as plt
 
 
 def evaluation(src_cor, tgt_cor, src_exp, tgt_exp, src_cell_type, tgt_cell_type):
 
@@ -142,15 +142,15 @@
     set2 = set2.iloc[:first_inflection_point,:]
 
 
     result = pd.merge(set1, set2, left_on=['tgt_index', 'src_index'], right_on=['tgt_index', 'src_index'], how='inner')
     src_sub = src[result['src_index'].to_numpy().astype(int), :]
     tgt_sub = tgt[result['tgt_index'].to_numpy().astype(int), :]
 
-    return src_sub, tgt_sub
+    return src_sub, tgt_sub,result
 
 
 def bin_adata(adata, bin_size=1, coords_key='spatial'):
     adata = adata.copy()
     adata.obsm[coords_key] = np.array(adata.obsm[coords_key], dtype=np.float32)
     adata.obsm[coords_key] = (adata.obsm[coords_key] // bin_size).astype(np.int32)
 
@@ -189,39 +189,38 @@
     softmax_denominator = torch.sum(exp_logits, dim=dim, keepdim=True)
     probabilities = exp_logits / softmax_denominator
     return probabilities
 
 
 def train_one_epoch(args, net, train_loader, opt):
     net.train()
-
     total_loss = 0
     num_examples = 0
     rotations_ab_pred = []
     translations_ab_pred = []
 
     for src, src_exp, target, target_exp in train_loader:
-        src = src.cuda()
-        src_exp = src_exp.cuda()
-        target = target.cuda()
-        target_exp = target_exp.cuda()
+        src = src.to(args.device)
+        src_exp = src_exp.to(args.device)
+        target = target.to(args.device)
+        target_exp = target_exp.to(args.device)
         batch_size = src.size(0)
         opt.zero_grad()
         num_examples += batch_size
         rotation_ab_pred, translation_ab_pred= net(src, src_exp, target, target_exp)
 
         ## save rotation and translation
 
         rotations_ab_pred.append(rotation_ab_pred.detach().cpu().numpy())
         translations_ab_pred.append(translation_ab_pred.detach().cpu().numpy())
         transformed_src = transform_point_cloud(src, rotation_ab_pred, translation_ab_pred)
         corr = torch.corrcoef(torch.cat((src_exp[0, :, :], target_exp[0, :, :]), dim=0))[:src_exp.shape[1],
                src_exp.shape[1]:]  # (src_cell_size,tgt_cell_size)
         dis = torch.cdist(transformed_src[0, :, :], target[0, :, :])  # (src,tgt)
-        softmin = custom_softmin(dis, 100, dim=1)  # (src,tgt)
+        softmin = custom_softmin(dis, 10, dim=1)  # (src,tgt)
 
         loss = args.alpha * 1 / (src_exp.shape[1]) * ((1 - corr) * softmin).sum() + \
                (1 - args.alpha) * 1 / (src_exp.shape[1]) * (dis * softmin).sum()
 
         loss.backward()
         opt.step()
         total_loss += loss.item() * batch_size
@@ -241,35 +240,35 @@
 
         scheduler.step()
         train_loss, train_rotations_ab_pred, train_translations_ab_pred = train_one_epoch(args, net, train_loader, opt)
         pbar.set_description(f'Epoch {epoch}, Loss: {train_loss}')
         gc.collect()
 
 
-def test(net, test_loader):
+def test(net, test_loader, args):
     net.eval()
     rotations_ab_pred = []
     translations_ab_pred = []
 
     for src, src_exp, target, target_exp in test_loader:
-        src = src.cuda()
-        src_exp = src_exp.cuda()
-        target = target.cuda()
-        target_exp = target_exp.cuda()
+        src = src.to(args.device)
+        src_exp = src_exp.to(args.device)
+        target = target.to(args.device)
+        target_exp = target_exp.to(args.device)
         rotation_ab_pred, translation_ab_pred = net(src, src_exp, target, target_exp)
         rotations_ab_pred.append(rotation_ab_pred.detach().cpu().numpy())
         translations_ab_pred.append(translation_ab_pred.detach().cpu().numpy())
     return rotations_ab_pred, translations_ab_pred
 
-def unify_feature(src, tgt, max_iter = 10):
+def unify_feature(src, tgt, max_iter = 20):
     '''use harmony to unify the feature space'''
     import harmonypy
     combined_data = ad.concat([src, tgt], join='inner')
     combined_data.obs['ids'] = ['source'] * src.shape[0] + ['target'] * tgt.shape[0]
-    sc.tl.pca(combined_data,n_comps=50)
+    sc.tl.pca(combined_data,n_comps=40)
     harmony_out = harmonypy.run_harmony(combined_data.obsm['X_pca'], combined_data.obs, 'ids', max_iter_harmony=max_iter)
     adjusted_matrix = harmony_out.Z_corr.T
     combined_data.obsm['X_pca_harmony'] = adjusted_matrix
     src = combined_data[:src.shape[0],:].copy()
     tgt = combined_data[src.shape[0]:,:].copy()
     new_src = ad.AnnData(X=src.obsm['X_pca_harmony'], obs=src.obs, obsm=src.obsm)
     new_tgt = ad.AnnData(X=tgt.obsm['X_pca_harmony'], obs=tgt.obs, obsm=tgt.obsm)
@@ -290,20 +289,20 @@
     torch.backends.cudnn.benchmark = True
     torch.backends.cudnn.deterministic = True
     torch.manual_seed(42)
     torch.cuda.manual_seed_all(42)
     np.random.seed(42)
     torch.cuda.empty_cache()
 
-
     comm_gene = intersect(src.var.index, tgt.var.index)
     src = src[:, comm_gene].copy()
     tgt = tgt[:, comm_gene].copy()
     args.exp_dim = len(comm_gene)
 
+
     if args.diff_omics:
         src, tgt = unify_feature(src, tgt)
         args.exp_dim = src.shape[1]
     src_cor = np.array(src.obsm['spatial'])
     tgt_cor = np.array(tgt.obsm['spatial'])
     if issparse(src.X):
         src.X = src.X.todense()
@@ -316,15 +315,16 @@
         aligned_source, coarse_R_ab, coarse_T_ab = coarse_align(src_cor, tgt_cor, src.X, tgt.X)
         src.obsm['spatial'] = aligned_source
         src.uns['original_spatial'] = src_cor
         plt.scatter(aligned_source[:, 0], aligned_source[:, 1], c='r', label='transformed', alpha=0.2,s=0.8)
 
     elif args.mode == 'stitch':
         print(f'You choose {args.mode}')
-        src, tgt = find_best_matching(src, tgt, k_list=[3,20,40])
+        src, tgt, result= find_best_matching(src, tgt, k_list=[5,10,20])
+
         aligned_source, coarse_R_ab, coarse_T_ab = coarse_stitch(src.obsm['spatial'], tgt.obsm['spatial'])
         src.obsm['spatial'] = aligned_source
         src.uns['original_spatial'] = src_cor
         whole_aligned_source = np.dot(src_cor, coarse_R_ab.T) + coarse_T_ab
         plt.scatter(whole_aligned_source[:, 0], whole_aligned_source[:, 1], c='r', label='transformed', alpha=0.2,s=0.8)
         print(f'Coarse stitching is finished, there are {src.shape[0]} matched pairs ')
 
@@ -343,18 +343,18 @@
     plt.show()
 
     pair_adatas = combine_training_data(src, tgt, is_preprocess=True)
     scale_factor1 = pair_adatas.uns['scale1']
     scale_factor2 = pair_adatas.uns['scale2']
 
     data_loader = DataLoader(STDataset([pair_adatas]))
-    net = Model(args).cuda()
+    net = Model(args).to(args.device)
 
     train(args, net, data_loader)
-    rotations_ab_pred, translations_ab_pred = test(net, data_loader)
+    rotations_ab_pred, translations_ab_pred = test(net, data_loader, args)
 
     if rotations_ab_pred[0].shape == (2,2):
         fine_R_ab = rotations_ab_pred[0]
     else:
         fine_R_ab = rotations_ab_pred[0][0,:,:]
 
     fine_T_ab = translations_ab_pred[0]
@@ -377,7 +377,8 @@
     plt.legend()
     plt.title("Visualization of fine alignment")
     plt.xlabel("X Coordinate")
     plt.ylabel("Y Coordinate")
     plt.show()
 
     return aligned_src_cor, trans_dict
+
```

### Comparing `SANTO-0.0.2/setup.py` & `SANTO-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import setuptools
 
 setuptools.setup(
     name="SANTO",
-    version="0.0.2",
+    version="0.0.3",
     author="Haoyang Li",
     author_email="lihy1995@gmail.com",
     description="SANTO: a coarse-to-fine stitching and alignment method for spatial omics",
     url="https://github.com/leihouyeung/SANTO",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     # 依赖模块
     install_requires=[
-        'torch==1.10.2',
-        'numpy==1.21.6',
+        'torch==1.11.0',
         'networkx==2.6.3',
-        'scipy==1.5.0',
-        'tqdm==4.65.0',
+        'scipy==1.12.0',
         'scanpy==1.9.3',
-        'anndata==0.8.0',
         'glob2==0.7',
-        'pandas==1.3.5',
         'ruptures==1.1.8',
-        'harmonypy==0.0.6'
+        'harmonypy==0.0.6',
+	    'easydict==1.13'
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.10',
 )
```

