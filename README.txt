PID: 15 Golf Shot Swing Recognition using Optical Flow.

CP_EXPERIMENTATION_FILE.ipynb: The File includes all experimental work done for a course project.
CV_CP.ipynb: The file is the final codebook of Course Project.

1. Dataset Processing 
2. Feature Extraction
3. Feature Optimization
4. Classification
5. Testing


Dataset Preprocessing (Dataset - https://www.kaggle.com/datasets/marcmarais/videos-160)
a. Cut videos into frame of specified classes
b. resize videos to 160x160

Feature Extraction
a. Apply Optical flow on class videos.
b. Store trajectory-related images in HSV and morphological images.
c. Extract Features of Trajectory. (8 features)
d. Apply HOG on trajectory-related image.
e. Store HOG features. ( 14 features)
f. Extract SIFT features from morphological image (128 features)
g. Store in features_lk.csv, features_gf.csv

Feature Optimization
a. Normalize all features in features_lk.csv and features_gf.csv
b. append data into features.csv

Classification
a. Divide data into Train and Test
b. Apply Decision Tree
c. Apply Decision Tree with Hyperparameter grid
d. Apply Random Forest
e. Apply Random Forest with Hyperparameter grid
f. Apply KNN
g. Apply KNN with Hyperparameter grid
h. Apply SVM

Testing
a. Load Random Forest model
b. Define Function for feature extraction and optimization
c. Give Input of video
d. Count of features from each class.
e. Print Majority Class.

Execution Instruction:
All paths of Project file are set according to local environment relative to this folder.




