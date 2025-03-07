# 📌 Application of Feature Extraction Techniques in Image Classification

### 📝 **Description**  
This project implements an image classification system based on feature extraction and machine learning. Two feature extraction algorithms are developed and compared to analyze their effectiveness in classifying images of animals into four categories: **cats, elephants, horses, and spiders**.

This project was developed as a final project for the **Computer Vision** course in the **third year** of the **Computer Engineering** degree at the **Universidad Pública de Navarra (UPNA)**.

### 🎯 **Objectives**  
✅ Implement and evaluate two feature extraction algorithms.  
✅ Apply different machine learning models for classification.  
✅ Compare the results obtained with each approach.  

---

## 🔹 **Technologies Used**  
- **Python** 🐍  
- **scikit-learn** ⚙️ (Classification models and cross-validation)  
- **scikit-image** 🖼️ (Image preprocessing)  
- **NumPy & Pandas** 📊 (Data handling)  

---

## 🔍 **Feature Extraction Algorithms**  

### 📌 **Algorithm 1: Histograms from Binary Transformation**  
- Converts each pixel to binary values by comparing with its neighbors.  
- Transforms the binary values to decimal and generates histograms by blocks.  
- **Improvement:** Introduction of **uniform transitions** to reduce complexity.  

### 📌 **Algorithm 2: Histogram of Oriented Gradients (HOG)**  
- Calculates the magnitude and orientation of the gradient at each pixel.  
- Generates histograms with 9 bins, summing the accumulated magnitudes.  
- **Improvement:** **Normalization with overlapping blocks** to enhance representation.  

---

## 📊 **Implemented Models**  

Various **machine learning** models were tested:  

- **SVM (Support Vector Machine)**  
- **Logistic and Polynomial Regression**  
- **Neural Networks (2 hidden layers, 50 neurons)**  
- **Ensemble techniques:**  
  - **Bagging (Bootstrap Aggregating)**  
  - **Boosting (AdaBoost)**  
  - **Random Forest**  
- **Naive Bayes**  
- **Multiclass approaches (OVO and OVA)**  

---

## 📈 **Results and Conclusions**  

🔹 **Best model with Algorithm 1:** **Bagging**, with a **67.33% cross-validation performance** and **57.42% on the test set**.  

🔹 **Best model with Algorithm 2:** **Neural Networks**, with a **73.58% cross-validation performance** and **63.58% on the test set**.  

📌 **Conclusion:**  
The second feature extraction algorithm has proven to be the most effective for this problem, achieving better results in the final classification.  
