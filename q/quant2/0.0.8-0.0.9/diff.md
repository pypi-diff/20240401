# Comparing `tmp/quant2-0.0.8.tar.gz` & `tmp/quant2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant2-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quant2-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quant2-0.0.8.tar` & `quant2-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      550 2024-03-23 04:30:30.169989 quant2-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.0.8/LICENSE
--rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.0.8/README.md
--rw-r--r--   0        0        0      658 2024-03-28 02:47:13.721511 quant2-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.0.8/quant/README.md
--rw-r--r--   0        0        0      559 2024-03-28 17:16:32.629233 quant2-0.0.8/quant/__init__.py
--rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.0.8/quant/__main__.py
--rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.0.8/quant/football/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.0.8/quant/football/data/__init__.py
--rw-r--r--   0        0        0     1617 2024-03-27 14:21:31.002567 quant2-0.0.8/quant/football/data/dataset.py
--rw-r--r--   0        0        0     1227 2024-03-27 14:21:31.002567 quant2-0.0.8/quant/football/data/functional.py
--rw-r--r--   0        0        0     1881 2024-03-28 05:23:26.661515 quant2-0.0.8/quant/football/data/stats.py
--rw-r--r--   0        0        0     4057 2024-03-28 04:00:36.851517 quant2-0.0.8/quant/football/data/utils.py
--rw-r--r--   0        0        0    11529 2024-03-26 04:17:29.502157 quant2-0.0.8/quant/football/etk_titan.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.335285 quant2-0.0.8/quant/football/models/__init__.py
--rw-r--r--   0        0        0     3742 2024-03-27 13:28:52.012568 quant2-0.0.8/quant/football/models/base.py
--rw-r--r--   0        0        0        0 2024-03-25 14:13:16.096778 quant2-0.0.8/quant/football/models/mtnet.py
--rw-r--r--   0        0        0        0 2024-03-25 14:13:22.146813 quant2-0.0.8/quant/football/models/rtnet.py
--rw-r--r--   0        0        0        0 2024-03-25 14:13:09.306739 quant2-0.0.8/quant/football/models/stnet.py
--rw-r--r--   0        0        0        0 2024-03-27 06:43:54.622569 quant2-0.0.8/quant/football/transforms/__init__.py
--rw-r--r--   0        0        0     4593 2024-03-28 12:07:47.723826 quant2-0.0.8/quant/football/transforms/table20240326.py
--rw-r--r--   0        0        0        0 2024-03-25 00:38:54.232911 quant2-0.0.8/quant/io/__init__.py
--rw-r--r--   0        0        0      496 2024-03-27 14:22:43.112566 quant2-0.0.8/quant/io/utils.py
--rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.0.8/quant/layers/layer_scale.py
--rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.0.8/quant/layers/mlp.py
--rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.0.8/quant/layers/normalization.py
--rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.0.8/quant/layers/swiglu_ffn.py
--rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.0.8/tests/football/data/test_utils.py
--rw-r--r--   0        0        0     4811 2024-03-28 17:15:19.811325 quant2-0.0.8/tools/experimental/train_table20240326_v1.py
--rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 quant2-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      556 2024-03-29 02:51:50.428398 quant2-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.0.9/LICENSE
+-rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.0.9/README.md
+-rw-r--r--   0        0        0      658 2024-03-28 02:47:13.721511 quant2-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.0.9/quant/README.md
+-rw-r--r--   0        0        0      559 2024-03-29 09:36:39.917189 quant2-0.0.9/quant/__init__.py
+-rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.0.9/quant/__main__.py
+-rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.0.9/quant/football/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.0.9/quant/football/data/__init__.py
+-rw-r--r--   0        0        0     1617 2024-03-27 14:21:31.002567 quant2-0.0.9/quant/football/data/dataset.py
+-rw-r--r--   0        0        0     1227 2024-03-27 14:21:31.002567 quant2-0.0.9/quant/football/data/functional.py
+-rw-r--r--   0        0        0     1881 2024-03-28 05:23:26.661515 quant2-0.0.9/quant/football/data/stats.py
+-rw-r--r--   0        0        0     4057 2024-03-28 04:00:36.851517 quant2-0.0.9/quant/football/data/utils.py
+-rw-r--r--   0        0        0    11529 2024-03-26 04:17:29.502157 quant2-0.0.9/quant/football/etk_titan.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.335285 quant2-0.0.9/quant/football/models/__init__.py
+-rw-r--r--   0        0        0     3742 2024-03-27 13:28:52.012568 quant2-0.0.9/quant/football/models/base.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:13:16.096778 quant2-0.0.9/quant/football/models/mtnet.py
+-rw-r--r--   0        0        0     3230 2024-03-30 04:08:13.910978 quant2-0.0.9/quant/football/models/stnet.py
+-rw-r--r--   0        0        0        0 2024-03-27 06:43:54.622569 quant2-0.0.9/quant/football/transforms/__init__.py
+-rw-r--r--   0        0        0     4858 2024-03-29 09:27:22.184980 quant2-0.0.9/quant/football/transforms/table20240326.py
+-rw-r--r--   0        0        0        0 2024-03-25 00:38:54.232911 quant2-0.0.9/quant/io/__init__.py
+-rw-r--r--   0        0        0      496 2024-03-27 14:22:43.112566 quant2-0.0.9/quant/io/utils.py
+-rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.0.9/quant/layers/layer_scale.py
+-rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.0.9/quant/layers/mlp.py
+-rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.0.9/quant/layers/normalization.py
+-rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.0.9/quant/layers/swiglu_ffn.py
+-rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.0.9/tests/football/data/test_utils.py
+-rw-r--r--   0        0        0     4837 2024-03-30 03:57:24.923775 quant2-0.0.9/tools/experimental/train_table20240326_v1.py
+-rw-r--r--   0        0        0     5038 2024-03-30 01:29:54.595817 quant2-0.0.9/tools/experimental/train_table20240326_v2.py
+-rw-r--r--   0        0        0     2173 1970-01-01 00:00:00.000000 quant2-0.0.9/PKG-INFO
```

### Comparing `quant2-0.0.8/.gitignore` & `quant2-0.0.9/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -53,10 +53,11 @@
 *.egg-info/
 
 # Sphinx documentation
 docs/build/
 
 # Outputs
 results/
+runs/
 
 # Sync
 .sync
```

### Comparing `quant2-0.0.8/LICENSE` & `quant2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/pyproject.toml` & `quant2-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/README.md` & `quant2-0.0.9/quant/README.md`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/__init__.py` & `quant2-0.0.9/quant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 help_doc_str = """\
 usage: quant [--version] [--help]
 
 shell command:
     quant -h
```

### Comparing `quant2-0.0.8/quant/football/data/dataset.py` & `quant2-0.0.9/quant/football/data/dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/football/data/functional.py` & `quant2-0.0.9/quant/football/data/functional.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/football/data/stats.py` & `quant2-0.0.9/quant/football/data/stats.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/football/data/utils.py` & `quant2-0.0.9/quant/football/data/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/football/etk_titan.py` & `quant2-0.0.9/quant/football/etk_titan.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/football/models/base.py` & `quant2-0.0.9/quant/football/models/base.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/football/transforms/table20240326.py` & `quant2-0.0.9/quant/football/transforms/table20240326.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 
     # 96: 8(n-key) * 6(n-cycle) + 8(n-key) * 6(n-cycle)
     xs = xs_home.reshape(-1).tolist() + xs_away.reshape(-1).tolist()
     return xs
 
 
 def parse_odds_data(data: dict):
-    first_1x2 = [v[-1] for v in data["odds_1x2"].values()]
-    first_overunder = [v[-1] for v in data["odds_overunder"].values()]
+    first_1x2 = [v[-1] for v in data["odds_1x2"].values() if v]
+    first_overunder = [v[-1] for v in data["odds_overunder"].values() if v]
     first_1x2 = odds_avg_max_min(first_1x2)
     first_overunder = odds_avg_max_min(first_overunder)
     # 18: 3(avg-max-min) * 3(1x2) + 3(avg-max-min) * 3(overunder)
     xs = first_1x2 + first_overunder
     return xs
 
 
@@ -90,16 +90,20 @@
 
 def check_samples(data: list[list]):
     good_row, bad_row, bad_msg = [], [], []
     for row in data:
         a = int(row[4])  # 主队得分
         b = int(row[5])  # 客队得分
         c = sum([row[i] for i in range(10, 58, 8)])  # 进球
+        c += sum([row[i] for i in range(14, 58, 8)])  # 乌龙
+        c += sum([row[i] for i in range(15, 58, 8)])  # 点球
         d = sum([row[i] for i in range(58, 106, 8)])  # 进球
-        if a == c and b == d:
+        d += sum([row[i] for i in range(62, 106, 8)])  # 乌龙
+        d += sum([row[i] for i in range(63, 106, 8)])  # 点球
+        if (a + b) == (c + d):
             good_row.append(row)
             continue
         bad_row.append(row)
         bad_msg.append([a, b, c, d])
     return good_row, bad_row, bad_msg
```

### Comparing `quant2-0.0.8/quant/layers/mlp.py` & `quant2-0.0.9/quant/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/layers/normalization.py` & `quant2-0.0.9/quant/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/quant/layers/swiglu_ffn.py` & `quant2-0.0.9/quant/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `quant2-0.0.8/tools/experimental/train_table20240326_v1.py` & `quant2-0.0.9/tools/experimental/train_table20240326_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# PYTHONPATH=/workspace/xlab/quant python tools/experimental/train_table20240326_v1.py
-# best_acc=0.62617, best_epoch=8, path=tmp/runs/20240329_011421
+# 1) PYTHONPATH=$(pwd) python tools/experimental/train_table20240326_v2.py
+# 2) python tools/experimental/train_table20240326_v2.py
 import numpy as np
 import random
 import time
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from pathlib import Path
@@ -18,25 +18,29 @@
         nn.init.normal_(m.weight, 0, 0.02)
         if hasattr(m, "bias") and m.bias is not None:
             nn.init.constant_(m.bias, 0.0)
 
 
 class Net(nn.Module):
 
-    def __init__(self, in_features, hidden_features, out_features, bias=True):
+    def __init__(self, in_features, hidden_features, out_features, n_layers=1, bias=True):
         super(Net, self).__init__()
-        self.stem = nn.Linear(in_features, hidden_features, bias=bias)
-        self.ffn_norm = RMSNorm(hidden_features)
-        self.ffn = SwiGLUFFN(hidden_features, bias=bias)
+        self.emb = nn.Linear(in_features, hidden_features, bias=bias)
+        self.layers = nn.ModuleList()
+        for _ in range(n_layers):
+            self.layers.append(RMSNorm(hidden_features))
+            self.layers.append(SwiGLUFFN(hidden_features, bias=bias))
+            self.layers.append(nn.SiLU())
         self.out_norm = RMSNorm(hidden_features)
         self.out = nn.Linear(hidden_features, out_features, bias=bias)
 
     def forward(self, x):
-        x = F.silu(self.stem(x))
-        x = F.silu(self.ffn(self.ffn_norm(x)))
+        x = F.silu(self.emb(x))
+        for layer in self.layers:
+            x = layer(x)
         x = self.out(self.out_norm(x))
         return x
 
 
 def train(model, device, train_loader, criterion, optimizer, epoch, log_interval=10, dry_run=False):
     model.train()
     for batch_idx, (data, target) in enumerate(train_loader):
@@ -70,15 +74,15 @@
 
     print("\nTest set: Average loss: {:.4f}, Accuracy: {}/{} ({:.0f}%)\n".format(
         test_loss, correct, len(test_loader.dataset),
         100. * correct / len(test_loader.dataset)))
     return correct / len(test_loader.dataset)
 
 
-def main(train_file, test_file, seed=1, device="cuda", batch_size=128, lr=0.1, epochs=90, log_interval=10):
+def main(train_file, test_file, seed=1, device="cuda", batch_size=128, n_layers=1, lr=0.1, epochs=90, log_interval=10):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.backends.cudnn.deterministic = True
     torch.backends.cudnn.benchmark = False
 
     if device == "cuda" and torch.cuda.is_available():
@@ -92,43 +96,46 @@
     train_loader = torch.utils.data.DataLoader(
         train_dataset, batch_size=batch_size, shuffle=True
     )
     test_loader = torch.utils.data.DataLoader(
         test_dataset, batch_size=1
     )
 
-    model = Net(806, 384, 10, True).to(device)
+    model = Net(806, 384, 10, n_layers, bias=True).to(device)
     # model.apply(init_weights)
     criterion = nn.CrossEntropyLoss().to(device)
     optimizer = torch.optim.SGD(model.parameters(), lr, 0.9, weight_decay=1e-4)
     scheduler = StepLR(optimizer, step_size=30, gamma=0.1)
-    out_dir = Path("tmp/runs") / time.strftime("%Y%m%d_%H%M%S")
+    out_dir = Path("runs") / time.strftime("%m%d%H%M%S")
     out_dir.mkdir(parents=True, exist_ok=True)
     best_acc = 0.0
     best_epoch = -1
     for epoch in range(1, epochs + 1):
         train(model, device, train_loader, criterion,
               optimizer, epoch, log_interval)
         curr_acc = test(model, device, test_loader, criterion)
         if curr_acc > best_acc:
             best_acc, best_epoch = curr_acc, epoch
         scheduler.step()
         torch.save(model.state_dict(), out_dir / f"model{epoch:03d}.pt")
-    print(f"\n[best model]\n\n{best_acc=:.5f}, {best_epoch=}, path={out_dir}")
 
-    print("\n[check train dataset]")
+    print("[best model]")
+    print(f"\n{best_acc=:.5f}, {best_epoch=}, path={out_dir}\n")
+
+    print("[check train dataset]")
     check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=1)
     test(model, device, check_loader, criterion)
 
 
 if __name__ == "__main__":
-    data_root = Path("/workspace/xlab/quant/tmp/table20240326_03281154_torch")
+    data_root = Path("/workspace/xlab/datasets")
     main(
-        train_file=data_root / "20240328_201607.dat",
-        test_file=data_root / "20240328_201609.dat",
+        train_file=data_root / "table20240326_03281154_torch_norm/20240329_101534.dat",
+        test_file=data_root / "table20240326_03281154_torch_norm/20240329_101539.dat",
         seed=1,
         device="cuda",
         batch_size=128,
+        n_layers=1,
         lr=0.1,
         epochs=90,
         log_interval=10,
     )
```

### Comparing `quant2-0.0.8/PKG-INFO` & `quant2-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: simplejson
 Requires-Dist: requests >=2.6
 Requires-Dist: scikit-learn
```

