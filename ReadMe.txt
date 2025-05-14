Traffic Sign Classification Using Classical Digital Image Processing Techniques
This project implements a complete rule-based traffic sign classification system using only classical digital image processing techniques. Unlike modern machine learning approaches, all image analysis tasks are performed using manual operations with NumPy and basic Python libraries.

📌 Objective
To develop an end-to-end traffic sign classifier capable of identifying signs based on their color, shape, and geometric features using traditional image processing techniques such as filtering, segmentation, and feature extraction.


➡️ Dataset Link: Google Drive Download
https://drive.google.com/file/d/1HXH-6fVv3qplhXTOGJnBen2Tc_HRpGnI/view

Classes used:
0 = speed limit 20 (prohibitory)
1 = speed limit 30 (prohibitory)
2 = speed limit 50 (prohibitory)
3 = speed limit 60 (prohibitory)
4 = speed limit 70 (prohibitory)
5 = speed limit 80 (prohibitory)
6 = restriction ends 80 (other)
7 = speed limit 100 (prohibitory)

⚙️ Features Implemented
1. Preprocessing
Mean, Gaussian, Median, and Adaptive Median Filters , Unsharp Masking & High-Boost Filtering

2. Color-Based Segmentation
Manual conversion to HSV
Mask creation for red and blue signs
Morphological operations and hole filling

3. Edge Detection
Canny edge detection (gradient → non-max suppression → hysteresis)

4. Geometric Normalization
Rotation, scaling, and optional perspective correction via affine transforms

5. Feature Extraction
Harris Corner Count
Circularity
Aspect Ratio
Extent
Average Hue

6. Rule-Based Classification
If-else rules using extracted features

Color and shape-based logic to distinguish sign classes

📈 Evaluation
The system's performance is evaluated using:
results.csv: Contains file name, ground truth, prediction, and correctness
metrics.txt: Reports accuracy, precision, and recall for each class
confusion_matrix.png: Visual representation of the confusion matrix

✅ Requirements
Python 3.x
NumPy
PIL or OpenCV (only for image loading)
Matplotlib / Seaborn (for visualization)



