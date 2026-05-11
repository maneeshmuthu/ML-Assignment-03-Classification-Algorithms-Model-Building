# Breast Cancer Classification using Machine Learning

## Project Overview
This project implements and compares multiple supervised machine learning classification algorithms using the Breast Cancer dataset available in the sklearn library.

The objective of this project is to evaluate the performance of different classification models in predicting whether a tumor is malignant or benign.

---

## Dataset
The dataset used in this project is the Breast Cancer Wisconsin Dataset from sklearn.

It contains:
- 569 samples
- 30 numerical input features
- Binary target classification:
  - Malignant
  - Benign

Dataset Source:
```python
from sklearn.datasets import load_breast_cancer
```

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

---

## Machine Learning Algorithms Implemented

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. Support Vector Machine (SVM)
5. k-Nearest Neighbors (k-NN)

---

## Preprocessing Steps
The following preprocessing steps were performed:

- Loaded dataset from sklearn
- Converted dataset into a Pandas DataFrame
- Checked for missing values
- Performed train-test split
- Applied feature scaling using StandardScaler

Feature scaling was necessary because algorithms such as:
- Logistic Regression
- SVM
- k-NN

are sensitive to differences in feature magnitudes.

---

## Model Evaluation
The models were evaluated using Accuracy Score.

### Sample Results

| Model | Accuracy |
|---|---|
| Logistic Regression | 97% |
| Decision Tree | 94% |
| Random Forest | 96% |
| SVM | 98% |
| k-NN | 95% |

---

## Best Performing Model
Support Vector Machine (SVM) achieved the highest accuracy among the implemented models.

---

## Project Structure

```text
Breast-Cancer-Classification/
│
├── ML_Assignment_3_Classification.ipynb
├── README.md
└── requirements.txt
```

---

## How to Run the Project

### Clone Repository
```bash
git clone https://github.com/your-username/your-repository-name.git
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

### Run Notebook
Open the Jupyter Notebook and run all cells.

---

## Notes
During implementation, a threadpoolctl/OpenBLAS compatibility issue occurred in the local Anaconda environment on macOS while running the k-NN model. The issue was resolved using an alternative algorithm parameter.

---

## Conclusion
This project demonstrates the implementation and comparison of multiple supervised learning algorithms for medical diagnosis classification tasks. The results show that SVM performed best on this dataset.

---

## Author
Maneesh M
