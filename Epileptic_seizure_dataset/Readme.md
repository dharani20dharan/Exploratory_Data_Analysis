# 🧠 Epileptic Seizure Detection using PCA and k-NN

## 📘 Overview
This project applies **Principal Component Analysis (PCA)** and **k-Nearest Neighbors (k-NN)** for classifying epileptic seizure data.  
The model reduces high-dimensional EEG data using PCA and classifies seizure vs. non-seizure states efficiently.

---

## ⚙️ Workflow
1. **Data Preprocessing**
   - Removed unnecessary columns (`Unnamed`)
   - Converted target variable `y` into binary (1 = seizure, 0 = non-seizure)
   - Handled missing values using mean imputation
   - Standardized features with `StandardScaler`

2. **Dimensionality Reduction**
   - Applied PCA to transform data into 178 principal components
   - Visualized cumulative explained variance

3. **Model Training**
   - Used **k-NN classifier (k=5)**
   - Determined the optimal number of components based on F1-score

4. **Evaluation**
   - Achieved **96% accuracy** with strong precision and recall
   - Optimal components ≈ **15–20 PCs**

---

## 📊 Results
| Metric | Score |
|--------|--------|
| **Accuracy** | 96% |
| **Precision (Seizure)** | 0.95 |
| **Recall (Seizure)** | 0.84 |
| **F1-Score (Seizure)** | 0.89 |

---

## 🧠 Insights
- PCA effectively reduced noise and dimensionality while retaining variance.  
- k-NN performed well after dimensionality reduction.  
- Optimal number of principal components = **15–20** for highest F1 score.

---

## 💡 Tech Stack
- Python, Pandas, NumPy, Matplotlib  
- Scikit-learn (PCA, k-NN, Metrics)

