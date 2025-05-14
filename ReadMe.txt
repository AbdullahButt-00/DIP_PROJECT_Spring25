🚦 Traffic Sign Classification Using Classical Digital Image Processing Techniques
This project implements a complete rule-based traffic sign classification system using only classical digital image processing techniques. Unlike modern machine learning approaches, all image analysis tasks are performed using manual operations with NumPy and basic Python libraries.

📌 Objective
To develop an end-to-end traffic sign classifier capable of identifying signs based on their color, shape, and geometric features using traditional image processing techniques such as:

Filtering

Segmentation

Feature extraction

Rule-based classification

📁 Dataset
Download Link:
📥 Google Drive Download: https://drive.google.com/file/d/1HXH-6fVv3qplhXTOGJnBen2Tc_HRpGnI/view

Classes Used:
Label	Description	Category
0	Speed Limit 20	Prohibitory
1	Speed Limit 30	Prohibitory
2	Speed Limit 50	Prohibitory
3	Speed Limit 60	Prohibitory
4	Speed Limit 70	Prohibitory
5	Speed Limit 80	Prohibitory
6	Restriction Ends 80	Other
7	Speed Limit 100	Prohibitory

⚙️ Features Implemented
1. Preprocessing
Mean Filter

Gaussian Filter

Median Filter

Adaptive Median Filter

Unsharp Masking & High-Boost Filtering

2. Color-Based Segmentation
Manual conversion to HSV

Mask creation for red and blue signs

Morphological operations

Hole filling and noise removal

3. Edge Detection
Canny Edge Detection (manual implementation)

Gradient Computation

Non-Maximum Suppression

Hysteresis Thresholding

4. Geometric Normalization
Rotation to upright orientation

Scaling to fixed size

Optional perspective transform (all in NumPy)

5. Feature Extraction
Harris Corner Count

Circularity

Aspect Ratio

Extent (region area / bounding box area)

Average Hue

6. Rule-Based Classification
If-else rules using extracted features

Logic based on color and shape

Distinguishes similar-looking sign classes

📈 Evaluation
The system’s performance is evaluated using the following outputs:

results.csv — filename, ground truth, prediction, and correctness

metrics.txt — accuracy, precision, recall (overall and per-class)

confusion_matrix.png — confusion matrix visualization

✅ Requirements
Python 3.x

NumPy

PIL or OpenCV (only for loading images)

Matplotlib / Seaborn (for visualization)
