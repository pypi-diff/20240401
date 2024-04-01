# Comparing `tmp/africanwhisper-0.2.4.tar.gz` & `tmp/africanwhisper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.2.4.tar", last modified: Sat Mar 30 20:46:17 2024, max compression
+gzip compressed data, was "africanwhisper-0.2.5.tar", last modified: Mon Apr  1 20:43:30 2024, max compression
```

## Comparing `africanwhisper-0.2.4.tar` & `africanwhisper-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:17.271571 africanwhisper-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-03-30 20:46:17.271571 africanwhisper-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-30 20:46:17.271571 africanwhisper-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:17.263571 africanwhisper-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:17.267571 africanwhisper-0.2.4/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-03-30 20:46:17.000000 africanwhisper-0.2.4/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-30 20:46:17.000000 africanwhisper-0.2.4/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:46:17.000000 africanwhisper-0.2.4/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-30 20:46:17.000000 africanwhisper-0.2.4/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 20:46:17.000000 africanwhisper-0.2.4/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:17.267571 africanwhisper-0.2.4/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/deployment/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:17.267571 africanwhisper-0.2.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:17.267571 africanwhisper-0.2.4/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-30 20:46:13.000000 africanwhisper-0.2.4/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.089303 africanwhisper-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.089303 africanwhisper-0.2.5/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/deployment/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.089303 africanwhisper-0.2.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.2.4/LICENSE` & `africanwhisper-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/PKG-INFO` & `africanwhisper-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -30,20 +30,26 @@
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
+  <a href="https://twitter.com/AfriWhisper">
+    <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
+  </a>
   <a href="https://github.com/KevKibe/African-Whisper/commits/">
-    <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?style=flat-square" alt="Last commit">
+    <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/blob/main/LICENSE">
-    <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?style=flat-square&color=blue" alt="License">
+    <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?" alt="License">
   </a>
+
+  
+
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
 ## Description
@@ -82,15 +88,15 @@
 5. Containerize your REST API endpoint and push to DockerHub.
 
 
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
-- Sign up ro wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
+- Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
 ## Usage on a Notebook
 
 ```python
 !pip install africanwhisper
 # restart the runtime/session: because of an issue with the latest transformers package version
 ```
@@ -106,14 +112,15 @@
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1"
 # choose a small dataset so as to not run out of memory, see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1
 language_abbr= "af" 
 model_id= "openai/whisper-small"
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
+# Note: PEFT only works on a notbeook with GPU-support.
 use_peft = True
 ```
 
 ```python
 # Downloading the model, tokenizer, feature extractor and processor
 process = DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task, use_peft)
 tokenizer, feature_extractor, feature_processor, model = process.prepare_model()
@@ -150,15 +157,15 @@
 source venv/bin/activate
 ```
 
 - Install dependencies by running this command
 ```
 pip install -r requirements.txt
 ```
-- Navigate to
+- Navigate to:
 ```
 cd src
 ```
 
 - To start the training , use the following command:
 ```
 python -m training.main \
@@ -183,15 +190,15 @@
 
 - **--model_id**: Identifier for the pre-trained model you wish to fine-tune. Example: 'openai/whisper-small'. This should match the model's identifier on the Hugging Face Model Hub.
 
 - **--processing_task**: Specifies the task for which the model is being trained. Example: 'transcribe'. This defines the objective of the model training, such as transcribing audio to text.
 
 - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used for logging and tracking the training process if you're using W&B for experiment tracking.
 
-- **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning.
+- **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning. PEFT only works on a notbeook with GPU-support.
 
 ## Inference
 
 - To get inference from your fine-tuned model, follow these steps:
 
 - Ensure that ffmpeg is installed by running the following commands:
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.4 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.5 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.1
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
@@ -10,15 +10,15 @@
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
 dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.4
 Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
 gradio==4.21.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
 scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
-                            _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
+                        _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 ## Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
 better recognize and transcribe African languages for all developers. ## Why
 Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
@@ -45,44 +45,45 @@
 huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on
 any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
 Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
 ). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
 fro transcription of Audio files. 5. Containerize your REST API endpoint and
 push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
 keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
-Sign up ro wandb and get your token keys use this [guide](https://app.wandb.ai/
-login?signup=true) ## Usage on a Notebook ```python !pip install africanwhisper
-# restart the runtime/session: because of an issue with the latest transformers
-package version ``` ```python from training.data_prep import DataPrep from
-training.model_trainer import Trainer from training.gradio_inference import
-WhisperDemo ``` ```python # refer to the Usage on VM section below to know more
-about these parameters huggingface_read_token = " " huggingface_write_token = "
-" dataset_name = "mozilla-foundation/common_voice_16_1" # choose a small
-dataset so as to not run out of memory, see abbreviations here https://
-huggingface.co/datasets/mozilla-foundation/common_voice_16_1 language_abbr=
-"af" model_id= "openai/whisper-small" processing_task= "automatic-speech-
-recognition" wandb_api_key = " " use_peft = True ``` ```python # Downloading
-the model, tokenizer, feature extractor and processor process = DataPrep
-(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task,
-use_peft) tokenizer, feature_extractor, feature_processor, model =
-process.prepare_model() ``` ```python # Preprocessing the Dataset
+Sign up for wandb and get your token keys use this [guide](https://
+app.wandb.ai/login?signup=true) ## Usage on a Notebook ```python !pip install
+africanwhisper # restart the runtime/session: because of an issue with the
+latest transformers package version ``` ```python from training.data_prep
+import DataPrep from training.model_trainer import Trainer from
+training.gradio_inference import WhisperDemo ``` ```python # refer to the Usage
+on VM section below to know more about these parameters huggingface_read_token
+= " " huggingface_write_token = " " dataset_name = "mozilla-foundation/
+common_voice_16_1" # choose a small dataset so as to not run out of memory, see
+abbreviations here https://huggingface.co/datasets/mozilla-foundation/
+common_voice_16_1 language_abbr= "af" model_id= "openai/whisper-small"
+processing_task= "automatic-speech-recognition" wandb_api_key = " " # Note:
+PEFT only works on a notbeook with GPU-support. use_peft = True ``` ```python #
+Downloading the model, tokenizer, feature extractor and processor process =
+DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id,
+processing_task, use_peft) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ```python # Preprocessing the Dataset
 processed_dataset = process.load_dataset(feature_extractor, tokenizer,
 feature_processor) ``` ```python # Training the model trainer = Trainer
 (huggingface_write_token, model_id, processed_dataset, model,
 feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key,
 use_peft) trainer.train() ``` ```python # Generate demo model_name = " " # Your
 finetuned model name on huggingface hub e.g ""KevinKibe/whisper-small-af" demo
 = WhisperDemo(model_name, huggingface_read_token) demo.generate_demo() ``` ##
 Usage on a Virtual Machine - Clone the Repository: Clone or download the
 application code to your local machine. ``` git clone https://github.com/
 KevKibe/African-Whisper.git ``` - Create a virtual environment for the project
 and activate it. ``` python3 -m venv env source venv/bin/activate ``` - Install
 dependencies by running this command ``` pip install -r requirements.txt ``` -
-Navigate to ``` cd src ``` - To start the training , use the following command:
-``` python -m training.main \ --huggingface_read_token
+Navigate to: ``` cd src ``` - To start the training , use the following
+command: ``` python -m training.main \ --huggingface_read_token
 YOUR_HUGGING_FACE_READ_TOKEN_HERE \ --huggingface_write_token
 YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name DATASET_NAME \ --
 language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --processing_task
 PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --use_peft ```
 Here's a short description of each argument used in the command: - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. - **--
@@ -97,21 +98,22 @@
 model you wish to fine-tune. Example: 'openai/whisper-small'. This should match
 the model's identifier on the Hugging Face Model Hub. - **--processing_task**:
 Specifies the task for which the model is being trained. Example: 'transcribe'.
 This defines the objective of the model training, such as transcribing audio to
 text. - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used
 for logging and tracking the training process if you're using W&B for
 experiment tracking. - **--use_peft**: Add this flag to fine-tune using PEFT
-method and omit it to do full fine-tuning. ## Inference - To get inference from
-your fine-tuned model, follow these steps: - Ensure that ffmpeg is installed by
-running the following commands: ``` # on Ubuntu or Debian sudo apt update &&
-sudo apt install ffmpeg # on Arch Linux sudo pacman -S ffmpeg # on MacOS using
-Homebrew (https://brew.sh/) brew install ffmpeg # on Windows using Chocolatey
-(https://chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https:
-//scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
+method and omit it to do full fine-tuning. PEFT only works on a notbeook with
+GPU-support. ## Inference - To get inference from your fine-tuned model, follow
+these steps: - Ensure that ffmpeg is installed by running the following
+commands: ``` # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg
+# on Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://
+brew.sh/) brew install ffmpeg # on Windows using Chocolatey (https://
+chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https://
+scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
 python -m training.gradio_demo \ --model_name YOUR_FINETUNED-MODEL \ --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \ ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. ##
 Deployment - To deploy your fine-tuned model (assuming it's on Hugging Face
```

### Comparing `africanwhisper-0.2.4/README.md` & `africanwhisper-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
+  <a href="https://twitter.com/AfriWhisper">
+    <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
+  </a>
   <a href="https://github.com/KevKibe/African-Whisper/commits/">
-    <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?style=flat-square" alt="Last commit">
+    <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/blob/main/LICENSE">
-    <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?style=flat-square&color=blue" alt="License">
+    <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?" alt="License">
   </a>
+
+  
+
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
 ## Description
@@ -49,15 +55,15 @@
 5. Containerize your REST API endpoint and push to DockerHub.
 
 
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
-- Sign up ro wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
+- Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
 ## Usage on a Notebook
 
 ```python
 !pip install africanwhisper
 # restart the runtime/session: because of an issue with the latest transformers package version
 ```
@@ -73,14 +79,15 @@
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1"
 # choose a small dataset so as to not run out of memory, see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1
 language_abbr= "af" 
 model_id= "openai/whisper-small"
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
+# Note: PEFT only works on a notbeook with GPU-support.
 use_peft = True
 ```
 
 ```python
 # Downloading the model, tokenizer, feature extractor and processor
 process = DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task, use_peft)
 tokenizer, feature_extractor, feature_processor, model = process.prepare_model()
@@ -117,15 +124,15 @@
 source venv/bin/activate
 ```
 
 - Install dependencies by running this command
 ```
 pip install -r requirements.txt
 ```
-- Navigate to
+- Navigate to:
 ```
 cd src
 ```
 
 - To start the training , use the following command:
 ```
 python -m training.main \
@@ -150,15 +157,15 @@
 
 - **--model_id**: Identifier for the pre-trained model you wish to fine-tune. Example: 'openai/whisper-small'. This should match the model's identifier on the Hugging Face Model Hub.
 
 - **--processing_task**: Specifies the task for which the model is being trained. Example: 'transcribe'. This defines the objective of the model training, such as transcribing audio to text.
 
 - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used for logging and tracking the training process if you're using W&B for experiment tracking.
 
-- **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning.
+- **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning. PEFT only works on a notbeook with GPU-support.
 
 ## Inference
 
 - To get inference from your fine-tuned model, follow these steps:
 
 - Ensure that ffmpeg is installed by running the following commands:
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
-                            _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
+                        _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 ## Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
 better recognize and transcribe African languages for all developers. ## Why
 Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
@@ -30,44 +30,45 @@
 huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on
 any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
 Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
 ). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
 fro transcription of Audio files. 5. Containerize your REST API endpoint and
 push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
 keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
-Sign up ro wandb and get your token keys use this [guide](https://app.wandb.ai/
-login?signup=true) ## Usage on a Notebook ```python !pip install africanwhisper
-# restart the runtime/session: because of an issue with the latest transformers
-package version ``` ```python from training.data_prep import DataPrep from
-training.model_trainer import Trainer from training.gradio_inference import
-WhisperDemo ``` ```python # refer to the Usage on VM section below to know more
-about these parameters huggingface_read_token = " " huggingface_write_token = "
-" dataset_name = "mozilla-foundation/common_voice_16_1" # choose a small
-dataset so as to not run out of memory, see abbreviations here https://
-huggingface.co/datasets/mozilla-foundation/common_voice_16_1 language_abbr=
-"af" model_id= "openai/whisper-small" processing_task= "automatic-speech-
-recognition" wandb_api_key = " " use_peft = True ``` ```python # Downloading
-the model, tokenizer, feature extractor and processor process = DataPrep
-(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task,
-use_peft) tokenizer, feature_extractor, feature_processor, model =
-process.prepare_model() ``` ```python # Preprocessing the Dataset
+Sign up for wandb and get your token keys use this [guide](https://
+app.wandb.ai/login?signup=true) ## Usage on a Notebook ```python !pip install
+africanwhisper # restart the runtime/session: because of an issue with the
+latest transformers package version ``` ```python from training.data_prep
+import DataPrep from training.model_trainer import Trainer from
+training.gradio_inference import WhisperDemo ``` ```python # refer to the Usage
+on VM section below to know more about these parameters huggingface_read_token
+= " " huggingface_write_token = " " dataset_name = "mozilla-foundation/
+common_voice_16_1" # choose a small dataset so as to not run out of memory, see
+abbreviations here https://huggingface.co/datasets/mozilla-foundation/
+common_voice_16_1 language_abbr= "af" model_id= "openai/whisper-small"
+processing_task= "automatic-speech-recognition" wandb_api_key = " " # Note:
+PEFT only works on a notbeook with GPU-support. use_peft = True ``` ```python #
+Downloading the model, tokenizer, feature extractor and processor process =
+DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id,
+processing_task, use_peft) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ```python # Preprocessing the Dataset
 processed_dataset = process.load_dataset(feature_extractor, tokenizer,
 feature_processor) ``` ```python # Training the model trainer = Trainer
 (huggingface_write_token, model_id, processed_dataset, model,
 feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key,
 use_peft) trainer.train() ``` ```python # Generate demo model_name = " " # Your
 finetuned model name on huggingface hub e.g ""KevinKibe/whisper-small-af" demo
 = WhisperDemo(model_name, huggingface_read_token) demo.generate_demo() ``` ##
 Usage on a Virtual Machine - Clone the Repository: Clone or download the
 application code to your local machine. ``` git clone https://github.com/
 KevKibe/African-Whisper.git ``` - Create a virtual environment for the project
 and activate it. ``` python3 -m venv env source venv/bin/activate ``` - Install
 dependencies by running this command ``` pip install -r requirements.txt ``` -
-Navigate to ``` cd src ``` - To start the training , use the following command:
-``` python -m training.main \ --huggingface_read_token
+Navigate to: ``` cd src ``` - To start the training , use the following
+command: ``` python -m training.main \ --huggingface_read_token
 YOUR_HUGGING_FACE_READ_TOKEN_HERE \ --huggingface_write_token
 YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name DATASET_NAME \ --
 language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --processing_task
 PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --use_peft ```
 Here's a short description of each argument used in the command: - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. - **--
@@ -82,21 +83,22 @@
 model you wish to fine-tune. Example: 'openai/whisper-small'. This should match
 the model's identifier on the Hugging Face Model Hub. - **--processing_task**:
 Specifies the task for which the model is being trained. Example: 'transcribe'.
 This defines the objective of the model training, such as transcribing audio to
 text. - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used
 for logging and tracking the training process if you're using W&B for
 experiment tracking. - **--use_peft**: Add this flag to fine-tune using PEFT
-method and omit it to do full fine-tuning. ## Inference - To get inference from
-your fine-tuned model, follow these steps: - Ensure that ffmpeg is installed by
-running the following commands: ``` # on Ubuntu or Debian sudo apt update &&
-sudo apt install ffmpeg # on Arch Linux sudo pacman -S ffmpeg # on MacOS using
-Homebrew (https://brew.sh/) brew install ffmpeg # on Windows using Chocolatey
-(https://chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https:
-//scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
+method and omit it to do full fine-tuning. PEFT only works on a notbeook with
+GPU-support. ## Inference - To get inference from your fine-tuned model, follow
+these steps: - Ensure that ffmpeg is installed by running the following
+commands: ``` # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg
+# on Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://
+brew.sh/) brew install ffmpeg # on Windows using Chocolatey (https://
+chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https://
+scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
 python -m training.gradio_demo \ --model_name YOUR_FINETUNED-MODEL \ --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \ ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. ##
 Deployment - To deploy your fine-tuned model (assuming it's on Hugging Face
```

### Comparing `africanwhisper-0.2.4/setup.cfg` & `africanwhisper-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.2.4
+version = 0.2.5
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
```

### Comparing `africanwhisper-0.2.4/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.2.5/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -30,20 +30,26 @@
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
+  <a href="https://twitter.com/AfriWhisper">
+    <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
+  </a>
   <a href="https://github.com/KevKibe/African-Whisper/commits/">
-    <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?style=flat-square" alt="Last commit">
+    <img src="https://img.shields.io/github/last-commit/KevKibe/African-Whisper?" alt="Last commit">
   </a>
   <a href="https://github.com/KevKibe/African-Whisper/blob/main/LICENSE">
-    <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?style=flat-square&color=blue" alt="License">
+    <img src="https://img.shields.io/github/license/KevKibe/African-Whisper?" alt="License">
   </a>
+
+  
+
 </p>
 
 <p align="center">
     <img src= "image.png" width="100">
 </p>
 
 ## Description
@@ -82,15 +88,15 @@
 5. Containerize your REST API endpoint and push to DockerHub.
 
 
 ## Prerequisites
 
 - Sign up to HuggingFace and get your token keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens).
 
-- Sign up ro wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
+- Sign up for wandb and get your token keys use this [guide](https://app.wandb.ai/login?signup=true)
 
 ## Usage on a Notebook
 
 ```python
 !pip install africanwhisper
 # restart the runtime/session: because of an issue with the latest transformers package version
 ```
@@ -106,14 +112,15 @@
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1"
 # choose a small dataset so as to not run out of memory, see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1
 language_abbr= "af" 
 model_id= "openai/whisper-small"
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
+# Note: PEFT only works on a notbeook with GPU-support.
 use_peft = True
 ```
 
 ```python
 # Downloading the model, tokenizer, feature extractor and processor
 process = DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task, use_peft)
 tokenizer, feature_extractor, feature_processor, model = process.prepare_model()
@@ -150,15 +157,15 @@
 source venv/bin/activate
 ```
 
 - Install dependencies by running this command
 ```
 pip install -r requirements.txt
 ```
-- Navigate to
+- Navigate to:
 ```
 cd src
 ```
 
 - To start the training , use the following command:
 ```
 python -m training.main \
@@ -183,15 +190,15 @@
 
 - **--model_id**: Identifier for the pre-trained model you wish to fine-tune. Example: 'openai/whisper-small'. This should match the model's identifier on the Hugging Face Model Hub.
 
 - **--processing_task**: Specifies the task for which the model is being trained. Example: 'transcribe'. This defines the objective of the model training, such as transcribing audio to text.
 
 - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used for logging and tracking the training process if you're using W&B for experiment tracking.
 
-- **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning.
+- **--use_peft**: Add this flag to fine-tune using PEFT method and omit it to do full fine-tuning. PEFT only works on a notbeook with GPU-support.
 
 ## Inference
 
 - To get inference from your fine-tuned model, follow these steps:
 
 - Ensure that ffmpeg is installed by running the following commands:
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.4 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.5 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.1
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
@@ -10,15 +10,15 @@
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
 dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.4
 Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
 gradio==4.21.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
 scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
-                            _[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
+                        _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 ## Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
 better recognize and transcribe African languages for all developers. ## Why
 Whisper? Whisper is an open-source Automatic Speech Recognition (ASR) system
@@ -45,44 +45,45 @@
 huggingface.co/collections/openai/whisper-release-6501bba2cf999715fd953013) on
 any dataset from [Mozilla's](https://huggingface.co/mozilla-foundation) Common
 Voice datasets. 2. View your training run metrics on [Wandb](https://wandb.ai/
 ). 3. Test your fine-tuned model using Gradio UI. 4. Deploy a REST API endpoint
 fro transcription of Audio files. 5. Containerize your REST API endpoint and
 push to DockerHub. ## Prerequisites - Sign up to HuggingFace and get your token
 keys use this [guide](https://huggingface.co/docs/hub/en/security-tokens). -
-Sign up ro wandb and get your token keys use this [guide](https://app.wandb.ai/
-login?signup=true) ## Usage on a Notebook ```python !pip install africanwhisper
-# restart the runtime/session: because of an issue with the latest transformers
-package version ``` ```python from training.data_prep import DataPrep from
-training.model_trainer import Trainer from training.gradio_inference import
-WhisperDemo ``` ```python # refer to the Usage on VM section below to know more
-about these parameters huggingface_read_token = " " huggingface_write_token = "
-" dataset_name = "mozilla-foundation/common_voice_16_1" # choose a small
-dataset so as to not run out of memory, see abbreviations here https://
-huggingface.co/datasets/mozilla-foundation/common_voice_16_1 language_abbr=
-"af" model_id= "openai/whisper-small" processing_task= "automatic-speech-
-recognition" wandb_api_key = " " use_peft = True ``` ```python # Downloading
-the model, tokenizer, feature extractor and processor process = DataPrep
-(huggingface_read_token, dataset_name,language_abbr,model_id, processing_task,
-use_peft) tokenizer, feature_extractor, feature_processor, model =
-process.prepare_model() ``` ```python # Preprocessing the Dataset
+Sign up for wandb and get your token keys use this [guide](https://
+app.wandb.ai/login?signup=true) ## Usage on a Notebook ```python !pip install
+africanwhisper # restart the runtime/session: because of an issue with the
+latest transformers package version ``` ```python from training.data_prep
+import DataPrep from training.model_trainer import Trainer from
+training.gradio_inference import WhisperDemo ``` ```python # refer to the Usage
+on VM section below to know more about these parameters huggingface_read_token
+= " " huggingface_write_token = " " dataset_name = "mozilla-foundation/
+common_voice_16_1" # choose a small dataset so as to not run out of memory, see
+abbreviations here https://huggingface.co/datasets/mozilla-foundation/
+common_voice_16_1 language_abbr= "af" model_id= "openai/whisper-small"
+processing_task= "automatic-speech-recognition" wandb_api_key = " " # Note:
+PEFT only works on a notbeook with GPU-support. use_peft = True ``` ```python #
+Downloading the model, tokenizer, feature extractor and processor process =
+DataPrep(huggingface_read_token, dataset_name,language_abbr,model_id,
+processing_task, use_peft) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ```python # Preprocessing the Dataset
 processed_dataset = process.load_dataset(feature_extractor, tokenizer,
 feature_processor) ``` ```python # Training the model trainer = Trainer
 (huggingface_write_token, model_id, processed_dataset, model,
 feature_processor, feature_extractor, tokenizer, language_abbr, wandb_api_key,
 use_peft) trainer.train() ``` ```python # Generate demo model_name = " " # Your
 finetuned model name on huggingface hub e.g ""KevinKibe/whisper-small-af" demo
 = WhisperDemo(model_name, huggingface_read_token) demo.generate_demo() ``` ##
 Usage on a Virtual Machine - Clone the Repository: Clone or download the
 application code to your local machine. ``` git clone https://github.com/
 KevKibe/African-Whisper.git ``` - Create a virtual environment for the project
 and activate it. ``` python3 -m venv env source venv/bin/activate ``` - Install
 dependencies by running this command ``` pip install -r requirements.txt ``` -
-Navigate to ``` cd src ``` - To start the training , use the following command:
-``` python -m training.main \ --huggingface_read_token
+Navigate to: ``` cd src ``` - To start the training , use the following
+command: ``` python -m training.main \ --huggingface_read_token
 YOUR_HUGGING_FACE_READ_TOKEN_HERE \ --huggingface_write_token
 YOUR_HUGGING_FACE_WRITE_TOKEN_HERE \ --dataset_name DATASET_NAME \ --
 language_abbr LANGUAGE_ABBREVIATION \ --model_id MODEL_ID \ --processing_task
 PROCESSING_TASK \ --wandb_api_key YOUR_WANDB_API_KEY_HERE \ --use_peft ```
 Here's a short description of each argument used in the command: - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. - **--
@@ -97,21 +98,22 @@
 model you wish to fine-tune. Example: 'openai/whisper-small'. This should match
 the model's identifier on the Hugging Face Model Hub. - **--processing_task**:
 Specifies the task for which the model is being trained. Example: 'transcribe'.
 This defines the objective of the model training, such as transcribing audio to
 text. - **--wandb_api_key**: Your Weights & Biases (W&B) API key. This is used
 for logging and tracking the training process if you're using W&B for
 experiment tracking. - **--use_peft**: Add this flag to fine-tune using PEFT
-method and omit it to do full fine-tuning. ## Inference - To get inference from
-your fine-tuned model, follow these steps: - Ensure that ffmpeg is installed by
-running the following commands: ``` # on Ubuntu or Debian sudo apt update &&
-sudo apt install ffmpeg # on Arch Linux sudo pacman -S ffmpeg # on MacOS using
-Homebrew (https://brew.sh/) brew install ffmpeg # on Windows using Chocolatey
-(https://chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https:
-//scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
+method and omit it to do full fine-tuning. PEFT only works on a notbeook with
+GPU-support. ## Inference - To get inference from your fine-tuned model, follow
+these steps: - Ensure that ffmpeg is installed by running the following
+commands: ``` # on Ubuntu or Debian sudo apt update && sudo apt install ffmpeg
+# on Arch Linux sudo pacman -S ffmpeg # on MacOS using Homebrew (https://
+brew.sh/) brew install ffmpeg # on Windows using Chocolatey (https://
+chocolatey.org/) choco install ffmpeg # on Windows using Scoop (https://
+scoop.sh/) scoop install ffmpeg ``` - To get the Gradio inference URL: ```
 python -m training.gradio_demo \ --model_name YOUR_FINETUNED-MODEL \ --
 huggingface_read_token YOUR_HUGGING_FACE_READ_TOKEN_HERE \ ``` - **--
 model_name**: Name of the fine-tuned model to use in your huggingfacehub repo.
 This should match the model's identifier on the Hugging Face Model Hub. - **--
 huggingface_read_token**: Your Hugging Face authentication token for read
 access. It allows you to download datasets and models from Hugging Face. ##
 Deployment - To deploy your fine-tuned model (assuming it's on Hugging Face
```

### Comparing `africanwhisper-0.2.4/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.2.5/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/deployment/main.py` & `africanwhisper-0.2.5/src/deployment/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/tests/test_dataset.py` & `africanwhisper-0.2.5/src/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/training/audio_data_processor.py` & `africanwhisper-0.2.5/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/training/collator.py` & `africanwhisper-0.2.5/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/training/data_prep.py` & `africanwhisper-0.2.5/src/training/data_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     WhisperForConditionalGeneration,
 )
 from .load_data import Dataset
 from .whisper_model_prep import WhisperModelPrep
 from .audio_data_processor import AudioDataProcessor
 from datasets import DatasetDict, Audio, IterableDatasetDict
 from typing import Tuple
-
+import warnings
+warnings.filterwarnings("ignore")
 
 class DataPrep:
     """
 
     A class to encapsulate preparing the speech dataset for model training, including dataset loading, cleaning, and preprocessing tasks like feature extraction and tokenization. .
 
     """
@@ -93,16 +94,24 @@
 
         Returns:
             DatasetDict: A dictionary containing the preprocessed 'train' and 'test' splits of the dataset,
                         ready for use in model training and evaluation. Each split has been cleaned and
                         processed to include only the necessary features for model input.
         """
         dataset = IterableDatasetDict()
+        # dataset= {}
         dataset["train"] = self.data_loader.load_streaming_dataset(split = "train")
         dataset["test"] = self.data_loader.load_streaming_dataset(split = "test")
         print(f"Training Dataset Size: {self.data_loader.count_examples(dataset['train'])}")
         print(f"Testing Dataset Size: {self.data_loader.count_examples(dataset['test'])}")
         dataset = dataset.cast_column("audio", Audio(sampling_rate=16000))
         processor = AudioDataProcessor(dataset, feature_extractor, tokenizer, processor)
         processed_datasets = dataset.map(processor.prepare_dataset, remove_columns=list(next(iter(dataset.values())).features)).with_format("torch")
+        #TODO: Feaature in testing
+        # processed_datasets = {}
+        # for key, value in dataset.items():
+        #     processed_datasets[key] = value.map(processor.prepare_dataset, remove_columns=list(value.features)).with_format("torch")
+
+        # print(f"dataset : {processed_datasets}")
+        # print(f"dataset : {processed_datasets['train']}")
         return processed_datasets
```

### Comparing `africanwhisper-0.2.4/src/training/evaluation.py` & `africanwhisper-0.2.5/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/training/gradio_demo.py` & `africanwhisper-0.2.5/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/training/gradio_inference.py` & `africanwhisper-0.2.5/src/training/gradio_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import torch
 import gradio as gr
 from transformers import pipeline
+import warnings
 
+warnings.filterwarnings("ignore")
 
 class WhisperDemo:
     def __init__(self, model_name, huggingface_read_token):
         self.model_name = model_name
         self.huggingface_read_token = huggingface_read_token
         self.pipe = None
```

### Comparing `africanwhisper-0.2.4/src/training/load_data.py` & `africanwhisper-0.2.5/src/training/load_data.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/training/main.py` & `africanwhisper-0.2.5/src/training/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
 from .data_prep import DataPrep
 from .model_trainer import Trainer
+import warnings
 
+warnings.filterwarnings("ignore")
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description="Run the training orchestrator with specified parameters."
     )
     parser.add_argument(
         "--huggingface_read_token",
```

### Comparing `africanwhisper-0.2.4/src/training/model_trainer.py` & `africanwhisper-0.2.5/src/training/model_trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 from transformers import Seq2SeqTrainingArguments, Seq2SeqTrainer
 from .collator import DataCollatorSpeechSeq2SeqWithPadding
 import evaluate
+import torch
 from datasets import DatasetDict, Dataset
 # from .wandb_callback import WandbProgressResultsCallback
 from transformers.trainer_pt_utils import IterableDatasetShard
 from torch.utils.data import IterableDataset
 from transformers import TrainerCallback
 from .whisper_model_prep import WhisperModelPrep
+import warnings
 
+warnings.filterwarnings("ignore")
 
 class ShuffleCallback(TrainerCallback):
     def on_epoch_begin(self, args, state, control, train_dataloader, **kwargs):
         if isinstance(train_dataloader.dataset, IterableDatasetShard):
             pass
         elif isinstance(train_dataloader.dataset, IterableDataset):
             train_dataloader.dataset.set_epoch(train_dataloader.dataset._epoch + 1)
@@ -92,15 +95,16 @@
             if i == (num_samples-1):
                 break
         sample_dataset = Dataset.from_list(samples)
 
         return sample_dataset
     
     def compute_spectrograms(self, example) -> dict:
-        waveform = example["audio"]["array"]
+        print(f"example of :{example}")
+        waveform = example["input_features"]
         model_prep = WhisperModelPrep(
             self.model_id, self.language_abbr, "transcribe", self.use_peft
         )
         feature_extractor = model_prep.initialize_feature_extractor()
         specs = feature_extractor(
             waveform, sampling_rate=16000, padding="do_not_pad"
         ).input_features[0]
@@ -108,44 +112,53 @@
 
     def train(self):
         """
 
         Conducts the training process using the specified model, dataset, and training configurations.
 
         """
+        # Checks if GPU is available
+        use_gpu = torch.cuda.is_available()
+
+        # Set fp16 and fp16_full_eval to True/False based on GPU availability
+        fp16 = use_gpu
+        # fp16_full_eval = use_gpu
+
         data_collator = DataCollatorSpeechSeq2SeqWithPadding(
             processor=self.feature_processor
         )
         training_args = Seq2SeqTrainingArguments(
             output_dir=f"./{self.model_id}-{self.language_abbr}",
-            per_device_train_batch_size=32,
+            per_device_train_batch_size=96,
             gradient_accumulation_steps=1,
             learning_rate=1e-5,
             max_steps=100,
             gradient_checkpointing=True,
-            fp16=False,
+            fp16=fp16,
+            # fp16_full_eval = fp16_full_eval,
             optim="adamw_bnb_8bit",
             evaluation_strategy="steps",
-            per_device_eval_batch_size=32,
+            per_device_eval_batch_size=64,
             predict_with_generate=True,
             generation_max_length=225,
             save_steps=25,
             eval_steps=25,
             logging_steps=25,
             load_best_model_at_end=True,
             metric_for_best_model="wer",
             greater_is_better=False,
             push_to_hub=True,
             hub_token=self.huggingface_write_token,
             report_to="wandb",
             remove_unused_columns=False,
             ignore_data_skip=True,
         )
-    
-        # eval_dataset = self.test_dataset.map(self.compute_spectrograms)
+
+
+        # eval_dataset = self.load_samples_dataset(self.dataset["test"].map(self.compute_spectrograms))
         eval_dataset = self.dataset["test"]
 
         trainer = Seq2SeqTrainer(
             args=training_args,
             model=self.model,
             train_dataset=self.dataset["train"],
             eval_dataset=eval_dataset,
```

### Comparing `africanwhisper-0.2.4/src/training/wandb_callback.py` & `africanwhisper-0.2.5/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.4/src/training/whisper_model_prep.py` & `africanwhisper-0.2.5/src/training/whisper_model_prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from transformers import WhisperFeatureExtractor, WhisperTokenizer, WhisperProcessor
 from transformers import WhisperForConditionalGeneration
 from peft import prepare_model_for_kbit_training
 from peft import LoraConfig, get_peft_model
+import warnings
 
+warnings.filterwarnings("ignore")
 
 class WhisperModelPrep:
     """Facilitates the preparation of datasets for fine-tuning with the Whisper model,
     encompassing feature extraction, tokenization, and dataset processing.
 
     Attributes
     ----------
@@ -84,14 +86,15 @@
         processing task specified during the class initialization.
 
         Returns
         -------
             WhisperForConditionalGeneration: The configured Whisper model ready for conditional generation tasks.
 
         """
+
         if self.use_peft:
             model = WhisperForConditionalGeneration.from_pretrained(
                 self.model_id,
                 cache_dir=f"./{self.language_abbr}/model",
                 load_in_8bit=True,
                 device_map="auto",
             )
```

