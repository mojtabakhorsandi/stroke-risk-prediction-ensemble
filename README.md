# Stroke Risk Prediction using Ensemble Learning, Hyperparameter Optimization, and Dimensionality Reduction

This repository contains the main code and methodology from my Master's thesis:
**"Hyperparameters Tuning and Dimension Reduction Effects on Stroke Prediction Using Ensemble Learning with Data Mining in Unbalanced Data."**

---

## 🎯 Goal
To develop a machine learning pipeline that predicts the risk of stroke before it occurs, focusing on:
- Handling highly imbalanced medical data
- Reducing noise and irrelevant features
- Optimizing model performance via hyperparameter tuning
- Maximizing recall and F1-score for early clinical risk detection

---

## 🧠 Dataset
- Source: Kaggle Stroke Prediction Dataset (~5110 samples, 12 clinical and demographic features)
- Main features: age, hypertension, heart disease, glucose level, BMI, smoking status, etc.
- Target: stroke (1 = stroke, 0 = no stroke)

The raw dataset is not shared due to privacy/ethics. See `data/README_DATA.txt`.

---

## 🧩 Methods

### 1. Data Preprocessing
- Label encoding for categorical variables  
- KNN Imputation for missing values  
- Outlier detection and removal  
- Power transform to normalize distributions  

### 2. Handling Imbalanced Data
- Oversampling using SMOTE-style techniques to balance minority class (stroke)

### 3. Dimensionality Reduction
- PCA, LDA, and t-SNE were tested to identify key features and improve generalization.

### 4. Model Training
- k-Nearest Neighbors (KNN)  
- Logistic Regression  
- Support Vector Machine (SVM)  
- Decision Tree  
- Random Forest  
- AdaBoost  
- Gradient Boosting  
- XGBoost  

### 5. Hyperparameter Optimization
- Grid Search for best-performing parameter sets

### 6. Evaluation
Metrics:
- Accuracy  
- Precision  
- Recall / Sensitivity  
- F1-score  
- Confusion Matrix  

Emphasis is placed on **recall of the stroke class** to minimize false negatives (missed high-risk patients).

---

## 📊 Results
- Ensemble models (Random Forest, Gradient Boosting, XGBoost) achieved **F1-scores ≈ 0.96–0.98**  
- Recall for the stroke class reached **≈ 0.99**, meaning nearly all high-risk cases were detected  
- Dimensionality reduction (t-SNE + KNN / Decision Tree) further improved sensitivity

---

## 🧰 Tech Stack
- Python (Jupyter Notebook)  
- scikit-learn  
- imbalanced-learn  
- XGBoost  
- matplotlib, seaborn  

---

## 📁 Project Structure


---

## 👨‍💻 Author
**Mojtaba Khorsandi Ebrahimi**  
M.Sc. in Bioelectric Biomedical Engineering  
University of Genoa  

---

## 🧩 Future Work
This work can be extended to real-time medical decision support systems, or integrated into cognitive modeling research on human health decision-making.
