# **Advanced Skin Disease Classification with Image Processing and Feature Extraction** 

This project focuses on classifying skin diseases using feature extraction techniques on images. The workflow involves data preprocessing, feature extraction, and model evaluation using machine learning algorithms such as SVM, KNN, and Decision Tree.

## 📋 Overview

The goal of this project is to classify skin diseases using images. The images undergo several preprocessing steps such as resizing, noise removal, and enhancement, followed by feature extraction to capture color, texture, and local binary patterns (LBP). The processed features are then fed into machine learning models to classify the diseases.

### 🩺 Skin Disease Categories

The dataset includes images from the following categories:

1. Actinic keratosis
2. Atopic Dermatitis
3. Benign keratosis
4. Dermatofibroma
5. Melanocytic nevus
6. Melanoma
7. Squamous cell carcinoma
8. Tinea Ringworm Candidiasis
9. Vascular lesion

## 🔬 Methodology

### 🛠️ Preprocessing

The preprocessing function resizes the images to a consistent size of 512x512 pixels and applies several transformations such as:

* **Hair Removal**: Using the black-hat transformation.
* **Inpainting**: Filling in areas identified as hair or background.
* **Gaussian Filtering**: Smoothing the image to reduce noise.

### 🧠 Feature Extraction

The following features are extracted from each image:

1. **Color Features**: Mean, standard deviation, and skewness for each color channel (RGB).
2. **Texture Features**: Using the Gray Level Co-occurrence Matrix (GLCM) to extract contrast, correlation, dissimilarity, energy, entropy, and homogeneity.
3. **Local Binary Pattern (LBP)**: Mean and standard deviation of the LBP image.

### 🤖 Modeling

Three machine learning models are trained and evaluated:

1. **Support Vector Machine (SVM)**
2. **K-Nearest Neighbors (KNN)**
3. **Decision Tree Classifier**

The models are tuned using GridSearchCV to find the best hyperparameters.

### 📊 Evaluation

Each model's performance is evaluated using:

* **Accuracy**
* **Precision, Recall, F1-Score**: From the classification report
* **Confusion Matrix**: To visualize model performance for each disease category

### 📈 Visualization

* **Preprocessing Visualization**: Display a comparison of images before and after preprocessing.
* **Feature Distribution**: Visualize the distribution of extracted features using histograms.



