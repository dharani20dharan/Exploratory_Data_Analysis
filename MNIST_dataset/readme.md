# MNIST Digit Classification using SGD

##  Objective
To classify digits **6** and **9** from the MNIST dataset using **Stochastic Gradient Descent (SGD)** and analyze the impact of different learning rates.

---

##  Steps Performed

1. **Dataset Loading**
   - Fetched MNIST dataset from OpenML.
   - Extracted data and converted targets to integers.

2. **Data Preparation**
   - Filtered digits 6 and 9 for binary classification.
   - Split into training and testing sets.
   - Shuffled data for randomness.

3. **Model Building**
   - Used `Pipeline` combining:
     - `StandardScaler()` for normalization.
     - `SGDClassifier(loss='log_loss')` for logistic regression.
   - Compared performance for two learning rates:  
     - `eta0 = 0.01`  
     - `eta0 = 0.000001`

4. **Evaluation**
   - Computed **log loss** over 10 iterations.
   - Plotted **Loss vs Iteration** curve for both learning rates.

---

##  Results

| Learning Rate | Observation |
|----------------|--------------|
| 0.01 | Faster convergence, lower loss |
| 0.000001 | Slower learning, higher loss |

---

##  Tech Stack
- **Language:** Python  
- **Libraries:** NumPy, Pandas, Matplotlib, Scikit-learn  

---

##  Output
- **Plot:** Iteration vs Loss Curve  
- Demonstrates effect of learning rate on model convergence.

---

# MNIST Digit Classification using SVM

##  Objective
To classify handwritten digits (0–9) from the **MNIST dataset** using **Linear** and **Nonlinear (RBF)** Support Vector Machines, and optimize model performance using **GridSearchCV**.

---

##  Steps Performed

1. **Dataset Preparation**
   - Loaded the MNIST dataset from OpenML.
   - Normalized pixel values and reshaped images to 1D arrays.
   - Split data into training and testing sets.

2. **Model Training**
   - Implemented two SVM pipelines:
     - **Linear SVM:** Kernel = 'linear'
     - **Nonlinear SVM:** Kernel = 'rbf'
   - Used `MinMaxScaler()` for feature scaling.

3. **Evaluation**
   - Computed **accuracy**, **confusion matrix**, and **classification report**.
   - Visualized confusion matrices with Seaborn heatmaps.

4. **Hyperparameter Tuning**
   - Applied `GridSearchCV` to optimize **C** and **gamma** parameters for the RBF kernel.

---

##  Results

| Model | Accuracy | Key Insight |
|--------|-----------|-------------|
| Linear SVM | **91.0%** | High precision and balanced class performance |
| Nonlinear SVM (RBF) | **87.0%** | Slightly lower accuracy but captures non-linear relations |
| Best Model (Grid Search) | **≈82% (Training)** | Optimal `C` and `gamma` found |

---

##  Tech Stack
- **Language:** Python  
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn  

---

##  Visualizations
- Sample digit grid (28×28 images)  
- Confusion matrices for both Linear and RBF kernels  
- Classification metrics for all models

---
