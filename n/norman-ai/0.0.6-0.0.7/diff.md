# Comparing `tmp/norman_ai-0.0.6.tar.gz` & `tmp/norman_ai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norman_ai-0.0.6.tar", last modified: Tue May 23 20:22:37 2023, max compression
+gzip compressed data, was "norman_ai-0.0.7.tar", last modified: Sat May 27 20:04:22 2023, max compression
```

## Comparing `norman_ai-0.0.6.tar` & `norman_ai-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.396718 norman_ai-0.0.6/
--rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    31048 2023-05-23 20:22:37.397958 norman_ai-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    30535 2023-05-23 20:06:43.000000 norman_ai-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      688 2023-05-23 20:22:37.397958 norman_ai-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.368092 norman_ai-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.387960 norman_ai-0.0.6/src/norman_ai/
--rw-rw-rw-   0        0        0       28 2023-05-23 14:39:46.000000 norman_ai-0.0.6/src/norman_ai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.395437 norman_ai-0.0.6/src/norman_ai/data/
--rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.0.6/src/norman_ai/data/norman_model1.h5
--rw-rw-rw-   0        0        0    48803 2023-05-23 20:22:08.000000 norman_ai-0.0.6/src/norman_ai/norman_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.393540 norman_ai-0.0.6/src/norman_ai.egg-info/
--rw-rw-rw-   0        0        0    31048 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.122078 norman_ai-0.0.7/
+-rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    31934 2023-05-27 20:04:22.122583 norman_ai-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    31421 2023-05-27 19:58:41.000000 norman_ai-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      688 2023-05-27 20:04:22.123725 norman_ai-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.093852 norman_ai-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.113648 norman_ai-0.0.7/src/norman_ai/
+-rw-rw-rw-   0        0        0       28 2023-05-23 14:39:46.000000 norman_ai-0.0.7/src/norman_ai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.119990 norman_ai-0.0.7/src/norman_ai/data/
+-rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.0.7/src/norman_ai/data/norman_model1.h5
+-rw-rw-rw-   0        0        0    54035 2023-05-27 20:00:01.000000 norman_ai-0.0.7/src/norman_ai/norman_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.118990 norman_ai-0.0.7/src/norman_ai.egg-info/
+-rw-rw-rw-   0        0        0    31934 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/top_level.txt
```

### Comparing `norman_ai-0.0.6/LICENSE.txt` & `norman_ai-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.6/PKG-INFO` & `norman_ai-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: norman_ai
-Version: 0.0.6
-Summary: A package for automation of the novel object recognition test.
-Home-page: https://github.com/Seyij/norman
-Author: seyij_p
-Author-email: seyi.ooj@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # The NORMAN System
 
 The Novel Object Recognition Mouse Analysis Network (NORMAN) system is a package for automation of the novel object recognition behavioural assay in neuroscience studies.
 
 PyPi link: https://pypi.org/project/norman-ai/
 
 This is part of work that will be presented as a poster at the [BNA Festival 2021](https://meetings.bna.org.uk/bna2021/) which runs from the 12-15th of April. It was developed as part of an MSci degree at the University of Dundee. The package and repository will be updated with video outlines and other details shortly, in the run up to the BNA festival.
@@ -476,14 +462,29 @@
 
 #show results rounded to 2 decimal places
 print(round(di, 2), round(tl , 2), round(tr,2) , round(fps, 2))
 0.35 20.81 43.66 18.07
 
 ```
 
+##### __*Converting maze project csv into one compatible with NORMAN*__
+
+Note: This function is only applicable to one specific project. This is a function to convert Deeplabcut output that was recorded from the bottom of the mouse to one compatible with the rest of the NORMAN system. It assumes the nose, mid and tailbase of the mouse marked were marked in Deeplabcut, and uses these to infer where the ears are, then creates a new CSV based on this. This csv file can then be used as a normal pose file in the system going forwards. It would be advisable to use this function in a loop to do a lot of files at once.
+
+```python
+#get name of the file you want to convert
+maze_pose_file = r"maze_dlc_output.csv"
+#name of the the new file you want to create
+new_file_name = "converted_file.csv"
+#convert the file
+nf.maze_file_convert(maze_pose_file, new_file_name)
+```
+
+
+
 ### Using Deeplabcut with NORMAN.
 
 Deeplabcut is a python library for marker-less tracking of animals using artificial neural networks. It provides a variety of functions centred around streamlining the process of tracking animals. The general workflow of the library is to use a neural network that has been pretrained on animal movement, train it to recognise features on the animal you wish to track by labelling images, then use the trained network to track animal movement on a selection of videos. For in depth details please refer to the official [deeplabcut tutorials on github](https://github.com/DeepLabCut/DeepLabCut/blob/master/docs/UseOverviewGuide.md). Here I will briefly discuss points that are relevant for using Deeplabcut in tandem with the NORMAN system.
 
 Installation – The tutorials recommend tensorflow-gpu installation for using Deeplabcut with hardware accelleration. But the previously discussed tensorflow-directml based environment allows a lot easier installation when using a GPU and allows you to have much more customizable environments, while remaining compatible with deeplabcut.
 
 Config file – When you start a new deeplabcut project it creates a folder with a “config.yaml” file. This config file is what all the functions use to find other files in the directory, such as the location of the trained models. The entire project folder can be moved, copied and shared. As long as the information in the config file is up do date, all the functions should work as normal.
```

### Comparing `norman_ai-0.0.6/README.md` & `norman_ai-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: norman_ai
+Version: 0.0.7
+Summary: A package for automation of the novel object recognition test.
+Home-page: https://github.com/Seyij/norman
+Author: seyij_p
+Author-email: seyi.ooj@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # The NORMAN System
 
 The Novel Object Recognition Mouse Analysis Network (NORMAN) system is a package for automation of the novel object recognition behavioural assay in neuroscience studies.
 
 PyPi link: https://pypi.org/project/norman-ai/
 
 This is part of work that will be presented as a poster at the [BNA Festival 2021](https://meetings.bna.org.uk/bna2021/) which runs from the 12-15th of April. It was developed as part of an MSci degree at the University of Dundee. The package and repository will be updated with video outlines and other details shortly, in the run up to the BNA festival.
@@ -462,14 +476,29 @@
 
 #show results rounded to 2 decimal places
 print(round(di, 2), round(tl , 2), round(tr,2) , round(fps, 2))
 0.35 20.81 43.66 18.07
 
 ```
 
+##### __*Converting maze project csv into one compatible with NORMAN*__
+
+Note: This function is only applicable to one specific project. This is a function to convert Deeplabcut output that was recorded from the bottom of the mouse to one compatible with the rest of the NORMAN system. It assumes the nose, mid and tailbase of the mouse marked were marked in Deeplabcut, and uses these to infer where the ears are, then creates a new CSV based on this. This csv file can then be used as a normal pose file in the system going forwards. It would be advisable to use this function in a loop to do a lot of files at once.
+
+```python
+#get name of the file you want to convert
+maze_pose_file = r"maze_dlc_output.csv"
+#name of the the new file you want to create
+new_file_name = "converted_file.csv"
+#convert the file
+nf.maze_file_convert(maze_pose_file, new_file_name)
+```
+
+
+
 ### Using Deeplabcut with NORMAN.
 
 Deeplabcut is a python library for marker-less tracking of animals using artificial neural networks. It provides a variety of functions centred around streamlining the process of tracking animals. The general workflow of the library is to use a neural network that has been pretrained on animal movement, train it to recognise features on the animal you wish to track by labelling images, then use the trained network to track animal movement on a selection of videos. For in depth details please refer to the official [deeplabcut tutorials on github](https://github.com/DeepLabCut/DeepLabCut/blob/master/docs/UseOverviewGuide.md). Here I will briefly discuss points that are relevant for using Deeplabcut in tandem with the NORMAN system.
 
 Installation – The tutorials recommend tensorflow-gpu installation for using Deeplabcut with hardware accelleration. But the previously discussed tensorflow-directml based environment allows a lot easier installation when using a GPU and allows you to have much more customizable environments, while remaining compatible with deeplabcut.
 
 Config file – When you start a new deeplabcut project it creates a folder with a “config.yaml” file. This config file is what all the functions use to find other files in the directory, such as the location of the trained models. The entire project folder can be moved, copied and shared. As long as the information in the config file is up do date, all the functions should work as normal.
```

### Comparing `norman_ai-0.0.6/setup.cfg` & `norman_ai-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6f72 6d61 6e5f 6169 0d0a 7665   = norman_ai..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 360d 0a61  rsion = 0.0.6..a
+00000020: 7273 696f 6e20 3d20 302e 302e 370d 0a61  rsion = 0.0.7..a
 00000030: 7574 686f 7220 3d20 7365 7969 6a5f 700d  uthor = seyij_p.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7365 7969 2e6f 6f6a 4067 6d61 696c 2e63  seyi.ooj@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 4120 7061 636b 6167 6520 666f 7220  = A package for 
 00000080: 6175 746f 6d61 7469 6f6e 206f 6620 7468  automation of th
 00000090: 6520 6e6f 7665 6c20 6f62 6a65 6374 2072  e novel object r
```

### Comparing `norman_ai-0.0.6/src/norman_ai/data/norman_model1.h5` & `norman_ai-0.0.7/src/norman_ai/data/norman_model1.h5`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.6/src/norman_ai/norman_functions.py` & `norman_ai-0.0.7/src/norman_ai/norman_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1016,17 +1016,17 @@
     #the class takes in a video and the associated deeplabcut pose file for it
     def __init__(self, video, pose_file, no_loc, draw_obj=False, model_path="normal"):
         #have the name of the video as a string
         self.video_name = video
         #the median image is a frame from the video without the mouse 
         self.median_img = median_filt_video(video)
         # object locations are the output of the find objects funtion
-        if draw_obj=True:
+        if draw_obj==True:
             self.object_locs, self.fo_img = find_objects(self.median_img, img_out = True)
-        if draw_obj=False:
+        if draw_obj==False:
             x = draw_objects(self.median_img)
             self.object_locs, self.fo_img = find_objects(x, img_out = True)
         # use relative position
         self.relative_pos = rel_pos(pose_file, self.object_locs)
         #get labels produced by the classification by norman
         self.labels = label_vid(self.relative_pos, model_path)  
         #get the discrimination index, seconds spent with left or right, and fps
@@ -1261,15 +1261,139 @@
     draw_button = Button(window, text = "Visualisation of NORMAN labelling. \nCreates mp4 video.", command = make_label_vid)
     draw_button["bg"] = "orange"
     draw_button.place(x = 300, y = 625, width = 275 , height = 50) 
     
     #this loop keeps the program working apparently
     window.mainloop()
 
+#%% 
 
+def maze_file_convert(poses_file, output_file_name):
+    """
+    Function to convert Deeplabcut output that was recorded from the bottom of the mouse to one compatible with the rest of the NORMAN system.
+    It assumes the nose, mid and tailbase of the mouse marked were marked, and uses these to infer where the ears are, then creates a new CSV based on this.
+
+    Parameters
+    ----------
+    poses_file : string
+        Path to deeplabcut file recorded from maze that you wish to convert.
+    output_file_name : string
+        What you want the new file name to be call
+
+    Returns
+    -------
+    TYPE
+        Outputs a csv file to feed into late parts of the NORMAN system.
+
+    """
+    
+    #make import distance function
+    def distance(point1, point2):
+        return np.sqrt((point2[0] - point1[0])**2 + (point2[1] - point1[1])**2)
+    
+        #make midpoint function
+    def midpoint(point1, point2):
+        return ((point2[0] + point1[0])/2 , (point2[1] + point1[1])/2)
+    
+    def ext_frame(vid_name, frame_index, out_name=False):
+        """ Extract a frame or multiple frames from a video.
+        
+        Keyword arguments:
+            vid_name -- name of input video
+            
+            frame_index -- frame or frame number to be extracted. Accepts integer for single frame. Accepts tuple or list with 2 numbers representing range of frames to be extracted.
+            
+            out_name -- name of image file output for single frame, or folder output for multiple frames (default False). 
+        
+        Returns:
+            If extracting single frame with out_name=False, the function returns image matrix, with a out_name it writes an image file in the current working directory. If extracting multiple frames it writes a folder of images or writes many images to the cwd. 
+        
+        """
+        if type(frame_index) == int:
+            vid = cv2.VideoCapture(vid_name)
+            print("Total amount of frames: " + str(vid.get(7)))
+            vid.set(1, frame_index)
+            ret, frame = vid.read()
+            vid.release()
+            if out_name == False:
+                return frame
+            else:
+                cv2.imwrite(out_name, frame)
+        #section for mutiple frames
+        else:
+            vid = cv2.VideoCapture(vid_name)
+            a,b = frame_index
+            if out_name == False:
+                out_name = ""
+                slash = ""
+            else:
+                os.mkdir(out_name)
+                slash = "\\"
+            #range cant iterate tuples, but it accepts multiple integers
+            for number in range(a, b):
+                vid.set(1, number)
+                ret, frame = vid.read()
+                cv2.imwrite(out_name+slash+str(number)+".png", frame)
+            vid.release()
+            
+    #% read in file
+    #poses_file = "maze_dlc_output.csv"
+    
+    #read in maze dlc data
+    maze_poses = pd.read_csv(poses_file, header=2)        
+    maze_poses.columns=["frame_no", "nose_x", "nose_y", "nose_prob", "mid_x", "mid_y","mid_prob", "tailbase_x", "tailbase_y", "tailbase_prob"]
+    
+    #% extract image from video for plotting
+    
+    #% extract coordinates from all key points
+    nose = (maze_poses["nose_x"], maze_poses["nose_y"])
+    mid = (maze_poses["mid_x"], maze_poses["mid_y"])
+    #tailbase = (maze_poses["tailbase_x"], maze_poses["tailbase_y"])
+    #the distance from the nose to the mid point
+    #nose2mid = distance((maze_poses["nose_x"], maze_poses["nose_y"]), (maze_poses["mid_x"], maze_poses["mid_y"]))
+    
+    #get point halway between nose and mid
+    between_nm = midpoint(nose, mid)
+    
+    
+    # start halway between nose and centre of mouse
+    x1 = between_nm[0]
+    y1 = between_nm[1]
+    # diagonaly opposite point is at the nose
+    x2 = nose[0]
+    y2 = nose[1]
+    #coords of center point
+    xc = (x1 + x2)/2 
+    yc = (y1 + y2)/2
+    #coords of Half-diagonal
+    xd = (x1 - x2)/2
+    yd = (y1 - y2)/2
+    
+    #corner 3 left ear
+    x3 = xc - yd
+    y3 = yc + xd
+    #corner right ear
+    x4 = xc + yd
+    y4 = yc - xd
+    
+    
+    #% make new data frame
+    
+    new_maze_df = pd.DataFrame({"frame_no":maze_poses["frame_no"],
+                  "nose_x":maze_poses["nose_x"], "nose_y":maze_poses["nose_y"], "nose_prob":maze_poses["nose_prob"],
+                  "l_ear_x":x3, "l_ear_y":y3, "l_ear_prob":maze_poses["nose_prob"],
+                  "r_ear_x":x4, "r_ear_y":y4,"r_ear_prob":maze_poses["nose_prob"],
+                  "tailbase_x":maze_poses["tailbase_x"], "tailbase_y":maze_poses["tailbase_y"], "tailbase_prob":maze_poses["tailbase_prob"]})
+    
+    
+    #% make new file and header
+    
+    with open(output_file_name, 'a', newline="\n") as file:
+        file.write('scorer, default, default, default, default, default, default, default, default, default, default, default, default\n bodyparts, nose, nose, nose, l_ear, l_ear, l_ear, r_ear, r_ear, r_ear, tailbase, tailbase, tailbase\n coords, x, y, likelihood, x, y, likelihood, x, y, likelihood, x, y, likelihood\n')
+        new_maze_df.to_csv(file, header=False, index=False, mode="a")
```

### Comparing `norman_ai-0.0.6/src/norman_ai.egg-info/PKG-INFO` & `norman_ai-0.0.7/src/norman_ai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norman-ai
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for automation of the novel object recognition test.
 Home-page: https://github.com/Seyij/norman
 Author: seyij_p
 Author-email: seyi.ooj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -476,14 +476,29 @@
 
 #show results rounded to 2 decimal places
 print(round(di, 2), round(tl , 2), round(tr,2) , round(fps, 2))
 0.35 20.81 43.66 18.07
 
 ```
 
+##### __*Converting maze project csv into one compatible with NORMAN*__
+
+Note: This function is only applicable to one specific project. This is a function to convert Deeplabcut output that was recorded from the bottom of the mouse to one compatible with the rest of the NORMAN system. It assumes the nose, mid and tailbase of the mouse marked were marked in Deeplabcut, and uses these to infer where the ears are, then creates a new CSV based on this. This csv file can then be used as a normal pose file in the system going forwards. It would be advisable to use this function in a loop to do a lot of files at once.
+
+```python
+#get name of the file you want to convert
+maze_pose_file = r"maze_dlc_output.csv"
+#name of the the new file you want to create
+new_file_name = "converted_file.csv"
+#convert the file
+nf.maze_file_convert(maze_pose_file, new_file_name)
+```
+
+
+
 ### Using Deeplabcut with NORMAN.
 
 Deeplabcut is a python library for marker-less tracking of animals using artificial neural networks. It provides a variety of functions centred around streamlining the process of tracking animals. The general workflow of the library is to use a neural network that has been pretrained on animal movement, train it to recognise features on the animal you wish to track by labelling images, then use the trained network to track animal movement on a selection of videos. For in depth details please refer to the official [deeplabcut tutorials on github](https://github.com/DeepLabCut/DeepLabCut/blob/master/docs/UseOverviewGuide.md). Here I will briefly discuss points that are relevant for using Deeplabcut in tandem with the NORMAN system.
 
 Installation – The tutorials recommend tensorflow-gpu installation for using Deeplabcut with hardware accelleration. But the previously discussed tensorflow-directml based environment allows a lot easier installation when using a GPU and allows you to have much more customizable environments, while remaining compatible with deeplabcut.
 
 Config file – When you start a new deeplabcut project it creates a folder with a “config.yaml” file. This config file is what all the functions use to find other files in the directory, such as the location of the trained models. The entire project folder can be moved, copied and shared. As long as the information in the config file is up do date, all the functions should work as normal.
```

