# Comparing `tmp/video_images_creator-0.2.8.tar.gz` & `tmp/video_images_creator-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_images_creator-0.2.8.tar", last modified: Thu Nov 16 10:36:09 2023, max compression
+gzip compressed data, was "video_images_creator-0.2.9.tar", last modified: Fri Mar  1 12:00:40 2024, max compression
```

## Comparing `video_images_creator-0.2.8.tar` & `video_images_creator-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2023-11-16 10:36:09.207824 video_images_creator-0.2.8/
--rw-r--r--   0 nikhilsharma   (501) staff       (20)     1324 2023-08-21 11:06:59.000000 video_images_creator-0.2.8/LICENSE
--rw-r--r--   0 nikhilsharma   (501) staff       (20)     1319 2023-11-16 10:36:09.207736 video_images_creator-0.2.8/PKG-INFO
--rw-r--r--   0 nikhilsharma   (501) staff       (20)      899 2023-08-22 10:52:35.000000 video_images_creator-0.2.8/README.md
--rw-r--r--   0 nikhilsharma   (501) staff       (20)       91 2023-08-22 10:39:40.000000 video_images_creator-0.2.8/pyproject.toml
--rw-r--r--   0 nikhilsharma   (501) staff       (20)      153 2023-11-16 10:36:09.208576 video_images_creator-0.2.8/setup.cfg
--rw-r--r--   0 nikhilsharma   (501) staff       (20)      837 2023-11-16 10:35:59.000000 video_images_creator-0.2.8/setup.py
-drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2023-11-16 10:36:09.193144 video_images_creator-0.2.8/src/
-drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2023-11-16 10:36:09.204766 video_images_creator-0.2.8/src/video_images_creator/
--rw-rw-r--   0 nikhilsharma   (501) staff       (20)   208320 2023-06-30 00:38:00.000000 video_images_creator-0.2.8/src/video_images_creator/Rubik-Bold.ttf
--rw-rw-rw-   0 nikhilsharma   (501) staff       (20)   216244 2015-10-14 10:02:36.000000 video_images_creator-0.2.8/src/video_images_creator/Rubik-Medium.ttf
--rw-r--r--   0 nikhilsharma   (501) staff       (20)      110 2023-08-21 11:06:59.000000 video_images_creator-0.2.8/src/video_images_creator/__init__.py
--rw-r--r--   0 nikhilsharma   (501) staff       (20)    39843 2023-09-21 08:47:33.000000 video_images_creator-0.2.8/src/video_images_creator/builderbackground.png
--rw-r--r--   0 nikhilsharma   (501) staff       (20)    37227 2023-10-12 10:30:24.000000 video_images_creator-0.2.8/src/video_images_creator/closingframe_f.png
--rw-r--r--   0 nikhilsharma   (501) staff       (20)   100150 2023-09-21 08:21:35.000000 video_images_creator-0.2.8/src/video_images_creator/combined_left.jpg
--rw-r--r--   0 nikhilsharma   (501) staff       (20)    99969 2023-09-21 08:21:40.000000 video_images_creator-0.2.8/src/video_images_creator/combined_right.jpg
--rw-r--r--   0 nikhilsharma   (501) staff       (20)  5816956 2023-11-16 10:34:26.000000 video_images_creator-0.2.8/src/video_images_creator/instantvideoaudio.wav
--rw-r--r--   0 nikhilsharma   (501) staff       (20)    28859 2023-11-14 19:14:11.000000 video_images_creator-0.2.8/src/video_images_creator/video_creator.py
-drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2023-11-16 10:36:09.207391 video_images_creator-0.2.8/src/video_images_creator.egg-info/
--rw-r--r--   0 nikhilsharma   (501) staff       (20)     1319 2023-11-16 10:36:09.000000 video_images_creator-0.2.8/src/video_images_creator.egg-info/PKG-INFO
--rw-r--r--   0 nikhilsharma   (501) staff       (20)      676 2023-11-16 10:36:09.000000 video_images_creator-0.2.8/src/video_images_creator.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilsharma   (501) staff       (20)        1 2023-11-16 10:36:09.000000 video_images_creator-0.2.8/src/video_images_creator.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilsharma   (501) staff       (20)       27 2023-11-16 10:36:09.000000 video_images_creator-0.2.8/src/video_images_creator.egg-info/requires.txt
--rw-r--r--   0 nikhilsharma   (501) staff       (20)       21 2023-11-16 10:36:09.000000 video_images_creator-0.2.8/src/video_images_creator.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2024-03-01 12:00:40.082089 video_images_creator-0.2.9/
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)     1324 2023-08-21 11:06:59.000000 video_images_creator-0.2.9/LICENSE
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)     1319 2024-03-01 12:00:40.082005 video_images_creator-0.2.9/PKG-INFO
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)      899 2023-08-22 10:52:35.000000 video_images_creator-0.2.9/README.md
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)       91 2023-08-22 10:39:40.000000 video_images_creator-0.2.9/pyproject.toml
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)      153 2024-03-01 12:00:40.082892 video_images_creator-0.2.9/setup.cfg
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)      837 2024-03-01 12:00:28.000000 video_images_creator-0.2.9/setup.py
+drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2024-03-01 12:00:40.058887 video_images_creator-0.2.9/src/
+drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2024-03-01 12:00:40.080321 video_images_creator-0.2.9/src/video_images_creator/
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)   269998 2024-03-01 08:35:04.000000 video_images_creator-0.2.9/src/video_images_creator/3featureframe.png
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)   271147 2024-03-01 08:35:30.000000 video_images_creator-0.2.9/src/video_images_creator/5featureframe.png
+-rw-rw-r--   0 nikhilsharma   (501) staff       (20)   208320 2023-06-30 00:38:00.000000 video_images_creator-0.2.9/src/video_images_creator/Rubik-Bold.ttf
+-rw-rw-rw-   0 nikhilsharma   (501) staff       (20)   216244 2015-10-14 10:02:36.000000 video_images_creator-0.2.9/src/video_images_creator/Rubik-Medium.ttf
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)      110 2023-08-21 11:06:59.000000 video_images_creator-0.2.9/src/video_images_creator/__init__.py
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)    39843 2023-09-21 08:47:33.000000 video_images_creator-0.2.9/src/video_images_creator/builderbackground.png
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)    37227 2023-10-12 10:30:24.000000 video_images_creator-0.2.9/src/video_images_creator/closingframe_f.png
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)   100150 2023-09-21 08:21:35.000000 video_images_creator-0.2.9/src/video_images_creator/combined_left.jpg
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)    99969 2023-09-21 08:21:40.000000 video_images_creator-0.2.9/src/video_images_creator/combined_right.jpg
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)   266733 2024-03-01 08:15:28.000000 video_images_creator-0.2.9/src/video_images_creator/featureframe.png
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)  5816956 2023-11-16 10:34:26.000000 video_images_creator-0.2.9/src/video_images_creator/instantvideoaudio.wav
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)    37490 2024-02-29 10:36:37.000000 video_images_creator-0.2.9/src/video_images_creator/preterminal.png
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)   262853 2024-03-01 08:12:20.000000 video_images_creator-0.2.9/src/video_images_creator/startfeatureframe.png
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)    51621 2024-02-29 10:14:36.000000 video_images_creator-0.2.9/src/video_images_creator/terminal.png
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)    44510 2024-03-01 12:00:24.000000 video_images_creator-0.2.9/src/video_images_creator/video_creator.py
+drwxr-xr-x   0 nikhilsharma   (501) staff       (20)        0 2024-03-01 12:00:40.081708 video_images_creator-0.2.9/src/video_images_creator.egg-info/
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)     1319 2024-03-01 12:00:40.000000 video_images_creator-0.2.9/src/video_images_creator.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)      930 2024-03-01 12:00:40.000000 video_images_creator-0.2.9/src/video_images_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)        1 2024-03-01 12:00:40.000000 video_images_creator-0.2.9/src/video_images_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)       27 2024-03-01 12:00:40.000000 video_images_creator-0.2.9/src/video_images_creator.egg-info/requires.txt
+-rw-r--r--   0 nikhilsharma   (501) staff       (20)       21 2024-03-01 12:00:40.000000 video_images_creator-0.2.9/src/video_images_creator.egg-info/top_level.txt
```

### Comparing `video_images_creator-0.2.8/LICENSE` & `video_images_creator-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/PKG-INFO` & `video_images_creator-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video_images_creator
-Version: 0.2.8
+Version: 0.2.9
 Summary: Create videos from images using the 'video_images_creator' package.
 Home-page: 
 Author: Nikhil Sharma
 Author-email: nikhilsharma972@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
```

### Comparing `video_images_creator-0.2.8/README.md` & `video_images_creator-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/setup.py` & `video_images_creator-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='video_images_creator',
-    version='0.2.8',
+    version='0.2.9',
     description= "Create videos from images using the 'video_images_creator' package.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='Nikhil Sharma',
     author_email='nikhilsharma972@gmail.com',
     license='BSD 2-clause',
```

### Comparing `video_images_creator-0.2.8/src/video_images_creator/Rubik-Bold.ttf` & `video_images_creator-0.2.9/src/video_images_creator/Rubik-Bold.ttf`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/src/video_images_creator/Rubik-Medium.ttf` & `video_images_creator-0.2.9/src/video_images_creator/Rubik-Medium.ttf`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/src/video_images_creator/builderbackground.png` & `video_images_creator-0.2.9/src/video_images_creator/builderbackground.png`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/src/video_images_creator/closingframe_f.png` & `video_images_creator-0.2.9/src/video_images_creator/closingframe_f.png`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/src/video_images_creator/combined_left.jpg` & `video_images_creator-0.2.9/src/video_images_creator/combined_left.jpg`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/src/video_images_creator/combined_right.jpg` & `video_images_creator-0.2.9/src/video_images_creator/combined_right.jpg`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/src/video_images_creator/instantvideoaudio.wav` & `video_images_creator-0.2.9/src/video_images_creator/instantvideoaudio.wav`

 * *Files identical despite different names*

### Comparing `video_images_creator-0.2.8/src/video_images_creator/video_creator.py` & `video_images_creator-0.2.9/src/video_images_creator/video_creator.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,402 @@
 
 def generate_random_string(length):
     characters = string.ascii_letters + string.digits
     random_string = ''.join(secrets.choice(characters) for _ in range(length))
     return random_string
 
 
+def add_alpha_channel(img):
+    if img.shape[2] == 4:  # Image already has an alpha channel
+        return img
+    else:  # Add alpha channel to the image
+        alpha_channel = np.ones((img.shape[0], img.shape[1], 1), dtype=img.dtype) * 255  # Fully opaque
+        return np.concatenate((img, alpha_channel), axis=-1)
+
+def set_transparency(img, opacity):
+    # Ensure the image has an alpha channel
+    img_with_alpha = add_alpha_channel(img)
+    # Adjust the alpha channel to set the desired opacity
+    img_with_alpha[:, :, 3] = img_with_alpha[:, :, 3] * opacity
+    return img_with_alpha
+
+def add_images_in_single_frame(blended_roi_obj, directory_name, current_index, transparency, frames):
+ 
+    x_coordinate = 1650
+    x, y = x_coordinate, 540
+    background = pkg_resources.resource_filename('video_images_creator', "featureframe.png")
+    blended_roi = blended_roi_obj["blended_roi"]
+    h_o = blended_roi_obj["h_o"]
+    w_o = blended_roi_obj["w_o"]
+
+    blended_roi = set_transparency(blended_roi, transparency)
+
+    #background[y:y+h_o, x:x+w_o] = blended_roi[:, :, :3] 
+
+
+    overlay_image = blended_roi[..., :3]  # RGB channels
+    mask = blended_roi[..., 3:] / 255.0  # Alpha channel normalized
+
+    background[y:y+h_o, x:x+w_o] = (1.0 - mask) * background[y:y+h_o, x:x+w_o] + mask * overlay_image
+
+
+    file_name = f'{directory_name}/frame_{current_index}.jpg' 
+    cv2.imwrite(file_name, background)
+
+    current_index_ = current_index
+
+    for i in range(1,frames): 
+        index = i + current_index_
+        destination = f'{directory_name}/frame_{index}.jpg'
+        shutil.copyfile(file_name, destination)
+        current_index = current_index + 1 
+
+    
+
+
+    return current_index
+
+
+def add_blank_background_frames(directory_name, current_index):
+  
+    # background = cv2.imread("features/startfeatureframe.png")
+    # file_name = f'{directory_name}/frame_{current_index}.jpg' 
+    # cv2.imwrite(file_name, background)
+
+    current_index_ = current_index + 1
+
+    ending_page_image = pkg_resources.resource_filename('video_images_creator', "startfeatureframe.png")
+
+    #create original image with cv2 imwrite
+    original_file_name = f'{directory_name}/frame_{current_index_}.jpg'
+    cv2.imwrite(original_file_name, ending_page_image)
+
+    for i in range(2,51): 
+        index = i + current_index_
+        destination = f'{directory_name}/frame_{index}.jpg'
+        shutil.copyfile(original_file_name, destination)
+        current_index = current_index + 1
+
+    return current_index
+
+
+def add_images_in_frameset(feature_images_urls_blended_rois, directory_name, current_index, total_frames, transparency):
+ 
+    x_coordinate_increement = 0 
+    initial_x_coordinate = 0
+
+    feature_images_urls = list(feature_images_urls_blended_rois.keys())
+    if len(feature_images_urls) == 5:
+        ###
+        x_coordinate_increement = 0
+        initial_x_coordinate = 400
+        background = pkg_resources.resource_filename('video_images_creator', "5featureframe.png")
+    elif len(feature_images_urls) == 4:
+        initial_x_coordinate = 713
+        background_img_url = "https://testkals.s3.amazonaws.com/4featureframe.png"
+    elif len(feature_images_urls) == 3:
+        initial_x_coordinate = 1025
+        background = pkg_resources.resource_filename('video_images_creator', "3featureframe.png")
+    elif len(feature_images_urls) == 2:
+        initial_x_coordinate = 1340
+        background_img_url = "https://testkals.s3.amazonaws.com/2featureframe.png" 
+    elif len(feature_images_urls) == 1:
+        initial_x_coordinate = 1650
+        background_img_url = "https://testkals.s3.amazonaws.com/featureframe.png"
+    else:
+        print("Exit?///") 
+
+    max_index = len(feature_images_urls) - 1
+    running_index = 0
+    
+  
+    for feature_images_url in feature_images_urls: 
+
+        x_coordinate = initial_x_coordinate + x_coordinate_increement
+
+        x, y = x_coordinate + 13, 650
+        # Generate the rounded image
+
+        blended_roi = feature_images_urls_blended_rois[feature_images_url]["blended_roi"]
+        w_o = feature_images_urls_blended_rois[feature_images_url]["w_o"]
+        h_o = feature_images_urls_blended_rois[feature_images_url]["h_o"]
+
+
+        if running_index == 0 or running_index == max_index:
+            blended_roi = set_transparency(blended_roi, transparency)
+            #background[y:y+h_o, x:x+w_o] = blended_roi[:, :, :3] 
+            overlay_image = blended_roi[..., :3]  # RGB channels
+            mask = blended_roi[..., 3:] / 255.0  # Alpha channel normalized
+
+            background[y:y+h_o, x:x+w_o] = (1.0 - mask) * background[y:y+h_o, x:x+w_o] + mask * overlay_image
+        else:
+            blended_roi = set_transparency(blended_roi, transparency)
+            background[y:y+h_o, x:x+w_o] = blended_roi[:, :, :3] 
+
+        running_index = running_index + 1
+
+        
+        #background[y:y+h_o, x:x+w_o] = blended_roi[:, :, :3] 
+
+        #background = overlay_transparent(background, blended_roi, x_coordinate, 650)  # Adjust y-coordinate as needed
+
+
+        x_coordinate_increement = x_coordinate_increement + 626 
+
+
+    file_name = f'{directory_name}/frame_{current_index}.jpg' 
+    cv2.imwrite(file_name, background)
+
+    current_index_ = current_index
+
+    for i in range(1,total_frames): 
+        index = i + current_index_
+        destination = f'{directory_name}/frame_{index}.jpg'
+        shutil.copyfile(file_name, destination)
+        current_index = current_index + 1
+
+    return current_index
+
+
+def create_feature_set_frames_v2(current_index, directory_name, feature_images_urls): 
+
+
+    current_index = add_blank_background_frames(directory_name, current_index)
+
+    overlay = read_image(feature_images_urls[0]) 
+    screen_width, screen_height = 551, 1210
+    overlay = cv2.resize(overlay, (screen_width, screen_height)) 
+    corner_radius = 30
+    mask = create_rounded_mask(overlay, corner_radius)
+    rounded_image = get_rounded_image(overlay, mask)
+    x, y = 1650, 540
+    background = pkg_resources.resource_filename('video_images_creator', "featureframe.png")
+    h_o, w_o, _ = rounded_image.shape 
+    blended_roi = refined_alpha_blend(background[y:y+h_o, x:x+w_o], rounded_image) 
+
+    blended_roi_obj = {"blended_roi": blended_roi, "h_o": h_o, "w_o": w_o}
+
+    current_index = add_images_in_single_frame(blended_roi_obj, directory_name, current_index, 0.1, 12)
+
+    current_index = add_images_in_single_frame(blended_roi_obj, directory_name, current_index, 0.5,12)
+
+    current_index = add_images_in_single_frame(blended_roi_obj, directory_name, current_index, 1,45)   
+
+    #current_index = add_images_in_frameset(feature_images_urls[:1], directory_name, current_index,100, 0.1) 
+
+    temp_feature_images_urls = feature_images_urls[:3] 
+    temp_feature_images_urls[0], temp_feature_images_urls[1] = temp_feature_images_urls[1], temp_feature_images_urls[0] 
+
+    feature_images_blended_roi_dict = {} 
+    x_coordinate_increement = 0
+    initial_x_coordinate = 1025
+
+    for temp_feature_images_url in temp_feature_images_urls:
+        overlay = read_image(temp_feature_images_url) 
+      
+        x_coordinate = initial_x_coordinate + x_coordinate_increement
+        screen_width, screen_height = 480, 1065
+        x, y = x_coordinate + 13, 650
+    
+        overlay = cv2.resize(overlay, (screen_width, screen_height))
+        background = pkg_resources.resource_filename('video_images_creator', "3featureframe.png")
+        corner_radius = 30
+        mask = create_rounded_mask(overlay, corner_radius)
+        # Generate the rounded image
+        rounded_image = get_rounded_image(overlay, mask)
+        h_o, w_o, _ = rounded_image.shape
+        blended_roi = refined_alpha_blend(background[y:y+h_o, x:x+w_o], rounded_image)
+        blended_roi_obj = {"blended_roi": blended_roi, "h_o": h_o, "w_o": w_o}
+
+        feature_images_blended_roi_dict[temp_feature_images_url] = blended_roi_obj  
+
+        x_coordinate_increement = x_coordinate_increement + 626 
+
+
+
+    current_index = add_images_in_frameset(feature_images_blended_roi_dict, directory_name, current_index,12, 0.1) 
+
+    current_index = add_images_in_frameset(feature_images_blended_roi_dict, directory_name, current_index,12, 0.5) 
+
+    current_index = add_images_in_frameset(feature_images_blended_roi_dict, directory_name, current_index,45, 1) 
+
+
+    temp_feature_images_urls = feature_images_urls[:5] 
+    temp_feature_images_urls[0], temp_feature_images_urls[2] = temp_feature_images_urls[2], temp_feature_images_urls[0]
+
+
+    feature_images_blended_roi_dict = {} 
+    x_coordinate_increement = 0
+    initial_x_coordinate = 400
+
+    for temp_feature_images_url in temp_feature_images_urls:
+        overlay = read_image(temp_feature_images_url) 
+        x_coordinate = initial_x_coordinate + x_coordinate_increement
+
+        screen_width, screen_height = 480, 1065
+        x, y = x_coordinate + 13, 650
+    
+        overlay = cv2.resize(overlay, (screen_width, screen_height))
+        background = pkg_resources.resource_filename('video_images_creator', "5featureframe.png")
+        corner_radius = 30
+        mask = create_rounded_mask(overlay, corner_radius)
+        # Generate the rounded image
+        rounded_image = get_rounded_image(overlay, mask)
+        h_o, w_o, _ = rounded_image.shape
+        blended_roi = refined_alpha_blend(background[y:y+h_o, x:x+w_o], rounded_image)
+        blended_roi_obj = {"blended_roi": blended_roi, "h_o": h_o, "w_o": w_o}
+
+        feature_images_blended_roi_dict[temp_feature_images_url] = blended_roi_obj  
+
+        x_coordinate_increement = x_coordinate_increement + 626 
+
+
+
+    current_index = add_images_in_frameset(feature_images_blended_roi_dict, directory_name, current_index, 12, 0.1)
+
+    current_index = add_images_in_frameset(feature_images_blended_roi_dict, directory_name, current_index, 12, 0.5)
+
+    current_index = add_images_in_frameset(feature_images_blended_roi_dict, directory_name, current_index,180, 1)
+
+
+    return current_index
+
+
+
+def create_starting_frames(current_index, directory_name, ending_page_image_url, total_frames):
+
+    if ending_page_image_url == "terminal":
+        ending_page_image = pkg_resources.resource_filename('video_images_creator', "terminal_image.png")
+
+    elif ending_page_image_url == "preterminal":
+        ending_page_image = pkg_resources.resource_filename('video_images_creator', "preterminal_image.png")
+    else:
+        return
+    
+    #create original image with cv2 imwrite
+    original_file_name = f'{directory_name}/frame_{current_index}.jpg'
+    cv2.imwrite(original_file_name, ending_page_image)
+    for i in range(1,total_frames): 
+        index = current_index + i
+        destination = f'{directory_name}/frame_{index}.jpg'
+        shutil.copyfile(original_file_name, destination)
+        #cv2.imwrite(destination, ending_page_image) 
+
+    return index
+
+def add_images_in_single_frame_V2(feature_images_url, font, directory_name, current_index, feature_title):
+    first_image = True 
+    background = ''
+    x_coordinate = 1650
+    overlay = read_image(feature_images_url) 
+    screen_width, screen_height = 551, 1210
+    x, y = x_coordinate, 540
+    background = pkg_resources.resource_filename('video_images_creator', "featureframe.png")
+
+    overlay = cv2.resize(overlay, (screen_width, screen_height))  
+    
+    if first_image == True:
+        first_image = False
+
+        corner_radius = 30
+        mask = create_rounded_mask(overlay, corner_radius)
+        # Generate the rounded image
+        rounded_image = get_rounded_image(overlay, mask)
+
+
+        h_o, w_o, _ = rounded_image.shape 
+        blended_roi = refined_alpha_blend(background[y:y+h_o, x:x+w_o], rounded_image) 
+
+
+        background[y:y+h_o, x:x+w_o] = blended_roi[:, :, :3] 
+
+        line = feature_title
+
+        pil_image = Image.fromarray(cv2.cvtColor(background, cv2.COLOR_BGR2RGB))
+        draw = ImageDraw.Draw(pil_image)
+        
+        print(x_coordinate) 
+        print(len(line))
+        if len(line) > 13: 
+            x_coordinate = int(max((3840 -  ( len(line) * 40 )  ),0) / 2 ) #tradeoff calc
+        print(x_coordinate)
+        draw.text((x_coordinate, 1910), line.strip(), font=font, fill=(0, 0, 0))  
+
+        background = cv2.cvtColor(np.array(pil_image), cv2.COLOR_RGB2BGR)
+
+
+        file_name = f'{directory_name}/frame_{current_index}.jpg' 
+        cv2.imwrite(file_name, background)
+
+        current_index_ = current_index
+
+        for i in range(1,180): 
+            index = i + current_index_
+            destination = f'{directory_name}/frame_{index}.jpg'
+            shutil.copyfile(file_name, destination)
+            current_index = current_index + 1 
+
+    
+
+
+    return current_index
+
+
+def add_feature_frames(feature_images_urls, directory_name, current_index, feature_titles):
+
+    index = 0
+     # Load the custom font
+    font_path = pkg_resources.resource_filename('video_images_creator', 'Rubik-Medium.ttf')
+    font_size = 84
+    font = ImageFont.truetype(font_path, font_size)
+  
+    
+    for feature_images_url in feature_images_urls:
+        current_index = add_images_in_single_frame_V2(feature_images_url, font, directory_name, current_index, feature_titles[index]) 
+        index = index + 1 
+
+    return current_index
+
+
+def build_v2(feature_images_urls, feature_names):
+
+    ensure_required_directories_existis()
+    current_index = 0
+    folder_name = generate_random_string(10)  
+    directory_name = f'images/{folder_name}'
+    os.mkdir(directory_name) 
+
+
+    current_running_index = create_starting_frames(current_index, directory_name, "terminal",400) 
+    #feature_images_urls = ["https://buildernowassets.azureedge.net/builder-now-beta/uploads/staging/build_card_hero_image/file/103054602/1a0d1594-1e81-4181-b4bb-92d31f197539.png", "https://buildernowassets.azureedge.net/builder-now-beta/uploads/staging/build_card_hero_image/file/103054583/30188996-01e3-4eab-9a36-552f70d1bb73.png", "https://buildernowassets.azureedge.net/builder-now-beta/uploads/staging/build_card_hero_image/file/130179838/d41999b6-b89d-4f3a-988b-3a3dd85dd986.png", "https://buildernowassets.azureedge.net/builder-now-beta/uploads/staging/build_card_hero_image/file/130179842/d9954a75-b307-4839-b634-f18c4e4b7b1a.png", "https://builderbuckets.blob.core.windows.net/builder-now-production/uploads/production/build_card_hero_image/file/40258072/987611d1-19cd-4931-a618-0897aa0d79d1.png", "https://builderbuckets.blob.core.windows.net/builder-now-production/uploads/production/build_card_hero_image/file/40258074/b82fae9a-4d79-45e9-a286-dc6f1b92a0c4.png", "https://builderbuckets.blob.core.windows.net/builder-now-production/uploads/production/build_card_hero_image/file/40258060/5cc635d6-b63a-4b20-929f-cf12eb178765.png"]
+    #feature_titles = ["Splash Screen", "User Profile", "Signup/ Login", "Categories/ Sub-Categories", "Order Summary", "Payment Details", "Order Summary"]
+
+    current_running_index = create_starting_frames(current_running_index, directory_name, "preterminal", 80)
+    current_running_index = create_feature_set_frames_v2(current_running_index, directory_name, feature_images_urls)
+
+
+    #current_running_index = create_feature_set_frames_v2(current_running_index, "images/mytest", feature_images_urls)
+
+    current_running_index = add_feature_frames(feature_images_urls, directory_name, current_running_index, feature_names) 
+
+    current_running_index = create_starting_frames(current_running_index, directory_name, "preterminal", 60)
+    current_running_index = create_starting_frames(current_running_index, directory_name, "terminal",180)
+
+
+    run_ffmpeg(directory_name, folder_name) 
+    return flush_video_images(directory_name, folder_name) 
+
+
+
+
+
+
+
+
+
 def build(image_file_paths, feature_names, project_name, logo_url):
     ensure_required_directories_existis()
     current_index = 0
     folder_name = generate_random_string(10)  
     directory_name = f'images/{folder_name}' 
     bg_image_path = pkg_resources.resource_filename('video_images_creator', "builderbackground.png") 
     bg_img = cv2.imread(bg_image_path)
```

### Comparing `video_images_creator-0.2.8/src/video_images_creator.egg-info/PKG-INFO` & `video_images_creator-0.2.9/src/video_images_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: video-images-creator
-Version: 0.2.8
+Name: video_images_creator
+Version: 0.2.9
 Summary: Create videos from images using the 'video_images_creator' package.
 Home-page: 
 Author: Nikhil Sharma
 Author-email: nikhilsharma972@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
```

### Comparing `video_images_creator-0.2.8/src/video_images_creator.egg-info/SOURCES.txt` & `video_images_creator-0.2.9/src/video_images_creator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+src/video_images_creator/3featureframe.png
+src/video_images_creator/5featureframe.png
 src/video_images_creator/Rubik-Bold.ttf
 src/video_images_creator/Rubik-Medium.ttf
 src/video_images_creator/__init__.py
 src/video_images_creator/builderbackground.png
 src/video_images_creator/closingframe_f.png
 src/video_images_creator/combined_left.jpg
 src/video_images_creator/combined_right.jpg
+src/video_images_creator/featureframe.png
 src/video_images_creator/instantvideoaudio.wav
+src/video_images_creator/preterminal.png
+src/video_images_creator/startfeatureframe.png
+src/video_images_creator/terminal.png
 src/video_images_creator/video_creator.py
 src/video_images_creator.egg-info/PKG-INFO
 src/video_images_creator.egg-info/SOURCES.txt
 src/video_images_creator.egg-info/dependency_links.txt
 src/video_images_creator.egg-info/requires.txt
 src/video_images_creator.egg-info/top_level.txt
```

