# Comparing `tmp/accmt-0.0.6.tar.gz` & `tmp/accmt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accmt-0.0.6.tar", last modified: Mon Apr  1 01:48:43 2024, max compression
+gzip compressed data, was "accmt-0.0.7.tar", last modified: Mon Apr  1 20:22:15 2024, max compression
```

## Comparing `accmt-0.0.6.tar` & `accmt-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 01:48:43.082575 accmt-0.0.6/
--rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3274 2024-04-01 01:48:43.080560 accmt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2627 2024-04-01 01:48:15.000000 accmt-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      786 2024-04-01 01:48:43.084575 accmt-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 01:48:43.037038 accmt-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 01:48:43.059031 accmt-0.0.6/src/accmt/
--rw-rw-rw-   0        0        0       97 2024-04-01 00:10:31.000000 accmt-0.0.6/src/accmt/__init__.py
--rw-rw-rw-   0        0        0    13317 2024-04-01 01:46:07.000000 accmt-0.0.6/src/accmt/accmt.py
--rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-0.0.6/src/accmt/config.py
-drwxrwxrwx   0        0        0        0 2024-04-01 01:48:43.079041 accmt-0.0.6/src/accmt.egg-info/
--rw-rw-rw-   0        0        0     3274 2024-04-01 01:48:43.000000 accmt-0.0.6/src/accmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-01 01:48:43.000000 accmt-0.0.6/src/accmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 01:48:43.000000 accmt-0.0.6/src/accmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-01 01:48:43.000000 accmt-0.0.6/src/accmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.189455 accmt-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3274 2024-04-01 20:22:15.188387 accmt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2627 2024-04-01 01:48:15.000000 accmt-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      786 2024-04-01 20:22:15.189455 accmt-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.130118 accmt-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.162374 accmt-0.0.7/src/accmt/
+-rw-rw-rw-   0        0        0       97 2024-04-01 00:10:31.000000 accmt-0.0.7/src/accmt/__init__.py
+-rw-rw-rw-   0        0        0    15050 2024-04-01 20:21:53.000000 accmt-0.0.7/src/accmt/accmt.py
+-rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-0.0.7/src/accmt/config.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:15.186371 accmt-0.0.7/src/accmt.egg-info/
+-rw-rw-rw-   0        0        0     3274 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-01 20:22:15.000000 accmt-0.0.7/src/accmt.egg-info/top_level.txt
```

### Comparing `accmt-0.0.6/LICENSE` & `accmt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `accmt-0.0.6/PKG-INFO` & `accmt-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/MartinPC-uls/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/MartinPC-uls/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `accmt-0.0.6/README.md` & `accmt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `accmt-0.0.6/setup.cfg` & `accmt-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6363 6d74 0d0a 7665 7273 696f   = accmt..versio
-00000020: 6e20 3d20 302e 302e 360d 0a61 7574 686f  n = 0.0.6..autho
+00000020: 6e20 3d20 302e 302e 370d 0a61 7574 686f  n = 0.0.7..autho
 00000030: 7220 3d20 6768 616e 7665 7274 0d0a 6175  r = ghanvert..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6172  thor_email = mar
 00000050: 7469 6e2e 7069 7a61 7272 6f40 6365 6e69  tin.pizarro@ceni
 00000060: 612e 636c 0d0a 6465 7363 7269 7074 696f  a.cl..descriptio
 00000070: 6e20 3d20 4163 6365 6c65 7261 746f 7220  n = Accelerator 
 00000080: 4d6f 6475 6c65 2061 6e64 2054 7261 696e  Module and Train
 00000090: 6572 2062 6173 6564 206f 6e20 4163 6365  er based on Acce
```

### Comparing `accmt-0.0.6/src/accmt/accmt.py` & `accmt-0.0.7/src/accmt/accmt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import torch
+import warnings
 
 from abc import ABC
 from accelerate import Accelerator
 from accelerate.utils import LoggerType, ProjectConfiguration
 from .config import read, save_status, read_status
 from torch.utils.data import Dataset
 from typing import Any
@@ -82,17 +83,20 @@
     def __init__(self,
                 hps_file_config: str,
                 checkpoint = "checkpoint1",
                 resume = False,
                 model_path: str = None,
                 model_saving = "best_valid_loss",
                 enable_checkpointing = True,
-                checkpoint_every=1,
+                checkpoint_every = 1,
                 logging_dir = "logs",
-                log_with = LoggerType.TENSORBOARD
+                log_with = LoggerType.TENSORBOARD,
+                log_every = 1,
+                grad_accumulation_steps=1,
+                set_to_none=True
     ):
         """
         Trainer constructor to set configuration.
 
         Args:
             hps_file_config (`str`):
                 YAML hyperparameters file path.
@@ -114,25 +118,38 @@
                 Whether to save checkpoint or not.
             checkpoint_every (`int`, *optional*, defaults to `1`):
                 Checkpoint every N steps. Only works if `enable_checkpointing` is set to `True`.
             logging_dir (`str`, *optional*, defaults to `logs`):
                 Path where to save logs to show progress.
             log_with (`str`, *optional*, defaults to `LoggerType.TENSORBOARD`):
                 `LoggerType` to log progress.
+            log_every (`int`, *optional*, defaults to `1`):
+                Log every N steps.
+            grad_accumulation_steps (`int`, *optional*, defaults to `1`):
+                Accumulate gradients for N steps. Useful for training large models and simulate
+                large batches when memory is not enough. If set to `1`, no accumulation will be perfomed.
+            set_to_none (`bool`, *optional*, defaults to `True`):
+                From PyTorch documentation: "instead of setting to zero, set the grads to None. This will
+                in general have lower memory footprint, and can modestly improve performance." Some
+                optimizers have a different behaviour if the gradient is 0 or None. See PyTorch docs
+                for more information: https://pytorch.org/docs/stable/generated/torch.optim.Optimizer.zero_grad.html
         """
 
         self.accelerator = Accelerator()
         self.hps_config = hps_file_config
         self.checkpoint = checkpoint
         self.resume = resume
         self.model_path = model_path
         self.model_saving = model_saving.lower()
         self.enable_checkpointing = enable_checkpointing
         self.checkpoint_every = checkpoint_every
         self.logging_dir = logging_dir
+        self.log_every = log_every
+        self.grad_accumulation_steps = grad_accumulation_steps
+        self.set_to_none = set_to_none
 
         self.accelerator.project_configuration = ProjectConfiguration(project_dir=".", logging_dir=logging_dir, total_limit=1)
         self.accelerator.log_with = [log_with]
 
     def fit(self,
             module: AcceleratorModule,
             train_dataset: Dataset,
@@ -184,14 +201,20 @@
                 self.model_saving = "best_train_loss"
         
         optimizer = getattr(torch.optim, optim["type"])(model.parameters(), lr=float(optim["lr"]), weight_decay=float(optim["weight_decay"]))
         scheduler = None
         if "type" in schlr:
             scheduler = getattr(torch.optim.lr_scheduler, schlr["type"])(optimizer, max_lr=float(schlr["max_lr"]), steps_per_epoch=len(train_dataloader), epochs=hps["epochs"])
 
+        if "log_every" in cfg:
+            self.log_every = cfg["log_every"]
+            warnings.warn("'log_every' parameter in HPS config file is deprecated and it'll be removed in "
+                          "v1.0.0. Use 'log_every' in Trainer constructor instead.\n"
+                          "Using 'log_every' from HPS config file.")
+
         model, train_dataloader, val_dataloader, optimizer, scheduler = self.accelerator.prepare(
             model, train_dataloader, val_dataloader, optimizer, scheduler
         )
         self.accelerator.init_trackers(cfg["version"])
 
         best_valid_loss = float("inf")
         best_train_loss = float("inf")
@@ -210,38 +233,43 @@
         epochs = hps["epochs"]
         global_step = 0
         eval_step = len(train_dataloader) // len(val_dataloader)
         for epoch in range(status_epoch, epochs):
             eval_global_step = global_step
             model.train()
             train_losses = []
-            for step, batch in tqdm(enumerate(train_dataloader), total=len(train_dataloader), desc=f"Epoch {epoch}/{epochs}", unit="batch"):
+            for step, batch in tqdm(enumerate(train_dataloader, 1), total=len(train_dataloader), desc=f"Epoch {epoch}/{epochs}", unit="batch"):
                 loss = module.training_step(batch)
 
+                if self.grad_accumulation_steps > 1:
+                    loss /= self.grad_accumulation_steps
+
                 train_losses.append(loss.item())
-                if step % cfg["log_every"] == 0:
+                if step % self.log_every == 0:
                     self.accelerator.log({"loss": {"train": loss.item()}}, step=global_step)
 
                 self.accelerator.backward(loss)
-                optimizer.step()
-                if scheduler:
-                    scheduler.step()
-                optimizer.zero_grad(set_to_none=True)
+
+                if (step % self.grad_accumulation_steps == 0) or (step == len(train_dataloader)):
+                    optimizer.step()
+                    if scheduler:
+                        scheduler.step()
+                    optimizer.zero_grad(set_to_none=self.set_to_none)
 
                 global_step += 1
             
             if all([val_dataloader, getattr(module, "validation_step", False)]):
                 model.eval()
                 eval_losses = []
                 with torch.no_grad():
-                    for step, batch in tqdm(enumerate(val_dataloader), total=len(val_dataloader), desc=f"Epoch {epoch}/{epochs}", unit="batch"):
+                    for step, batch in tqdm(enumerate(val_dataloader, 1), total=len(val_dataloader), desc=f"Epoch {epoch}/{epochs}", unit="batch"):
                         loss = module.validation_step(batch)
 
                         eval_losses.append(loss.item())
-                        if step % cfg["log_every"] == 0:
+                        if step % self.log_every == 0:
                             self.accelerator.log({"loss": {"valid": loss.item()}}, step=eval_global_step)
 
                         eval_global_step += eval_step
 
                 best_valid_loss, best_train_loss = self._save_model_on_criteria(
                     model, eval_losses, train_losses, best_valid_loss, best_train_loss
                 )
```

### Comparing `accmt-0.0.6/src/accmt.egg-info/PKG-INFO` & `accmt-0.0.7/src/accmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/MartinPC-uls/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/MartinPC-uls/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

