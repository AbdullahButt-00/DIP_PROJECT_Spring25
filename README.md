# 🚦 Traffic Sign Classification Using Classical Digital Image Processing Techniques

This project implements a complete rule-based traffic sign classification system using **classical digital image processing techniques only**. Unlike modern deep learning-based approaches, all tasks here are performed manually using **NumPy** and core Python libraries.

---

## 📌 Objective

To develop an **end-to-end traffic sign classifier** that identifies signs using:

- 🎨 **Color-based analysis**
- 🔷 **Shape and geometric features**
- 🔍 **Hand-crafted rule-based classification**

---

## 📁 Dataset

- 📥 **[Download via Google Drive](https://drive.google.com/file/d/1HXH-6fVv3qplhXTOGJnBen2Tc_HRpGnI/view)**

### 🔢 Classes Used

| Label | Description            | Category     |
|-------|------------------------|--------------|
| 0     | Speed Limit 20         | Prohibitory  |
| 1     | Speed Limit 30         | Prohibitory  |
| 2     | Speed Limit 50         | Prohibitory  |
| 3     | Speed Limit 60         | Prohibitory  |
| 4     | Speed Limit 70         | Prohibitory  |
| 5     | Speed Limit 80         | Prohibitory  |
| 6     | Restriction Ends 80    | Other        |
| 7     | Speed Limit 100        | Prohibitory  |

---

## ⚙️ Features Implemented

### 1️⃣ Preprocessing

- ✅ Mean Filter  
- ✅ Gaussian Filter  
- ✅ Median Filter  
- ✅ Adaptive Median Filter  
- ✅ Unsharp Masking & High-Boost Filtering

### 2️⃣ Color-Based Segmentation

- ✅ Manual RGB → HSV conversion  
- ✅ Red & Blue color masking  
- ✅ Morphological Operations  
- ✅ Hole Filling and Noise Removal

### 3️⃣ Edge Detection

- ✅ Manual Canny Edge Detection  
  - Gradient Computation  
  - Non-Maximum Suppression  
  - Hysteresis Thresholding

### 4️⃣ Geometric Normalization

- ✅ Rotation Correction  
- ✅ Rescaling to Uniform Size  
- ✅ Optional Perspective Transform

### 5️⃣ Feature Extraction

- ✅ Harris Corner Count  
- ✅ Circularity  
- ✅ Aspect Ratio  
- ✅ Extent (Region Area / Bounding Box Area)  
- ✅ Average Hue

### 6️⃣ Rule-Based Classification

- ✅ If-Else Based Rule Set  
- ✅ Shape & Color Logic  
- ✅ Disambiguation of Similar Signs

---

## 📈 Evaluation

- 📄 **results.csv** — filename, ground truth, prediction, correctness  
- 📝 **metrics.txt** — accuracy, precision, recall (overall and per-class)  
- 📊 **confusion_matrix.png** — visual confusion matrix  

---

## ✅ Requirements

Install required libraries using pip:

```bash
pip install numpy matplotlib pillow
```

### 🔧 Core Libraries

- Python 3.x
- NumPy
- PIL (or OpenCV for image loading)
- Matplotlib / Seaborn (for visualization)

---

## 🧠 Project Highlights

- 🚫 No machine learning or CNNs
- 🧮 Fully handcrafted digital image processing pipeline
- 🧪 Educational and interpretable approach to image classification

---

## 🙋‍♂️ Note

Developed as part of a classical DIP course project.  

---

