# Task6
# Iris Classification using K-Nearest Neighbors (KNN)

This project implements a **K-Nearest Neighbors (KNN)** classifier on the Iris dataset to classify flower species based on sepal and petal measurements.  
It includes feature normalization, experimentation with different values of `K`, model evaluation, and a decision boundary visualization.

---

## Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  

---

## Steps and Implementation

### 1. Choose a Classification Dataset and Normalize Features
- Loaded the **Iris dataset** using scikit-learn
- Selected the first two features (`sepal length` and `sepal width`) for easy visualization
- Normalized features using `StandardScaler`

### 2. Use KNeighborsClassifier from sklearn
- Trained a `KNeighborsClassifier` with default parameters
- Used the Euclidean distance metric to find nearest neighbors

### 3. Experiment with Different Values of K
- Trained and evaluated models for K values from 1 to 15
- Plotted K vs Accuracy to choose the best value

### 4. Evaluate Model using Accuracy and Confusion Matrix
- Reported performance using:
  - Accuracy
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-Score)

### 5. Visualize Decision Boundaries
- Created a mesh grid over the feature space
- Visualized how the KNN classifier partitions the feature space for each class

---

## Example Output

Best K: 5 Accuracy (K=5): 0.933 Confusion Matrix: [[10 0 0] [ 0 10 1] [ 0 1 8]] Classification Report: precision recall f1-score support
      - 0       1.00      1.00      1.00        10
      - 1       0.91      0.91      0.91        11
      - 2       0.89      0.89      0.89         9
